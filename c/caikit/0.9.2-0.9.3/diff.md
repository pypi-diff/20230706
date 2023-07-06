# Comparing `tmp/caikit-0.9.2.tar.gz` & `tmp/caikit-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-0.9.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "caikit-0.9.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `caikit-0.9.2.tar` & `caikit-0.9.3.tar`

### file list

```diff
@@ -1,321 +1,322 @@
--rw-r--r--   0        0        0       60 2023-06-29 16:53:05.230679 caikit-0.9.2/.coveragerc
--rw-r--r--   0        0        0      676 2023-06-29 16:53:05.230679 caikit-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-06-29 16:53:05.230679 caikit-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-06-29 16:53:05.230679 caikit-0.9.2/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0      106 2023-06-29 16:53:05.230679 caikit-0.9.2/.github/dependabot.yml
--rw-r--r--   0        0        0     1698 2023-06-29 16:53:05.230679 caikit-0.9.2/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1328 2023-06-29 16:53:05.230679 caikit-0.9.2/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1117 2023-06-29 16:53:05.230679 caikit-0.9.2/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      260 2023-06-29 16:53:05.230679 caikit-0.9.2/.gitignore
--rw-r--r--   0        0        0      324 2023-06-29 16:53:05.230679 caikit-0.9.2/.isort.cfg
--rw-r--r--   0        0        0      370 2023-06-29 16:53:05.230679 caikit-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      122 2023-06-29 16:53:05.230679 caikit-0.9.2/.prettierignore
--rw-r--r--   0        0        0       12 2023-06-29 16:53:05.230679 caikit-0.9.2/.prettierrc.yaml
--rw-r--r--   0        0        0    21434 2023-06-29 16:53:05.230679 caikit-0.9.2/.pylintrc
--rw-r--r--   0        0        0      599 2023-06-29 16:53:05.230679 caikit-0.9.2/.readthedocs.yaml
--rw-r--r--   0        0        0       78 2023-06-29 16:53:05.230679 caikit-0.9.2/.whitesource
--rw-r--r--   0        0        0      368 2023-06-29 16:53:05.230679 caikit-0.9.2/CODEOWNERS
--rw-r--r--   0        0        0     7164 2023-06-29 16:53:05.230679 caikit-0.9.2/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-06-29 16:53:05.230679 caikit-0.9.2/LICENSE
--rw-r--r--   0        0        0     6317 2023-06-29 16:53:05.230679 caikit-0.9.2/README.md
--rw-r--r--   0        0        0      152 2023-06-29 16:53:05.230679 caikit-0.9.2/SECURITY.md
--rw-r--r--   0        0        0    44878 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit-overview.png
--rw-r--r--   0        0        0      427 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/__init__.py
--rw-r--r--   0        0        0      727 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/config/__init__.py
--rw-r--r--   0        0        0     6035 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/config/config.py
--rw-r--r--   0        0        0     6388 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/config/config.yml
--rw-r--r--   0        0        0     1642 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/__init__.py
--rw-r--r--   0        0        0      812 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/augmentors/__init__.py
--rw-r--r--   0        0        0     3509 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/augmentors/base.py
--rw-r--r--   0        0        0     2817 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/augmentors/merged_augmentor.py
--rw-r--r--   0        0        0      355 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/augmentors/schemes/__init__.py
--rw-r--r--   0        0        0     2029 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/augmentors/schemes/always_selection_scheme.py
--rw-r--r--   0        0        0     3141 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/augmentors/schemes/base.py
--rw-r--r--   0        0        0     3243 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
--rw-r--r--   0        0        0     2875 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/augmentors/schemes/random_single_selection_scheme.py
--rw-r--r--   0        0        0     1027 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/data_model/__init__.py
--rw-r--r--   0        0        0    40051 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/data_model/base.py
--rw-r--r--   0        0        0      750 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     2402 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/data_model/data_backends/base.py
--rw-r--r--   0        0        0     4983 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/data_model/data_backends/dict_backend.py
--rw-r--r--   0        0        0    17602 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/data_model/dataobject.py
--rw-r--r--   0        0        0     4988 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/data_model/enums.py
--rw-r--r--   0        0        0     5127 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/data_model/json_dict.py
--rw-r--r--   0        0        0     1564 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/data_model/producer.py
--rw-r--r--   0        0        0     3920 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/data_model/protobufs/__init__.py
--rw-r--r--   0        0        0      577 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/data_model/streams/__init__.py
--rw-r--r--   0        0        0     5446 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/data_model/streams/converter.py
--rw-r--r--   0        0        0     4776 2023-06-29 16:53:05.230679 caikit-0.9.2/caikit/core/data_model/streams/csv_column_formatter.py
--rw-r--r--   0        0        0    39907 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/data_model/streams/data_stream.py
--rw-r--r--   0        0        0     3580 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/data_model/streams/resolver.py
--rw-r--r--   0        0        0     5217 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/data_model/streams/validator.py
--rw-r--r--   0        0        0    21179 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/model_manager.py
--rw-r--r--   0        0        0      684 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/module_backends/__init__.py
--rw-r--r--   0        0        0     2824 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/module_backends/backend_types.py
--rw-r--r--   0        0        0     4717 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/module_backends/base.py
--rw-r--r--   0        0        0     2880 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/module_backends/local_backend.py
--rw-r--r--   0        0        0     5982 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/module_backends/module_backend_config.py
--rw-r--r--   0        0        0      742 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/modules/__init__.py
--rw-r--r--   0        0        0    30052 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/modules/base.py
--rw-r--r--   0        0        0     6145 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/modules/config.py
--rw-r--r--   0        0        0    11011 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/modules/decorator.py
--rw-r--r--   0        0        0     4141 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/modules/loader.py
--rw-r--r--   0        0        0     6013 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/modules/meta.py
--rw-r--r--   0        0        0    12931 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/modules/saver.py
--rw-r--r--   0        0        0     3885 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/registries.py
--rw-r--r--   0        0        0      654 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/signature_parsing/__init__.py
--rw-r--r--   0        0        0    10666 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/signature_parsing/docstrings.py
--rw-r--r--   0        0        0     4688 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/signature_parsing/module_signature.py
--rw-r--r--   0        0        0     8221 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/signature_parsing/parsers.py
--rw-r--r--   0        0        0    10542 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/task.py
--rw-r--r--   0        0        0      982 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/toolkit/__init__.py
--rw-r--r--   0        0        0     4704 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/toolkit/compatibility.py
--rw-r--r--   0        0        0      637 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/toolkit/errors/__init__.py
--rw-r--r--   0        0        0    21349 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/toolkit/errors/error_handler.py
--rw-r--r--   0        0        0     1400 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/toolkit/errors/validation_error.py
--rw-r--r--   0        0        0     3240 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/toolkit/factory.py
--rw-r--r--   0        0        0     4914 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/toolkit/fileio.py
--rw-r--r--   0        0        0     1648 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/toolkit/logging.py
--rw-r--r--   0        0        0    31633 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/toolkit/quality_evaluation.py
--rw-r--r--   0        0        0     3356 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/toolkit/serializers.py
--rw-r--r--   0        0        0     2148 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/toolkit/sync_to_async.py
--rw-r--r--   0        0        0     5965 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/core/toolkit/wip_decorator.py
--rw-r--r--   0        0        0     1056 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/interfaces/__init__.py
--rw-r--r--   0        0        0      748 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/interfaces/common/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/interfaces/common/data_model/__init__.py
--rw-r--r--   0        0        0     1431 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/interfaces/common/data_model/producer.py
--rw-r--r--   0        0        0      618 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/interfaces/nlp/__init__.py
--rw-r--r--   0        0        0      809 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/interfaces/nlp/data_model/__init__.py
--rw-r--r--   0        0        0      740 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/interfaces/nlp/data_model/package.py
--rw-r--r--   0        0        0     2254 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/interfaces/nlp/data_model/text_generation.py
--rw-r--r--   0        0        0     1383 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/interfaces/nlp/tasks.py
--rw-r--r--   0        0        0      611 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/interfaces/runtime/__init__.py
--rw-r--r--   0        0        0      763 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/interfaces/runtime/data_model/__init__.py
--rw-r--r--   0        0        0     1886 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/interfaces/runtime/data_model/training_management.py
--rw-r--r--   0        0        0      577 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/runtime/__init__.py
--rw-r--r--   0        0        0     1662 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/runtime/dump_services.py
--rw-r--r--   0        0        0    14262 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/runtime/grpc_server.py
--rw-r--r--   0        0        0      577 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/runtime/interceptors/__init__.py
--rw-r--r--   0        0        0    15627 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
--rw-r--r--   0        0        0      577 2023-06-29 16:53:05.234679 caikit-0.9.2/caikit/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     4645 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/metrics/rpc_meter.py
--rw-r--r--   0        0        0      577 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    17083 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/model_management/batcher.py
--rw-r--r--   0        0        0     2606 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/model_management/loaded_model.py
--rw-r--r--   0        0        0     5802 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/model_management/model_loader.py
--rw-r--r--   0        0        0    12089 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/model_management/model_manager.py
--rw-r--r--   0        0        0     4310 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/model_management/model_sizer.py
--rw-r--r--   0        0        0     1642 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/model_management/training_manager.py
--rw-r--r--   0        0        0      367 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/protobufs/README.md
--rw-r--r--   0        0        0      698 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/protobufs/__init__.py
--rw-r--r--   0        0        0    11375 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/protobufs/model_mesh_pb2.py
--rw-r--r--   0        0        0    12846 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
--rw-r--r--   0        0        0    10107 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/protobufs/model_runtime_pb2.py
--rw-r--r--   0        0        0    10556 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     5535 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/protobufs/process_pb2.py
--rw-r--r--   0        0        0     2569 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/protobufs/process_pb2_grpc.py
--rw-r--r--   0        0        0     8844 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/protobufs/protos/model-mesh.proto
--rw-r--r--   0        0        0     6795 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/protobufs/protos/model-runtime.proto
--rw-r--r--   0        0        0     2479 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/protobufs/protos/process.proto
--rw-r--r--   0        0        0     9572 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/service_factory.py
--rw-r--r--   0        0        0      109 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     1779 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/service_generation/compatibility_checker.py
--rw-r--r--   0        0        0     4229 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/service_generation/create_service.py
--rw-r--r--   0        0        0    12070 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/service_generation/data_stream_source.py
--rw-r--r--   0        0        0     6146 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/service_generation/protoable.py
--rw-r--r--   0        0        0    12152 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/service_generation/rpcs.py
--rw-r--r--   0        0        0     2216 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/service_generation/type_helpers.py
--rw-r--r--   0        0        0      577 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/servicers/__init__.py
--rw-r--r--   0        0        0    12641 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/servicers/global_predict_servicer.py
--rw-r--r--   0        0        0    12451 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/servicers/global_train_servicer.py
--rw-r--r--   0        0        0    10637 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/servicers/model_runtime_servicer.py
--rw-r--r--   0        0        0     5440 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/servicers/model_train_servicer.py
--rw-r--r--   0        0        0     1667 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/servicers/training_management_servicer.py
--rw-r--r--   0        0        0      577 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/types/__init__.py
--rw-r--r--   0        0        0      957 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/types/aborted_exception.py
--rw-r--r--   0        0        0     1558 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/types/caikit_runtime_exception.py
--rw-r--r--   0        0        0      960 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/types/thread_destroyed_exception.py
--rw-r--r--   0        0        0      577 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/utils/__init__.py
--rw-r--r--   0        0        0     6790 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/utils/import_util.py
--rw-r--r--   0        0        0    13825 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/utils/servicer_util.py
--rw-r--r--   0        0        0      577 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     3732 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/work_management/abortable_action.py
--rw-r--r--   0        0        0     2969 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/work_management/call_aborter.py
--rw-r--r--   0        0        0     7596 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/work_management/destroyable_thread.py
--rw-r--r--   0        0        0    11924 2023-06-29 16:53:05.238680 caikit-0.9.2/caikit/runtime/work_management/train_executors.py
--rw-r--r--   0        0        0      169 2023-06-29 16:53:05.238680 caikit-0.9.2/code-of-conduct.md
--rw-r--r--   0        0        0      639 2023-06-29 16:53:05.238680 caikit-0.9.2/docs/Makefile
--rw-r--r--   0        0        0     6860 2023-06-29 16:53:05.238680 caikit-0.9.2/docs/adrs/001-module.md
--rw-r--r--   0        0        0     1610 2023-06-29 16:53:05.238680 caikit-0.9.2/docs/adrs/010-data-model-definition.md
--rw-r--r--   0        0        0     2352 2023-06-29 16:53:05.238680 caikit-0.9.2/docs/adrs/015-runtime-service-generation.md
--rw-r--r--   0        0        0     2581 2023-06-29 16:53:05.238680 caikit-0.9.2/docs/adrs/018-shared-backends.md
--rw-r--r--   0        0        0     1223 2023-06-29 16:53:05.238680 caikit-0.9.2/docs/adrs/019-loader-stack.md
--rw-r--r--   0        0        0      404 2023-06-29 16:53:05.238680 caikit-0.9.2/docs/adrs/README.md
--rw-r--r--   0        0        0     2423 2023-06-29 16:53:05.242679 caikit-0.9.2/docs/architecture_club/04-25-23.md
--rw-r--r--   0        0        0      342 2023-06-29 16:53:05.242679 caikit-0.9.2/docs/architecture_club/README.md
--rw-r--r--   0        0        0      805 2023-06-29 16:53:05.242679 caikit-0.9.2/docs/make.bat
--rw-r--r--   0        0        0     3053 2023-06-29 16:53:05.242679 caikit-0.9.2/docs/source/conf.py
--rw-r--r--   0        0        0      225 2023-06-29 16:53:05.242679 caikit-0.9.2/docs/source/index.rst
--rw-r--r--   0        0        0      837 2023-06-29 16:53:05.242679 caikit-0.9.2/examples/start_runtime_with_sample_lib.py
--rw-r--r--   0        0        0     6095 2023-06-29 16:53:05.242679 caikit-0.9.2/examples/text-sentiment/README.md
--rw-r--r--   0        0        0     1475 2023-06-29 16:53:05.242679 caikit-0.9.2/examples/text-sentiment/client.py
--rw-r--r--   0        0        0      673 2023-06-29 16:53:05.242679 caikit-0.9.2/examples/text-sentiment/models/text_sentiment/config.yml
--rw-r--r--   0        0        0       77 2023-06-29 16:53:05.242679 caikit-0.9.2/examples/text-sentiment/requirements.txt
--rw-r--r--   0        0        0      961 2023-06-29 16:53:05.242679 caikit-0.9.2/examples/text-sentiment/start_runtime.py
--rw-r--r--   0        0        0      816 2023-06-29 16:53:05.242679 caikit-0.9.2/examples/text-sentiment/text_sentiment/__init__.py
--rw-r--r--   0        0        0      615 2023-06-29 16:53:05.242679 caikit-0.9.2/examples/text-sentiment/text_sentiment/config.yml
--rw-r--r--   0        0        0      661 2023-06-29 16:53:05.242679 caikit-0.9.2/examples/text-sentiment/text_sentiment/data_model/__init__.py
--rw-r--r--   0        0        0     1422 2023-06-29 16:53:05.242679 caikit-0.9.2/examples/text-sentiment/text_sentiment/data_model/classification.py
--rw-r--r--   0        0        0      645 2023-06-29 16:53:05.242679 caikit-0.9.2/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
--rw-r--r--   0        0        0     3283 2023-06-29 16:53:05.242679 caikit-0.9.2/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py
--rw-r--r--   0        0        0     2058 2023-06-29 16:53:12.858712 caikit-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     2952 2023-06-29 16:53:05.242679 caikit-0.9.2/releases.md
--rwxr-xr-x   0        0        0      639 2023-06-29 16:53:05.242679 caikit-0.9.2/scripts/check_deps.sh
--rw-r--r--   0        0        0    13757 2023-06-29 16:53:05.242679 caikit-0.9.2/scripts/dsconverter.py
--rwxr-xr-x   0        0        0      720 2023-06-29 16:53:05.242679 caikit-0.9.2/scripts/fmt.sh
--rw-r--r--   0        0        0    25639 2023-06-29 16:53:05.242679 caikit-0.9.2/scripts/test_dsconverter.py
--rw-r--r--   0        0        0       33 2023-06-29 16:53:05.242679 caikit-0.9.2/setup_requirements.txt
--rw-r--r--   0        0        0     1006 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/__init__.py
--rw-r--r--   0        0        0     5240 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/base.py
--rw-r--r--   0        0        0        0 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/config/__init__.py
--rw-r--r--   0        0        0     5358 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/config/test_configs.py
--rw-r--r--   0        0        0     4508 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/core/__init__.py
--rw-r--r--   0        0        0     2853 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/core/augmentors/test_augmentor_base.py
--rw-r--r--   0        0        0     9114 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/core/augmentors/test_merged_augmentors.py
--rw-r--r--   0        0        0        0 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/core/data_model/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     5034 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/core/data_model/data_backends/test_dict_backend.py
--rw-r--r--   0        0        0     3306 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/core/data_model/streams/test_converter.py
--rw-r--r--   0        0        0     3314 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/core/data_model/streams/test_csv_column_formatter.py
--rw-r--r--   0        0        0    26951 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/core/data_model/streams/test_data_stream.py
--rw-r--r--   0        0        0     3498 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/core/data_model/streams/test_resolver.py
--rw-r--r--   0        0        0     2908 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/core/data_model/streams/test_validator.py
--rw-r--r--   0        0        0    16237 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/core/data_model/test_base.py
--rw-r--r--   0        0        0    32651 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/core/data_model/test_dataobject.py
--rw-r--r--   0        0        0     5083 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/core/data_model/test_enums.py
--rw-r--r--   0        0        0     2358 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/core/data_model/test_json_dict.py
--rw-r--r--   0        0        0     1104 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/core/data_model/test_producer.py
--rw-r--r--   0        0        0     4378 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/core/helpers.py
--rw-r--r--   0        0        0        0 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/core/module_backends/__init__.py
--rw-r--r--   0        0        0     2320 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/core/module_backends/test_backend_types.py
--rw-r--r--   0        0        0     6888 2023-06-29 16:53:05.242679 caikit-0.9.2/tests/core/module_backends/test_module_backend_config.py
--rw-r--r--   0        0        0        0 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/core/modules/__init__.py
--rw-r--r--   0        0        0    13033 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/core/modules/test_module.py
--rw-r--r--   0        0        0     6274 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/core/modules/test_module_metadata.py
--rw-r--r--   0        0        0      577 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/core/signature_parsing/__init__.py
--rw-r--r--   0        0        0     4872 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/core/signature_parsing/test_docstrings.py
--rw-r--r--   0        0        0     8595 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/core/signature_parsing/test_parsers.py
--rw-r--r--   0        0        0      521 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/core/test_imports.py
--rw-r--r--   0        0        0    21743 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/core/test_model_manager.py
--rw-r--r--   0        0        0     1038 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/core/test_no_write_permissions.py
--rw-r--r--   0        0        0     7497 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/core/test_task.py
--rw-r--r--   0        0        0        0 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/core/toolkit/__init__.py
--rw-r--r--   0        0        0     7967 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/core/toolkit/test_compatibility.py
--rw-r--r--   0        0        0    18396 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/core/toolkit/test_error_handler.py
--rw-r--r--   0        0        0     2372 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/core/toolkit/test_factory.py
--rw-r--r--   0        0        0     4997 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/core/toolkit/test_fileio.py
--rw-r--r--   0        0        0    25851 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/core/toolkit/test_quality_evaluation.py
--rw-r--r--   0        0        0     2634 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/core/toolkit/test_serializers.py
--rw-r--r--   0        0        0     3956 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/core/toolkit/test_sync_to_async.py
--rw-r--r--   0        0        0     7824 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/core/toolkit/test_wip_decorator.py
--rw-r--r--   0        0        0     6782 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/data_model_helpers.py
--rw-r--r--   0        0        0        0 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/examples/__init__.py
--rw-r--r--   0        0        0     2537 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/examples/shared.py
--rw-r--r--   0        0        0     2417 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/examples/test_examples.py
--rw-r--r--   0        0        0       39 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/__init__.py
--rw-r--r--   0        0        0      591 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/config/config.yml
--rw-r--r--   0        0        0       27 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/data_stream_inputs/bad_file.json
--rw-r--r--   0        0        0      154 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/data_stream_inputs/control_chars.jsonl
--rw-r--r--   0        0        0      106 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/data_stream_inputs/sample.csv
--rw-r--r--   0        0        0       66 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/data_stream_inputs/sample.json
--rw-r--r--   0        0        0      233 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/data_stream_inputs/sample.jsonl
--rw-r--r--   0        0        0     1322 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/data_stream_inputs/sample.txt
--rw-r--r--   0        0        0       11 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
--rw-r--r--   0        0        0       11 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
--rw-r--r--   0        0        0       11 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
--rw-r--r--   0        0        0       27 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
--rw-r--r--   0        0        0       27 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
--rw-r--r--   0        0        0       63 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
--rw-r--r--   0        0        0      147 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
--rw-r--r--   0        0        0      218 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
--rw-r--r--   0        0        0       87 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
--rw-r--r--   0        0        0       52 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
--rw-r--r--   0        0        0       56 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
--rw-r--r--   0        0        0       55 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
--rw-r--r--   0        0        0      125 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/data_stream_inputs/sample_w_header.csv
--rw-r--r--   0        0        0      222 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/dummy_dataset.json
--rw-r--r--   0        0        0     1017 2023-06-29 16:53:05.246679 caikit-0.9.2/tests/fixtures/dummy_module.zip
--rw-r--r--   0        0        0      675 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/dummy_module/config.yml
--rw-r--r--   0        0        0      299 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/dummy_module/data.json
--rw-r--r--   0        0        0       14 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/dummy_module/data.pkl
--rw-r--r--   0        0        0      191 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/dummy_module_backend/config.yml
--rw-r--r--   0        0        0      179 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/dummy_module_foo/config.yml
--rw-r--r--   0        0        0      508 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/dummy_module_no_id/config.yml
--rw-r--r--   0        0        0      508 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/dummy_module_no_nesting.zip
--rw-r--r--   0        0        0      570 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/dummy_module_singleton/config.yml
--rw-r--r--   0        0        0      299 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/dummy_module_singleton/data.json
--rw-r--r--   0        0        0       14 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/dummy_module_singleton/data.pkl
--rw-r--r--   0        0        0      230 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/dummy_resource/config.yml
--rw-r--r--   0        0        0      326 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/dummy_streaming_module/config.yml
--rw-r--r--   0        0        0     3034 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      918 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/invalid.zip
--rw-r--r--   0        0        0     2551 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/linux.txt
--rw-r--r--   0        0        0       10 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/models/bad_archive.zip
--rw-r--r--   0        0        0      349 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/models/bad_model.zip
--rw-r--r--   0        0        0      360 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/models/bar/config.yml
--rw-r--r--   0        0        0      364 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/models/foo/config.yml
--rw-r--r--   0        0        0      396 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/models/foo_archive.zip
--rw-r--r--   0        0        0       24 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      294 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/sample_lib/__init__.py
--rw-r--r--   0        0        0      296 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/sample_lib/config.yml
--rw-r--r--   0        0        0      176 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/sample_lib/data_model/__init__.py
--rw-r--r--   0        0        0     1474 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/sample_lib/data_model/sample.py
--rw-r--r--   0        0        0      156 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/sample_lib/modules/__init__.py
--rw-r--r--   0        0        0       89 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/sample_lib/modules/other_task/__init__.py
--rw-r--r--   0        0        0     1946 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/sample_lib/modules/other_task/other_implementation.py
--rw-r--r--   0        0        0      296 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/sample_lib/modules/sample_task/__init__.py
--rw-r--r--   0        0        0     1720 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/sample_lib/modules/sample_task/composite_module.py
--rw-r--r--   0        0        0      902 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/sample_lib/modules/sample_task/inner_module.py
--rw-r--r--   0        0        0     2463 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py
--rw-r--r--   0        0        0     3576 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py
--rw-r--r--   0        0        0     2720 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py
--rw-r--r--   0        0        0     1514 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/sample_lib/modules/sample_task/streaming_module.py
--rw-r--r--   0        0        0      364 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/fixtures/sample_module/config.yml
--rw-r--r--   0        0        0      577 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/interfaces/__init__.py
--rw-r--r--   0        0        0      577 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/interfaces/nlp/__init__.py
--rw-r--r--   0        0        0     2859 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/interfaces/nlp/test_nlp_tasks.py
--rw-r--r--   0        0        0        0 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/runtime/__init__.py
--rw-r--r--   0        0        0     6754 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/runtime/conftest.py
--rw-r--r--   0        0        0      756 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/runtime/generated/__init__.py
--rw-r--r--   0        0        0      577 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     3845 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/runtime/metrics/test_rpc_meter.py
--rw-r--r--   0        0        0      577 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    14101 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/runtime/model_management/test_batcher.py
--rw-r--r--   0        0        0    10266 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/runtime/model_management/test_model_loader.py
--rw-r--r--   0        0        0    17911 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/runtime/model_management/test_model_manager.py
--rw-r--r--   0        0        0     5303 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/runtime/model_management/test_model_sizer.py
--rw-r--r--   0        0        0     2401 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/runtime/model_management/test_training_manager.py
--rw-r--r--   0        0        0        0 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     4035 2023-06-29 16:53:05.250680 caikit-0.9.2/tests/runtime/service_generation/test_create_service.py
--rw-r--r--   0        0        0    17954 2023-06-29 16:53:05.254680 caikit-0.9.2/tests/runtime/service_generation/test_data_stream_source.py
--rw-r--r--   0        0        0     3796 2023-06-29 16:53:05.254680 caikit-0.9.2/tests/runtime/service_generation/test_protoable.py
--rw-r--r--   0        0        0     2345 2023-06-29 16:53:05.254680 caikit-0.9.2/tests/runtime/service_generation/test_rpcs.py
--rw-r--r--   0        0        0     1376 2023-06-29 16:53:05.254680 caikit-0.9.2/tests/runtime/service_generation/test_type_helpers.py
--rw-r--r--   0        0        0      577 2023-06-29 16:53:05.254680 caikit-0.9.2/tests/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     8875 2023-06-29 16:53:05.254680 caikit-0.9.2/tests/runtime/servicers/test_global_predict_servicer_impl.py
--rw-r--r--   0        0        0    16259 2023-06-29 16:53:05.254680 caikit-0.9.2/tests/runtime/servicers/test_global_train_servicer_impl.py
--rw-r--r--   0        0        0     4088 2023-06-29 16:53:05.254680 caikit-0.9.2/tests/runtime/servicers/test_model_runtime_servicer_impl.py
--rw-r--r--   0        0        0     7776 2023-06-29 16:53:05.254680 caikit-0.9.2/tests/runtime/servicers/test_model_train_servicer_impl.py
--rw-r--r--   0        0        0     4204 2023-06-29 16:53:05.254680 caikit-0.9.2/tests/runtime/servicers/test_training_management_servicer.py
--rw-r--r--   0        0        0    38335 2023-06-29 16:53:05.254680 caikit-0.9.2/tests/runtime/test_grpc_server.py
--rw-r--r--   0        0        0     5072 2023-06-29 16:53:05.254680 caikit-0.9.2/tests/runtime/test_service_factory.py
--rw-r--r--   0        0        0      577 2023-06-29 16:53:05.254680 caikit-0.9.2/tests/runtime/utils/__init__.py
--rw-r--r--   0        0        0     4899 2023-06-29 16:53:05.254680 caikit-0.9.2/tests/runtime/utils/test_import_util.py
--rw-r--r--   0        0        0    17329 2023-06-29 16:53:05.254680 caikit-0.9.2/tests/runtime/utils/test_servicer_util.py
--rw-r--r--   0        0        0      577 2023-06-29 16:53:05.254680 caikit-0.9.2/tests/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     2758 2023-06-29 16:53:05.254680 caikit-0.9.2/tests/runtime/work_management/test_abortable_action.py
--rw-r--r--   0        0        0     1868 2023-06-29 16:53:05.254680 caikit-0.9.2/tests/runtime/work_management/test_call_aborter.py
--rw-r--r--   0        0        0     3819 2023-06-29 16:53:05.254680 caikit-0.9.2/tests/runtime/work_management/test_destroyable_thread.py
--rw-r--r--   0        0        0     2209 2023-06-29 16:53:05.254680 caikit-0.9.2/tox.ini
--rw-r--r--   0        0        0     8606 1970-01-01 00:00:00.000000 caikit-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-07-06 16:52:07.809360 caikit-0.9.3/.coveragerc
+-rw-r--r--   0        0        0      676 2023-07-06 16:52:07.809360 caikit-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-07-06 16:52:07.809360 caikit-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-07-06 16:52:07.809360 caikit-0.9.3/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0      106 2023-07-06 16:52:07.809360 caikit-0.9.3/.github/dependabot.yml
+-rw-r--r--   0        0        0     1698 2023-07-06 16:52:07.809360 caikit-0.9.3/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1328 2023-07-06 16:52:07.809360 caikit-0.9.3/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1117 2023-07-06 16:52:07.809360 caikit-0.9.3/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      260 2023-07-06 16:52:07.809360 caikit-0.9.3/.gitignore
+-rw-r--r--   0        0        0      324 2023-07-06 16:52:07.809360 caikit-0.9.3/.isort.cfg
+-rw-r--r--   0        0        0      370 2023-07-06 16:52:07.809360 caikit-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      122 2023-07-06 16:52:07.809360 caikit-0.9.3/.prettierignore
+-rw-r--r--   0        0        0       12 2023-07-06 16:52:07.809360 caikit-0.9.3/.prettierrc.yaml
+-rw-r--r--   0        0        0    21434 2023-07-06 16:52:07.809360 caikit-0.9.3/.pylintrc
+-rw-r--r--   0        0        0      599 2023-07-06 16:52:07.809360 caikit-0.9.3/.readthedocs.yaml
+-rw-r--r--   0        0        0       78 2023-07-06 16:52:07.809360 caikit-0.9.3/.whitesource
+-rw-r--r--   0        0        0      368 2023-07-06 16:52:07.809360 caikit-0.9.3/CODEOWNERS
+-rw-r--r--   0        0        0     7164 2023-07-06 16:52:07.809360 caikit-0.9.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-07-06 16:52:07.809360 caikit-0.9.3/LICENSE
+-rw-r--r--   0        0        0     6317 2023-07-06 16:52:07.809360 caikit-0.9.3/README.md
+-rw-r--r--   0        0        0      152 2023-07-06 16:52:07.809360 caikit-0.9.3/SECURITY.md
+-rw-r--r--   0        0        0    44878 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit-overview.png
+-rw-r--r--   0        0        0      427 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/__init__.py
+-rw-r--r--   0        0        0      727 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/config/__init__.py
+-rw-r--r--   0        0        0     6035 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/config/config.py
+-rw-r--r--   0        0        0     6388 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/config/config.yml
+-rw-r--r--   0        0        0     1642 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/__init__.py
+-rw-r--r--   0        0        0      812 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/augmentors/__init__.py
+-rw-r--r--   0        0        0     3509 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/augmentors/base.py
+-rw-r--r--   0        0        0     2817 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/augmentors/merged_augmentor.py
+-rw-r--r--   0        0        0      355 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/augmentors/schemes/__init__.py
+-rw-r--r--   0        0        0     2029 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/augmentors/schemes/always_selection_scheme.py
+-rw-r--r--   0        0        0     3141 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/augmentors/schemes/base.py
+-rw-r--r--   0        0        0     3243 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
+-rw-r--r--   0        0        0     2875 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/augmentors/schemes/random_single_selection_scheme.py
+-rw-r--r--   0        0        0     1027 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/data_model/__init__.py
+-rw-r--r--   0        0        0    40051 2023-07-06 16:52:07.809360 caikit-0.9.3/caikit/core/data_model/base.py
+-rw-r--r--   0        0        0      750 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     2402 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/data_backends/base.py
+-rw-r--r--   0        0        0     4983 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/data_backends/dict_backend.py
+-rw-r--r--   0        0        0    17602 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/dataobject.py
+-rw-r--r--   0        0        0     4988 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/enums.py
+-rw-r--r--   0        0        0     5127 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/json_dict.py
+-rw-r--r--   0        0        0     1564 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/producer.py
+-rw-r--r--   0        0        0     3920 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/protobufs/__init__.py
+-rw-r--r--   0        0        0      577 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/streams/__init__.py
+-rw-r--r--   0        0        0     5446 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/streams/converter.py
+-rw-r--r--   0        0        0     4776 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/streams/csv_column_formatter.py
+-rw-r--r--   0        0        0    39907 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/streams/data_stream.py
+-rw-r--r--   0        0        0     3580 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/streams/resolver.py
+-rw-r--r--   0        0        0     5217 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/data_model/streams/validator.py
+-rw-r--r--   0        0        0    21179 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/model_manager.py
+-rw-r--r--   0        0        0      684 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     2824 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/module_backends/backend_types.py
+-rw-r--r--   0        0        0     4717 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/module_backends/base.py
+-rw-r--r--   0        0        0     2880 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/module_backends/local_backend.py
+-rw-r--r--   0        0        0     5982 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/module_backends/module_backend_config.py
+-rw-r--r--   0        0        0      742 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/modules/__init__.py
+-rw-r--r--   0        0        0    30052 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/modules/base.py
+-rw-r--r--   0        0        0     6145 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/modules/config.py
+-rw-r--r--   0        0        0    11011 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/modules/decorator.py
+-rw-r--r--   0        0        0     4141 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/modules/loader.py
+-rw-r--r--   0        0        0     6013 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/modules/meta.py
+-rw-r--r--   0        0        0    12931 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/modules/saver.py
+-rw-r--r--   0        0        0     3885 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/registries.py
+-rw-r--r--   0        0        0      654 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/signature_parsing/__init__.py
+-rw-r--r--   0        0        0    10666 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/signature_parsing/docstrings.py
+-rw-r--r--   0        0        0     4688 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/signature_parsing/module_signature.py
+-rw-r--r--   0        0        0     8221 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/signature_parsing/parsers.py
+-rw-r--r--   0        0        0    10542 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/task.py
+-rw-r--r--   0        0        0      982 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     4704 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/compatibility.py
+-rw-r--r--   0        0        0      637 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/errors/__init__.py
+-rw-r--r--   0        0        0    21349 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/errors/error_handler.py
+-rw-r--r--   0        0        0     1400 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/errors/validation_error.py
+-rw-r--r--   0        0        0     3240 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/factory.py
+-rw-r--r--   0        0        0     4914 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/fileio.py
+-rw-r--r--   0        0        0     1648 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/logging.py
+-rw-r--r--   0        0        0    31633 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/quality_evaluation.py
+-rw-r--r--   0        0        0     3356 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/serializers.py
+-rw-r--r--   0        0        0     2148 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/sync_to_async.py
+-rw-r--r--   0        0        0     5965 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/core/toolkit/wip_decorator.py
+-rw-r--r--   0        0        0     1056 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/interfaces/__init__.py
+-rw-r--r--   0        0        0      748 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/interfaces/common/__init__.py
+-rw-r--r--   0        0        0     1211 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/interfaces/common/data_model/__init__.py
+-rw-r--r--   0        0        0     1169 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/interfaces/common/data_model/producer.py
+-rw-r--r--   0        0        0      618 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/interfaces/nlp/__init__.py
+-rw-r--r--   0        0        0      809 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/interfaces/nlp/data_model/__init__.py
+-rw-r--r--   0        0        0      740 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/interfaces/nlp/data_model/package.py
+-rw-r--r--   0        0        0     2254 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/interfaces/nlp/data_model/text_generation.py
+-rw-r--r--   0        0        0     1383 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/interfaces/nlp/tasks.py
+-rw-r--r--   0        0        0      611 2023-07-06 16:52:07.813361 caikit-0.9.3/caikit/interfaces/runtime/__init__.py
+-rw-r--r--   0        0        0      763 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/interfaces/runtime/data_model/__init__.py
+-rw-r--r--   0        0        0     1886 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/interfaces/runtime/data_model/training_management.py
+-rw-r--r--   0        0        0      577 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/__init__.py
+-rw-r--r--   0        0        0     1662 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/dump_services.py
+-rw-r--r--   0        0        0    14262 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/grpc_server.py
+-rw-r--r--   0        0        0      577 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/interceptors/__init__.py
+-rw-r--r--   0        0        0    15627 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
+-rw-r--r--   0        0        0      577 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     4645 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/metrics/rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    17083 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/model_management/batcher.py
+-rw-r--r--   0        0        0     2606 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/model_management/loaded_model.py
+-rw-r--r--   0        0        0     5802 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/model_management/model_loader.py
+-rw-r--r--   0        0        0    12089 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/model_management/model_manager.py
+-rw-r--r--   0        0        0     4310 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/model_management/model_sizer.py
+-rw-r--r--   0        0        0     1642 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/model_management/training_manager.py
+-rw-r--r--   0        0        0      367 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/README.md
+-rw-r--r--   0        0        0      698 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/__init__.py
+-rw-r--r--   0        0        0    11375 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/model_mesh_pb2.py
+-rw-r--r--   0        0        0    12846 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
+-rw-r--r--   0        0        0    10107 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/model_runtime_pb2.py
+-rw-r--r--   0        0        0    10556 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     5535 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/process_pb2.py
+-rw-r--r--   0        0        0     2569 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/process_pb2_grpc.py
+-rw-r--r--   0        0        0     8844 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/protos/model-mesh.proto
+-rw-r--r--   0        0        0     6795 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/protos/model-runtime.proto
+-rw-r--r--   0        0        0     2479 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/protobufs/protos/process.proto
+-rw-r--r--   0        0        0     9572 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/service_factory.py
+-rw-r--r--   0        0        0      109 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     1779 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/service_generation/compatibility_checker.py
+-rw-r--r--   0        0        0     4229 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/service_generation/create_service.py
+-rw-r--r--   0        0        0    12070 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/service_generation/data_stream_source.py
+-rw-r--r--   0        0        0     6146 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/service_generation/protoable.py
+-rw-r--r--   0        0        0    12152 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/service_generation/rpcs.py
+-rw-r--r--   0        0        0     2216 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/service_generation/type_helpers.py
+-rw-r--r--   0        0        0      577 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0    12641 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/servicers/global_predict_servicer.py
+-rw-r--r--   0        0        0    12451 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/servicers/global_train_servicer.py
+-rw-r--r--   0        0        0    10637 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/servicers/model_runtime_servicer.py
+-rw-r--r--   0        0        0     5440 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/servicers/model_train_servicer.py
+-rw-r--r--   0        0        0     1667 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/servicers/training_management_servicer.py
+-rw-r--r--   0        0        0      577 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/types/__init__.py
+-rw-r--r--   0        0        0      957 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/types/aborted_exception.py
+-rw-r--r--   0        0        0     1558 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/types/caikit_runtime_exception.py
+-rw-r--r--   0        0        0      960 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/types/thread_destroyed_exception.py
+-rw-r--r--   0        0        0      577 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     6790 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/utils/import_util.py
+-rw-r--r--   0        0        0    13825 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/utils/servicer_util.py
+-rw-r--r--   0        0        0      577 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     3732 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/work_management/abortable_action.py
+-rw-r--r--   0        0        0     2969 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/work_management/call_aborter.py
+-rw-r--r--   0        0        0     7596 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/work_management/destroyable_thread.py
+-rw-r--r--   0        0        0    12228 2023-07-06 16:52:07.817361 caikit-0.9.3/caikit/runtime/work_management/train_executors.py
+-rw-r--r--   0        0        0      169 2023-07-06 16:52:07.817361 caikit-0.9.3/code-of-conduct.md
+-rw-r--r--   0        0        0      639 2023-07-06 16:52:07.817361 caikit-0.9.3/docs/Makefile
+-rw-r--r--   0        0        0     6860 2023-07-06 16:52:07.817361 caikit-0.9.3/docs/adrs/001-module.md
+-rw-r--r--   0        0        0     1610 2023-07-06 16:52:07.817361 caikit-0.9.3/docs/adrs/010-data-model-definition.md
+-rw-r--r--   0        0        0     2352 2023-07-06 16:52:07.817361 caikit-0.9.3/docs/adrs/015-runtime-service-generation.md
+-rw-r--r--   0        0        0     2581 2023-07-06 16:52:07.817361 caikit-0.9.3/docs/adrs/018-shared-backends.md
+-rw-r--r--   0        0        0     1223 2023-07-06 16:52:07.817361 caikit-0.9.3/docs/adrs/019-loader-stack.md
+-rw-r--r--   0        0        0      404 2023-07-06 16:52:07.821361 caikit-0.9.3/docs/adrs/README.md
+-rw-r--r--   0        0        0     2423 2023-07-06 16:52:07.821361 caikit-0.9.3/docs/architecture_club/04-25-23.md
+-rw-r--r--   0        0        0      342 2023-07-06 16:52:07.821361 caikit-0.9.3/docs/architecture_club/README.md
+-rw-r--r--   0        0        0      805 2023-07-06 16:52:07.821361 caikit-0.9.3/docs/make.bat
+-rw-r--r--   0        0        0     3053 2023-07-06 16:52:07.821361 caikit-0.9.3/docs/source/conf.py
+-rw-r--r--   0        0        0      225 2023-07-06 16:52:07.821361 caikit-0.9.3/docs/source/index.rst
+-rw-r--r--   0        0        0      837 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/start_runtime_with_sample_lib.py
+-rw-r--r--   0        0        0     6095 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/README.md
+-rw-r--r--   0        0        0     1475 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/client.py
+-rw-r--r--   0        0        0      673 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/models/text_sentiment/config.yml
+-rw-r--r--   0        0        0       77 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/requirements.txt
+-rw-r--r--   0        0        0      961 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/start_runtime.py
+-rw-r--r--   0        0        0      816 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/text_sentiment/__init__.py
+-rw-r--r--   0        0        0      615 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/text_sentiment/config.yml
+-rw-r--r--   0        0        0      661 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/text_sentiment/data_model/__init__.py
+-rw-r--r--   0        0        0     1422 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/text_sentiment/data_model/classification.py
+-rw-r--r--   0        0        0      645 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/text_sentiment/runtime_model/__init__.py
+-rw-r--r--   0        0        0     3283 2023-07-06 16:52:07.821361 caikit-0.9.3/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py
+-rw-r--r--   0        0        0     2058 2023-07-06 16:52:11.645575 caikit-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     2952 2023-07-06 16:52:07.821361 caikit-0.9.3/releases.md
+-rwxr-xr-x   0        0        0      639 2023-07-06 16:52:07.821361 caikit-0.9.3/scripts/check_deps.sh
+-rw-r--r--   0        0        0    13757 2023-07-06 16:52:07.821361 caikit-0.9.3/scripts/dsconverter.py
+-rwxr-xr-x   0        0        0      720 2023-07-06 16:52:07.821361 caikit-0.9.3/scripts/fmt.sh
+-rw-r--r--   0        0        0    25639 2023-07-06 16:52:07.821361 caikit-0.9.3/scripts/test_dsconverter.py
+-rw-r--r--   0        0        0       33 2023-07-06 16:52:07.821361 caikit-0.9.3/setup_requirements.txt
+-rw-r--r--   0        0        0     1006 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/__init__.py
+-rw-r--r--   0        0        0     5240 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/base.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/config/__init__.py
+-rw-r--r--   0        0        0     5358 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/config/test_configs.py
+-rw-r--r--   0        0        0     4508 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/__init__.py
+-rw-r--r--   0        0        0     2853 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/augmentors/test_augmentor_base.py
+-rw-r--r--   0        0        0     9114 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/augmentors/test_merged_augmentors.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     5034 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/data_backends/test_dict_backend.py
+-rw-r--r--   0        0        0     3306 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/streams/test_converter.py
+-rw-r--r--   0        0        0     3314 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/streams/test_csv_column_formatter.py
+-rw-r--r--   0        0        0    26951 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/streams/test_data_stream.py
+-rw-r--r--   0        0        0     3498 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/streams/test_resolver.py
+-rw-r--r--   0        0        0     2908 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/streams/test_validator.py
+-rw-r--r--   0        0        0    16237 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/test_base.py
+-rw-r--r--   0        0        0    32651 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/test_dataobject.py
+-rw-r--r--   0        0        0     5083 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/test_enums.py
+-rw-r--r--   0        0        0     2358 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/test_json_dict.py
+-rw-r--r--   0        0        0     1104 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/data_model/test_producer.py
+-rw-r--r--   0        0        0     4378 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/helpers.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     2320 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/module_backends/test_backend_types.py
+-rw-r--r--   0        0        0     6888 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/module_backends/test_module_backend_config.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/modules/__init__.py
+-rw-r--r--   0        0        0    13033 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/modules/test_module.py
+-rw-r--r--   0        0        0     6274 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/modules/test_module_metadata.py
+-rw-r--r--   0        0        0      577 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/signature_parsing/__init__.py
+-rw-r--r--   0        0        0     4872 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/signature_parsing/test_docstrings.py
+-rw-r--r--   0        0        0     8595 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/signature_parsing/test_parsers.py
+-rw-r--r--   0        0        0      521 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/test_imports.py
+-rw-r--r--   0        0        0    21743 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/test_model_manager.py
+-rw-r--r--   0        0        0     1038 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/test_no_write_permissions.py
+-rw-r--r--   0        0        0     7497 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/test_task.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     7967 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/toolkit/test_compatibility.py
+-rw-r--r--   0        0        0    18396 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/toolkit/test_error_handler.py
+-rw-r--r--   0        0        0     2372 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/toolkit/test_factory.py
+-rw-r--r--   0        0        0     4997 2023-07-06 16:52:07.821361 caikit-0.9.3/tests/core/toolkit/test_fileio.py
+-rw-r--r--   0        0        0    25851 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/core/toolkit/test_quality_evaluation.py
+-rw-r--r--   0        0        0     2634 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/core/toolkit/test_serializers.py
+-rw-r--r--   0        0        0     3956 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/core/toolkit/test_sync_to_async.py
+-rw-r--r--   0        0        0     7824 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/core/toolkit/test_wip_decorator.py
+-rw-r--r--   0        0        0     6782 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/data_model_helpers.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/examples/__init__.py
+-rw-r--r--   0        0        0     2537 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/examples/shared.py
+-rw-r--r--   0        0        0     2417 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/examples/test_examples.py
+-rw-r--r--   0        0        0       39 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0      591 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/config/config.yml
+-rw-r--r--   0        0        0       27 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/bad_file.json
+-rw-r--r--   0        0        0      154 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/control_chars.jsonl
+-rw-r--r--   0        0        0      106 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample.csv
+-rw-r--r--   0        0        0       66 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample.json
+-rw-r--r--   0        0        0      233 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample.jsonl
+-rw-r--r--   0        0        0     1322 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample.txt
+-rw-r--r--   0        0        0       11 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
+-rw-r--r--   0        0        0       11 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
+-rw-r--r--   0        0        0       11 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
+-rw-r--r--   0        0        0       27 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
+-rw-r--r--   0        0        0       27 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
+-rw-r--r--   0        0        0       63 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
+-rw-r--r--   0        0        0      147 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
+-rw-r--r--   0        0        0      218 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
+-rw-r--r--   0        0        0       87 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
+-rw-r--r--   0        0        0       52 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
+-rw-r--r--   0        0        0       56 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
+-rw-r--r--   0        0        0       55 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
+-rw-r--r--   0        0        0      125 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/data_stream_inputs/sample_w_header.csv
+-rw-r--r--   0        0        0      222 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_dataset.json
+-rw-r--r--   0        0        0     1017 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module.zip
+-rw-r--r--   0        0        0      675 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module/config.yml
+-rw-r--r--   0        0        0      299 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module/data.json
+-rw-r--r--   0        0        0       14 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module/data.pkl
+-rw-r--r--   0        0        0      191 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module_backend/config.yml
+-rw-r--r--   0        0        0      179 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module_foo/config.yml
+-rw-r--r--   0        0        0      508 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module_no_id/config.yml
+-rw-r--r--   0        0        0      508 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module_no_nesting.zip
+-rw-r--r--   0        0        0      570 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module_singleton/config.yml
+-rw-r--r--   0        0        0      299 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module_singleton/data.json
+-rw-r--r--   0        0        0       14 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_module_singleton/data.pkl
+-rw-r--r--   0        0        0      230 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_resource/config.yml
+-rw-r--r--   0        0        0      326 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/dummy_streaming_module/config.yml
+-rw-r--r--   0        0        0     3034 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      918 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/invalid.zip
+-rw-r--r--   0        0        0     2551 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/linux.txt
+-rw-r--r--   0        0        0       10 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/models/bad_archive.zip
+-rw-r--r--   0        0        0      349 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/models/bad_model.zip
+-rw-r--r--   0        0        0      360 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/models/bar/config.yml
+-rw-r--r--   0        0        0      364 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/models/foo/config.yml
+-rw-r--r--   0        0        0      396 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/models/foo_archive.zip
+-rw-r--r--   0        0        0       24 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      294 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/__init__.py
+-rw-r--r--   0        0        0      296 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/config.yml
+-rw-r--r--   0        0        0      176 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/data_model/__init__.py
+-rw-r--r--   0        0        0     1474 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/data_model/sample.py
+-rw-r--r--   0        0        0      156 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/modules/__init__.py
+-rw-r--r--   0        0        0       89 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/modules/other_task/__init__.py
+-rw-r--r--   0        0        0     1946 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/modules/other_task/other_implementation.py
+-rw-r--r--   0        0        0      296 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/__init__.py
+-rw-r--r--   0        0        0     1720 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/composite_module.py
+-rw-r--r--   0        0        0      902 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/inner_module.py
+-rw-r--r--   0        0        0     2463 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py
+-rw-r--r--   0        0        0     3576 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py
+-rw-r--r--   0        0        0     2720 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0     1514 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/streaming_module.py
+-rw-r--r--   0        0        0      364 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/fixtures/sample_module/config.yml
+-rw-r--r--   0        0        0      577 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/interfaces/__init__.py
+-rw-r--r--   0        0        0     1658 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/interfaces/common/test_producer.py
+-rw-r--r--   0        0        0      577 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/interfaces/nlp/__init__.py
+-rw-r--r--   0        0        0     2859 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/interfaces/nlp/test_nlp_tasks.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/__init__.py
+-rw-r--r--   0        0        0     6754 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/conftest.py
+-rw-r--r--   0        0        0      756 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/generated/__init__.py
+-rw-r--r--   0        0        0      577 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     3845 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/metrics/test_rpc_meter.py
+-rw-r--r--   0        0        0      577 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    14101 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/model_management/test_batcher.py
+-rw-r--r--   0        0        0    10266 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/model_management/test_model_loader.py
+-rw-r--r--   0        0        0    17911 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/model_management/test_model_manager.py
+-rw-r--r--   0        0        0     5303 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/model_management/test_model_sizer.py
+-rw-r--r--   0        0        0     2401 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/model_management/test_training_manager.py
+-rw-r--r--   0        0        0        0 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     4035 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/service_generation/test_create_service.py
+-rw-r--r--   0        0        0    17954 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/service_generation/test_data_stream_source.py
+-rw-r--r--   0        0        0     3796 2023-07-06 16:52:07.825361 caikit-0.9.3/tests/runtime/service_generation/test_protoable.py
+-rw-r--r--   0        0        0     2345 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/service_generation/test_rpcs.py
+-rw-r--r--   0        0        0     1376 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/service_generation/test_type_helpers.py
+-rw-r--r--   0        0        0      577 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     8875 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/servicers/test_global_predict_servicer_impl.py
+-rw-r--r--   0        0        0    16401 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/servicers/test_global_train_servicer_impl.py
+-rw-r--r--   0        0        0     4088 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/servicers/test_model_runtime_servicer_impl.py
+-rw-r--r--   0        0        0     7776 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/servicers/test_model_train_servicer_impl.py
+-rw-r--r--   0        0        0     4204 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/servicers/test_training_management_servicer.py
+-rw-r--r--   0        0        0    38335 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/test_grpc_server.py
+-rw-r--r--   0        0        0     5072 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/test_service_factory.py
+-rw-r--r--   0        0        0      577 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     4899 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/utils/test_import_util.py
+-rw-r--r--   0        0        0    17329 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/utils/test_servicer_util.py
+-rw-r--r--   0        0        0      577 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     2758 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/work_management/test_abortable_action.py
+-rw-r--r--   0        0        0     1868 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/work_management/test_call_aborter.py
+-rw-r--r--   0        0        0     3819 2023-07-06 16:52:07.829362 caikit-0.9.3/tests/runtime/work_management/test_destroyable_thread.py
+-rw-r--r--   0        0        0     2209 2023-07-06 16:52:07.829362 caikit-0.9.3/tox.ini
+-rw-r--r--   0        0        0     8606 1970-01-01 00:00:00.000000 caikit-0.9.3/PKG-INFO
```

