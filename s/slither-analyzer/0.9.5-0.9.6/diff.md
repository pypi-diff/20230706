# Comparing `tmp/slither-analyzer-0.9.5.tar.gz` & `tmp/slither-analyzer-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slither-analyzer-0.9.5.tar", last modified: Wed Jun 28 12:47:57 2023, max compression
+gzip compressed data, was "slither-analyzer-0.9.6.tar", last modified: Thu Jul  6 16:34:57 2023, max compression
```

## Comparing `slither-analyzer-0.9.5.tar` & `slither-analyzer-0.9.6.tar`

### file list

```diff
@@ -1,623 +1,623 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.016896 slither-analyzer-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28463 2023-06-28 12:47:57.016896 slither-analyzer-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28072 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 12:47:57.016896 slither-analyzer-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.940894 slither-analyzer-0.9.5/slither/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32143 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/all_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.940894 slither-analyzer-0.9.5/slither/analyses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/analyses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.944894 slither-analyzer-0.9.5/slither/analyses/data_dependency/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/analyses/data_dependency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/analyses/data_dependency/data_dependency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.944894 slither-analyzer-0.9.5/slither/analyses/evm/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/analyses/evm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/analyses/evm/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/analyses/evm/evm_cfg_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.944894 slither-analyzer-0.9.5/slither/analyses/write/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/analyses/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/analyses/write/are_variables_written.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.944894 slither-analyzer-0.9.5/slither/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.944894 slither-analyzer-0.9.5/slither/core/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/cfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39734 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/cfg/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/cfg/scope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.944894 slither-analyzer-0.9.5/slither/core/children/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/children/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/children/child_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/compilation_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.944894 slither-analyzer-0.9.5/slither/core/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/context/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.948894 slither-analyzer-0.9.5/slither/core/declarations/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    60320 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/contract_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/custom_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/custom_error_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/custom_error_top_level.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/enum_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/enum_top_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    69220 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/function_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/function_top_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/import_directive.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/pragma_directive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/solidity_import_placeholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/solidity_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/structure_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/structure_top_level.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/top_level.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/declarations/using_for_top_level.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.948894 slither-analyzer-0.9.5/slither/core/dominators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/dominators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/dominators/node_dominator_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/dominators/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.948894 slither-analyzer-0.9.5/slither/core/expressions/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/expressions/assignment_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/expressions/binary_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/expressions/call_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/expressions/conditional_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/expressions/elementary_type_name_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/expressions/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/expressions/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/expressions/index_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/expressions/literal.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/expressions/member_access.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/expressions/new_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/expressions/new_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/expressions/new_elementary_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/expressions/super_call_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/expressions/super_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/expressions/tuple_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/expressions/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/expressions/unary_operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.952895 slither-analyzer-0.9.5/slither/core/scope/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/scope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/scope/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    22013 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/slither_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.952895 slither-analyzer-0.9.5/slither/core/solidity_types/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/solidity_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/solidity_types/array_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/solidity_types/elementary_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/solidity_types/function_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/solidity_types/mapping_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/solidity_types/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/solidity_types/type_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/solidity_types/type_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/solidity_types/user_defined_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.952895 slither-analyzer-0.9.5/slither/core/source_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/source_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/source_mapping/source_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.952895 slither-analyzer-0.9.5/slither/core/variables/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/variables/event_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/variables/function_type_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/variables/local_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/variables/local_variable_init_from_tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/variables/state_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/variables/structure_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/variables/top_level_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/core/variables/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.952895 slither-analyzer-0.9.5/slither/detectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/abstract_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/all_detectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.952895 slither-analyzer-0.9.5/slither/detectors/assembly/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/assembly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/assembly/shift_parameter_mixup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.956894 slither-analyzer-0.9.5/slither/detectors/attributes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/attributes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/attributes/const_functions_asm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/attributes/const_functions_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/attributes/constant_pragma.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/attributes/incorrect_solc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/attributes/locked_ether.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/attributes/unimplemented_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.956894 slither-analyzer-0.9.5/slither/detectors/compiler_bugs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/compiler_bugs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/compiler_bugs/array_by_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/compiler_bugs/enum_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/compiler_bugs/multiple_constructor_schemes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/compiler_bugs/public_mapping_nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/compiler_bugs/reused_base_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/compiler_bugs/storage_ABIEncoderV2_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/compiler_bugs/storage_signed_integer_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/compiler_bugs/uninitialized_function_ptr_in_constructor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.956894 slither-analyzer-0.9.5/slither/detectors/erc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/erc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.956894 slither-analyzer-0.9.5/slither/detectors/erc/erc20/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/erc/erc20/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/erc/erc20/arbitrary_send_erc20.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/erc/erc20/arbitrary_send_erc20_no_permit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/erc/erc20/arbitrary_send_erc20_permit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/erc/erc20/incorrect_erc20_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/erc/incorrect_erc721_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/erc/unindexed_event_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.956894 slither-analyzer-0.9.5/slither/detectors/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/examples/backdoor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.956894 slither-analyzer-0.9.5/slither/detectors/functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/functions/arbitrary_send_eth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/functions/codex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/functions/cyclomatic_complexity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/functions/dead_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    12558 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/functions/external_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/functions/modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/functions/permit_domain_signature_collision.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/functions/protected_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/functions/suicidal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/functions/unimplemented.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.956894 slither-analyzer-0.9.5/slither/detectors/naming_convention/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/naming_convention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/naming_convention/naming_convention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.960895 slither-analyzer-0.9.5/slither/detectors/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/operations/bad_prng.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/operations/block_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/operations/cache_array_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/operations/encode_packed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/operations/low_level_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/operations/missing_events_access_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/operations/missing_events_arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/operations/missing_zero_address_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/operations/unchecked_low_level_return_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/operations/unchecked_send_return_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/operations/unchecked_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/operations/unused_return_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/operations/void_constructor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.960895 slither-analyzer-0.9.5/slither/detectors/reentrancy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/reentrancy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/reentrancy/reentrancy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/reentrancy/reentrancy_benign.py
--rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/reentrancy/reentrancy_eth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/reentrancy/reentrancy_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/reentrancy/reentrancy_no_gas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/reentrancy/reentrancy_read_before_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/reentrancy/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.960895 slither-analyzer-0.9.5/slither/detectors/shadowing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/shadowing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/shadowing/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/shadowing/builtin_symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/shadowing/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/shadowing/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/shadowing/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.960895 slither-analyzer-0.9.5/slither/detectors/slither/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/slither/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/slither/name_reused.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.960895 slither-analyzer-0.9.5/slither/detectors/source/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/source/rtlo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.964895 slither-analyzer-0.9.5/slither/detectors/statements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/array_length_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/assert_state_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/boolean_constant_equality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/boolean_constant_misuse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/calls_in_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/controlled_delegatecall.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/costly_operations_in_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/delegatecall_in_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/deprecated_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/divide_before_multiply.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/incorrect_strict_equality.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/incorrect_using_for.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/mapping_deletion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/msg_value_in_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/redundant_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/too_many_digits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/tx_origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/type_based_tautology.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/unary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/unprotected_upgradeable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/statements/write_after_write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.964895 slither-analyzer-0.9.5/slither/detectors/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/variables/could_be_constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/variables/could_be_immutable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/variables/function_init_state_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/variables/predeclaration_usage_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/variables/similar_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/variables/unchanged_state_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/variables/uninitialized_local_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/variables/uninitialized_state_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/variables/uninitialized_storage_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/variables/unused_state_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/detectors/variables/var_read_using_this.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.968895 slither-analyzer-0.9.5/slither/formatters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/formatters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.968895 slither-analyzer-0.9.5/slither/formatters/attributes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/formatters/attributes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/formatters/attributes/const_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/formatters/attributes/constant_pragma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/formatters/attributes/incorrect_solc.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/formatters/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.968895 slither-analyzer-0.9.5/slither/formatters/functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/formatters/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/formatters/functions/external_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.968895 slither-analyzer-0.9.5/slither/formatters/naming_convention/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/formatters/naming_convention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27353 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/formatters/naming_convention/naming_convention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.968895 slither-analyzer-0.9.5/slither/formatters/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/formatters/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/formatters/utils/patches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.968895 slither-analyzer-0.9.5/slither/formatters/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/formatters/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/formatters/variables/unchanged_state_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/formatters/variables/unused_state_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.968895 slither-analyzer-0.9.5/slither/printers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/abstract_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/all_printers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.968895 slither-analyzer-0.9.5/slither/printers/call/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/call/call_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.968895 slither-analyzer-0.9.5/slither/printers/functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/functions/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/functions/cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/functions/dominator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.968895 slither-analyzer-0.9.5/slither/printers/guidance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/guidance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17840 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/guidance/echidna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.968895 slither-analyzer-0.9.5/slither/printers/inheritance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/inheritance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/inheritance/inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/inheritance/inheritance_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.972895 slither-analyzer-0.9.5/slither/printers/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/summary/constructor_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/summary/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/summary/data_depenency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/summary/declaration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/summary/evm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/summary/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/summary/function_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    14949 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/summary/human_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/summary/loc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/summary/modifier_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/summary/require_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/summary/slithir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/summary/slithir_ssa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/summary/variable_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/printers/summary/when_not_paused.py
--rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slither.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.972895 slither-analyzer-0.9.5/slither/slithir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    74572 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.980895 slither-analyzer-0.9.5/slither/slithir/operations/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/call.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/codesize.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/event_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/high_level_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/init_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/internal_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/internal_dynamic_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/length.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/library_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/low_level_call.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/lvalue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/new_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/new_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/new_elementary_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/new_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/nop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/phi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/phi_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/return_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/send.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/solidity_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/unary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/operations/unpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.980895 slither-analyzer-0.9.5/slither/slithir/tmp_operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/tmp_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/tmp_operations/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/tmp_operations/tmp_call.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/tmp_operations/tmp_new_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/tmp_operations/tmp_new_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/tmp_operations/tmp_new_elementary_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/tmp_operations/tmp_new_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.980895 slither-analyzer-0.9.5/slither/slithir/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34585 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/utils/ssa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.980895 slither-analyzer-0.9.5/slither/slithir/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/variables/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/variables/local_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/variables/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/variables/reference_ssa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/variables/state_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/variables/temporary.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/variables/temporary_ssa.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/variables/tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/variables/tuple_ssa.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/slithir/variables/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.984895 slither-analyzer-0.9.5/slither/solc_parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.984895 slither-analyzer-0.9.5/slither/solc_parsing/cfg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/cfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/cfg/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.984895 slither-analyzer-0.9.5/slither/solc_parsing/declarations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/declarations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/declarations/caller_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    36106 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/declarations/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/declarations/custom_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/declarations/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    63686 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/declarations/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/declarations/modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/declarations/structure_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/declarations/structure_top_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/declarations/using_for_top_level.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.984895 slither-analyzer-0.9.5/slither/solc_parsing/expressions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27772 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/expressions/expression_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    16797 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/expressions/find_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    36018 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/slither_compilation_unit_solc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.984895 slither-analyzer-0.9.5/slither/solc_parsing/solidity_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/solidity_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20463 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/solidity_types/type_parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.988895 slither-analyzer-0.9.5/slither/solc_parsing/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/variables/event_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/variables/function_type_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/variables/local_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/variables/local_variable_init_from_tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/variables/state_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/variables/structure_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/variables/top_level_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/variables/variable_declaration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.988895 slither-analyzer-0.9.5/slither/solc_parsing/yul/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/yul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/yul/evm_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    30919 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/solc_parsing/yul/parse_yul.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.988895 slither-analyzer-0.9.5/slither/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.988895 slither-analyzer-0.9.5/slither/tools/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/demo/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.988895 slither-analyzer-0.9.5/slither/tools/doctor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/doctor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/doctor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.988895 slither-analyzer-0.9.5/slither/tools/doctor/checks/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/doctor/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/doctor/checks/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/doctor/checks/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/doctor/checks/versions.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/doctor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.988895 slither-analyzer-0.9.5/slither/tools/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/documentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/documentation/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.988895 slither-analyzer-0.9.5/slither/tools/erc_conformance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/erc_conformance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/erc_conformance/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.988895 slither-analyzer-0.9.5/slither/tools/erc_conformance/erc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/erc_conformance/erc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/erc_conformance/erc/erc1155.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/erc_conformance/erc/erc20.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/erc_conformance/erc/ercs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.988895 slither-analyzer-0.9.5/slither/tools/flattening/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/flattening/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/flattening/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.992895 slither-analyzer-0.9.5/slither/tools/flattening/export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/flattening/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/flattening/export/export.py
--rw-r--r--   0 runner    (1001) docker     (123)    20013 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/flattening/flattening.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.992895 slither-analyzer-0.9.5/slither/tools/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/interface/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.992895 slither-analyzer-0.9.5/slither/tools/kspec_coverage/
--rwxr-xr-x   0 runner    (1001) docker     (123)       36 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/kspec_coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/kspec_coverage/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6900 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/kspec_coverage/analysis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      534 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/kspec_coverage/kspec_coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.992895 slither-analyzer-0.9.5/slither/tools/mutator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/mutator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/mutator/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.992895 slither-analyzer-0.9.5/slither/tools/mutator/mutators/
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/mutator/mutators/MIA.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/mutator/mutators/MVIE.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/mutator/mutators/MVIV.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/mutator/mutators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/mutator/mutators/abstract_mutator.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/mutator/mutators/all_mutators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.992895 slither-analyzer-0.9.5/slither/tools/mutator/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/mutator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/mutator/utils/command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/mutator/utils/generic_patching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.992895 slither-analyzer-0.9.5/slither/tools/possible_paths/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/possible_paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/possible_paths/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/possible_paths/possible_paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.992895 slither-analyzer-0.9.5/slither/tools/properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.992895 slither-analyzer-0.9.5/slither/tools/properties/addresses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/addresses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/addresses/address.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.992895 slither-analyzer-0.9.5/slither/tools/properties/platforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/platforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/platforms/echidna.py
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/platforms/truffle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.996895 slither-analyzer-0.9.5/slither/tools/properties/properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/properties/erc20.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.996895 slither-analyzer-0.9.5/slither/tools/properties/properties/ercs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/properties/ercs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.996895 slither-analyzer-0.9.5/slither/tools/properties/properties/ercs/erc20/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/properties/ercs/erc20/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.996895 slither-analyzer-0.9.5/slither/tools/properties/properties/ercs/erc20/properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/properties/ercs/erc20/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/properties/ercs/erc20/properties/burn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/properties/ercs/erc20/properties/initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/properties/ercs/erc20/properties/mint.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/properties/ercs/erc20/properties/mint_and_burn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/properties/ercs/erc20/properties/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.996895 slither-analyzer-0.9.5/slither/tools/properties/properties/ercs/erc20/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/properties/ercs/erc20/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/properties/ercs/erc20/unit_tests/truffle.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/properties/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.996895 slither-analyzer-0.9.5/slither/tools/properties/solidity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/solidity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/solidity/generate_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/properties/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.996895 slither-analyzer-0.9.5/slither/tools/read_storage/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/read_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/read_storage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37543 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/read_storage/read_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:56.996895 slither-analyzer-0.9.5/slither/tools/read_storage/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/read_storage/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/read_storage/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.000895 slither-analyzer-0.9.5/slither/tools/similarity/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/similarity/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2701 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/similarity/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/similarity/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/similarity/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/similarity/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/similarity/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/similarity/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/similarity/similarity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1825 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/similarity/test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/similarity/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.000895 slither-analyzer-0.9.5/slither/tools/slither_format/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/slither_format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/slither_format/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/slither_format/slither_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.000895 slither-analyzer-0.9.5/slither/tools/upgradeability/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/upgradeability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/upgradeability/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.000895 slither-analyzer-0.9.5/slither/tools/upgradeability/checks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/upgradeability/checks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/upgradeability/checks/abstract_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/upgradeability/checks/all_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/upgradeability/checks/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/upgradeability/checks/functions_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/upgradeability/checks/initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/upgradeability/checks/variable_initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/upgradeability/checks/variables_order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.000895 slither-analyzer-0.9.5/slither/tools/upgradeability/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/upgradeability/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/upgradeability/utils/command_line.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.000895 slither-analyzer-0.9.5/slither/tools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/tools/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.004895 slither-analyzer-0.9.5/slither/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/code_complexity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/code_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/codex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/comparable_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)    12953 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/erc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/expression_manipulations.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/inheritance_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/integer_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/loc.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/myprettytable.py
--rw-r--r--   0 runner    (1001) docker     (123)    27046 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/output_capture.py
--rw-r--r--   0 runner    (1001) docker     (123)   251870 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/oz_hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/source_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/standard_libraries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/tests_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/type.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/type_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    30264 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/upgradeability.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.008895 slither-analyzer-0.9.5/slither/visitors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/visitors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.008895 slither-analyzer-0.9.5/slither/visitors/expression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/visitors/expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/visitors/expression/constants_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/visitors/expression/export_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/visitors/expression/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/visitors/expression/expression_printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/visitors/expression/find_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/visitors/expression/has_conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/visitors/expression/read_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/visitors/expression/write_var.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.008895 slither-analyzer-0.9.5/slither/visitors/slithir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/visitors/slithir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27707 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/slither/visitors/slithir/expression_to_slithir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.008895 slither-analyzer-0.9.5/slither_analyzer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28463 2023-06-28 12:47:56.000000 slither-analyzer-0.9.5/slither_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21926 2023-06-28 12:47:56.000000 slither-analyzer-0.9.5/slither_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 12:47:56.000000 slither-analyzer-0.9.5/slither_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-28 12:47:56.000000 slither-analyzer-0.9.5/slither_analyzer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-28 12:47:56.000000 slither-analyzer-0.9.5/slither_analyzer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-28 12:47:56.000000 slither-analyzer-0.9.5/slither_analyzer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.008895 slither-analyzer-0.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.008895 slither-analyzer-0.9.5/tests/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/tests/e2e/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.008895 slither-analyzer-0.9.5/tests/e2e/compilation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/tests/e2e/compilation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/tests/e2e/compilation/test_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/tests/e2e/compilation/test_source_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.012895 slither-analyzer-0.9.5/tests/e2e/detectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/tests/e2e/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42416 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/tests/e2e/detectors/test_detectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.012895 slither-analyzer-0.9.5/tests/e2e/solc_parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/tests/e2e/solc_parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21918 2023-06-28 12:47:43.000000 slither-analyzer-0.9.5/tests/e2e/solc_parsing/test_ast_parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.012895 slither-analyzer-0.9.5/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.012895 slither-analyzer-0.9.5/tests/tools/read-storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/tools/read-storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/tools/read-storage/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/tools/read-storage/test_read_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.012895 slither-analyzer-0.9.5/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.012895 slither-analyzer-0.9.5/tests/unit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/core/test_arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/core/test_code_comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/core/test_constant_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/core/test_contract_declaration.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/core/test_error_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/core/test_fallback_receive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/core/test_function_declaration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/core/test_source_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/core/test_storage_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/core/test_using_for.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.012895 slither-analyzer-0.9.5/tests/unit/slithir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/slithir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/slithir/test_operation_reads.py
--rw-r--r--   0 runner    (1001) docker     (123)    37161 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/slithir/test_ssa_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/slithir/test_ternary_expressions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:57.016896 slither-analyzer-0.9.5/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/utils/test_code_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/utils/test_functions_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/utils/test_type_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/unit/utils/test_upgradeability_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-28 12:47:44.000000 slither-analyzer-0.9.5/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.428304 slither-analyzer-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29278 2023-07-06 16:34:57.428304 slither-analyzer-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28887 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 16:34:57.428304 slither-analyzer-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.360302 slither-analyzer-0.9.6/slither/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32143 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/all_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.360302 slither-analyzer-0.9.6/slither/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/analyses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.360302 slither-analyzer-0.9.6/slither/analyses/data_dependency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/analyses/data_dependency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/analyses/data_dependency/data_dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.360302 slither-analyzer-0.9.6/slither/analyses/evm/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/analyses/evm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/analyses/evm/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/analyses/evm/evm_cfg_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.360302 slither-analyzer-0.9.6/slither/analyses/write/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/analyses/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/analyses/write/are_variables_written.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.360302 slither-analyzer-0.9.6/slither/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.364302 slither-analyzer-0.9.6/slither/core/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/cfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39734 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/cfg/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/cfg/scope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.364302 slither-analyzer-0.9.6/slither/core/children/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/children/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/children/child_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11741 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/compilation_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.364302 slither-analyzer-0.9.6/slither/core/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/context/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.364302 slither-analyzer-0.9.6/slither/core/declarations/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60320 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/contract_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/custom_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/custom_error_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/custom_error_top_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/enum_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/enum_top_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69220 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/function_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/function_top_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/import_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/pragma_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/solidity_import_placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/solidity_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/structure_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/structure_top_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/top_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/declarations/using_for_top_level.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.368302 slither-analyzer-0.9.6/slither/core/dominators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/dominators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/dominators/node_dominator_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/dominators/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.368302 slither-analyzer-0.9.6/slither/core/expressions/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/expressions/assignment_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/expressions/binary_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/expressions/call_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/expressions/conditional_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/expressions/elementary_type_name_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/expressions/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/expressions/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/expressions/index_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/expressions/literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/expressions/member_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/expressions/new_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/expressions/new_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/expressions/new_elementary_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/expressions/super_call_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/expressions/super_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/expressions/tuple_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/expressions/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/expressions/unary_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.368302 slither-analyzer-0.9.6/slither/core/scope/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/scope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/scope/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22013 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/slither_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.372302 slither-analyzer-0.9.6/slither/core/solidity_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/solidity_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/solidity_types/array_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/solidity_types/elementary_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/solidity_types/function_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/solidity_types/mapping_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/solidity_types/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/solidity_types/type_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/solidity_types/type_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/solidity_types/user_defined_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.372302 slither-analyzer-0.9.6/slither/core/source_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/source_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7159 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/source_mapping/source_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.372302 slither-analyzer-0.9.6/slither/core/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/variables/event_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/variables/function_type_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/variables/local_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/variables/local_variable_init_from_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/variables/state_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/variables/structure_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/variables/top_level_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/core/variables/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.372302 slither-analyzer-0.9.6/slither/detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/abstract_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/all_detectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.372302 slither-analyzer-0.9.6/slither/detectors/assembly/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/assembly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/assembly/shift_parameter_mixup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.372302 slither-analyzer-0.9.6/slither/detectors/attributes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/attributes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/attributes/const_functions_asm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/attributes/const_functions_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/attributes/constant_pragma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/attributes/incorrect_solc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/attributes/locked_ether.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/attributes/unimplemented_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.376303 slither-analyzer-0.9.6/slither/detectors/compiler_bugs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/compiler_bugs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/compiler_bugs/array_by_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/compiler_bugs/enum_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/compiler_bugs/multiple_constructor_schemes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/compiler_bugs/public_mapping_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/compiler_bugs/reused_base_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/compiler_bugs/storage_ABIEncoderV2_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/compiler_bugs/storage_signed_integer_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/compiler_bugs/uninitialized_function_ptr_in_constructor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.376303 slither-analyzer-0.9.6/slither/detectors/erc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/erc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.376303 slither-analyzer-0.9.6/slither/detectors/erc/erc20/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/erc/erc20/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/erc/erc20/arbitrary_send_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/erc/erc20/arbitrary_send_erc20_no_permit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/erc/erc20/arbitrary_send_erc20_permit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/erc/erc20/incorrect_erc20_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/erc/incorrect_erc721_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/erc/unindexed_event_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.376303 slither-analyzer-0.9.6/slither/detectors/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/examples/backdoor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.380303 slither-analyzer-0.9.6/slither/detectors/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/functions/arbitrary_send_eth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/functions/codex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/functions/cyclomatic_complexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/functions/dead_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12558 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/functions/external_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/functions/modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/functions/permit_domain_signature_collision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/functions/protected_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/functions/suicidal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/functions/unimplemented.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.380303 slither-analyzer-0.9.6/slither/detectors/naming_convention/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/naming_convention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/naming_convention/naming_convention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.380303 slither-analyzer-0.9.6/slither/detectors/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/operations/bad_prng.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/operations/block_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/operations/cache_array_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/operations/encode_packed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/operations/low_level_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/operations/missing_events_access_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/operations/missing_events_arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/operations/missing_zero_address_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/operations/unchecked_low_level_return_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/operations/unchecked_send_return_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/operations/unchecked_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/operations/unused_return_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/operations/void_constructor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.384303 slither-analyzer-0.9.6/slither/detectors/reentrancy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/reentrancy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10740 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/reentrancy/reentrancy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/reentrancy/reentrancy_benign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8599 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/reentrancy/reentrancy_eth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/reentrancy/reentrancy_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9222 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/reentrancy/reentrancy_no_gas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/reentrancy/reentrancy_read_before_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/reentrancy/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.384303 slither-analyzer-0.9.6/slither/detectors/shadowing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/shadowing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/shadowing/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/shadowing/builtin_symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/shadowing/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/shadowing/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/shadowing/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.384303 slither-analyzer-0.9.6/slither/detectors/slither/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/slither/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/slither/name_reused.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.384303 slither-analyzer-0.9.6/slither/detectors/source/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/source/rtlo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.388303 slither-analyzer-0.9.6/slither/detectors/statements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/array_length_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/assert_state_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/boolean_constant_equality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/boolean_constant_misuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/calls_in_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/controlled_delegatecall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/costly_operations_in_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/delegatecall_in_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/deprecated_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/divide_before_multiply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/incorrect_strict_equality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/incorrect_using_for.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/mapping_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/msg_value_in_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/redundant_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/too_many_digits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/tx_origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/type_based_tautology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/unary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/unprotected_upgradeable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/statements/write_after_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.388303 slither-analyzer-0.9.6/slither/detectors/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/variables/could_be_constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/variables/could_be_immutable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/variables/function_init_state_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/variables/predeclaration_usage_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/variables/similar_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/variables/unchanged_state_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/variables/uninitialized_local_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/variables/uninitialized_state_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/variables/uninitialized_storage_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/variables/unused_state_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/detectors/variables/var_read_using_this.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.388303 slither-analyzer-0.9.6/slither/formatters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/formatters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.388303 slither-analyzer-0.9.6/slither/formatters/attributes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/formatters/attributes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/formatters/attributes/const_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/formatters/attributes/constant_pragma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/formatters/attributes/incorrect_solc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/formatters/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.392303 slither-analyzer-0.9.6/slither/formatters/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/formatters/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/formatters/functions/external_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.392303 slither-analyzer-0.9.6/slither/formatters/naming_convention/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/formatters/naming_convention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27353 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/formatters/naming_convention/naming_convention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.392303 slither-analyzer-0.9.6/slither/formatters/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/formatters/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/formatters/utils/patches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.392303 slither-analyzer-0.9.6/slither/formatters/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/formatters/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/formatters/variables/unchanged_state_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/formatters/variables/unused_state_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.392303 slither-analyzer-0.9.6/slither/printers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/abstract_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/all_printers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.392303 slither-analyzer-0.9.6/slither/printers/call/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/call/call_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.392303 slither-analyzer-0.9.6/slither/printers/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/functions/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/functions/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/functions/dominator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.392303 slither-analyzer-0.9.6/slither/printers/guidance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/guidance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17840 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/guidance/echidna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.392303 slither-analyzer-0.9.6/slither/printers/inheritance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/inheritance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/inheritance/inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/inheritance/inheritance_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.396303 slither-analyzer-0.9.6/slither/printers/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/summary/constructor_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/summary/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/summary/data_depenency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/summary/declaration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/summary/evm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/summary/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/summary/function_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14949 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/summary/human_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/summary/loc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/summary/modifier_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/summary/require_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/summary/slithir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/summary/slithir_ssa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/summary/variable_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/printers/summary/when_not_paused.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slither.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.396303 slither-analyzer-0.9.6/slither/slithir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74572 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.400303 slither-analyzer-0.9.6/slither/slithir/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/codesize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/event_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/high_level_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/init_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/internal_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/internal_dynamic_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/library_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/low_level_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/lvalue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/new_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/new_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/new_elementary_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/new_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/nop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/phi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/phi_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/return_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/solidity_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/unary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/operations/unpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.404303 slither-analyzer-0.9.6/slither/slithir/tmp_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/tmp_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/tmp_operations/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/tmp_operations/tmp_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/tmp_operations/tmp_new_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/tmp_operations/tmp_new_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/tmp_operations/tmp_new_elementary_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/tmp_operations/tmp_new_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.404303 slither-analyzer-0.9.6/slither/slithir/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34585 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/utils/ssa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.404303 slither-analyzer-0.9.6/slither/slithir/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/variables/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/variables/local_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/variables/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/variables/reference_ssa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/variables/state_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/variables/temporary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/variables/temporary_ssa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/variables/tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/variables/tuple_ssa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/slithir/variables/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.404303 slither-analyzer-0.9.6/slither/solc_parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.404303 slither-analyzer-0.9.6/slither/solc_parsing/cfg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/cfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/cfg/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.404303 slither-analyzer-0.9.6/slither/solc_parsing/declarations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/declarations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/declarations/caller_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36106 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/declarations/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/declarations/custom_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/declarations/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63686 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/declarations/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/declarations/modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/declarations/structure_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/declarations/structure_top_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/declarations/using_for_top_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.404303 slither-analyzer-0.9.6/slither/solc_parsing/expressions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27772 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/expressions/expression_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16797 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/expressions/find_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36018 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/slither_compilation_unit_solc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.404303 slither-analyzer-0.9.6/slither/solc_parsing/solidity_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/solidity_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20463 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/solidity_types/type_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.408303 slither-analyzer-0.9.6/slither/solc_parsing/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/variables/event_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/variables/function_type_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/variables/local_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/variables/local_variable_init_from_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/variables/state_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/variables/structure_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/variables/top_level_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8341 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/variables/variable_declaration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.408303 slither-analyzer-0.9.6/slither/solc_parsing/yul/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/yul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/yul/evm_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30919 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/solc_parsing/yul/parse_yul.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.408303 slither-analyzer-0.9.6/slither/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.408303 slither-analyzer-0.9.6/slither/tools/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/demo/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.408303 slither-analyzer-0.9.6/slither/tools/doctor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/doctor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/doctor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.408303 slither-analyzer-0.9.6/slither/tools/doctor/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/doctor/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/doctor/checks/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/doctor/checks/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/doctor/checks/versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/doctor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.408303 slither-analyzer-0.9.6/slither/tools/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/documentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8470 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/documentation/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.408303 slither-analyzer-0.9.6/slither/tools/erc_conformance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/erc_conformance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/erc_conformance/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.408303 slither-analyzer-0.9.6/slither/tools/erc_conformance/erc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/erc_conformance/erc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/erc_conformance/erc/erc1155.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/erc_conformance/erc/erc20.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/erc_conformance/erc/ercs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.408303 slither-analyzer-0.9.6/slither/tools/flattening/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/flattening/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/flattening/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.408303 slither-analyzer-0.9.6/slither/tools/flattening/export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/flattening/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/flattening/export/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20013 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/flattening/flattening.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.412304 slither-analyzer-0.9.6/slither/tools/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/interface/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.412304 slither-analyzer-0.9.6/slither/tools/kspec_coverage/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       36 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/kspec_coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/kspec_coverage/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6900 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/kspec_coverage/analysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      534 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/kspec_coverage/kspec_coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.412304 slither-analyzer-0.9.6/slither/tools/mutator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/mutator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/mutator/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.412304 slither-analyzer-0.9.6/slither/tools/mutator/mutators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/mutator/mutators/MIA.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/mutator/mutators/MVIE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/mutator/mutators/MVIV.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/mutator/mutators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/mutator/mutators/abstract_mutator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/mutator/mutators/all_mutators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.412304 slither-analyzer-0.9.6/slither/tools/mutator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/mutator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/mutator/utils/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/mutator/utils/generic_patching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.412304 slither-analyzer-0.9.6/slither/tools/possible_paths/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/possible_paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/possible_paths/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/possible_paths/possible_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.412304 slither-analyzer-0.9.6/slither/tools/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.412304 slither-analyzer-0.9.6/slither/tools/properties/addresses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/addresses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/addresses/address.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.412304 slither-analyzer-0.9.6/slither/tools/properties/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/platforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/platforms/echidna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/platforms/truffle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.412304 slither-analyzer-0.9.6/slither/tools/properties/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/properties/erc20.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.412304 slither-analyzer-0.9.6/slither/tools/properties/properties/ercs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/properties/ercs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.412304 slither-analyzer-0.9.6/slither/tools/properties/properties/ercs/erc20/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/properties/ercs/erc20/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.416303 slither-analyzer-0.9.6/slither/tools/properties/properties/ercs/erc20/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/properties/ercs/erc20/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/properties/ercs/erc20/properties/burn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/properties/ercs/erc20/properties/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/properties/ercs/erc20/properties/mint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/properties/ercs/erc20/properties/mint_and_burn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/properties/ercs/erc20/properties/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.416303 slither-analyzer-0.9.6/slither/tools/properties/properties/ercs/erc20/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/properties/ercs/erc20/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/properties/ercs/erc20/unit_tests/truffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/properties/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.416303 slither-analyzer-0.9.6/slither/tools/properties/solidity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/solidity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/solidity/generate_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/properties/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.416303 slither-analyzer-0.9.6/slither/tools/read_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/read_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/read_storage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37543 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/read_storage/read_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.416303 slither-analyzer-0.9.6/slither/tools/read_storage/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/read_storage/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/read_storage/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.416303 slither-analyzer-0.9.6/slither/tools/similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/similarity/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2701 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/similarity/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/similarity/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/similarity/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/similarity/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/similarity/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/similarity/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/similarity/similarity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1825 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/similarity/test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/similarity/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.416303 slither-analyzer-0.9.6/slither/tools/slither_format/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/slither_format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/slither_format/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/slither_format/slither_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.416303 slither-analyzer-0.9.6/slither/tools/upgradeability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/upgradeability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/upgradeability/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.416303 slither-analyzer-0.9.6/slither/tools/upgradeability/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/upgradeability/checks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/upgradeability/checks/abstract_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/upgradeability/checks/all_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/upgradeability/checks/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/upgradeability/checks/functions_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/upgradeability/checks/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/upgradeability/checks/variable_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/upgradeability/checks/variables_order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.416303 slither-analyzer-0.9.6/slither/tools/upgradeability/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/upgradeability/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/upgradeability/utils/command_line.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.416303 slither-analyzer-0.9.6/slither/tools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/tools/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.420304 slither-analyzer-0.9.6/slither/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/code_complexity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/code_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/codex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/comparable_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12953 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/erc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/expression_manipulations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/inheritance_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/integer_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/loc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/myprettytable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27046 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/output_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)   251870 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/oz_hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/source_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/standard_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/tests_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/type_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30264 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/upgradeability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.420304 slither-analyzer-0.9.6/slither/visitors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/visitors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.424304 slither-analyzer-0.9.6/slither/visitors/expression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/visitors/expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/visitors/expression/constants_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/visitors/expression/export_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/visitors/expression/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/visitors/expression/expression_printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/visitors/expression/find_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/visitors/expression/has_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/visitors/expression/read_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/visitors/expression/write_var.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.424304 slither-analyzer-0.9.6/slither/visitors/slithir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/visitors/slithir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27707 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/slither/visitors/slithir/expression_to_slithir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.424304 slither-analyzer-0.9.6/slither_analyzer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29278 2023-07-06 16:34:57.000000 slither-analyzer-0.9.6/slither_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21926 2023-07-06 16:34:57.000000 slither-analyzer-0.9.6/slither_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 16:34:57.000000 slither-analyzer-0.9.6/slither_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-06 16:34:57.000000 slither-analyzer-0.9.6/slither_analyzer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-06 16:34:57.000000 slither-analyzer-0.9.6/slither_analyzer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 16:34:57.000000 slither-analyzer-0.9.6/slither_analyzer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.424304 slither-analyzer-0.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.424304 slither-analyzer-0.9.6/tests/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/e2e/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.424304 slither-analyzer-0.9.6/tests/e2e/compilation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/e2e/compilation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/e2e/compilation/test_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/e2e/compilation/test_source_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.424304 slither-analyzer-0.9.6/tests/e2e/detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/e2e/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42416 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/e2e/detectors/test_detectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.424304 slither-analyzer-0.9.6/tests/e2e/solc_parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/e2e/solc_parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21918 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/e2e/solc_parsing/test_ast_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.424304 slither-analyzer-0.9.6/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.424304 slither-analyzer-0.9.6/tests/tools/read-storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/tools/read-storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/tools/read-storage/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/tools/read-storage/test_read_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.424304 slither-analyzer-0.9.6/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.424304 slither-analyzer-0.9.6/tests/unit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/core/test_arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/core/test_code_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/core/test_constant_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/core/test_contract_declaration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/core/test_error_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/core/test_fallback_receive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/core/test_function_declaration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/core/test_source_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/core/test_storage_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/core/test_using_for.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.428304 slither-analyzer-0.9.6/tests/unit/slithir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/slithir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/slithir/test_operation_reads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37161 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/slithir/test_ssa_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/slithir/test_ternary_expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:57.428304 slither-analyzer-0.9.6/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/utils/test_code_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/utils/test_functions_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/utils/test_type_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/unit/utils/test_upgradeability_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-06 16:34:45.000000 slither-analyzer-0.9.6/tests/utils.py
```

### Comparing `slither-analyzer-0.9.5/LICENSE` & `slither-analyzer-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/PKG-INFO` & `slither-analyzer-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,80 +1,96 @@
 Metadata-Version: 2.1
 Name: slither-analyzer
-Version: 0.9.5
+Version: 0.9.6
 Summary: Slither is a Solidity static analysis framework written in Python 3.
 Home-page: https://github.com/crytic/slither
 Author: Trail of Bits
 License: AGPL-3.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: lint
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: dev
 License-File: LICENSE
 
-# Slither, the Solidity source analyzer
+# [Slither, the Solidity source analyzer](https://crytic.github.io/slither/slither.html)
 
-<img src="https://raw.githubusercontent.com/crytic/slither/master/logo.png" alt="Logo" width="500"/>
+<img src="https://raw.githubusercontent.com/crytic/slither/master/logo.png" alt="Slither Static Analysis Framework Logo" width="500" />
 
 [![Build Status](https://img.shields.io/github/actions/workflow/status/crytic/slither/ci.yml?branch=master)](https://github.com/crytic/slither/actions?query=workflow%3ACI)
-[![Slack Status](https://empireslacking.herokuapp.com/badge.svg)](https://empireslacking.herokuapp.com)
-[![PyPI version](https://badge.fury.io/py/slither-analyzer.svg)](https://badge.fury.io/py/slither-analyzer)
-
-Slither is a Solidity static analysis framework written in Python3. It runs a suite of vulnerability detectors, prints visual information about contract details, and provides an API to easily write custom analyses. Slither enables developers to find vulnerabilities, enhance their code comprehension, and quickly prototype custom analyses.
-
-- [Features](#features)
-- [Usage](#usage)
-- [How to Install](#how-to-install)
-- [Detectors](#detectors)
-- [Printers](#printers)
-- [Tools](#tools)
-- [API Documentation](#api-documentation)
-- [Getting Help](#getting-help)
-- [FAQ](#faq)
-- [Publications](#publications)
+![PyPI](https://img.shields.io/pypi/v/slither-analyzer?logo=python&logoColor=white&label=slither-analyzer)
+[![Slither - Read the Docs](https://img.shields.io/badge/Slither-Read_the_Docs-2ea44f)](https://crytic.github.io/slither/slither.html)
+[![Slither - Wiki](https://img.shields.io/badge/Slither-Wiki-2ea44f)](https://github.com/crytic/slither/wiki/SlithIR)
+
+> Join the Empire Hacking Slack  
+>
+> [![Slack Status](https://slack.empirehacking.nyc/badge.svg)](https://slack.empirehacking.nyc/)
+> > <sub><i>- Discussions and Support </i></sub>
+
+**Slither** is a Solidity static analysis framework written in Python3. It runs a suite of vulnerability detectors, prints visual information about contract details, and provides an API to easily write custom analyses. Slither enables developers to find vulnerabilities, enhance their code comprehension, and quickly prototype custom analyses.
+
+* [Features](#features)
+* [Usage](#usage)
+* [How to install](#how-to-install)
+  * [Using Pip](#using-pip)
+  * [Using Git](#using-git)
+  * [Using Docker](#using-docker)
+  * [Integration](#integration)
+* [Detectors](#detectors)
+* [Printers](#printers)
+  * [Quick Review Printers](#quick-review-printers)
+  * [In-Depth Review Printers](#in-depth-review-printers)
+* [Tools](#tools)
+* [API Documentation](#api-documentation)
+* [Getting Help](#getting-help)
+* [FAQ](#faq)
+* [License](#license)
+* [Publications](#publications)
+  * [Trail of Bits publication](#trail-of-bits-publication)
+  * [External publications](#external-publications)
 
 ## Features
 
-- Detects vulnerable Solidity code with low false positives (see the list of [trophies](./trophies.md))
-- Identifies where the error condition occurs in the source code
-- Easily integrates into continuous integration and Hardhat/Foundry builds
-- Built-in 'printers' quickly report crucial contract information
-- Detector API to write custom analyses in Python
-- Ability to analyze contracts written with Solidity >= 0.4
-- Intermediate representation ([SlithIR](https://github.com/trailofbits/slither/wiki/SlithIR)) enables simple, high-precision analyses
-- Correctly parses 99.9% of all public Solidity code
-- Average execution time of less than 1 second per contract
-- Integrates with Github's code scanning in [CI](https://github.com/marketplace/actions/slither-action)
+* Detects vulnerable Solidity code with low false positives (see the list of [trophies](./trophies.md))
+* Identifies where the error condition occurs in the source code
+* Easily integrates into continuous integration and Hardhat/Foundry builds
+* Built-in 'printers' quickly report crucial contract information
+* Detector API to write custom analyses in Python
+* Ability to analyze contracts written with Solidity >= 0.4
+* Intermediate representation ([SlithIR](https://github.com/trailofbits/slither/wiki/SlithIR)) enables simple, high-precision analyses
+* Correctly parses 99.9% of all public Solidity code
+* Average execution time of less than 1 second per contract
+* Integrates with Github's code scanning in [CI](https://github.com/marketplace/actions/slither-action)
 
 ## Usage
 
 Run Slither on a Hardhat/Foundry/Dapp/Brownie application:
 
-```bash
+```console
 slither .
 ```
 
 This is the preferred option if your project has dependencies as Slither relies on the underlying compilation framework to compile source code.
 
 However, you can run Slither on a single file that does not import dependencies:
 
-```bash
+```console
 slither tests/uninitialized.sol
 ```
 
 ## How to install
 
-Slither requires Python 3.8+.
+> **Note** <br />
+> Slither requires Python 3.8+.
 If you're **not** going to use one of the [supported compilation frameworks](https://github.com/crytic/crytic-compile), you need [solc](https://github.com/ethereum/solidity/), the Solidity compiler; we recommend using [solc-select](https://github.com/crytic/solc-select) to conveniently switch between solc versions.
 
 ### Using Pip
 
-```bash
+```console
 pip3 install slither-analyzer
 ```
 
 ### Using Git
 
 ```bash
 git clone https://github.com/crytic/slither.git && cd slither
@@ -95,17 +111,17 @@
 
 ```bash
 docker run -it -v /home/share:/share trailofbits/eth-security-toolbox
 ```
 
 ### Integration
 
-- For GitHub action integration, use [slither-action](https://github.com/marketplace/actions/slither-action).
-- To generate a Markdown report, use `slither [target] --checklist`.
-- To generate a Markdown with GitHub source code highlighting, use `slither [target] --checklist --markdown-root https://github.com/ORG/REPO/blob/COMMIT/` (replace `ORG`, `REPO`, `COMMIT`)
+* For GitHub action integration, use [slither-action](https://github.com/marketplace/actions/slither-action).
+* To generate a Markdown report, use `slither [target] --checklist`.
+* To generate a Markdown with GitHub source code highlighting, use `slither [target] --checklist --markdown-root https://github.com/ORG/REPO/blob/COMMIT/` (replace `ORG`, `REPO`, `COMMIT`)
 
 ## Detectors
 
 Num | Detector | What it Detects | Impact | Confidence
 --- | --- | --- | --- | ---
 1 | `abiencoderv2-array` | [Storage abiencoderv2 array](https://github.com/crytic/slither/wiki/Detector-Documentation#storage-abiencoderv2-array) | High | High
 2 | `arbitrary-send-erc20` | [transferFrom uses arbitrary `from`](https://github.com/crytic/slither/wiki/Detector-Documentation#arbitrary-from-in-transferfrom) | High | High
@@ -193,90 +209,91 @@
 84 | `constable-states` | [State variables that could be declared constant](https://github.com/crytic/slither/wiki/Detector-Documentation#state-variables-that-could-be-declared-constant) | Optimization | High
 85 | `external-function` | [Public function that could be declared external](https://github.com/crytic/slither/wiki/Detector-Documentation#public-function-that-could-be-declared-external) | Optimization | High
 86 | `immutable-states` | [State variables that could be declared immutable](https://github.com/crytic/slither/wiki/Detector-Documentation#state-variables-that-could-be-declared-immutable) | Optimization | High
 87 | `var-read-using-this` | [Contract reads its own variable using `this`](https://github.com/crytic/slither/wiki/Detector-Documentation#public-variable-read-in-external-context) | Optimization | High
 
 For more information, see
 
-- The [Detector Documentation](https://github.com/crytic/slither/wiki/Detector-Documentation) for details on each detector
-- The [Detection Selection](https://github.com/crytic/slither/wiki/Usage#detector-selection) to run only selected detectors. By default, all the detectors are run.
-- The [Triage Mode](https://github.com/crytic/slither/wiki/Usage#triage-mode) to filter individual results
+* The [Detector Documentation](https://github.com/crytic/slither/wiki/Detector-Documentation) for details on each detector
+* The [Detection Selection](https://github.com/crytic/slither/wiki/Usage#detector-selection) to run only selected detectors. By default, all the detectors are run.
+* The [Triage Mode](https://github.com/crytic/slither/wiki/Usage#triage-mode) to filter individual results
 
 ## Printers
+
 ### Quick Review Printers
-- `human-summary`: [Print a human-readable summary of the contracts](https://github.com/trailofbits/slither/wiki/Printer-documentation#human-summary)
-- `inheritance-graph`: [Export the inheritance graph of each contract to a dot file](https://github.com/trailofbits/slither/wiki/Printer-documentation#inheritance-graph)
-- `contract-summary`: [Print a summary of the contracts](https://github.com/trailofbits/slither/wiki/Printer-documentation#contract-summary)
-- `loc`: [Count the total number lines of code (LOC), source lines of code (SLOC), and comment lines of code (CLOC) found in source files (SRC), dependencies (DEP), and test files (TEST).](https://github.com/trailofbits/slither/wiki/Printer-documentation#loc)
+* `human-summary`: [Print a human-readable summary of the contracts](https://github.com/trailofbits/slither/wiki/Printer-documentation#human-summary)
+* `inheritance-graph`: [Export the inheritance graph of each contract to a dot file](https://github.com/trailofbits/slither/wiki/Printer-documentation#inheritance-graph)
+* `contract-summary`: [Print a summary of the contracts](https://github.com/trailofbits/slither/wiki/Printer-documentation#contract-summary)
+* `loc`: [Count the total number lines of code (LOC), source lines of code (SLOC), and comment lines of code (CLOC) found in source files (SRC), dependencies (DEP), and test files (TEST).](https://github.com/trailofbits/slither/wiki/Printer-documentation#loc)
 
 ### In-Depth Review Printers
-- `call-graph`: [Export the call-graph of the contracts to a dot file](https://github.com/trailofbits/slither/wiki/Printer-documentation#call-graph)
-- `cfg`: [Export the CFG of each functions](https://github.com/trailofbits/slither/wiki/Printer-documentation#cfg)
-- `function-summary`: [Print a summary of the functions](https://github.com/trailofbits/slither/wiki/Printer-documentation#function-summary)
-- `vars-and-auth`: [Print the state variables written and the authorization of the functions](https://github.com/crytic/slither/wiki/Printer-documentation#variables-written-and-authorization)
-- `not-pausable`: [Print functions that do not use `whenNotPaused` modifier](https://github.com/trailofbits/slither/wiki/Printer-documentation#when-not-paused).
+* `call-graph`: [Export the call-graph of the contracts to a dot file](https://github.com/trailofbits/slither/wiki/Printer-documentation#call-graph)
+* `cfg`: [Export the CFG of each functions](https://github.com/trailofbits/slither/wiki/Printer-documentation#cfg)
+* `function-summary`: [Print a summary of the functions](https://github.com/trailofbits/slither/wiki/Printer-documentation#function-summary)
+* `vars-and-auth`: [Print the state variables written and the authorization of the functions](https://github.com/crytic/slither/wiki/Printer-documentation#variables-written-and-authorization)
+* `not-pausable`: [Print functions that do not use `whenNotPaused` modifier](https://github.com/trailofbits/slither/wiki/Printer-documentation#when-not-paused).
 
 To run a printer, use `--print` and a comma-separated list of printers.
 
 See the [Printer documentation](https://github.com/crytic/slither/wiki/Printer-documentation) for the complete lists.
 
 ## Tools
 
-- `slither-check-upgradeability`: [Review `delegatecall`-based upgradeability](https://github.com/crytic/slither/wiki/Upgradeability-Checks)
-- `slither-prop`: [Automatic unit test and property generation](https://github.com/crytic/slither/wiki/Property-generation)
-- `slither-flat`: [Flatten a codebase](https://github.com/crytic/slither/wiki/Contract-Flattening)
-- `slither-check-erc`: [Check the ERC's conformance](https://github.com/crytic/slither/wiki/ERC-Conformance)
-- `slither-format`: [Automatic patch generation](https://github.com/crytic/slither/wiki/Slither-format)
-- `slither-read-storage`: [Read storage values from contracts](./slither/tools/read_storage/README.md)
-- `slither-interface`: [Generate an interface for a contract](./slither/tools/interface/README.md)
+* `slither-check-upgradeability`: [Review `delegatecall`-based upgradeability](https://github.com/crytic/slither/wiki/Upgradeability-Checks)
+* `slither-prop`: [Automatic unit test and property generation](https://github.com/crytic/slither/wiki/Property-generation)
+* `slither-flat`: [Flatten a codebase](https://github.com/crytic/slither/wiki/Contract-Flattening)
+* `slither-check-erc`: [Check the ERC's conformance](https://github.com/crytic/slither/wiki/ERC-Conformance)
+* `slither-format`: [Automatic patch generation](https://github.com/crytic/slither/wiki/Slither-format)
+* `slither-read-storage`: [Read storage values from contracts](./slither/tools/read_storage/README.md)
+* `slither-interface`: [Generate an interface for a contract](./slither/tools/interface/README.md)
 
 See the [Tool documentation](https://github.com/crytic/slither/wiki/Tool-Documentation) for additional tools.
 
 [Contact us](https://www.trailofbits.com/contact/) to get help on building custom tools.
 
 ## API Documentation
 
 Documentation on Slither's internals is available [here](https://crytic.github.io/slither/slither.html).
 
 ## Getting Help
 
 Feel free to stop by our [Slack channel](https://empireslacking.herokuapp.com) (#ethereum) for help using or extending Slither.
 
-- The [Printer documentation](https://github.com/trailofbits/slither/wiki/Printer-documentation) describes the information Slither is capable of visualizing for each contract.
+* The [Printer documentation](https://github.com/trailofbits/slither/wiki/Printer-documentation) describes the information Slither is capable of visualizing for each contract.
 
-- The [Detector documentation](https://github.com/trailofbits/slither/wiki/Adding-a-new-detector) describes how to write a new vulnerability analyses.
+* The [Detector documentation](https://github.com/trailofbits/slither/wiki/Adding-a-new-detector) describes how to write a new vulnerability analyses.
 
-- The [API documentation](https://github.com/crytic/slither/wiki/Python-API) describes the methods and objects available for custom analyses.
+* The [API documentation](https://github.com/crytic/slither/wiki/Python-API) describes the methods and objects available for custom analyses.
 
-- The [SlithIR documentation](https://github.com/trailofbits/slither/wiki/SlithIR) describes the SlithIR intermediate representation.
+* The [SlithIR documentation](https://github.com/trailofbits/slither/wiki/SlithIR) describes the SlithIR intermediate representation.
 
 ## FAQ
 
 How do I exclude mocks or tests?
 
-- View our documentation on [path filtering](https://github.com/crytic/slither/wiki/Usage#path-filtering).
+* View our documentation on [path filtering](https://github.com/crytic/slither/wiki/Usage#path-filtering).
 
 How do I fix "unknown file" or compilation issues?
 
-- Because slither requires the solc AST, it must have all dependencies available.
+* Because slither requires the solc AST, it must have all dependencies available.
 If a contract has dependencies, `slither contract.sol` will fail.
 Instead, use `slither .` in the parent directory of `contracts/` (you should see `contracts/` when you run `ls`).
 If you have a `node_modules/` folder, it must be in the same directory as `contracts/`. To verify that this issue is related to slither,
 run the compilation command for the framework you are using e.g `npx hardhat compile`. That must work successfully;
 otherwise, slither's compilation engine, crytic-compile, cannot generate the AST.
 
 ## License
 
 Slither is licensed and distributed under the AGPLv3 license. [Contact us](mailto:opensource@trailofbits.com) if you're looking for an exception to the terms.
 
 ## Publications
 
 ### Trail of Bits publication
 
-- [Slither: A Static Analysis Framework For Smart Contracts](https://arxiv.org/abs/1908.09878), Josselin Feist, Gustavo Grieco, Alex Groce - WETSEB '19
+* [Slither: A Static Analysis Framework For Smart Contracts](https://arxiv.org/abs/1908.09878), Josselin Feist, Gustavo Grieco, Alex Groce - WETSEB '19
 
 ### External publications
 
 Title | Usage | Authors | Venue | Code
 --- | --- | --- | --- | ---
 [ReJection: A AST-Based Reentrancy Vulnerability Detection Method](https://www.researchgate.net/publication/339354823_ReJection_A_AST-Based_Reentrancy_Vulnerability_Detection_Method) | AST-based analysis built on top of Slither | Rui Ma, Zefeng Jian, Guangyuan Chen, Ke Ma, Yujia Chen | CTCIS 19
 [MPro: Combining Static and Symbolic Analysis forScalable Testing of Smart Contract](https://arxiv.org/pdf/1911.00570.pdf) | Leverage data dependency through Slither | William Zhang, Sebastian Banescu, Leodardo Pasos, Steven Stewart, Vijay Ganesh | ISSRE 2019 | [MPro](https://github.com/QuanZhang-William/M-Pro)
```

### Comparing `slither-analyzer-0.9.5/README.md` & `slither-analyzer-0.9.6/slither_analyzer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,65 +1,96 @@
-# Slither, the Solidity source analyzer
+Metadata-Version: 2.1
+Name: slither-analyzer
+Version: 0.9.6
+Summary: Slither is a Solidity static analysis framework written in Python 3.
+Home-page: https://github.com/crytic/slither
+Author: Trail of Bits
+License: AGPL-3.0
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: lint
+Provides-Extra: test
+Provides-Extra: doc
+Provides-Extra: dev
+License-File: LICENSE
 
-<img src="https://raw.githubusercontent.com/crytic/slither/master/logo.png" alt="Logo" width="500"/>
+# [Slither, the Solidity source analyzer](https://crytic.github.io/slither/slither.html)
 
-[![Build Status](https://img.shields.io/github/actions/workflow/status/crytic/slither/ci.yml?branch=master)](https://github.com/crytic/slither/actions?query=workflow%3ACI)
-[![Slack Status](https://empireslacking.herokuapp.com/badge.svg)](https://empireslacking.herokuapp.com)
-[![PyPI version](https://badge.fury.io/py/slither-analyzer.svg)](https://badge.fury.io/py/slither-analyzer)
-
-Slither is a Solidity static analysis framework written in Python3. It runs a suite of vulnerability detectors, prints visual information about contract details, and provides an API to easily write custom analyses. Slither enables developers to find vulnerabilities, enhance their code comprehension, and quickly prototype custom analyses.
+<img src="https://raw.githubusercontent.com/crytic/slither/master/logo.png" alt="Slither Static Analysis Framework Logo" width="500" />
 
-- [Features](#features)
-- [Usage](#usage)
-- [How to Install](#how-to-install)
-- [Detectors](#detectors)
-- [Printers](#printers)
-- [Tools](#tools)
-- [API Documentation](#api-documentation)
-- [Getting Help](#getting-help)
-- [FAQ](#faq)
-- [Publications](#publications)
+[![Build Status](https://img.shields.io/github/actions/workflow/status/crytic/slither/ci.yml?branch=master)](https://github.com/crytic/slither/actions?query=workflow%3ACI)
+![PyPI](https://img.shields.io/pypi/v/slither-analyzer?logo=python&logoColor=white&label=slither-analyzer)
+[![Slither - Read the Docs](https://img.shields.io/badge/Slither-Read_the_Docs-2ea44f)](https://crytic.github.io/slither/slither.html)
+[![Slither - Wiki](https://img.shields.io/badge/Slither-Wiki-2ea44f)](https://github.com/crytic/slither/wiki/SlithIR)
+
+> Join the Empire Hacking Slack  
+>
+> [![Slack Status](https://slack.empirehacking.nyc/badge.svg)](https://slack.empirehacking.nyc/)
+> > <sub><i>- Discussions and Support </i></sub>
+
+**Slither** is a Solidity static analysis framework written in Python3. It runs a suite of vulnerability detectors, prints visual information about contract details, and provides an API to easily write custom analyses. Slither enables developers to find vulnerabilities, enhance their code comprehension, and quickly prototype custom analyses.
+
+* [Features](#features)
+* [Usage](#usage)
+* [How to install](#how-to-install)
+  * [Using Pip](#using-pip)
+  * [Using Git](#using-git)
+  * [Using Docker](#using-docker)
+  * [Integration](#integration)
+* [Detectors](#detectors)
+* [Printers](#printers)
+  * [Quick Review Printers](#quick-review-printers)
+  * [In-Depth Review Printers](#in-depth-review-printers)
+* [Tools](#tools)
+* [API Documentation](#api-documentation)
+* [Getting Help](#getting-help)
+* [FAQ](#faq)
+* [License](#license)
+* [Publications](#publications)
+  * [Trail of Bits publication](#trail-of-bits-publication)
+  * [External publications](#external-publications)
 
 ## Features
 
-- Detects vulnerable Solidity code with low false positives (see the list of [trophies](./trophies.md))
-- Identifies where the error condition occurs in the source code
-- Easily integrates into continuous integration and Hardhat/Foundry builds
-- Built-in 'printers' quickly report crucial contract information
-- Detector API to write custom analyses in Python
-- Ability to analyze contracts written with Solidity >= 0.4
-- Intermediate representation ([SlithIR](https://github.com/trailofbits/slither/wiki/SlithIR)) enables simple, high-precision analyses
-- Correctly parses 99.9% of all public Solidity code
-- Average execution time of less than 1 second per contract
-- Integrates with Github's code scanning in [CI](https://github.com/marketplace/actions/slither-action)
+* Detects vulnerable Solidity code with low false positives (see the list of [trophies](./trophies.md))
+* Identifies where the error condition occurs in the source code
+* Easily integrates into continuous integration and Hardhat/Foundry builds
+* Built-in 'printers' quickly report crucial contract information
+* Detector API to write custom analyses in Python
+* Ability to analyze contracts written with Solidity >= 0.4
+* Intermediate representation ([SlithIR](https://github.com/trailofbits/slither/wiki/SlithIR)) enables simple, high-precision analyses
+* Correctly parses 99.9% of all public Solidity code
+* Average execution time of less than 1 second per contract
+* Integrates with Github's code scanning in [CI](https://github.com/marketplace/actions/slither-action)
 
 ## Usage
 
 Run Slither on a Hardhat/Foundry/Dapp/Brownie application:
 
-```bash
+```console
 slither .
 ```
 
 This is the preferred option if your project has dependencies as Slither relies on the underlying compilation framework to compile source code.
 
 However, you can run Slither on a single file that does not import dependencies:
 
-```bash
+```console
 slither tests/uninitialized.sol
 ```
 
 ## How to install
 
-Slither requires Python 3.8+.
+> **Note** <br />
+> Slither requires Python 3.8+.
 If you're **not** going to use one of the [supported compilation frameworks](https://github.com/crytic/crytic-compile), you need [solc](https://github.com/ethereum/solidity/), the Solidity compiler; we recommend using [solc-select](https://github.com/crytic/solc-select) to conveniently switch between solc versions.
 
 ### Using Pip
 
-```bash
+```console
 pip3 install slither-analyzer
 ```
 
 ### Using Git
 
 ```bash
 git clone https://github.com/crytic/slither.git && cd slither
@@ -80,17 +111,17 @@
 
 ```bash
 docker run -it -v /home/share:/share trailofbits/eth-security-toolbox
 ```
 
 ### Integration
 
-- For GitHub action integration, use [slither-action](https://github.com/marketplace/actions/slither-action).
-- To generate a Markdown report, use `slither [target] --checklist`.
-- To generate a Markdown with GitHub source code highlighting, use `slither [target] --checklist --markdown-root https://github.com/ORG/REPO/blob/COMMIT/` (replace `ORG`, `REPO`, `COMMIT`)
+* For GitHub action integration, use [slither-action](https://github.com/marketplace/actions/slither-action).
+* To generate a Markdown report, use `slither [target] --checklist`.
+* To generate a Markdown with GitHub source code highlighting, use `slither [target] --checklist --markdown-root https://github.com/ORG/REPO/blob/COMMIT/` (replace `ORG`, `REPO`, `COMMIT`)
 
 ## Detectors
 
 Num | Detector | What it Detects | Impact | Confidence
 --- | --- | --- | --- | ---
 1 | `abiencoderv2-array` | [Storage abiencoderv2 array](https://github.com/crytic/slither/wiki/Detector-Documentation#storage-abiencoderv2-array) | High | High
 2 | `arbitrary-send-erc20` | [transferFrom uses arbitrary `from`](https://github.com/crytic/slither/wiki/Detector-Documentation#arbitrary-from-in-transferfrom) | High | High
@@ -178,90 +209,91 @@
 84 | `constable-states` | [State variables that could be declared constant](https://github.com/crytic/slither/wiki/Detector-Documentation#state-variables-that-could-be-declared-constant) | Optimization | High
 85 | `external-function` | [Public function that could be declared external](https://github.com/crytic/slither/wiki/Detector-Documentation#public-function-that-could-be-declared-external) | Optimization | High
 86 | `immutable-states` | [State variables that could be declared immutable](https://github.com/crytic/slither/wiki/Detector-Documentation#state-variables-that-could-be-declared-immutable) | Optimization | High
 87 | `var-read-using-this` | [Contract reads its own variable using `this`](https://github.com/crytic/slither/wiki/Detector-Documentation#public-variable-read-in-external-context) | Optimization | High
 
 For more information, see
 
-- The [Detector Documentation](https://github.com/crytic/slither/wiki/Detector-Documentation) for details on each detector
-- The [Detection Selection](https://github.com/crytic/slither/wiki/Usage#detector-selection) to run only selected detectors. By default, all the detectors are run.
-- The [Triage Mode](https://github.com/crytic/slither/wiki/Usage#triage-mode) to filter individual results
+* The [Detector Documentation](https://github.com/crytic/slither/wiki/Detector-Documentation) for details on each detector
+* The [Detection Selection](https://github.com/crytic/slither/wiki/Usage#detector-selection) to run only selected detectors. By default, all the detectors are run.
+* The [Triage Mode](https://github.com/crytic/slither/wiki/Usage#triage-mode) to filter individual results
 
 ## Printers
+
 ### Quick Review Printers
-- `human-summary`: [Print a human-readable summary of the contracts](https://github.com/trailofbits/slither/wiki/Printer-documentation#human-summary)
-- `inheritance-graph`: [Export the inheritance graph of each contract to a dot file](https://github.com/trailofbits/slither/wiki/Printer-documentation#inheritance-graph)
-- `contract-summary`: [Print a summary of the contracts](https://github.com/trailofbits/slither/wiki/Printer-documentation#contract-summary)
-- `loc`: [Count the total number lines of code (LOC), source lines of code (SLOC), and comment lines of code (CLOC) found in source files (SRC), dependencies (DEP), and test files (TEST).](https://github.com/trailofbits/slither/wiki/Printer-documentation#loc)
+* `human-summary`: [Print a human-readable summary of the contracts](https://github.com/trailofbits/slither/wiki/Printer-documentation#human-summary)
+* `inheritance-graph`: [Export the inheritance graph of each contract to a dot file](https://github.com/trailofbits/slither/wiki/Printer-documentation#inheritance-graph)
+* `contract-summary`: [Print a summary of the contracts](https://github.com/trailofbits/slither/wiki/Printer-documentation#contract-summary)
+* `loc`: [Count the total number lines of code (LOC), source lines of code (SLOC), and comment lines of code (CLOC) found in source files (SRC), dependencies (DEP), and test files (TEST).](https://github.com/trailofbits/slither/wiki/Printer-documentation#loc)
 
 ### In-Depth Review Printers
-- `call-graph`: [Export the call-graph of the contracts to a dot file](https://github.com/trailofbits/slither/wiki/Printer-documentation#call-graph)
-- `cfg`: [Export the CFG of each functions](https://github.com/trailofbits/slither/wiki/Printer-documentation#cfg)
-- `function-summary`: [Print a summary of the functions](https://github.com/trailofbits/slither/wiki/Printer-documentation#function-summary)
-- `vars-and-auth`: [Print the state variables written and the authorization of the functions](https://github.com/crytic/slither/wiki/Printer-documentation#variables-written-and-authorization)
-- `not-pausable`: [Print functions that do not use `whenNotPaused` modifier](https://github.com/trailofbits/slither/wiki/Printer-documentation#when-not-paused).
+* `call-graph`: [Export the call-graph of the contracts to a dot file](https://github.com/trailofbits/slither/wiki/Printer-documentation#call-graph)
+* `cfg`: [Export the CFG of each functions](https://github.com/trailofbits/slither/wiki/Printer-documentation#cfg)
+* `function-summary`: [Print a summary of the functions](https://github.com/trailofbits/slither/wiki/Printer-documentation#function-summary)
+* `vars-and-auth`: [Print the state variables written and the authorization of the functions](https://github.com/crytic/slither/wiki/Printer-documentation#variables-written-and-authorization)
+* `not-pausable`: [Print functions that do not use `whenNotPaused` modifier](https://github.com/trailofbits/slither/wiki/Printer-documentation#when-not-paused).
 
 To run a printer, use `--print` and a comma-separated list of printers.
 
 See the [Printer documentation](https://github.com/crytic/slither/wiki/Printer-documentation) for the complete lists.
 
 ## Tools
 
-- `slither-check-upgradeability`: [Review `delegatecall`-based upgradeability](https://github.com/crytic/slither/wiki/Upgradeability-Checks)
-- `slither-prop`: [Automatic unit test and property generation](https://github.com/crytic/slither/wiki/Property-generation)
-- `slither-flat`: [Flatten a codebase](https://github.com/crytic/slither/wiki/Contract-Flattening)
-- `slither-check-erc`: [Check the ERC's conformance](https://github.com/crytic/slither/wiki/ERC-Conformance)
-- `slither-format`: [Automatic patch generation](https://github.com/crytic/slither/wiki/Slither-format)
-- `slither-read-storage`: [Read storage values from contracts](./slither/tools/read_storage/README.md)
-- `slither-interface`: [Generate an interface for a contract](./slither/tools/interface/README.md)
+* `slither-check-upgradeability`: [Review `delegatecall`-based upgradeability](https://github.com/crytic/slither/wiki/Upgradeability-Checks)
+* `slither-prop`: [Automatic unit test and property generation](https://github.com/crytic/slither/wiki/Property-generation)
+* `slither-flat`: [Flatten a codebase](https://github.com/crytic/slither/wiki/Contract-Flattening)
+* `slither-check-erc`: [Check the ERC's conformance](https://github.com/crytic/slither/wiki/ERC-Conformance)
+* `slither-format`: [Automatic patch generation](https://github.com/crytic/slither/wiki/Slither-format)
+* `slither-read-storage`: [Read storage values from contracts](./slither/tools/read_storage/README.md)
+* `slither-interface`: [Generate an interface for a contract](./slither/tools/interface/README.md)
 
 See the [Tool documentation](https://github.com/crytic/slither/wiki/Tool-Documentation) for additional tools.
 
 [Contact us](https://www.trailofbits.com/contact/) to get help on building custom tools.
 
 ## API Documentation
 
 Documentation on Slither's internals is available [here](https://crytic.github.io/slither/slither.html).
 
 ## Getting Help
 
 Feel free to stop by our [Slack channel](https://empireslacking.herokuapp.com) (#ethereum) for help using or extending Slither.
 
-- The [Printer documentation](https://github.com/trailofbits/slither/wiki/Printer-documentation) describes the information Slither is capable of visualizing for each contract.
+* The [Printer documentation](https://github.com/trailofbits/slither/wiki/Printer-documentation) describes the information Slither is capable of visualizing for each contract.
 
-- The [Detector documentation](https://github.com/trailofbits/slither/wiki/Adding-a-new-detector) describes how to write a new vulnerability analyses.
+* The [Detector documentation](https://github.com/trailofbits/slither/wiki/Adding-a-new-detector) describes how to write a new vulnerability analyses.
 
-- The [API documentation](https://github.com/crytic/slither/wiki/Python-API) describes the methods and objects available for custom analyses.
+* The [API documentation](https://github.com/crytic/slither/wiki/Python-API) describes the methods and objects available for custom analyses.
 
-- The [SlithIR documentation](https://github.com/trailofbits/slither/wiki/SlithIR) describes the SlithIR intermediate representation.
+* The [SlithIR documentation](https://github.com/trailofbits/slither/wiki/SlithIR) describes the SlithIR intermediate representation.
 
 ## FAQ
 
 How do I exclude mocks or tests?
 
-- View our documentation on [path filtering](https://github.com/crytic/slither/wiki/Usage#path-filtering).
+* View our documentation on [path filtering](https://github.com/crytic/slither/wiki/Usage#path-filtering).
 
 How do I fix "unknown file" or compilation issues?
 
-- Because slither requires the solc AST, it must have all dependencies available.
+* Because slither requires the solc AST, it must have all dependencies available.
 If a contract has dependencies, `slither contract.sol` will fail.
 Instead, use `slither .` in the parent directory of `contracts/` (you should see `contracts/` when you run `ls`).
 If you have a `node_modules/` folder, it must be in the same directory as `contracts/`. To verify that this issue is related to slither,
 run the compilation command for the framework you are using e.g `npx hardhat compile`. That must work successfully;
 otherwise, slither's compilation engine, crytic-compile, cannot generate the AST.
 
 ## License
 
 Slither is licensed and distributed under the AGPLv3 license. [Contact us](mailto:opensource@trailofbits.com) if you're looking for an exception to the terms.
 
 ## Publications
 
 ### Trail of Bits publication
 
-- [Slither: A Static Analysis Framework For Smart Contracts](https://arxiv.org/abs/1908.09878), Josselin Feist, Gustavo Grieco, Alex Groce - WETSEB '19
+* [Slither: A Static Analysis Framework For Smart Contracts](https://arxiv.org/abs/1908.09878), Josselin Feist, Gustavo Grieco, Alex Groce - WETSEB '19
 
 ### External publications
 
 Title | Usage | Authors | Venue | Code
 --- | --- | --- | --- | ---
 [ReJection: A AST-Based Reentrancy Vulnerability Detection Method](https://www.researchgate.net/publication/339354823_ReJection_A_AST-Based_Reentrancy_Vulnerability_Detection_Method) | AST-based analysis built on top of Slither | Rui Ma, Zefeng Jian, Guangyuan Chen, Ke Ma, Yujia Chen | CTCIS 19
 [MPro: Combining Static and Symbolic Analysis forScalable Testing of Smart Contract](https://arxiv.org/pdf/1911.00570.pdf) | Leverage data dependency through Slither | William Zhang, Sebastian Banescu, Leodardo Pasos, Steven Stewart, Vijay Ganesh | ISSRE 2019 | [MPro](https://github.com/QuanZhang-William/M-Pro)
```

### Comparing `slither-analyzer-0.9.5/setup.py` & `slither-analyzer-0.9.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,22 @@
     long_description = f.read()
 
 setup(
     name="slither-analyzer",
     description="Slither is a Solidity static analysis framework written in Python 3.",
     url="https://github.com/crytic/slither",
     author="Trail of Bits",
-    version="0.9.5",
+    version="0.9.6",
     packages=find_packages(),
     python_requires=">=3.8",
     install_requires=[
         "packaging",
         "prettytable>=3.3.0",
         "pycryptodome>=3.4.6",
-        "crytic-compile>=0.3.2,<0.4.0",
+        "crytic-compile>=0.3.3,<0.4.0",
         # "crytic-compile@git+https://github.com/crytic/crytic-compile.git@dev#egg=crytic-compile",
         "web3>=6.0.0",
         "eth-abi>=4.0.0",
         "eth-typing>=3.0.0",
         "eth-utils>=2.1.0",
     ],
     extras_require={
@@ -32,15 +32,14 @@
             "pytest-cov",
             "pytest-xdist",
             "deepdiff",
             "numpy",
             "coverage[toml]",
             "filelock",
             "pytest-insta",
-            "solc-select>=1.0.4",
         ],
         "doc": [
             "pdoc",
         ],
         "dev": [
             "slither-analyzer[lint,test,doc]",
             "openai",
```

### Comparing `slither-analyzer-0.9.5/slither/__main__.py` & `slither-analyzer-0.9.6/slither/__main__.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/analyses/data_dependency/data_dependency.py` & `slither-analyzer-0.9.6/slither/analyses/data_dependency/data_dependency.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/analyses/evm/convert.py` & `slither-analyzer-0.9.6/slither/analyses/evm/convert.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/analyses/evm/evm_cfg_builder.py` & `slither-analyzer-0.9.6/slither/analyses/evm/evm_cfg_builder.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/analyses/write/are_variables_written.py` & `slither-analyzer-0.9.6/slither/analyses/write/are_variables_written.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/cfg/node.py` & `slither-analyzer-0.9.6/slither/core/cfg/node.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/compilation_unit.py` & `slither-analyzer-0.9.6/slither/core/compilation_unit.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/declarations/__init__.py` & `slither-analyzer-0.9.6/slither/core/declarations/__init__.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/declarations/contract.py` & `slither-analyzer-0.9.6/slither/core/declarations/contract.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/declarations/contract_level.py` & `slither-analyzer-0.9.6/slither/core/declarations/contract_level.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/declarations/custom_error.py` & `slither-analyzer-0.9.6/slither/core/declarations/custom_error.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/declarations/custom_error_contract.py` & `slither-analyzer-0.9.6/slither/core/declarations/custom_error_contract.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/declarations/custom_error_top_level.py` & `slither-analyzer-0.9.6/slither/core/declarations/custom_error_top_level.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/declarations/enum.py` & `slither-analyzer-0.9.6/slither/core/declarations/enum.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/declarations/event.py` & `slither-analyzer-0.9.6/slither/core/declarations/event.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/declarations/function.py` & `slither-analyzer-0.9.6/slither/core/declarations/function.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/declarations/function_contract.py` & `slither-analyzer-0.9.6/slither/core/declarations/function_contract.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/declarations/function_top_level.py` & `slither-analyzer-0.9.6/slither/core/declarations/function_top_level.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/declarations/import_directive.py` & `slither-analyzer-0.9.6/slither/core/declarations/import_directive.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/declarations/pragma_directive.py` & `slither-analyzer-0.9.6/slither/core/declarations/pragma_directive.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/declarations/solidity_import_placeholder.py` & `slither-analyzer-0.9.6/slither/core/declarations/solidity_import_placeholder.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/declarations/solidity_variables.py` & `slither-analyzer-0.9.6/slither/core/declarations/solidity_variables.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/declarations/structure.py` & `slither-analyzer-0.9.6/slither/core/declarations/structure.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/declarations/using_for_top_level.py` & `slither-analyzer-0.9.6/slither/core/declarations/using_for_top_level.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/dominators/node_dominator_tree.py` & `slither-analyzer-0.9.6/slither/core/dominators/node_dominator_tree.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/dominators/utils.py` & `slither-analyzer-0.9.6/slither/core/dominators/utils.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/expressions/__init__.py` & `slither-analyzer-0.9.6/slither/core/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/expressions/assignment_operation.py` & `slither-analyzer-0.9.6/slither/core/expressions/assignment_operation.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/expressions/binary_operation.py` & `slither-analyzer-0.9.6/slither/core/expressions/binary_operation.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/expressions/call_expression.py` & `slither-analyzer-0.9.6/slither/core/expressions/call_expression.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/expressions/conditional_expression.py` & `slither-analyzer-0.9.6/slither/core/expressions/conditional_expression.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/expressions/elementary_type_name_expression.py` & `slither-analyzer-0.9.6/slither/core/expressions/elementary_type_name_expression.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/expressions/identifier.py` & `slither-analyzer-0.9.6/slither/core/expressions/identifier.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/expressions/index_access.py` & `slither-analyzer-0.9.6/slither/core/expressions/index_access.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/expressions/literal.py` & `slither-analyzer-0.9.6/slither/core/expressions/literal.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/expressions/member_access.py` & `slither-analyzer-0.9.6/slither/core/expressions/member_access.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/expressions/new_array.py` & `slither-analyzer-0.9.6/slither/core/expressions/new_array.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/expressions/new_contract.py` & `slither-analyzer-0.9.6/slither/core/expressions/new_contract.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/expressions/tuple_expression.py` & `slither-analyzer-0.9.6/slither/core/expressions/tuple_expression.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/expressions/type_conversion.py` & `slither-analyzer-0.9.6/slither/core/expressions/type_conversion.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/expressions/unary_operation.py` & `slither-analyzer-0.9.6/slither/core/expressions/unary_operation.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/scope/scope.py` & `slither-analyzer-0.9.6/slither/core/scope/scope.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/slither_core.py` & `slither-analyzer-0.9.6/slither/core/slither_core.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/solidity_types/array_type.py` & `slither-analyzer-0.9.6/slither/core/solidity_types/array_type.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/solidity_types/elementary_type.py` & `slither-analyzer-0.9.6/slither/core/solidity_types/elementary_type.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/solidity_types/function_type.py` & `slither-analyzer-0.9.6/slither/core/solidity_types/function_type.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/solidity_types/mapping_type.py` & `slither-analyzer-0.9.6/slither/core/solidity_types/mapping_type.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/solidity_types/type.py` & `slither-analyzer-0.9.6/slither/core/solidity_types/type.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/solidity_types/type_alias.py` & `slither-analyzer-0.9.6/slither/core/solidity_types/type_alias.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/solidity_types/type_information.py` & `slither-analyzer-0.9.6/slither/core/solidity_types/type_information.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/solidity_types/user_defined_type.py` & `slither-analyzer-0.9.6/slither/core/solidity_types/user_defined_type.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/source_mapping/source_mapping.py` & `slither-analyzer-0.9.6/slither/core/source_mapping/source_mapping.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/variables/event_variable.py` & `slither-analyzer-0.9.6/slither/core/variables/event_variable.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/variables/local_variable.py` & `slither-analyzer-0.9.6/slither/core/variables/local_variable.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/variables/local_variable_init_from_tuple.py` & `slither-analyzer-0.9.6/slither/core/variables/local_variable_init_from_tuple.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/variables/state_variable.py` & `slither-analyzer-0.9.6/slither/core/variables/state_variable.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/variables/top_level_variable.py` & `slither-analyzer-0.9.6/slither/core/variables/top_level_variable.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/core/variables/variable.py` & `slither-analyzer-0.9.6/slither/core/variables/variable.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/abstract_detector.py` & `slither-analyzer-0.9.6/slither/detectors/abstract_detector.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/all_detectors.py` & `slither-analyzer-0.9.6/slither/detectors/all_detectors.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/assembly/shift_parameter_mixup.py` & `slither-analyzer-0.9.6/slither/detectors/assembly/shift_parameter_mixup.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/attributes/const_functions_asm.py` & `slither-analyzer-0.9.6/slither/detectors/attributes/const_functions_asm.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/attributes/const_functions_state.py` & `slither-analyzer-0.9.6/slither/detectors/attributes/const_functions_state.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/attributes/constant_pragma.py` & `slither-analyzer-0.9.6/slither/detectors/attributes/constant_pragma.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/attributes/incorrect_solc.py` & `slither-analyzer-0.9.6/slither/detectors/attributes/incorrect_solc.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/attributes/locked_ether.py` & `slither-analyzer-0.9.6/slither/detectors/attributes/locked_ether.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/attributes/unimplemented_interface.py` & `slither-analyzer-0.9.6/slither/detectors/attributes/unimplemented_interface.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/compiler_bugs/array_by_reference.py` & `slither-analyzer-0.9.6/slither/detectors/compiler_bugs/array_by_reference.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/compiler_bugs/enum_conversion.py` & `slither-analyzer-0.9.6/slither/detectors/compiler_bugs/enum_conversion.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/compiler_bugs/multiple_constructor_schemes.py` & `slither-analyzer-0.9.6/slither/detectors/compiler_bugs/multiple_constructor_schemes.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/compiler_bugs/public_mapping_nested.py` & `slither-analyzer-0.9.6/slither/detectors/compiler_bugs/public_mapping_nested.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/compiler_bugs/reused_base_constructor.py` & `slither-analyzer-0.9.6/slither/detectors/compiler_bugs/reused_base_constructor.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/compiler_bugs/storage_ABIEncoderV2_array.py` & `slither-analyzer-0.9.6/slither/detectors/compiler_bugs/storage_ABIEncoderV2_array.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/compiler_bugs/storage_signed_integer_array.py` & `slither-analyzer-0.9.6/slither/detectors/compiler_bugs/storage_signed_integer_array.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/compiler_bugs/uninitialized_function_ptr_in_constructor.py` & `slither-analyzer-0.9.6/slither/detectors/compiler_bugs/uninitialized_function_ptr_in_constructor.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/erc/erc20/arbitrary_send_erc20.py` & `slither-analyzer-0.9.6/slither/detectors/erc/erc20/arbitrary_send_erc20.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/erc/erc20/arbitrary_send_erc20_no_permit.py` & `slither-analyzer-0.9.6/slither/detectors/erc/erc20/arbitrary_send_erc20_no_permit.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/erc/erc20/arbitrary_send_erc20_permit.py` & `slither-analyzer-0.9.6/slither/detectors/erc/erc20/arbitrary_send_erc20_permit.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/erc/erc20/incorrect_erc20_interface.py` & `slither-analyzer-0.9.6/slither/detectors/erc/erc20/incorrect_erc20_interface.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/erc/incorrect_erc721_interface.py` & `slither-analyzer-0.9.6/slither/detectors/erc/incorrect_erc721_interface.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/erc/unindexed_event_parameters.py` & `slither-analyzer-0.9.6/slither/detectors/erc/unindexed_event_parameters.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/examples/backdoor.py` & `slither-analyzer-0.9.6/slither/detectors/examples/backdoor.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/functions/arbitrary_send_eth.py` & `slither-analyzer-0.9.6/slither/detectors/functions/arbitrary_send_eth.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/functions/codex.py` & `slither-analyzer-0.9.6/slither/detectors/functions/codex.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/functions/cyclomatic_complexity.py` & `slither-analyzer-0.9.6/slither/detectors/functions/cyclomatic_complexity.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/functions/dead_code.py` & `slither-analyzer-0.9.6/slither/detectors/functions/dead_code.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/functions/external_function.py` & `slither-analyzer-0.9.6/slither/detectors/functions/external_function.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/functions/modifier.py` & `slither-analyzer-0.9.6/slither/detectors/functions/modifier.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/functions/permit_domain_signature_collision.py` & `slither-analyzer-0.9.6/slither/detectors/functions/permit_domain_signature_collision.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/functions/protected_variable.py` & `slither-analyzer-0.9.6/slither/detectors/functions/protected_variable.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/functions/suicidal.py` & `slither-analyzer-0.9.6/slither/detectors/functions/suicidal.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/functions/unimplemented.py` & `slither-analyzer-0.9.6/slither/detectors/functions/unimplemented.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/naming_convention/naming_convention.py` & `slither-analyzer-0.9.6/slither/detectors/naming_convention/naming_convention.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/operations/bad_prng.py` & `slither-analyzer-0.9.6/slither/detectors/operations/bad_prng.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/operations/block_timestamp.py` & `slither-analyzer-0.9.6/slither/detectors/operations/block_timestamp.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/operations/cache_array_length.py` & `slither-analyzer-0.9.6/slither/detectors/operations/cache_array_length.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import List, Set
 
 from slither.core.cfg.node import Node, NodeType
 from slither.core.declarations import Function
 from slither.core.expressions import BinaryOperation, Identifier, MemberAccess, UnaryOperation
 from slither.core.solidity_types import ArrayType
-from slither.core.source_mapping.source_mapping import SourceMapping
 from slither.core.variables import StateVariable
 from slither.detectors.abstract_detector import AbstractDetector, DetectorClassification
 from slither.slithir.operations import Length, Delete, HighLevelCall
 
 
 class CacheArrayLength(AbstractDetector):
     """
@@ -130,25 +129,30 @@
                     # take into account only delete entire array, since delete array[i] doesn't change `array.length`
                     if (
                         isinstance(op.expression, UnaryOperation)
                         and isinstance(op.expression.expression, Identifier)
                         and op.expression.expression.value == array
                     ):
                         return True
-                if isinstance(op, HighLevelCall) and not op.function.view and not op.function.pure:
+                if (
+                    isinstance(op, HighLevelCall)
+                    and isinstance(op.function, Function)
+                    and not op.function.view
+                    and not op.function.pure
+                ):
                     return True
 
         for son in node.sons:
             if son not in visited:
                 if CacheArrayLength._is_loop_referencing_array_length(son, visited, array, depth):
                     return True
         return False
 
     @staticmethod
-    def _handle_loops(nodes: List[Node], non_optimal_array_len_usages: List[SourceMapping]) -> None:
+    def _handle_loops(nodes: List[Node], non_optimal_array_len_usages: List[Node]) -> None:
         """
         For each loop, checks if it has a comparison with `length` array member and, if it has, checks whether that
         array size could potentially change in that loop.
         If it cannot, the loop condition is added to `non_optimal_array_len_usages`.
         There may be some false negatives here - see docs for `_is_loop_referencing_array_length` for more information.
         """
         for node in nodes:
@@ -176,29 +180,29 @@
                 visited: Set[Node] = set()
                 if not CacheArrayLength._is_loop_referencing_array_length(
                     if_node, visited, array, 1
                 ):
                     non_optimal_array_len_usages.append(if_node)
 
     @staticmethod
-    def _get_non_optimal_array_len_usages_for_function(f: Function) -> List[SourceMapping]:
+    def _get_non_optimal_array_len_usages_for_function(f: Function) -> List[Node]:
         """
         Finds non-optimal usages of array length in loop conditions in a given function.
         """
-        non_optimal_array_len_usages: List[SourceMapping] = []
+        non_optimal_array_len_usages: List[Node] = []
         CacheArrayLength._handle_loops(f.nodes, non_optimal_array_len_usages)
 
         return non_optimal_array_len_usages
 
     @staticmethod
-    def _get_non_optimal_array_len_usages(functions: List[Function]) -> List[SourceMapping]:
+    def _get_non_optimal_array_len_usages(functions: List[Function]) -> List[Node]:
         """
         Finds non-optimal usages of array length in loop conditions in given functions.
         """
-        non_optimal_array_len_usages: List[SourceMapping] = []
+        non_optimal_array_len_usages: List[Node] = []
 
         for f in functions:
             non_optimal_array_len_usages += (
                 CacheArrayLength._get_non_optimal_array_len_usages_for_function(f)
             )
 
         return non_optimal_array_len_usages
@@ -207,15 +211,16 @@
         results = []
 
         non_optimal_array_len_usages = CacheArrayLength._get_non_optimal_array_len_usages(
             self.compilation_unit.functions
         )
         for usage in non_optimal_array_len_usages:
             info = [
-                "Loop condition at ",
-                usage,
-                " should use cached array length instead of referencing `length` member "
+                "Loop condition ",
+                f"`{usage.source_mapping.content}` ",
+                f"({usage.source_mapping}) ",
+                "should use cached array length instead of referencing `length` member "
                 "of the storage array.\n ",
             ]
             res = self.generate_result(info)
             results.append(res)
         return results
```

### Comparing `slither-analyzer-0.9.5/slither/detectors/operations/encode_packed.py` & `slither-analyzer-0.9.6/slither/detectors/operations/encode_packed.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/operations/low_level_calls.py` & `slither-analyzer-0.9.6/slither/detectors/operations/low_level_calls.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/operations/missing_events_access_control.py` & `slither-analyzer-0.9.6/slither/detectors/operations/missing_events_access_control.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/operations/missing_events_arithmetic.py` & `slither-analyzer-0.9.6/slither/detectors/operations/missing_events_arithmetic.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/operations/missing_zero_address_validation.py` & `slither-analyzer-0.9.6/slither/detectors/operations/missing_zero_address_validation.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/operations/unchecked_low_level_return_values.py` & `slither-analyzer-0.9.6/slither/detectors/operations/unchecked_low_level_return_values.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 """
 Module detecting unused return values from low level
 """
-from slither.detectors.abstract_detector import DetectorClassification
-from slither.detectors.operations.unused_return_values import UnusedReturnValues
+from typing import List
+
+from slither.core.cfg.node import Node
 from slither.slithir.operations import LowLevelCall
-from slither.slithir.operations.operation import Operation
+
+from slither.core.declarations.function_contract import FunctionContract
+from slither.core.variables.state_variable import StateVariable
+from slither.detectors.abstract_detector import (
+    AbstractDetector,
+    DetectorClassification,
+    DETECTOR_INFO,
+)
+from slither.utils.output import Output
 
 
-class UncheckedLowLevel(UnusedReturnValues):
+class UncheckedLowLevel(AbstractDetector):
     """
-    If the return value of a send is not checked, it might lead to losing ether
+    If the return value of a low-level call is not checked, it might lead to losing ether
     """
 
     ARGUMENT = "unchecked-lowlevel"
     HELP = "Unchecked low-level calls"
     IMPACT = DetectorClassification.MEDIUM
     CONFIDENCE = DetectorClassification.MEDIUM
 
@@ -34,9 +43,48 @@
 The return value of the low-level call is not checked, so if the call fails, the Ether will be locked in the contract.
 If the low level is used to prevent blocking operations, consider logging failed calls.
     """
     # endregion wiki_exploit_scenario
 
     WIKI_RECOMMENDATION = "Ensure that the return value of a low-level call is checked or logged."
 
-    def _is_instance(self, ir: Operation) -> bool:  # pylint: disable=no-self-use
-        return isinstance(ir, LowLevelCall)
+    @staticmethod
+    def detect_unused_return_values(f: FunctionContract) -> List[Node]:
+        """
+        Return the nodes where the return value of a call is unused
+        Args:
+            f (Function)
+        Returns:
+            list(Node)
+        """
+        values_returned = []
+        nodes_origin = {}
+        for n in f.nodes:
+            for ir in n.irs:
+                if isinstance(ir, LowLevelCall):
+                    # if a return value is stored in a state variable, it's ok
+                    if ir.lvalue and not isinstance(ir.lvalue, StateVariable):
+                        values_returned.append(ir.lvalue)
+                        nodes_origin[ir.lvalue] = ir
+
+                for read in ir.read:
+                    if read in values_returned:
+                        values_returned.remove(read)
+
+        return [nodes_origin[value].node for value in values_returned]
+
+    def _detect(self) -> List[Output]:
+        """Detect low level calls where the success value is not checked"""
+        results = []
+        for c in self.compilation_unit.contracts_derived:
+            for f in c.functions_and_modifiers:
+                unused_return = UncheckedLowLevel.detect_unused_return_values(f)
+                if unused_return:
+
+                    for node in unused_return:
+                        info: DETECTOR_INFO = [f, " ignores return value by ", node, "\n"]
+
+                        res = self.generate_result(info)
+
+                        results.append(res)
+
+        return results
```

### Comparing `slither-analyzer-0.9.5/slither/detectors/operations/unchecked_send_return_value.py` & `slither-analyzer-0.9.6/slither/detectors/operations/unchecked_send_return_value.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/operations/unchecked_transfer.py` & `slither-analyzer-0.9.6/slither/detectors/operations/unchecked_transfer.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/operations/unused_return_values.py` & `slither-analyzer-0.9.6/slither/detectors/operations/unused_return_values.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,18 +97,16 @@
                             values_returned.remove((remove[0], None))
                         values_returned.remove(remove)
         return [nodes_origin[value].node for (value, _) in values_returned]
 
     def _detect(self) -> List[Output]:
         """Detect high level calls which return a value that are never used"""
         results = []
-        for c in self.compilation_unit.contracts:
-            for f in c.functions + c.modifiers:
-                if f.contract_declarer != c:
-                    continue
+        for c in self.compilation_unit.contracts_derived:
+            for f in c.functions_and_modifiers:
                 unused_return = self.detect_unused_return_values(f)
                 if unused_return:
 
                     for node in unused_return:
                         info: DETECTOR_INFO = [f, " ignores return value by ", node, "\n"]
 
                         res = self.generate_result(info)
```

### Comparing `slither-analyzer-0.9.5/slither/detectors/operations/void_constructor.py` & `slither-analyzer-0.9.6/slither/detectors/operations/void_constructor.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/reentrancy/reentrancy.py` & `slither-analyzer-0.9.6/slither/detectors/reentrancy/reentrancy.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/reentrancy/reentrancy_benign.py` & `slither-analyzer-0.9.6/slither/detectors/reentrancy/reentrancy_benign.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/reentrancy/reentrancy_eth.py` & `slither-analyzer-0.9.6/slither/detectors/reentrancy/reentrancy_eth.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/reentrancy/reentrancy_events.py` & `slither-analyzer-0.9.6/slither/detectors/reentrancy/reentrancy_events.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/reentrancy/reentrancy_no_gas.py` & `slither-analyzer-0.9.6/slither/detectors/reentrancy/reentrancy_no_gas.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/reentrancy/reentrancy_read_before_write.py` & `slither-analyzer-0.9.6/slither/detectors/reentrancy/reentrancy_read_before_write.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/reentrancy/token.py` & `slither-analyzer-0.9.6/slither/detectors/reentrancy/token.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/shadowing/abstract.py` & `slither-analyzer-0.9.6/slither/detectors/shadowing/abstract.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/shadowing/builtin_symbols.py` & `slither-analyzer-0.9.6/slither/detectors/shadowing/builtin_symbols.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/shadowing/common.py` & `slither-analyzer-0.9.6/slither/detectors/shadowing/common.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/shadowing/local.py` & `slither-analyzer-0.9.6/slither/detectors/shadowing/local.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/shadowing/state.py` & `slither-analyzer-0.9.6/slither/detectors/shadowing/state.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/slither/name_reused.py` & `slither-analyzer-0.9.6/slither/detectors/slither/name_reused.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/source/rtlo.py` & `slither-analyzer-0.9.6/slither/detectors/source/rtlo.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/array_length_assignment.py` & `slither-analyzer-0.9.6/slither/detectors/statements/array_length_assignment.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/assembly.py` & `slither-analyzer-0.9.6/slither/detectors/statements/assembly.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/assert_state_change.py` & `slither-analyzer-0.9.6/slither/detectors/statements/assert_state_change.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/boolean_constant_equality.py` & `slither-analyzer-0.9.6/slither/detectors/statements/boolean_constant_equality.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/boolean_constant_misuse.py` & `slither-analyzer-0.9.6/slither/detectors/statements/boolean_constant_misuse.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/calls_in_loop.py` & `slither-analyzer-0.9.6/slither/detectors/statements/calls_in_loop.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/controlled_delegatecall.py` & `slither-analyzer-0.9.6/slither/detectors/statements/controlled_delegatecall.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/costly_operations_in_loop.py` & `slither-analyzer-0.9.6/slither/detectors/statements/costly_operations_in_loop.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/delegatecall_in_loop.py` & `slither-analyzer-0.9.6/slither/detectors/statements/delegatecall_in_loop.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/deprecated_calls.py` & `slither-analyzer-0.9.6/slither/detectors/statements/deprecated_calls.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/divide_before_multiply.py` & `slither-analyzer-0.9.6/slither/detectors/statements/divide_before_multiply.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/incorrect_strict_equality.py` & `slither-analyzer-0.9.6/slither/detectors/statements/incorrect_strict_equality.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/incorrect_using_for.py` & `slither-analyzer-0.9.6/slither/detectors/statements/incorrect_using_for.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/mapping_deletion.py` & `slither-analyzer-0.9.6/slither/detectors/statements/mapping_deletion.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/msg_value_in_loop.py` & `slither-analyzer-0.9.6/slither/detectors/statements/msg_value_in_loop.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/redundant_statements.py` & `slither-analyzer-0.9.6/slither/detectors/statements/redundant_statements.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/too_many_digits.py` & `slither-analyzer-0.9.6/slither/detectors/statements/too_many_digits.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/tx_origin.py` & `slither-analyzer-0.9.6/slither/detectors/statements/tx_origin.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/type_based_tautology.py` & `slither-analyzer-0.9.6/slither/detectors/statements/type_based_tautology.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/unary.py` & `slither-analyzer-0.9.6/slither/detectors/statements/unary.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/unprotected_upgradeable.py` & `slither-analyzer-0.9.6/slither/detectors/statements/unprotected_upgradeable.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/statements/write_after_write.py` & `slither-analyzer-0.9.6/slither/detectors/statements/write_after_write.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/variables/could_be_constant.py` & `slither-analyzer-0.9.6/slither/detectors/variables/could_be_constant.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/variables/could_be_immutable.py` & `slither-analyzer-0.9.6/slither/detectors/variables/could_be_immutable.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/variables/function_init_state_variables.py` & `slither-analyzer-0.9.6/slither/detectors/variables/function_init_state_variables.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/variables/predeclaration_usage_local.py` & `slither-analyzer-0.9.6/slither/detectors/variables/predeclaration_usage_local.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/variables/similar_variables.py` & `slither-analyzer-0.9.6/slither/detectors/variables/similar_variables.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/variables/unchanged_state_variables.py` & `slither-analyzer-0.9.6/slither/detectors/variables/unchanged_state_variables.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/variables/uninitialized_local_variables.py` & `slither-analyzer-0.9.6/slither/detectors/variables/uninitialized_local_variables.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/variables/uninitialized_state_variables.py` & `slither-analyzer-0.9.6/slither/detectors/variables/uninitialized_state_variables.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/variables/uninitialized_storage_variables.py` & `slither-analyzer-0.9.6/slither/detectors/variables/uninitialized_storage_variables.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/variables/unused_state_variables.py` & `slither-analyzer-0.9.6/slither/detectors/variables/unused_state_variables.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/detectors/variables/var_read_using_this.py` & `slither-analyzer-0.9.6/slither/detectors/variables/var_read_using_this.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/formatters/attributes/const_functions.py` & `slither-analyzer-0.9.6/slither/formatters/attributes/const_functions.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/formatters/attributes/constant_pragma.py` & `slither-analyzer-0.9.6/slither/formatters/attributes/constant_pragma.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/formatters/attributes/incorrect_solc.py` & `slither-analyzer-0.9.6/slither/formatters/attributes/incorrect_solc.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/formatters/functions/external_function.py` & `slither-analyzer-0.9.6/slither/formatters/functions/external_function.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/formatters/naming_convention/naming_convention.py` & `slither-analyzer-0.9.6/slither/formatters/naming_convention/naming_convention.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/formatters/utils/patches.py` & `slither-analyzer-0.9.6/slither/formatters/utils/patches.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/formatters/variables/unchanged_state_variables.py` & `slither-analyzer-0.9.6/slither/formatters/variables/unchanged_state_variables.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/formatters/variables/unused_state_variables.py` & `slither-analyzer-0.9.6/slither/formatters/variables/unused_state_variables.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/abstract_printer.py` & `slither-analyzer-0.9.6/slither/printers/abstract_printer.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/all_printers.py` & `slither-analyzer-0.9.6/slither/printers/all_printers.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/call/call_graph.py` & `slither-analyzer-0.9.6/slither/printers/call/call_graph.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/functions/authorization.py` & `slither-analyzer-0.9.6/slither/printers/functions/authorization.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/functions/cfg.py` & `slither-analyzer-0.9.6/slither/printers/functions/cfg.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/functions/dominator.py` & `slither-analyzer-0.9.6/slither/printers/functions/dominator.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/guidance/echidna.py` & `slither-analyzer-0.9.6/slither/printers/guidance/echidna.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/inheritance/inheritance.py` & `slither-analyzer-0.9.6/slither/printers/inheritance/inheritance.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/inheritance/inheritance_graph.py` & `slither-analyzer-0.9.6/slither/printers/inheritance/inheritance_graph.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/summary/constructor_calls.py` & `slither-analyzer-0.9.6/slither/printers/summary/constructor_calls.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/summary/contract.py` & `slither-analyzer-0.9.6/slither/printers/summary/contract.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/summary/data_depenency.py` & `slither-analyzer-0.9.6/slither/printers/summary/data_depenency.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/summary/declaration.py` & `slither-analyzer-0.9.6/slither/printers/summary/declaration.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/summary/evm.py` & `slither-analyzer-0.9.6/slither/printers/summary/evm.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/summary/function.py` & `slither-analyzer-0.9.6/slither/printers/summary/function.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/summary/function_ids.py` & `slither-analyzer-0.9.6/slither/printers/summary/function_ids.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/summary/human_summary.py` & `slither-analyzer-0.9.6/slither/printers/summary/human_summary.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/summary/loc.py` & `slither-analyzer-0.9.6/slither/printers/summary/loc.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/summary/modifier_calls.py` & `slither-analyzer-0.9.6/slither/printers/summary/modifier_calls.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/summary/require_calls.py` & `slither-analyzer-0.9.6/slither/printers/summary/require_calls.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/summary/slithir.py` & `slither-analyzer-0.9.6/slither/printers/summary/slithir.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/summary/slithir_ssa.py` & `slither-analyzer-0.9.6/slither/printers/summary/slithir_ssa.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/summary/variable_order.py` & `slither-analyzer-0.9.6/slither/printers/summary/variable_order.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/printers/summary/when_not_paused.py` & `slither-analyzer-0.9.6/slither/printers/summary/when_not_paused.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slither.py` & `slither-analyzer-0.9.6/slither/slither.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/convert.py` & `slither-analyzer-0.9.6/slither/slithir/convert.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/__init__.py` & `slither-analyzer-0.9.6/slither/slithir/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/assignment.py` & `slither-analyzer-0.9.6/slither/slithir/operations/assignment.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/binary.py` & `slither-analyzer-0.9.6/slither/slithir/operations/binary.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/call.py` & `slither-analyzer-0.9.6/slither/slithir/operations/call.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/codesize.py` & `slither-analyzer-0.9.6/slither/slithir/operations/codesize.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/condition.py` & `slither-analyzer-0.9.6/slither/slithir/operations/condition.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/delete.py` & `slither-analyzer-0.9.6/slither/slithir/operations/delete.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/event_call.py` & `slither-analyzer-0.9.6/slither/slithir/operations/event_call.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/high_level_call.py` & `slither-analyzer-0.9.6/slither/slithir/operations/high_level_call.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/index.py` & `slither-analyzer-0.9.6/slither/slithir/operations/index.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/init_array.py` & `slither-analyzer-0.9.6/slither/slithir/operations/init_array.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/internal_call.py` & `slither-analyzer-0.9.6/slither/slithir/operations/internal_call.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/internal_dynamic_call.py` & `slither-analyzer-0.9.6/slither/slithir/operations/internal_dynamic_call.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/length.py` & `slither-analyzer-0.9.6/slither/slithir/operations/length.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/library_call.py` & `slither-analyzer-0.9.6/slither/slithir/operations/library_call.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/low_level_call.py` & `slither-analyzer-0.9.6/slither/slithir/operations/low_level_call.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/lvalue.py` & `slither-analyzer-0.9.6/slither/slithir/operations/lvalue.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/member.py` & `slither-analyzer-0.9.6/slither/slithir/operations/member.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/new_array.py` & `slither-analyzer-0.9.6/slither/slithir/operations/new_array.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/new_contract.py` & `slither-analyzer-0.9.6/slither/slithir/operations/new_contract.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/new_elementary_type.py` & `slither-analyzer-0.9.6/slither/slithir/operations/new_elementary_type.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/new_structure.py` & `slither-analyzer-0.9.6/slither/slithir/operations/new_structure.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/operation.py` & `slither-analyzer-0.9.6/slither/slithir/operations/operation.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/phi.py` & `slither-analyzer-0.9.6/slither/slithir/operations/phi.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/phi_callback.py` & `slither-analyzer-0.9.6/slither/slithir/operations/phi_callback.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/return_operation.py` & `slither-analyzer-0.9.6/slither/slithir/operations/return_operation.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/send.py` & `slither-analyzer-0.9.6/slither/slithir/operations/send.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/solidity_call.py` & `slither-analyzer-0.9.6/slither/slithir/operations/solidity_call.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/transfer.py` & `slither-analyzer-0.9.6/slither/slithir/operations/transfer.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/type_conversion.py` & `slither-analyzer-0.9.6/slither/slithir/operations/type_conversion.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/unary.py` & `slither-analyzer-0.9.6/slither/slithir/operations/unary.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/operations/unpack.py` & `slither-analyzer-0.9.6/slither/slithir/operations/unpack.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/tmp_operations/argument.py` & `slither-analyzer-0.9.6/slither/slithir/tmp_operations/argument.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/tmp_operations/tmp_call.py` & `slither-analyzer-0.9.6/slither/slithir/tmp_operations/tmp_call.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/tmp_operations/tmp_new_array.py` & `slither-analyzer-0.9.6/slither/slithir/tmp_operations/tmp_new_array.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/tmp_operations/tmp_new_contract.py` & `slither-analyzer-0.9.6/slither/slithir/tmp_operations/tmp_new_contract.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/tmp_operations/tmp_new_elementary_type.py` & `slither-analyzer-0.9.6/slither/slithir/tmp_operations/tmp_new_elementary_type.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/utils/ssa.py` & `slither-analyzer-0.9.6/slither/slithir/utils/ssa.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/utils/utils.py` & `slither-analyzer-0.9.6/slither/slithir/utils/utils.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/variables/constant.py` & `slither-analyzer-0.9.6/slither/slithir/variables/constant.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/variables/local_variable.py` & `slither-analyzer-0.9.6/slither/slithir/variables/local_variable.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/variables/reference.py` & `slither-analyzer-0.9.6/slither/slithir/variables/reference.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/variables/reference_ssa.py` & `slither-analyzer-0.9.6/slither/slithir/variables/reference_ssa.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/variables/state_variable.py` & `slither-analyzer-0.9.6/slither/slithir/variables/state_variable.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/variables/temporary.py` & `slither-analyzer-0.9.6/slither/slithir/variables/temporary.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/variables/temporary_ssa.py` & `slither-analyzer-0.9.6/slither/slithir/variables/temporary_ssa.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/variables/tuple.py` & `slither-analyzer-0.9.6/slither/slithir/variables/tuple.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/slithir/variables/tuple_ssa.py` & `slither-analyzer-0.9.6/slither/slithir/variables/tuple_ssa.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/cfg/node.py` & `slither-analyzer-0.9.6/slither/solc_parsing/cfg/node.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/declarations/caller_context.py` & `slither-analyzer-0.9.6/slither/solc_parsing/declarations/caller_context.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/declarations/contract.py` & `slither-analyzer-0.9.6/slither/solc_parsing/declarations/contract.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/declarations/custom_error.py` & `slither-analyzer-0.9.6/slither/solc_parsing/declarations/custom_error.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/declarations/event.py` & `slither-analyzer-0.9.6/slither/solc_parsing/declarations/event.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/declarations/function.py` & `slither-analyzer-0.9.6/slither/solc_parsing/declarations/function.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/declarations/modifier.py` & `slither-analyzer-0.9.6/slither/solc_parsing/declarations/modifier.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/declarations/structure_contract.py` & `slither-analyzer-0.9.6/slither/solc_parsing/declarations/structure_contract.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/declarations/structure_top_level.py` & `slither-analyzer-0.9.6/slither/solc_parsing/declarations/structure_top_level.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/declarations/using_for_top_level.py` & `slither-analyzer-0.9.6/slither/solc_parsing/declarations/using_for_top_level.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/expressions/expression_parsing.py` & `slither-analyzer-0.9.6/slither/solc_parsing/expressions/expression_parsing.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/expressions/find_variable.py` & `slither-analyzer-0.9.6/slither/solc_parsing/expressions/find_variable.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/slither_compilation_unit_solc.py` & `slither-analyzer-0.9.6/slither/solc_parsing/slither_compilation_unit_solc.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/solidity_types/type_parsing.py` & `slither-analyzer-0.9.6/slither/solc_parsing/solidity_types/type_parsing.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/variables/event_variable.py` & `slither-analyzer-0.9.6/slither/solc_parsing/variables/event_variable.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/variables/function_type_variable.py` & `slither-analyzer-0.9.6/slither/solc_parsing/variables/function_type_variable.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/variables/local_variable.py` & `slither-analyzer-0.9.6/slither/solc_parsing/variables/local_variable.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/variables/local_variable_init_from_tuple.py` & `slither-analyzer-0.9.6/slither/solc_parsing/variables/local_variable_init_from_tuple.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/variables/state_variable.py` & `slither-analyzer-0.9.6/slither/solc_parsing/variables/state_variable.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/variables/structure_variable.py` & `slither-analyzer-0.9.6/slither/solc_parsing/variables/structure_variable.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/variables/top_level_variable.py` & `slither-analyzer-0.9.6/slither/solc_parsing/variables/top_level_variable.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/variables/variable_declaration.py` & `slither-analyzer-0.9.6/slither/solc_parsing/variables/variable_declaration.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/yul/evm_functions.py` & `slither-analyzer-0.9.6/slither/solc_parsing/yul/evm_functions.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/solc_parsing/yul/parse_yul.py` & `slither-analyzer-0.9.6/slither/solc_parsing/yul/parse_yul.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/demo/__main__.py` & `slither-analyzer-0.9.6/slither/tools/demo/__main__.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/doctor/__main__.py` & `slither-analyzer-0.9.6/slither/tools/doctor/__main__.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/doctor/checks/__init__.py` & `slither-analyzer-0.9.6/slither/tools/doctor/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/doctor/checks/paths.py` & `slither-analyzer-0.9.6/slither/tools/doctor/checks/paths.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/doctor/checks/platform.py` & `slither-analyzer-0.9.6/slither/tools/doctor/checks/platform.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/doctor/checks/versions.py` & `slither-analyzer-0.9.6/slither/tools/doctor/checks/versions.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/doctor/utils.py` & `slither-analyzer-0.9.6/slither/tools/doctor/utils.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/documentation/__main__.py` & `slither-analyzer-0.9.6/slither/tools/documentation/__main__.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/erc_conformance/__main__.py` & `slither-analyzer-0.9.6/slither/tools/erc_conformance/__main__.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/erc_conformance/erc/erc1155.py` & `slither-analyzer-0.9.6/slither/tools/erc_conformance/erc/erc1155.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/erc_conformance/erc/erc20.py` & `slither-analyzer-0.9.6/slither/tools/erc_conformance/erc/erc20.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/erc_conformance/erc/ercs.py` & `slither-analyzer-0.9.6/slither/tools/erc_conformance/erc/ercs.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/flattening/__main__.py` & `slither-analyzer-0.9.6/slither/tools/flattening/__main__.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/flattening/export/export.py` & `slither-analyzer-0.9.6/slither/tools/flattening/export/export.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/flattening/flattening.py` & `slither-analyzer-0.9.6/slither/tools/flattening/flattening.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/interface/__main__.py` & `slither-analyzer-0.9.6/slither/tools/interface/__main__.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/kspec_coverage/__main__.py` & `slither-analyzer-0.9.6/slither/tools/kspec_coverage/__main__.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/kspec_coverage/analysis.py` & `slither-analyzer-0.9.6/slither/tools/kspec_coverage/analysis.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/kspec_coverage/kspec_coverage.py` & `slither-analyzer-0.9.6/slither/tools/kspec_coverage/kspec_coverage.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/mutator/__main__.py` & `slither-analyzer-0.9.6/slither/tools/mutator/__main__.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/mutator/mutators/MIA.py` & `slither-analyzer-0.9.6/slither/tools/mutator/mutators/MIA.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/mutator/mutators/MVIE.py` & `slither-analyzer-0.9.6/slither/tools/mutator/mutators/MVIE.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/mutator/mutators/MVIV.py` & `slither-analyzer-0.9.6/slither/tools/mutator/mutators/MVIV.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/mutator/mutators/abstract_mutator.py` & `slither-analyzer-0.9.6/slither/tools/mutator/mutators/abstract_mutator.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/mutator/utils/command_line.py` & `slither-analyzer-0.9.6/slither/tools/mutator/utils/command_line.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/mutator/utils/generic_patching.py` & `slither-analyzer-0.9.6/slither/tools/mutator/utils/generic_patching.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/possible_paths/__main__.py` & `slither-analyzer-0.9.6/slither/tools/possible_paths/__main__.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/possible_paths/possible_paths.py` & `slither-analyzer-0.9.6/slither/tools/possible_paths/possible_paths.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/properties/__main__.py` & `slither-analyzer-0.9.6/slither/tools/properties/__main__.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/properties/addresses/address.py` & `slither-analyzer-0.9.6/slither/tools/properties/addresses/address.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/properties/platforms/echidna.py` & `slither-analyzer-0.9.6/slither/tools/properties/platforms/echidna.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/properties/platforms/truffle.py` & `slither-analyzer-0.9.6/slither/tools/properties/platforms/truffle.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/properties/properties/erc20.py` & `slither-analyzer-0.9.6/slither/tools/properties/properties/erc20.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/properties/properties/ercs/erc20/properties/burn.py` & `slither-analyzer-0.9.6/slither/tools/properties/properties/ercs/erc20/properties/burn.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/properties/properties/ercs/erc20/properties/initialization.py` & `slither-analyzer-0.9.6/slither/tools/properties/properties/ercs/erc20/properties/initialization.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/properties/properties/ercs/erc20/properties/mint.py` & `slither-analyzer-0.9.6/slither/tools/properties/properties/ercs/erc20/properties/mint.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/properties/properties/ercs/erc20/properties/mint_and_burn.py` & `slither-analyzer-0.9.6/slither/tools/properties/properties/ercs/erc20/properties/mint_and_burn.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/properties/properties/ercs/erc20/properties/transfer.py` & `slither-analyzer-0.9.6/slither/tools/properties/properties/ercs/erc20/properties/transfer.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/properties/properties/ercs/erc20/unit_tests/truffle.py` & `slither-analyzer-0.9.6/slither/tools/properties/properties/ercs/erc20/unit_tests/truffle.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/properties/properties/properties.py` & `slither-analyzer-0.9.6/slither/tools/properties/properties/properties.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/properties/solidity/generate_properties.py` & `slither-analyzer-0.9.6/slither/tools/properties/solidity/generate_properties.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/properties/utils.py` & `slither-analyzer-0.9.6/slither/tools/properties/utils.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/read_storage/__main__.py` & `slither-analyzer-0.9.6/slither/tools/read_storage/__main__.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/read_storage/read_storage.py` & `slither-analyzer-0.9.6/slither/tools/read_storage/read_storage.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/read_storage/utils/utils.py` & `slither-analyzer-0.9.6/slither/tools/read_storage/utils/utils.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/similarity/__main__.py` & `slither-analyzer-0.9.6/slither/tools/similarity/__main__.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/similarity/cache.py` & `slither-analyzer-0.9.6/slither/tools/similarity/cache.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/similarity/encode.py` & `slither-analyzer-0.9.6/slither/tools/similarity/encode.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/similarity/info.py` & `slither-analyzer-0.9.6/slither/tools/similarity/info.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/similarity/plot.py` & `slither-analyzer-0.9.6/slither/tools/similarity/plot.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/similarity/test.py` & `slither-analyzer-0.9.6/slither/tools/similarity/test.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/similarity/train.py` & `slither-analyzer-0.9.6/slither/tools/similarity/train.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/slither_format/__main__.py` & `slither-analyzer-0.9.6/slither/tools/slither_format/__main__.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/slither_format/slither_format.py` & `slither-analyzer-0.9.6/slither/tools/slither_format/slither_format.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/upgradeability/__main__.py` & `slither-analyzer-0.9.6/slither/tools/upgradeability/__main__.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/upgradeability/checks/abstract_checks.py` & `slither-analyzer-0.9.6/slither/tools/upgradeability/checks/abstract_checks.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/upgradeability/checks/all_checks.py` & `slither-analyzer-0.9.6/slither/tools/upgradeability/checks/all_checks.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/upgradeability/checks/constant.py` & `slither-analyzer-0.9.6/slither/tools/upgradeability/checks/constant.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/upgradeability/checks/functions_ids.py` & `slither-analyzer-0.9.6/slither/tools/upgradeability/checks/functions_ids.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/upgradeability/checks/initialization.py` & `slither-analyzer-0.9.6/slither/tools/upgradeability/checks/initialization.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/upgradeability/checks/variable_initialization.py` & `slither-analyzer-0.9.6/slither/tools/upgradeability/checks/variable_initialization.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/upgradeability/checks/variables_order.py` & `slither-analyzer-0.9.6/slither/tools/upgradeability/checks/variables_order.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/tools/upgradeability/utils/command_line.py` & `slither-analyzer-0.9.6/slither/tools/upgradeability/utils/command_line.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/arithmetic.py` & `slither-analyzer-0.9.6/slither/utils/arithmetic.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/code_complexity.py` & `slither-analyzer-0.9.6/slither/utils/code_complexity.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/code_generation.py` & `slither-analyzer-0.9.6/slither/utils/code_generation.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/codex.py` & `slither-analyzer-0.9.6/slither/utils/codex.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/colors.py` & `slither-analyzer-0.9.6/slither/utils/colors.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/command_line.py` & `slither-analyzer-0.9.6/slither/utils/command_line.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/comparable_enum.py` & `slither-analyzer-0.9.6/slither/utils/comparable_enum.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/erc.py` & `slither-analyzer-0.9.6/slither/utils/erc.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/expression_manipulations.py` & `slither-analyzer-0.9.6/slither/utils/expression_manipulations.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/inheritance_analysis.py` & `slither-analyzer-0.9.6/slither/utils/inheritance_analysis.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/integer_conversion.py` & `slither-analyzer-0.9.6/slither/utils/integer_conversion.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/loc.py` & `slither-analyzer-0.9.6/slither/utils/loc.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/myprettytable.py` & `slither-analyzer-0.9.6/slither/utils/myprettytable.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/output.py` & `slither-analyzer-0.9.6/slither/utils/output.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/output_capture.py` & `slither-analyzer-0.9.6/slither/utils/output_capture.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/oz_hashes.py` & `slither-analyzer-0.9.6/slither/utils/oz_hashes.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/source_mapping.py` & `slither-analyzer-0.9.6/slither/utils/source_mapping.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/standard_libraries.py` & `slither-analyzer-0.9.6/slither/utils/standard_libraries.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/tests_pattern.py` & `slither-analyzer-0.9.6/slither/utils/tests_pattern.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/type.py` & `slither-analyzer-0.9.6/slither/utils/type.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/type_helpers.py` & `slither-analyzer-0.9.6/slither/utils/type_helpers.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/utils/upgradeability.py` & `slither-analyzer-0.9.6/slither/utils/upgradeability.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/visitors/expression/constants_folding.py` & `slither-analyzer-0.9.6/slither/visitors/expression/constants_folding.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/visitors/expression/export_values.py` & `slither-analyzer-0.9.6/slither/visitors/expression/export_values.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/visitors/expression/expression.py` & `slither-analyzer-0.9.6/slither/visitors/expression/expression.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/visitors/expression/expression_printer.py` & `slither-analyzer-0.9.6/slither/visitors/expression/expression_printer.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/visitors/expression/find_calls.py` & `slither-analyzer-0.9.6/slither/visitors/expression/find_calls.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/visitors/expression/has_conditional.py` & `slither-analyzer-0.9.6/slither/visitors/expression/has_conditional.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/visitors/expression/read_var.py` & `slither-analyzer-0.9.6/slither/visitors/expression/read_var.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/visitors/expression/write_var.py` & `slither-analyzer-0.9.6/slither/visitors/expression/write_var.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither/visitors/slithir/expression_to_slithir.py` & `slither-analyzer-0.9.6/slither/visitors/slithir/expression_to_slithir.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither_analyzer.egg-info/PKG-INFO` & `slither-analyzer-0.9.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,80 +1,81 @@
-Metadata-Version: 2.1
-Name: slither-analyzer
-Version: 0.9.5
-Summary: Slither is a Solidity static analysis framework written in Python 3.
-Home-page: https://github.com/crytic/slither
-Author: Trail of Bits
-License: AGPL-3.0
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: lint
-Provides-Extra: test
-Provides-Extra: doc
-Provides-Extra: dev
-License-File: LICENSE
+# [Slither, the Solidity source analyzer](https://crytic.github.io/slither/slither.html)
 
-# Slither, the Solidity source analyzer
-
-<img src="https://raw.githubusercontent.com/crytic/slither/master/logo.png" alt="Logo" width="500"/>
+<img src="https://raw.githubusercontent.com/crytic/slither/master/logo.png" alt="Slither Static Analysis Framework Logo" width="500" />
 
 [![Build Status](https://img.shields.io/github/actions/workflow/status/crytic/slither/ci.yml?branch=master)](https://github.com/crytic/slither/actions?query=workflow%3ACI)
-[![Slack Status](https://empireslacking.herokuapp.com/badge.svg)](https://empireslacking.herokuapp.com)
-[![PyPI version](https://badge.fury.io/py/slither-analyzer.svg)](https://badge.fury.io/py/slither-analyzer)
-
-Slither is a Solidity static analysis framework written in Python3. It runs a suite of vulnerability detectors, prints visual information about contract details, and provides an API to easily write custom analyses. Slither enables developers to find vulnerabilities, enhance their code comprehension, and quickly prototype custom analyses.
-
-- [Features](#features)
-- [Usage](#usage)
-- [How to Install](#how-to-install)
-- [Detectors](#detectors)
-- [Printers](#printers)
-- [Tools](#tools)
-- [API Documentation](#api-documentation)
-- [Getting Help](#getting-help)
-- [FAQ](#faq)
-- [Publications](#publications)
+![PyPI](https://img.shields.io/pypi/v/slither-analyzer?logo=python&logoColor=white&label=slither-analyzer)
+[![Slither - Read the Docs](https://img.shields.io/badge/Slither-Read_the_Docs-2ea44f)](https://crytic.github.io/slither/slither.html)
+[![Slither - Wiki](https://img.shields.io/badge/Slither-Wiki-2ea44f)](https://github.com/crytic/slither/wiki/SlithIR)
+
+> Join the Empire Hacking Slack  
+>
+> [![Slack Status](https://slack.empirehacking.nyc/badge.svg)](https://slack.empirehacking.nyc/)
+> > <sub><i>- Discussions and Support </i></sub>
+
+**Slither** is a Solidity static analysis framework written in Python3. It runs a suite of vulnerability detectors, prints visual information about contract details, and provides an API to easily write custom analyses. Slither enables developers to find vulnerabilities, enhance their code comprehension, and quickly prototype custom analyses.
+
+* [Features](#features)
+* [Usage](#usage)
+* [How to install](#how-to-install)
+  * [Using Pip](#using-pip)
+  * [Using Git](#using-git)
+  * [Using Docker](#using-docker)
+  * [Integration](#integration)
+* [Detectors](#detectors)
+* [Printers](#printers)
+  * [Quick Review Printers](#quick-review-printers)
+  * [In-Depth Review Printers](#in-depth-review-printers)
+* [Tools](#tools)
+* [API Documentation](#api-documentation)
+* [Getting Help](#getting-help)
+* [FAQ](#faq)
+* [License](#license)
+* [Publications](#publications)
+  * [Trail of Bits publication](#trail-of-bits-publication)
+  * [External publications](#external-publications)
 
 ## Features
 
-- Detects vulnerable Solidity code with low false positives (see the list of [trophies](./trophies.md))
-- Identifies where the error condition occurs in the source code
-- Easily integrates into continuous integration and Hardhat/Foundry builds
-- Built-in 'printers' quickly report crucial contract information
-- Detector API to write custom analyses in Python
-- Ability to analyze contracts written with Solidity >= 0.4
-- Intermediate representation ([SlithIR](https://github.com/trailofbits/slither/wiki/SlithIR)) enables simple, high-precision analyses
-- Correctly parses 99.9% of all public Solidity code
-- Average execution time of less than 1 second per contract
-- Integrates with Github's code scanning in [CI](https://github.com/marketplace/actions/slither-action)
+* Detects vulnerable Solidity code with low false positives (see the list of [trophies](./trophies.md))
+* Identifies where the error condition occurs in the source code
+* Easily integrates into continuous integration and Hardhat/Foundry builds
+* Built-in 'printers' quickly report crucial contract information
+* Detector API to write custom analyses in Python
+* Ability to analyze contracts written with Solidity >= 0.4
+* Intermediate representation ([SlithIR](https://github.com/trailofbits/slither/wiki/SlithIR)) enables simple, high-precision analyses
+* Correctly parses 99.9% of all public Solidity code
+* Average execution time of less than 1 second per contract
+* Integrates with Github's code scanning in [CI](https://github.com/marketplace/actions/slither-action)
 
 ## Usage
 
 Run Slither on a Hardhat/Foundry/Dapp/Brownie application:
 
-```bash
+```console
 slither .
 ```
 
 This is the preferred option if your project has dependencies as Slither relies on the underlying compilation framework to compile source code.
 
 However, you can run Slither on a single file that does not import dependencies:
 
-```bash
+```console
 slither tests/uninitialized.sol
 ```
 
 ## How to install
 
-Slither requires Python 3.8+.
+> **Note** <br />
+> Slither requires Python 3.8+.
 If you're **not** going to use one of the [supported compilation frameworks](https://github.com/crytic/crytic-compile), you need [solc](https://github.com/ethereum/solidity/), the Solidity compiler; we recommend using [solc-select](https://github.com/crytic/solc-select) to conveniently switch between solc versions.
 
 ### Using Pip
 
-```bash
+```console
 pip3 install slither-analyzer
 ```
 
 ### Using Git
 
 ```bash
 git clone https://github.com/crytic/slither.git && cd slither
@@ -95,17 +96,17 @@
 
 ```bash
 docker run -it -v /home/share:/share trailofbits/eth-security-toolbox
 ```
 
 ### Integration
 
-- For GitHub action integration, use [slither-action](https://github.com/marketplace/actions/slither-action).
-- To generate a Markdown report, use `slither [target] --checklist`.
-- To generate a Markdown with GitHub source code highlighting, use `slither [target] --checklist --markdown-root https://github.com/ORG/REPO/blob/COMMIT/` (replace `ORG`, `REPO`, `COMMIT`)
+* For GitHub action integration, use [slither-action](https://github.com/marketplace/actions/slither-action).
+* To generate a Markdown report, use `slither [target] --checklist`.
+* To generate a Markdown with GitHub source code highlighting, use `slither [target] --checklist --markdown-root https://github.com/ORG/REPO/blob/COMMIT/` (replace `ORG`, `REPO`, `COMMIT`)
 
 ## Detectors
 
 Num | Detector | What it Detects | Impact | Confidence
 --- | --- | --- | --- | ---
 1 | `abiencoderv2-array` | [Storage abiencoderv2 array](https://github.com/crytic/slither/wiki/Detector-Documentation#storage-abiencoderv2-array) | High | High
 2 | `arbitrary-send-erc20` | [transferFrom uses arbitrary `from`](https://github.com/crytic/slither/wiki/Detector-Documentation#arbitrary-from-in-transferfrom) | High | High
@@ -193,90 +194,91 @@
 84 | `constable-states` | [State variables that could be declared constant](https://github.com/crytic/slither/wiki/Detector-Documentation#state-variables-that-could-be-declared-constant) | Optimization | High
 85 | `external-function` | [Public function that could be declared external](https://github.com/crytic/slither/wiki/Detector-Documentation#public-function-that-could-be-declared-external) | Optimization | High
 86 | `immutable-states` | [State variables that could be declared immutable](https://github.com/crytic/slither/wiki/Detector-Documentation#state-variables-that-could-be-declared-immutable) | Optimization | High
 87 | `var-read-using-this` | [Contract reads its own variable using `this`](https://github.com/crytic/slither/wiki/Detector-Documentation#public-variable-read-in-external-context) | Optimization | High
 
 For more information, see
 
-- The [Detector Documentation](https://github.com/crytic/slither/wiki/Detector-Documentation) for details on each detector
-- The [Detection Selection](https://github.com/crytic/slither/wiki/Usage#detector-selection) to run only selected detectors. By default, all the detectors are run.
-- The [Triage Mode](https://github.com/crytic/slither/wiki/Usage#triage-mode) to filter individual results
+* The [Detector Documentation](https://github.com/crytic/slither/wiki/Detector-Documentation) for details on each detector
+* The [Detection Selection](https://github.com/crytic/slither/wiki/Usage#detector-selection) to run only selected detectors. By default, all the detectors are run.
+* The [Triage Mode](https://github.com/crytic/slither/wiki/Usage#triage-mode) to filter individual results
 
 ## Printers
+
 ### Quick Review Printers
-- `human-summary`: [Print a human-readable summary of the contracts](https://github.com/trailofbits/slither/wiki/Printer-documentation#human-summary)
-- `inheritance-graph`: [Export the inheritance graph of each contract to a dot file](https://github.com/trailofbits/slither/wiki/Printer-documentation#inheritance-graph)
-- `contract-summary`: [Print a summary of the contracts](https://github.com/trailofbits/slither/wiki/Printer-documentation#contract-summary)
-- `loc`: [Count the total number lines of code (LOC), source lines of code (SLOC), and comment lines of code (CLOC) found in source files (SRC), dependencies (DEP), and test files (TEST).](https://github.com/trailofbits/slither/wiki/Printer-documentation#loc)
+* `human-summary`: [Print a human-readable summary of the contracts](https://github.com/trailofbits/slither/wiki/Printer-documentation#human-summary)
+* `inheritance-graph`: [Export the inheritance graph of each contract to a dot file](https://github.com/trailofbits/slither/wiki/Printer-documentation#inheritance-graph)
+* `contract-summary`: [Print a summary of the contracts](https://github.com/trailofbits/slither/wiki/Printer-documentation#contract-summary)
+* `loc`: [Count the total number lines of code (LOC), source lines of code (SLOC), and comment lines of code (CLOC) found in source files (SRC), dependencies (DEP), and test files (TEST).](https://github.com/trailofbits/slither/wiki/Printer-documentation#loc)
 
 ### In-Depth Review Printers
-- `call-graph`: [Export the call-graph of the contracts to a dot file](https://github.com/trailofbits/slither/wiki/Printer-documentation#call-graph)
-- `cfg`: [Export the CFG of each functions](https://github.com/trailofbits/slither/wiki/Printer-documentation#cfg)
-- `function-summary`: [Print a summary of the functions](https://github.com/trailofbits/slither/wiki/Printer-documentation#function-summary)
-- `vars-and-auth`: [Print the state variables written and the authorization of the functions](https://github.com/crytic/slither/wiki/Printer-documentation#variables-written-and-authorization)
-- `not-pausable`: [Print functions that do not use `whenNotPaused` modifier](https://github.com/trailofbits/slither/wiki/Printer-documentation#when-not-paused).
+* `call-graph`: [Export the call-graph of the contracts to a dot file](https://github.com/trailofbits/slither/wiki/Printer-documentation#call-graph)
+* `cfg`: [Export the CFG of each functions](https://github.com/trailofbits/slither/wiki/Printer-documentation#cfg)
+* `function-summary`: [Print a summary of the functions](https://github.com/trailofbits/slither/wiki/Printer-documentation#function-summary)
+* `vars-and-auth`: [Print the state variables written and the authorization of the functions](https://github.com/crytic/slither/wiki/Printer-documentation#variables-written-and-authorization)
+* `not-pausable`: [Print functions that do not use `whenNotPaused` modifier](https://github.com/trailofbits/slither/wiki/Printer-documentation#when-not-paused).
 
 To run a printer, use `--print` and a comma-separated list of printers.
 
 See the [Printer documentation](https://github.com/crytic/slither/wiki/Printer-documentation) for the complete lists.
 
 ## Tools
 
-- `slither-check-upgradeability`: [Review `delegatecall`-based upgradeability](https://github.com/crytic/slither/wiki/Upgradeability-Checks)
-- `slither-prop`: [Automatic unit test and property generation](https://github.com/crytic/slither/wiki/Property-generation)
-- `slither-flat`: [Flatten a codebase](https://github.com/crytic/slither/wiki/Contract-Flattening)
-- `slither-check-erc`: [Check the ERC's conformance](https://github.com/crytic/slither/wiki/ERC-Conformance)
-- `slither-format`: [Automatic patch generation](https://github.com/crytic/slither/wiki/Slither-format)
-- `slither-read-storage`: [Read storage values from contracts](./slither/tools/read_storage/README.md)
-- `slither-interface`: [Generate an interface for a contract](./slither/tools/interface/README.md)
+* `slither-check-upgradeability`: [Review `delegatecall`-based upgradeability](https://github.com/crytic/slither/wiki/Upgradeability-Checks)
+* `slither-prop`: [Automatic unit test and property generation](https://github.com/crytic/slither/wiki/Property-generation)
+* `slither-flat`: [Flatten a codebase](https://github.com/crytic/slither/wiki/Contract-Flattening)
+* `slither-check-erc`: [Check the ERC's conformance](https://github.com/crytic/slither/wiki/ERC-Conformance)
+* `slither-format`: [Automatic patch generation](https://github.com/crytic/slither/wiki/Slither-format)
+* `slither-read-storage`: [Read storage values from contracts](./slither/tools/read_storage/README.md)
+* `slither-interface`: [Generate an interface for a contract](./slither/tools/interface/README.md)
 
 See the [Tool documentation](https://github.com/crytic/slither/wiki/Tool-Documentation) for additional tools.
 
 [Contact us](https://www.trailofbits.com/contact/) to get help on building custom tools.
 
 ## API Documentation
 
 Documentation on Slither's internals is available [here](https://crytic.github.io/slither/slither.html).
 
 ## Getting Help
 
 Feel free to stop by our [Slack channel](https://empireslacking.herokuapp.com) (#ethereum) for help using or extending Slither.
 
-- The [Printer documentation](https://github.com/trailofbits/slither/wiki/Printer-documentation) describes the information Slither is capable of visualizing for each contract.
+* The [Printer documentation](https://github.com/trailofbits/slither/wiki/Printer-documentation) describes the information Slither is capable of visualizing for each contract.
 
-- The [Detector documentation](https://github.com/trailofbits/slither/wiki/Adding-a-new-detector) describes how to write a new vulnerability analyses.
+* The [Detector documentation](https://github.com/trailofbits/slither/wiki/Adding-a-new-detector) describes how to write a new vulnerability analyses.
 
-- The [API documentation](https://github.com/crytic/slither/wiki/Python-API) describes the methods and objects available for custom analyses.
+* The [API documentation](https://github.com/crytic/slither/wiki/Python-API) describes the methods and objects available for custom analyses.
 
-- The [SlithIR documentation](https://github.com/trailofbits/slither/wiki/SlithIR) describes the SlithIR intermediate representation.
+* The [SlithIR documentation](https://github.com/trailofbits/slither/wiki/SlithIR) describes the SlithIR intermediate representation.
 
 ## FAQ
 
 How do I exclude mocks or tests?
 
-- View our documentation on [path filtering](https://github.com/crytic/slither/wiki/Usage#path-filtering).
+* View our documentation on [path filtering](https://github.com/crytic/slither/wiki/Usage#path-filtering).
 
 How do I fix "unknown file" or compilation issues?
 
-- Because slither requires the solc AST, it must have all dependencies available.
+* Because slither requires the solc AST, it must have all dependencies available.
 If a contract has dependencies, `slither contract.sol` will fail.
 Instead, use `slither .` in the parent directory of `contracts/` (you should see `contracts/` when you run `ls`).
 If you have a `node_modules/` folder, it must be in the same directory as `contracts/`. To verify that this issue is related to slither,
 run the compilation command for the framework you are using e.g `npx hardhat compile`. That must work successfully;
 otherwise, slither's compilation engine, crytic-compile, cannot generate the AST.
 
 ## License
 
 Slither is licensed and distributed under the AGPLv3 license. [Contact us](mailto:opensource@trailofbits.com) if you're looking for an exception to the terms.
 
 ## Publications
 
 ### Trail of Bits publication
 
-- [Slither: A Static Analysis Framework For Smart Contracts](https://arxiv.org/abs/1908.09878), Josselin Feist, Gustavo Grieco, Alex Groce - WETSEB '19
+* [Slither: A Static Analysis Framework For Smart Contracts](https://arxiv.org/abs/1908.09878), Josselin Feist, Gustavo Grieco, Alex Groce - WETSEB '19
 
 ### External publications
 
 Title | Usage | Authors | Venue | Code
 --- | --- | --- | --- | ---
 [ReJection: A AST-Based Reentrancy Vulnerability Detection Method](https://www.researchgate.net/publication/339354823_ReJection_A_AST-Based_Reentrancy_Vulnerability_Detection_Method) | AST-based analysis built on top of Slither | Rui Ma, Zefeng Jian, Guangyuan Chen, Ke Ma, Yujia Chen | CTCIS 19
 [MPro: Combining Static and Symbolic Analysis forScalable Testing of Smart Contract](https://arxiv.org/pdf/1911.00570.pdf) | Leverage data dependency through Slither | William Zhang, Sebastian Banescu, Leodardo Pasos, Steven Stewart, Vijay Ganesh | ISSRE 2019 | [MPro](https://github.com/QuanZhang-William/M-Pro)
```

### Comparing `slither-analyzer-0.9.5/slither_analyzer.egg-info/SOURCES.txt` & `slither-analyzer-0.9.6/slither_analyzer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/slither_analyzer.egg-info/entry_points.txt` & `slither-analyzer-0.9.6/slither_analyzer.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/conftest.py` & `slither-analyzer-0.9.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/e2e/compilation/test_resolution.py` & `slither-analyzer-0.9.6/tests/e2e/compilation/test_resolution.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/e2e/compilation/test_source_unit.py` & `slither-analyzer-0.9.6/tests/e2e/compilation/test_source_unit.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/e2e/detectors/test_detectors.py` & `slither-analyzer-0.9.6/tests/e2e/detectors/test_detectors.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/e2e/solc_parsing/test_ast_parsing.py` & `slither-analyzer-0.9.6/tests/e2e/solc_parsing/test_ast_parsing.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/tools/read-storage/conftest.py` & `slither-analyzer-0.9.6/tests/tools/read-storage/conftest.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/tools/read-storage/test_read_storage.py` & `slither-analyzer-0.9.6/tests/tools/read-storage/test_read_storage.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/unit/core/test_arithmetic.py` & `slither-analyzer-0.9.6/tests/unit/core/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/unit/core/test_code_comments.py` & `slither-analyzer-0.9.6/tests/unit/core/test_code_comments.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/unit/core/test_constant_folding.py` & `slither-analyzer-0.9.6/tests/unit/core/test_constant_folding.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/unit/core/test_contract_declaration.py` & `slither-analyzer-0.9.6/tests/unit/core/test_contract_declaration.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/unit/core/test_error_messages.py` & `slither-analyzer-0.9.6/tests/unit/core/test_error_messages.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/unit/core/test_fallback_receive.py` & `slither-analyzer-0.9.6/tests/unit/core/test_fallback_receive.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/unit/core/test_function_declaration.py` & `slither-analyzer-0.9.6/tests/unit/core/test_function_declaration.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/unit/core/test_source_mapping.py` & `slither-analyzer-0.9.6/tests/unit/core/test_source_mapping.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/unit/core/test_storage_layout.py` & `slither-analyzer-0.9.6/tests/unit/core/test_storage_layout.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/unit/core/test_using_for.py` & `slither-analyzer-0.9.6/tests/unit/core/test_using_for.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/unit/slithir/test_operation_reads.py` & `slither-analyzer-0.9.6/tests/unit/slithir/test_operation_reads.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/unit/slithir/test_ssa_generation.py` & `slither-analyzer-0.9.6/tests/unit/slithir/test_ssa_generation.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/unit/slithir/test_ternary_expressions.py` & `slither-analyzer-0.9.6/tests/unit/slithir/test_ternary_expressions.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/unit/utils/test_code_generation.py` & `slither-analyzer-0.9.6/tests/unit/utils/test_code_generation.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/unit/utils/test_functions_ids.py` & `slither-analyzer-0.9.6/tests/unit/utils/test_functions_ids.py`

 * *Files identical despite different names*

### Comparing `slither-analyzer-0.9.5/tests/unit/utils/test_upgradeability_util.py` & `slither-analyzer-0.9.6/tests/unit/utils/test_upgradeability_util.py`

 * *Files identical despite different names*