### Comparing `caikit-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-0.9.3/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/.github/workflows/build-library.yml` & `caikit-0.9.3/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/.github/workflows/lint-code.yml` & `caikit-0.9.3/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/.github/workflows/publish-library.yml` & `caikit-0.9.3/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/.pylintrc` & `caikit-0.9.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/.readthedocs.yaml` & `caikit-0.9.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/CONTRIBUTING.md` & `caikit-0.9.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/LICENSE` & `caikit-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/README.md` & `caikit-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit-overview.png` & `caikit-0.9.3/caikit-overview.png`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/config/__init__.py` & `caikit-0.9.3/caikit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/config/config.py` & `caikit-0.9.3/caikit/config/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/config/config.yml` & `caikit-0.9.3/caikit/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/__init__.py` & `caikit-0.9.3/caikit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/augmentors/__init__.py` & `caikit-0.9.3/caikit/core/augmentors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/augmentors/base.py` & `caikit-0.9.3/caikit/core/augmentors/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/augmentors/merged_augmentor.py` & `caikit-0.9.3/caikit/core/augmentors/merged_augmentor.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/augmentors/schemes/always_selection_scheme.py` & `caikit-0.9.3/caikit/core/augmentors/schemes/always_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/augmentors/schemes/base.py` & `caikit-0.9.3/caikit/core/augmentors/schemes/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/augmentors/schemes/random_multi_selection_scheme.py` & `caikit-0.9.3/caikit/core/augmentors/schemes/random_multi_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/augmentors/schemes/random_single_selection_scheme.py` & `caikit-0.9.3/caikit/core/augmentors/schemes/random_single_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/data_model/__init__.py` & `caikit-0.9.3/caikit/core/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/data_model/base.py` & `caikit-0.9.3/caikit/core/data_model/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/data_model/data_backends/__init__.py` & `caikit-0.9.3/caikit/core/data_model/data_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/data_model/data_backends/base.py` & `caikit-0.9.3/caikit/core/data_model/data_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/data_model/data_backends/dict_backend.py` & `caikit-0.9.3/caikit/core/data_model/data_backends/dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/data_model/dataobject.py` & `caikit-0.9.3/caikit/core/data_model/dataobject.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/data_model/enums.py` & `caikit-0.9.3/caikit/core/data_model/enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/data_model/json_dict.py` & `caikit-0.9.3/caikit/core/data_model/json_dict.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/data_model/producer.py` & `caikit-0.9.3/caikit/core/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/data_model/protobufs/__init__.py` & `caikit-0.9.3/caikit/core/data_model/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/data_model/streams/__init__.py` & `caikit-0.9.3/caikit/core/data_model/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/data_model/streams/converter.py` & `caikit-0.9.3/caikit/core/data_model/streams/converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/data_model/streams/csv_column_formatter.py` & `caikit-0.9.3/caikit/core/data_model/streams/csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/data_model/streams/data_stream.py` & `caikit-0.9.3/caikit/core/data_model/streams/data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/data_model/streams/resolver.py` & `caikit-0.9.3/caikit/core/data_model/streams/resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/data_model/streams/validator.py` & `caikit-0.9.3/caikit/core/data_model/streams/validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/model_manager.py` & `caikit-0.9.3/caikit/core/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/module_backends/__init__.py` & `caikit-0.9.3/caikit/core/module_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/module_backends/backend_types.py` & `caikit-0.9.3/caikit/core/module_backends/backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/module_backends/base.py` & `caikit-0.9.3/caikit/core/module_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/module_backends/local_backend.py` & `caikit-0.9.3/caikit/core/module_backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/module_backends/module_backend_config.py` & `caikit-0.9.3/caikit/core/module_backends/module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/modules/__init__.py` & `caikit-0.9.3/caikit/core/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/modules/base.py` & `caikit-0.9.3/caikit/core/modules/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/modules/config.py` & `caikit-0.9.3/caikit/core/modules/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/modules/decorator.py` & `caikit-0.9.3/caikit/core/modules/decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/modules/loader.py` & `caikit-0.9.3/caikit/core/modules/loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/modules/meta.py` & `caikit-0.9.3/caikit/core/modules/meta.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/modules/saver.py` & `caikit-0.9.3/caikit/core/modules/saver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/registries.py` & `caikit-0.9.3/caikit/core/registries.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/signature_parsing/__init__.py` & `caikit-0.9.3/caikit/core/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/signature_parsing/docstrings.py` & `caikit-0.9.3/caikit/core/signature_parsing/docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/signature_parsing/module_signature.py` & `caikit-0.9.3/caikit/core/signature_parsing/module_signature.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/signature_parsing/parsers.py` & `caikit-0.9.3/caikit/core/signature_parsing/parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/task.py` & `caikit-0.9.3/caikit/core/task.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/toolkit/__init__.py` & `caikit-0.9.3/caikit/core/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/toolkit/compatibility.py` & `caikit-0.9.3/caikit/core/toolkit/compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/toolkit/errors/__init__.py` & `caikit-0.9.3/caikit/core/toolkit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/toolkit/errors/error_handler.py` & `caikit-0.9.3/caikit/core/toolkit/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/toolkit/errors/validation_error.py` & `caikit-0.9.3/caikit/core/toolkit/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/toolkit/factory.py` & `caikit-0.9.3/caikit/core/toolkit/factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/toolkit/fileio.py` & `caikit-0.9.3/caikit/core/toolkit/fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/toolkit/logging.py` & `caikit-0.9.3/caikit/core/toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/toolkit/quality_evaluation.py` & `caikit-0.9.3/caikit/core/toolkit/quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/toolkit/serializers.py` & `caikit-0.9.3/caikit/core/toolkit/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/toolkit/sync_to_async.py` & `caikit-0.9.3/caikit/core/toolkit/sync_to_async.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/core/toolkit/wip_decorator.py` & `caikit-0.9.3/caikit/core/toolkit/wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/interfaces/__init__.py` & `caikit-0.9.3/caikit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/interfaces/common/__init__.py` & `caikit-0.9.3/caikit/interfaces/common/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/interfaces/common/data_model/__init__.py` & `caikit-0.9.3/caikit/interfaces/common/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/interfaces/common/data_model/producer.py` & `caikit-0.9.3/caikit/interfaces/common/data_model/producer.py`

 * *Files 21% similar despite different names*

```diff
@@ -34,17 +34,8 @@
 @dataobject(PACKAGE_COMMON)
 class ProducerPriority(DataObjectBase):
     """An ordered list of ProducerId structures in descending order of priority.
     This is used when handling conflicts between multiple producers of the same
     data structure.
     """
 
-    elements: List[ProducerId]
-
-    def __init__(self, producers):
-        """Construct a new ProducerPriority
-
-        Args:
-            producers (list(ProducerId))
-        """
-        error.type_check_all("<COR01353088E>", ProducerId, producers=producers)
-        self.producers = producers
+    producers: List[ProducerId]
```

### Comparing `caikit-0.9.2/caikit/interfaces/nlp/__init__.py` & `caikit-0.9.3/caikit/interfaces/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/interfaces/nlp/data_model/__init__.py` & `caikit-0.9.3/caikit/interfaces/nlp/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/interfaces/nlp/data_model/package.py` & `caikit-0.9.3/caikit/interfaces/nlp/data_model/package.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/interfaces/nlp/data_model/text_generation.py` & `caikit-0.9.3/caikit/interfaces/nlp/data_model/text_generation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/interfaces/nlp/tasks.py` & `caikit-0.9.3/caikit/interfaces/nlp/tasks.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/interfaces/runtime/__init__.py` & `caikit-0.9.3/caikit/interfaces/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/interfaces/runtime/data_model/__init__.py` & `caikit-0.9.3/caikit/interfaces/runtime/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/interfaces/runtime/data_model/training_management.py` & `caikit-0.9.3/caikit/interfaces/runtime/data_model/training_management.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/__init__.py` & `caikit-0.9.3/caikit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/dump_services.py` & `caikit-0.9.3/caikit/runtime/dump_services.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/grpc_server.py` & `caikit-0.9.3/caikit/runtime/grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/interceptors/__init__.py` & `caikit-0.9.3/caikit/runtime/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py` & `caikit-0.9.3/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/metrics/__init__.py` & `caikit-0.9.3/caikit/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/metrics/rpc_meter.py` & `caikit-0.9.3/caikit/runtime/metrics/rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/model_management/__init__.py` & `caikit-0.9.3/caikit/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/model_management/batcher.py` & `caikit-0.9.3/caikit/runtime/model_management/batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/model_management/loaded_model.py` & `caikit-0.9.3/caikit/runtime/model_management/loaded_model.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/model_management/model_loader.py` & `caikit-0.9.3/caikit/runtime/model_management/model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/model_management/model_manager.py` & `caikit-0.9.3/caikit/runtime/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/model_management/model_sizer.py` & `caikit-0.9.3/caikit/runtime/model_management/model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/model_management/training_manager.py` & `caikit-0.9.3/caikit/runtime/model_management/training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/protobufs/__init__.py` & `caikit-0.9.3/caikit/runtime/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/protobufs/model_mesh_pb2.py` & `caikit-0.9.3/caikit/runtime/protobufs/model_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/protobufs/model_mesh_pb2_grpc.py` & `caikit-0.9.3/caikit/runtime/protobufs/model_mesh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/protobufs/model_runtime_pb2.py` & `caikit-0.9.3/caikit/runtime/protobufs/model_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/protobufs/model_runtime_pb2_grpc.py` & `caikit-0.9.3/caikit/runtime/protobufs/model_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/protobufs/process_pb2.py` & `caikit-0.9.3/caikit/runtime/protobufs/process_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/protobufs/process_pb2_grpc.py` & `caikit-0.9.3/caikit/runtime/protobufs/process_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/protobufs/protos/model-mesh.proto` & `caikit-0.9.3/caikit/runtime/protobufs/protos/model-mesh.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/protobufs/protos/model-runtime.proto` & `caikit-0.9.3/caikit/runtime/protobufs/protos/model-runtime.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/protobufs/protos/process.proto` & `caikit-0.9.3/caikit/runtime/protobufs/protos/process.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/service_factory.py` & `caikit-0.9.3/caikit/runtime/service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/service_generation/compatibility_checker.py` & `caikit-0.9.3/caikit/runtime/service_generation/compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/service_generation/create_service.py` & `caikit-0.9.3/caikit/runtime/service_generation/create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/service_generation/data_stream_source.py` & `caikit-0.9.3/caikit/runtime/service_generation/data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/service_generation/protoable.py` & `caikit-0.9.3/caikit/runtime/service_generation/protoable.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/service_generation/rpcs.py` & `caikit-0.9.3/caikit/runtime/service_generation/rpcs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/service_generation/type_helpers.py` & `caikit-0.9.3/caikit/runtime/service_generation/type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/servicers/__init__.py` & `caikit-0.9.3/caikit/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/servicers/global_predict_servicer.py` & `caikit-0.9.3/caikit/runtime/servicers/global_predict_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/servicers/global_train_servicer.py` & `caikit-0.9.3/caikit/runtime/servicers/global_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/servicers/model_runtime_servicer.py` & `caikit-0.9.3/caikit/runtime/servicers/model_runtime_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/servicers/model_train_servicer.py` & `caikit-0.9.3/caikit/runtime/servicers/model_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/servicers/training_management_servicer.py` & `caikit-0.9.3/caikit/runtime/servicers/training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/types/__init__.py` & `caikit-0.9.3/caikit/runtime/types/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/types/aborted_exception.py` & `caikit-0.9.3/caikit/runtime/types/aborted_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/types/caikit_runtime_exception.py` & `caikit-0.9.3/caikit/runtime/types/caikit_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/types/thread_destroyed_exception.py` & `caikit-0.9.3/caikit/runtime/types/thread_destroyed_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/utils/__init__.py` & `caikit-0.9.3/caikit/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/utils/import_util.py` & `caikit-0.9.3/caikit/runtime/utils/import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/utils/servicer_util.py` & `caikit-0.9.3/caikit/runtime/utils/servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/work_management/__init__.py` & `caikit-0.9.3/caikit/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/work_management/abortable_action.py` & `caikit-0.9.3/caikit/runtime/work_management/abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/work_management/call_aborter.py` & `caikit-0.9.3/caikit/runtime/work_management/call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/work_management/destroyable_thread.py` & `caikit-0.9.3/caikit/runtime/work_management/destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/caikit/runtime/work_management/train_executors.py` & `caikit-0.9.3/caikit/runtime/work_management/train_executors.py`

 * *Files 6% similar despite different names*

```diff
@@ -195,31 +195,40 @@
             2. Due to the auto-generated classes with stream sources, "spawn"
                can result in missing classes since it performs a full re-import,
                but does not regenerate the service APIs
         """
 
         def __init__(self, *args, event=None, **kwargs):
             super().__init__(*args, **kwargs)
-            self.error = None
+            self._error = None
+            self._parent_conn, self._child_conn = multiprocessing.Pipe()
             self._completion_event = event
 
         def run(self, *args, **kwargs):
             try:
-                return super().run(*args, **kwargs)
+                super().run(*args, **kwargs)
+                self._child_conn.send(None)
 
             # Catch any errors thrown within a subprocess so that they can be
             # forwarded to the parent
             # pylint: disable=broad-exception-caught
             except Exception as err:
-                log.error("<RUN69863806E>", "Caught exception in training", repr(err))
-                self.error = err
-
+                err_str = repr(err)
+                log.error("<RUN69863806E>", "Caught exception in training", err_str)
+                self._child_conn.send(err_str)
             finally:
                 self._completion_event.set()
 
+        @property
+        def error(self):
+            # NOTE: below is relying on child only sending error back and no other message
+            if self._parent_conn.poll():
+                self._error = self._parent_conn.recv()
+            return self._error
+
     def __init__(self, cancel_event) -> None:
 
         self.complete_event = multiprocessing.Event()
         self.events = [cancel_event, self.complete_event]
 
         self._worker = None
         self.__cancel_event = cancel_event
@@ -297,20 +306,18 @@
         # this should happen instantly in either of cases:
         # training is complete or cancellation is requested
         cancellation_thread.join()
 
         # If an error occurred, reraise it here
         # TODO: Make sure the stack trace is preserved
         if self._worker.error is not None:
-            if isinstance(self._worker.error, CaikitRuntimeException):
-                raise self._worker.error
             raise CaikitRuntimeException(
                 StatusCode.INTERNAL,
-                "Error caught in training subprocess",
-            ) from self._worker.error
+                f"Exception raised during training: {self._worker.error}",
+            )
 
         # If process exited with a non-zero exit code
         if self._worker.exitcode and self._worker.exitcode != os.EX_OK:
             if self._worker.exitcode == OOM_EXIT_CODE:
                 exception = CaikitRuntimeException(
                     StatusCode.RESOURCE_EXHAUSTED,
                     "Training process died with OOM error!",
```

### Comparing `caikit-0.9.2/docs/Makefile` & `caikit-0.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/docs/adrs/001-module.md` & `caikit-0.9.3/docs/adrs/001-module.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/docs/adrs/010-data-model-definition.md` & `caikit-0.9.3/docs/adrs/010-data-model-definition.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/docs/adrs/015-runtime-service-generation.md` & `caikit-0.9.3/docs/adrs/015-runtime-service-generation.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/docs/adrs/018-shared-backends.md` & `caikit-0.9.3/docs/adrs/018-shared-backends.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/docs/adrs/019-loader-stack.md` & `caikit-0.9.3/docs/adrs/019-loader-stack.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/docs/architecture_club/04-25-23.md` & `caikit-0.9.3/docs/architecture_club/04-25-23.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/docs/make.bat` & `caikit-0.9.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/docs/source/conf.py` & `caikit-0.9.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/examples/start_runtime_with_sample_lib.py` & `caikit-0.9.3/examples/start_runtime_with_sample_lib.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/examples/text-sentiment/README.md` & `caikit-0.9.3/examples/text-sentiment/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/examples/text-sentiment/client.py` & `caikit-0.9.3/examples/text-sentiment/client.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/examples/text-sentiment/models/text_sentiment/config.yml` & `caikit-0.9.3/examples/text-sentiment/models/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/examples/text-sentiment/start_runtime.py` & `caikit-0.9.3/examples/text-sentiment/start_runtime.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/examples/text-sentiment/text_sentiment/__init__.py` & `caikit-0.9.3/examples/text-sentiment/text_sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/examples/text-sentiment/text_sentiment/config.yml` & `caikit-0.9.3/examples/text-sentiment/text_sentiment/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/examples/text-sentiment/text_sentiment/data_model/__init__.py` & `caikit-0.9.3/examples/text-sentiment/text_sentiment/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/examples/text-sentiment/text_sentiment/data_model/classification.py` & `caikit-0.9.3/examples/text-sentiment/text_sentiment/data_model/classification.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/examples/text-sentiment/text_sentiment/runtime_model/__init__.py` & `caikit-0.9.3/examples/text-sentiment/text_sentiment/runtime_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py` & `caikit-0.9.3/examples/text-sentiment/text_sentiment/runtime_model/hf_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/pyproject.toml` & `caikit-0.9.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit"
 # Not the actual current version: overwritten by CI
-version = "0.9.2"
+version = "0.9.3"
 description = "AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = "~=3.8"
 classifiers=[
     "License :: OSI Approved :: Apache Software License"
 ]
@@ -17,15 +17,15 @@
 dependencies = [
     "alchemy-config>=1.1.1,<2.0.0",
     "alchemy-logging>=1.0.4,<2.0.0",
     "anytree>=2.7.0,<3.0",
     "docstring-parser>=0.14.1,<0.16.0",
     "grpcio>=1.35.0,<2.0,!=1.55.0",
     "ijson>=3.1.4,<3.3.0",
-    "munch>=2.5.0,<4.0",
+    "munch>=2.5.0,<5.0",
     "numpy>=1.20,<2",
     "protobuf>=3.19.0,<5",
     "py-to-proto>=0.4.0,<0.5.0,!=0.2.1",
     "PyYAML>=6.0,<7.0",
     "semver>=2.13.0,<4.0",
     "six>=1.16.0,<2.0.0",
     "tqdm>=4.59.0,<5.0.0",
```

### Comparing `caikit-0.9.2/releases.md` & `caikit-0.9.3/releases.md`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/scripts/check_deps.sh` & `caikit-0.9.3/scripts/check_deps.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/scripts/dsconverter.py` & `caikit-0.9.3/scripts/dsconverter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/scripts/fmt.sh` & `caikit-0.9.3/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/scripts/test_dsconverter.py` & `caikit-0.9.3/scripts/test_dsconverter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/__init__.py` & `caikit-0.9.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/base.py` & `caikit-0.9.3/tests/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/config/test_configs.py` & `caikit-0.9.3/tests/config/test_configs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/conftest.py` & `caikit-0.9.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/augmentors/test_augmentor_base.py` & `caikit-0.9.3/tests/core/augmentors/test_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/augmentors/test_merged_augmentors.py` & `caikit-0.9.3/tests/core/augmentors/test_merged_augmentors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/data_model/data_backends/test_dict_backend.py` & `caikit-0.9.3/tests/core/data_model/data_backends/test_dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/data_model/streams/test_converter.py` & `caikit-0.9.3/tests/core/data_model/streams/test_converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/data_model/streams/test_csv_column_formatter.py` & `caikit-0.9.3/tests/core/data_model/streams/test_csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/data_model/streams/test_data_stream.py` & `caikit-0.9.3/tests/core/data_model/streams/test_data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/data_model/streams/test_resolver.py` & `caikit-0.9.3/tests/core/data_model/streams/test_resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/data_model/streams/test_validator.py` & `caikit-0.9.3/tests/core/data_model/streams/test_validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/data_model/test_base.py` & `caikit-0.9.3/tests/core/data_model/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/data_model/test_dataobject.py` & `caikit-0.9.3/tests/core/data_model/test_dataobject.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/data_model/test_enums.py` & `caikit-0.9.3/tests/core/data_model/test_enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/data_model/test_json_dict.py` & `caikit-0.9.3/tests/core/data_model/test_json_dict.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/data_model/test_producer.py` & `caikit-0.9.3/tests/core/data_model/test_producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/helpers.py` & `caikit-0.9.3/tests/core/helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/module_backends/test_backend_types.py` & `caikit-0.9.3/tests/core/module_backends/test_backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/module_backends/test_module_backend_config.py` & `caikit-0.9.3/tests/core/module_backends/test_module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/modules/test_module.py` & `caikit-0.9.3/tests/core/modules/test_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/modules/test_module_metadata.py` & `caikit-0.9.3/tests/core/modules/test_module_metadata.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/signature_parsing/__init__.py` & `caikit-0.9.3/tests/core/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/signature_parsing/test_docstrings.py` & `caikit-0.9.3/tests/core/signature_parsing/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/signature_parsing/test_parsers.py` & `caikit-0.9.3/tests/core/signature_parsing/test_parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/test_imports.py` & `caikit-0.9.3/tests/core/test_imports.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/test_model_manager.py` & `caikit-0.9.3/tests/core/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/test_no_write_permissions.py` & `caikit-0.9.3/tests/core/test_no_write_permissions.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/test_task.py` & `caikit-0.9.3/tests/core/test_task.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/toolkit/test_compatibility.py` & `caikit-0.9.3/tests/core/toolkit/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/toolkit/test_error_handler.py` & `caikit-0.9.3/tests/core/toolkit/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/toolkit/test_factory.py` & `caikit-0.9.3/tests/core/toolkit/test_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/toolkit/test_fileio.py` & `caikit-0.9.3/tests/core/toolkit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/toolkit/test_quality_evaluation.py` & `caikit-0.9.3/tests/core/toolkit/test_quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/toolkit/test_serializers.py` & `caikit-0.9.3/tests/core/toolkit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/toolkit/test_sync_to_async.py` & `caikit-0.9.3/tests/core/toolkit/test_sync_to_async.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/core/toolkit/test_wip_decorator.py` & `caikit-0.9.3/tests/core/toolkit/test_wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/data_model_helpers.py` & `caikit-0.9.3/tests/data_model_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/examples/shared.py` & `caikit-0.9.3/tests/examples/shared.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/examples/test_examples.py` & `caikit-0.9.3/tests/examples/test_examples.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/fixtures/config/config.yml` & `caikit-0.9.3/tests/fixtures/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/fixtures/data_stream_inputs/sample.txt` & `caikit-0.9.3/tests/fixtures/data_stream_inputs/sample.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/fixtures/dummy_module.zip` & `caikit-0.9.3/tests/fixtures/dummy_module.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/fixtures/dummy_module/config.yml` & `caikit-0.9.3/tests/fixtures/dummy_module/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/fixtures/dummy_module_singleton/config.yml` & `caikit-0.9.3/tests/fixtures/dummy_module_singleton/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/fixtures/fixtures.py` & `caikit-0.9.3/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/fixtures/invalid.zip` & `caikit-0.9.3/tests/fixtures/invalid.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/fixtures/linux.txt` & `caikit-0.9.3/tests/fixtures/linux.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/fixtures/sample_lib/data_model/sample.py` & `caikit-0.9.3/tests/fixtures/sample_lib/data_model/sample.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/fixtures/sample_lib/modules/other_task/other_implementation.py` & `caikit-0.9.3/tests/fixtures/sample_lib/modules/other_task/other_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/fixtures/sample_lib/modules/sample_task/composite_module.py` & `caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/composite_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/fixtures/sample_lib/modules/sample_task/inner_module.py` & `caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/inner_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py` & `caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/list_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py` & `caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/primitive_party_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py` & `caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/fixtures/sample_lib/modules/sample_task/streaming_module.py` & `caikit-0.9.3/tests/fixtures/sample_lib/modules/sample_task/streaming_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/interfaces/__init__.py` & `caikit-0.9.3/tests/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/interfaces/nlp/__init__.py` & `caikit-0.9.3/tests/interfaces/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/interfaces/nlp/test_nlp_tasks.py` & `caikit-0.9.3/tests/interfaces/nlp/test_nlp_tasks.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/conftest.py` & `caikit-0.9.3/tests/runtime/conftest.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/generated/__init__.py` & `caikit-0.9.3/tests/runtime/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/metrics/__init__.py` & `caikit-0.9.3/tests/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/metrics/test_rpc_meter.py` & `caikit-0.9.3/tests/runtime/metrics/test_rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/model_management/__init__.py` & `caikit-0.9.3/tests/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/model_management/test_batcher.py` & `caikit-0.9.3/tests/runtime/model_management/test_batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/model_management/test_model_loader.py` & `caikit-0.9.3/tests/runtime/model_management/test_model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/model_management/test_model_manager.py` & `caikit-0.9.3/tests/runtime/model_management/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/model_management/test_model_sizer.py` & `caikit-0.9.3/tests/runtime/model_management/test_model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/model_management/test_training_manager.py` & `caikit-0.9.3/tests/runtime/model_management/test_training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/service_generation/test_create_service.py` & `caikit-0.9.3/tests/runtime/service_generation/test_create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/service_generation/test_data_stream_source.py` & `caikit-0.9.3/tests/runtime/service_generation/test_data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/service_generation/test_protoable.py` & `caikit-0.9.3/tests/runtime/service_generation/test_protoable.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/service_generation/test_rpcs.py` & `caikit-0.9.3/tests/runtime/service_generation/test_rpcs.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/service_generation/test_type_helpers.py` & `caikit-0.9.3/tests/runtime/service_generation/test_type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/servicers/__init__.py` & `caikit-0.9.3/tests/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/servicers/test_global_predict_servicer_impl.py` & `caikit-0.9.3/tests/runtime/servicers/test_global_predict_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/servicers/test_global_train_servicer_impl.py` & `caikit-0.9.3/tests/runtime/servicers/test_global_train_servicer_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,20 +36,23 @@
 from tests.fixtures import Fixtures
 import caikit.core
 
 ## Helpers #####################################################################
 
 
 @pytest.fixture(autouse=True, params=[True, False])
-def set_train_location(request):
+def set_train_location(request, sample_train_servicer):
     """This fixture ensures that all tests in this file will be run with both
     subprocess and local training styles
     """
-    with temp_config({"training": {"use_subprocess": request.param}}):
-        yield
+    prev_value = sample_train_servicer.use_subprocess
+    sample_train_servicer.use_subprocess = request.param
+    yield
+    # Reset use_subprocess to previous value
+    sample_train_servicer.use_subprocess = prev_value
 
 
 # Train tests for the GlobalTrainServicer class ############################################################
 ##############
 # Normal cases
 ##############
 
@@ -74,14 +77,15 @@
         batch_size=42,
         training_data=training_data,
     )
 
     training_response = sample_train_servicer.Train(
         train_request, Fixtures.build_context("foo")
     )
+
     assert training_response.model_name == model_name
 
     assert training_response.training_id is not None
     assert isinstance(training_response.training_id, str)
 
     result = sample_train_servicer.training_map.get(
         training_response.training_id
@@ -336,30 +340,31 @@
     sample_train_service, sample_train_servicer
 ):
     """Test that if a module raises a ValueError, we should surface it to the user in a helpful way"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
     training_data = stream_type(
         jsondata=stream_type.JsonData(data=[SampleTrainingType(1)])
     ).to_proto()
+
     train_request = sample_train_service.messages.SampleTaskSampleModuleTrainRequest(
         model_name=random_test_id(),
         batch_size=999,
         training_data=training_data,
     )
 
     with pytest.raises(CaikitRuntimeException) as context:
         training_response = sample_train_servicer.Train(
             train_request, Fixtures.build_context("foo")
         )
 
-        training_result = sample_train_servicer.training_map.get(
+        _ = sample_train_servicer.training_map.get(
             training_response.training_id
         ).result()
 
-    assert f"This may be a problem with your input" in str(context.value.message)
+    assert f"Batch size of 999 is not allowed!" in str(context.value.message)
 
 
 def test_global_train_returns_exit_code_with_oom(
     sample_train_service, sample_train_servicer
 ):
     """Test that if module goes into OOM we are able to surface error code"""
     stream_type = caikit.interfaces.common.data_model.DataStreamSourceSampleTrainingType
```

### Comparing `caikit-0.9.2/tests/runtime/servicers/test_model_runtime_servicer_impl.py` & `caikit-0.9.3/tests/runtime/servicers/test_model_runtime_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/servicers/test_model_train_servicer_impl.py` & `caikit-0.9.3/tests/runtime/servicers/test_model_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/servicers/test_training_management_servicer.py` & `caikit-0.9.3/tests/runtime/servicers/test_training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/test_grpc_server.py` & `caikit-0.9.3/tests/runtime/test_grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/test_service_factory.py` & `caikit-0.9.3/tests/runtime/test_service_factory.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/utils/__init__.py` & `caikit-0.9.3/tests/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/utils/test_import_util.py` & `caikit-0.9.3/tests/runtime/utils/test_import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/utils/test_servicer_util.py` & `caikit-0.9.3/tests/runtime/utils/test_servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/work_management/__init__.py` & `caikit-0.9.3/tests/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/work_management/test_abortable_action.py` & `caikit-0.9.3/tests/runtime/work_management/test_abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/work_management/test_call_aborter.py` & `caikit-0.9.3/tests/runtime/work_management/test_call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tests/runtime/work_management/test_destroyable_thread.py` & `caikit-0.9.3/tests/runtime/work_management/test_destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/tox.ini` & `caikit-0.9.3/tox.ini`

 * *Files identical despite different names*

### Comparing `caikit-0.9.2/PKG-INFO` & `caikit-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: caikit
-Version: 0.9.2
+Version: 0.9.3
 Summary: AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: alchemy-config>=1.1.1,<2.0.0
 Requires-Dist: alchemy-logging>=1.0.4,<2.0.0
 Requires-Dist: anytree>=2.7.0,<3.0
 Requires-Dist: docstring-parser>=0.14.1,<0.16.0
 Requires-Dist: grpcio>=1.35.0,<2.0,!=1.55.0
 Requires-Dist: ijson>=3.1.4,<3.3.0
-Requires-Dist: munch>=2.5.0,<4.0
+Requires-Dist: munch>=2.5.0,<5.0
 Requires-Dist: numpy>=1.20,<2
 Requires-Dist: protobuf>=3.19.0,<5
 Requires-Dist: py-to-proto>=0.4.0,<0.5.0,!=0.2.1
 Requires-Dist: PyYAML>=6.0,<7.0
 Requires-Dist: semver>=2.13.0,<4.0
 Requires-Dist: six>=1.16.0,<2.0.0
 Requires-Dist: tqdm>=4.59.0,<5.0.0
```

