# Comparing `tmp/dbt_quicksight_lineage-0.2.0.tar.gz` & `tmp/dbt_quicksight_lineage-0.3.0.tar.gz`

## Comparing `dbt_quicksight_lineage-0.2.0.tar` & `dbt_quicksight_lineage-0.3.0.tar`

### file list

```diff
@@ -1,69 +1,71 @@
--rw-r--r--   0        0        0    21501 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/.pylintrc
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/.python-version
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/.tagpr
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/requirements-dev.lock
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/requirements.lock
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/.github/dependabot.yaml
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/.github/release.yml
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/.github/workflows/reviewdog.yaml
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/.github/workflows/tagpr.yaml
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0   208760 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/docs/images/dataset.png
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/__about__.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/__init__.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/__main__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/cli/__init__.py
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/cli/main.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/cli/requires.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/core/__init__.py
--rw-r--r--   0        0        0    17669 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/core/app.py
--rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/core/dbt.py
--rw-r--r--   0        0        0    29104 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/core/quicksight.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0    11639 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/core/test_app.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/core/test_dbt.py
--rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/core/test_quicksight.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/describe_data_set_output.json
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/expected_schema.yml
--rw-r--r--   0        0        0   302180 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/manifest.json
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/modified_data_set.json
--rw-r--r--   0        0        0   305700 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/partial_parse.msgpack
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/schema.yml
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/data_set.json
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_add_to_field_folder_move.golden.json
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_add_to_field_folder_not_exits.golden.json
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_add_to_field_folder_same_folder.golden.json
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_add_to_projected_columns_exists.golden.json
--rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_add_to_projected_columns_not_exists.golden.json
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_cast_column_type_operation_exists_replace.golden.json
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_cast_column_type_operation_not_exists.golden.json
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_cast_column_type_operation_same_type.golden.json
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_rename_column_oeration_not_exists.golden.json
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_rename_operation_exits_replace.golden.json
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_tag_column_geographic_role_operation_exists_replace.golden.json
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_tag_column_geographic_role_operation_not_exists.golden.json
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_tag_column_operation_description_exists_replace.golden.json
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_tag_column_operation_description_not_exists.golden.json
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/models/example/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/models/example/.gitkeep
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/.gitignore
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/.user.yml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/Makefile
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/README.md
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/dbt_project.yml
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/docker-compose.yaml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/profiles.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/analyses/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/macros/.gitkeep
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/models/example/schema.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/seeds/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/snapshots/.gitkeep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/tests/data/test_project/tests/.gitkeep
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/LICENSE
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/README.md
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    21501 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/.pylintrc
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/.python-version
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/.tagpr
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/requirements-dev.lock
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/requirements.lock
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/.github/dependabot.yaml
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/.github/release.yml
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/.github/workflows/reviewdog.yaml
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/.github/workflows/tagpr.yaml
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/.github/workflows/test.yaml
+-rw-r--r--   0        0        0   208760 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/docs/images/dataset.png
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/src/dbt_quicksight_lineage/__about__.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/src/dbt_quicksight_lineage/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/src/dbt_quicksight_lineage/__main__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/src/dbt_quicksight_lineage/cli/__init__.py
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/src/dbt_quicksight_lineage/cli/main.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/src/dbt_quicksight_lineage/cli/requires.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/src/dbt_quicksight_lineage/core/__init__.py
+-rw-r--r--   0        0        0    17710 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/src/dbt_quicksight_lineage/core/app.py
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/src/dbt_quicksight_lineage/core/dbt.py
+-rw-r--r--   0        0        0    30331 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/src/dbt_quicksight_lineage/core/quicksight.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0    11639 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/core/test_app.py
+-rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/core/test_dbt.py
+-rw-r--r--   0        0        0     8600 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/core/test_quicksight.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/describe_data_set_output.json
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/expected_schema.yml
+-rw-r--r--   0        0        0   302180 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/manifest.json
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/modified_data_set.json
+-rw-r--r--   0        0        0   305700 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/partial_parse.msgpack
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/schema.yml
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/fixture/data_set.json
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_add_to_field_folder_move.golden.json
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_add_to_field_folder_not_exits.golden.json
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_add_to_field_folder_same_folder.golden.json
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_add_to_field_folder_same_folder_same_field.golden.json
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_add_to_projected_columns_exists.golden.json
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_add_to_projected_columns_not_exists.golden.json
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_set_cast_column_type_operation_exists_replace.golden.json
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_set_cast_column_type_operation_not_exists.golden.json
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_set_cast_column_type_operation_same_type.golden.json
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_set_rename_column_oeration_not_exists.golden.json
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_set_rename_operation_exits_replace.golden.json
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_set_tag_column_geographic_role_operation_exists_replace.golden.json
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_set_tag_column_geographic_role_operation_not_exists.golden.json
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_set_tag_column_operation_description_empty.golden.json
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_set_tag_column_operation_description_exists_replace.golden.json
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_set_tag_column_operation_description_not_exists.golden.json
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/models/example/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/models/example/.gitkeep
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/test_project/.gitignore
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/test_project/.user.yml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/test_project/Makefile
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/test_project/README.md
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/test_project/dbt_project.yml
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/test_project/docker-compose.yaml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/test_project/profiles.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/test_project/analyses/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/test_project/macros/.gitkeep
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/test_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/test_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/test_project/models/example/schema.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/test_project/seeds/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/test_project/snapshots/.gitkeep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/tests/data/test_project/tests/.gitkeep
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/README.md
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 dbt_quicksight_lineage-0.3.0/PKG-INFO
```

### Comparing `dbt_quicksight_lineage-0.2.0/.pylintrc` & `dbt_quicksight_lineage-0.3.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/.tagpr` & `dbt_quicksight_lineage-0.3.0/.tagpr`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/CHANGELOG.md` & `dbt_quicksight_lineage-0.3.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## [v0.3.0](https://github.com/mashiike/dbt-quicksight-lineage/compare/v0.2.0...v0.3.0) - 2023-07-06
+- fix if field aleady exists in folder, duplicate by @mashiike in https://github.com/mashiike/dbt-quicksight-lineage/pull/15
+- if dry-run , output stdout update data set input palyoad by @mashiike in https://github.com/mashiike/dbt-quicksight-lineage/pull/16
+- if description is empty set remove operation by @mashiike in https://github.com/mashiike/dbt-quicksight-lineage/pull/17
+
 ## [v0.2.0](https://github.com/mashiike/dbt-quicksight-lineage/compare/v0.1.1...v0.2.0) - 2023-07-05
 - できる限り、元のDataSetの定義を維持したい by @mashiike in https://github.com/mashiike/dbt-quicksight-lineage/pull/7
 - add hidden on init command by @mashiike in https://github.com/mashiike/dbt-quicksight-lineage/pull/9
 - add geographic role by @mashiike in https://github.com/mashiike/dbt-quicksight-lineage/pull/10
 - data_type meta for CastColumnTypeOperation by @mashiike in https://github.com/mashiike/dbt-quicksight-lineage/pull/11
 
 ## [v0.1.1](https://github.com/mashiike/dbt-quicksight-lineage/compare/v0.1.0...v0.1.1) - 2023-07-04
```

### Comparing `dbt_quicksight_lineage-0.2.0/requirements-dev.lock` & `dbt_quicksight_lineage-0.3.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/requirements.lock` & `dbt_quicksight_lineage-0.3.0/requirements.lock`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/.github/workflows/reviewdog.yaml` & `dbt_quicksight_lineage-0.3.0/.github/workflows/reviewdog.yaml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/.github/workflows/tagpr.yaml` & `dbt_quicksight_lineage-0.3.0/.github/workflows/tagpr.yaml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/docs/images/dataset.png` & `dbt_quicksight_lineage-0.3.0/docs/images/dataset.png`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/cli/main.py` & `dbt_quicksight_lineage-0.3.0/src/dbt_quicksight_lineage/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """dbt-quicksight-lineage: DBT to QuickSight Lineage commandline definition"""
 import sys
 import logging
 from typing import Optional
+import json
 import colorlog
 import click
 from dbt_quicksight_lineage.cli import requires
 from dbt_quicksight_lineage.core import App
 from dbt_quicksight_lineage.__about__ import __version__
 
 
@@ -116,11 +117,16 @@
 ):
     """Update QuickSight DataSet from DBT Manifest"""
     app = App(
         manifest=ctx.obj['manifest'],
     )
     click.echo(
         f"Updating QuickSight DataSet: {data_set_id} on {app.aws_account_id}")
-    app.update_data_set(
+    _, update_data_set_input = app.update_data_set(
         data_set_id=data_set_id,
         dry_run=dry_run,
     )
+    if dry_run:
+        click.echo(
+            f"Update DataSet: {data_set_id} on {app.aws_account_id} (dry run)")
+        click.echo(json.dumps(update_data_set_input, indent=2, default=str, ensure_ascii=False))
+        return
```

### Comparing `dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/cli/requires.py` & `dbt_quicksight_lineage-0.3.0/src/dbt_quicksight_lineage/cli/requires.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/core/app.py` & `dbt_quicksight_lineage-0.3.0/src/dbt_quicksight_lineage/core/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,16 @@
                 data_set,
                 physical_table,
                 node,
             )
         update_data_set_input = data_set.generate_update_data_set_input(
             self.aws_account_id
         )
-        logger.debug(json.dumps(update_data_set_input, indent=2, default=str))
+        logger.debug(json.dumps(update_data_set_input,
+                     indent=2, default=str, ensure_ascii=False))
         if dry_run:
             return None, update_data_set_input
         output = self.quicksight_client.update_data_set(
             **update_data_set_input
         )
         if output.get('Status') != 200:
             raise ValueError(
```

### Comparing `dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/core/dbt.py` & `dbt_quicksight_lineage-0.3.0/src/dbt_quicksight_lineage/core/dbt.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/src/dbt_quicksight_lineage/core/quicksight.py` & `dbt_quicksight_lineage-0.3.0/src/dbt_quicksight_lineage/core/quicksight.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,22 +193,46 @@
             if operation.get('TagColumnOperation') is not None:
                 if operation['TagColumnOperation']['ColumnName'] == target_column_name:
                     for tag in operation['TagColumnOperation']['Tags']:
                         if tag.get('ColumnDescription') is not None:
                             return tag['ColumnDescription']['Text']
         return None
 
+    def remove_tag_column_description_operation(
+        self,
+        physical_column_name: str
+    ) -> None:
+        """
+        TagColumnOperationのColumnDescriptionを削除します
+        """
+        target_column_name = self.get_output_column_name(physical_column_name)
+        for index, operation in enumerate(self._logical_table['DataTransforms']):
+            if operation.get('TagColumnOperation') is not None:
+                last_tag_column_index = index
+                if operation['TagColumnOperation']['ColumnName'] != target_column_name:
+                    continue
+                for j, tag in enumerate(operation['TagColumnOperation']['Tags']):
+                    if tag.get('ColumnDescription') is not None:
+                        if len(operation['TagColumnOperation']['Tags']) == 1:
+                            self._logical_table['DataTransforms'].pop(index)
+                        else:
+                            operation['TagColumnOperation']['Tags'].pop(j)
+                        return
+
     def set_tag_column_description_operation(
         self,
         physical_column_name: str,
         description: str
     ) -> None:
         """
         TagColumnOperationのColumnDescriptionを設定します
         """
+        if description is None or description == '':
+            self.remove_tag_column_description_operation(physical_column_name)
+            return
         target_column_name = self.get_output_column_name(physical_column_name)
         exits = False
         last_tag_column_index = self._before_project_operation_index()
         for index, operation in enumerate(self._logical_table['DataTransforms']):
             if operation.get('TagColumnOperation') is not None:
                 last_tag_column_index = index
                 if operation['TagColumnOperation']['ColumnName'] != target_column_name:
@@ -457,15 +481,16 @@
         self.columns.remove(column_name)
 
     def add_column(
             self,
             column_name: str
     ) -> None:
         """指定したカラム名を追加します"""
-        self.columns.append(column_name)
+        if column_name not in self.columns:
+            self.columns.append(column_name)
 
     @property
     def column_count(self) -> int:
         """カラム数"""
         return len(self.columns)
```

### Comparing `dbt_quicksight_lineage-0.2.0/tests/core/test_app.py` & `dbt_quicksight_lineage-0.3.0/tests/core/test_app.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/tests/core/test_dbt.py` & `dbt_quicksight_lineage-0.3.0/tests/core/test_dbt.py`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/tests/core/test_quicksight.py` & `dbt_quicksight_lineage-0.3.0/tests/core/test_quicksight.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,26 @@
             description='Geometory of city',
         )
         assert_json_golden(
             "tests/data/fixture/test_set_tag_column_operation_description_not_exists.golden.json",
             data_set.to_dict(),
         )
 
+    def test_set_tag_column_operation_description_empty(self, source_data_set_dict):
+        data_set = DataSet(source_data_set_dict)
+        data_set.set_tag_column_description_operation(
+            physical_table_id=self.physical_table_id,
+            physical_column_name='id',
+            description='',
+        )
+        assert_json_golden(
+            "tests/data/fixture/test_set_tag_column_operation_description_empty.golden.json",
+            data_set.to_dict(),
+        )
+
     def test_set_tag_column_operation_description_exists_replace(self, source_data_set_dict):
         data_set = DataSet(source_data_set_dict)
         data_set.set_tag_column_description_operation(
             physical_table_id=self.physical_table_id,
             physical_column_name='id',
             description='Row ID of this data set. it is PrimaryKey',
         )
@@ -187,7 +199,19 @@
             physical_column_name='geo',
             field_folder_path='Key',
         )
         assert_json_golden(
             "tests/data/fixture/test_add_to_field_folder_same_folder.golden.json",
             data_set.to_dict(),
         )
+
+    def test_add_to_field_folder_same_folder_same_field(self, source_data_set_dict):
+        data_set = DataSet(source_data_set_dict)
+        data_set.add_to_field_folder(
+            physical_table_id=self.physical_table_id,
+            physical_column_name='id',
+            field_folder_path='Key',
+        )
+        assert_json_golden(
+            "tests/data/fixture/test_add_to_field_folder_same_folder_same_field.golden.json",
+            data_set.to_dict(),
+        )
```

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/describe_data_set_output.json` & `dbt_quicksight_lineage-0.3.0/tests/data/describe_data_set_output.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/expected_schema.yml` & `dbt_quicksight_lineage-0.3.0/tests/data/expected_schema.yml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/manifest.json` & `dbt_quicksight_lineage-0.3.0/tests/data/manifest.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/modified_data_set.json` & `dbt_quicksight_lineage-0.3.0/tests/data/modified_data_set.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/partial_parse.msgpack` & `dbt_quicksight_lineage-0.3.0/tests/data/partial_parse.msgpack`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/fixture/data_set.json` & `dbt_quicksight_lineage-0.3.0/tests/data/fixture/data_set.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_add_to_field_folder_move.golden.json` & `dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_add_to_field_folder_move.golden.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_add_to_field_folder_not_exits.golden.json` & `dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_add_to_field_folder_not_exits.golden.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_add_to_field_folder_same_folder.golden.json` & `dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_add_to_field_folder_same_folder.golden.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_add_to_projected_columns_exists.golden.json` & `dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_add_to_field_folder_same_folder_same_field.golden.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_add_to_projected_columns_not_exists.golden.json` & `dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_add_to_projected_columns_not_exists.golden.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_cast_column_type_operation_exists_replace.golden.json` & `dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_set_cast_column_type_operation_not_exists.golden.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98671875%*

 * *Differences: {"'FieldFolders'": "{'Key': {'description': 'this is key folder'}}",*

 * * "'LogicalTableMap'": "{'23456781-9abc-def0-1234-56789abcdef0': {'DataTransforms': {1: "*

 * *                      "{'CastColumnTypeOperation': {'NewColumnType': 'BOOLEAN'}}, insert: [(2, "*

 * *                      "OrderedDict([('CastColumnTypeOperation', OrderedDict([('ColumnName', "*

 * *                      "'updated_at'), ('NewColumnType', 'STRING')]))]))]}}}"}*

```diff
@@ -7,15 +7,16 @@
         "DisableUseAsDirectQuerySource": false,
         "DisableUseAsImportedSource": false
     },
     "FieldFolders": {
         "Key": {
             "columns": [
                 "ID"
-            ]
+            ],
+            "description": "this is key folder"
         }
     },
     "ImportMode": "SPICE",
     "LogicalTableMap": {
         "23456781-9abc-def0-1234-56789abcdef0": {
             "Alias": "My First DBT Model",
             "DataTransforms": [
@@ -24,15 +25,21 @@
                         "ColumnName": "id",
                         "NewColumnName": "ID"
                     }
                 },
                 {
                     "CastColumnTypeOperation": {
                         "ColumnName": "rate",
-                        "NewColumnType": "INTEGER"
+                        "NewColumnType": "BOOLEAN"
+                    }
+                },
+                {
+                    "CastColumnTypeOperation": {
+                        "ColumnName": "updated_at",
+                        "NewColumnType": "STRING"
                     }
                 },
                 {
                     "TagColumnOperation": {
                         "ColumnName": "ID",
                         "Tags": [
                             {
```

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_cast_column_type_operation_not_exists.golden.json` & `dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_add_to_projected_columns_exists.golden.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9868055555555555%*

 * *Differences: {"'FieldFolders'": "{'Key': {'description': 'this is key folder'}}",*

 * * "'LogicalTableMap'": "{'23456781-9abc-def0-1234-56789abcdef0': {'DataTransforms': {delete: [2]}}}"}*

```diff
@@ -7,15 +7,16 @@
         "DisableUseAsDirectQuerySource": false,
         "DisableUseAsImportedSource": false
     },
     "FieldFolders": {
         "Key": {
             "columns": [
                 "ID"
-            ]
+            ],
+            "description": "this is key folder"
         }
     },
     "ImportMode": "SPICE",
     "LogicalTableMap": {
         "23456781-9abc-def0-1234-56789abcdef0": {
             "Alias": "My First DBT Model",
             "DataTransforms": [
@@ -28,20 +29,14 @@
                 {
                     "CastColumnTypeOperation": {
                         "ColumnName": "rate",
                         "NewColumnType": "BOOLEAN"
                     }
                 },
                 {
-                    "CastColumnTypeOperation": {
-                        "ColumnName": "updated_at",
-                        "NewColumnType": "STRING"
-                    }
-                },
-                {
                     "TagColumnOperation": {
                         "ColumnName": "ID",
                         "Tags": [
                             {
                                 "ColumnDescription": {
                                     "Text": "The primary key for this table"
                                 }
```

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_cast_column_type_operation_same_type.golden.json` & `dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_set_cast_column_type_operation_same_type.golden.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'FieldFolders'": "{'Key': {'description': 'this is key folder'}}"}*

```diff
@@ -7,15 +7,16 @@
         "DisableUseAsDirectQuerySource": false,
         "DisableUseAsImportedSource": false
     },
     "FieldFolders": {
         "Key": {
             "columns": [
                 "ID"
-            ]
+            ],
+            "description": "this is key folder"
         }
     },
     "ImportMode": "SPICE",
     "LogicalTableMap": {
         "23456781-9abc-def0-1234-56789abcdef0": {
             "Alias": "My First DBT Model",
             "DataTransforms": [
```

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_rename_column_oeration_not_exists.golden.json` & `dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_set_rename_column_oeration_not_exists.golden.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_rename_operation_exits_replace.golden.json` & `dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_set_rename_operation_exits_replace.golden.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_tag_column_geographic_role_operation_exists_replace.golden.json` & `dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_set_tag_column_geographic_role_operation_exists_replace.golden.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'FieldFolders'": "{'Key': {'description': 'this is key folder'}}"}*

```diff
@@ -7,15 +7,16 @@
         "DisableUseAsDirectQuerySource": false,
         "DisableUseAsImportedSource": false
     },
     "FieldFolders": {
         "Key": {
             "columns": [
                 "ID"
-            ]
+            ],
+            "description": "this is key folder"
         }
     },
     "ImportMode": "SPICE",
     "LogicalTableMap": {
         "23456781-9abc-def0-1234-56789abcdef0": {
             "Alias": "My First DBT Model",
             "DataTransforms": [
```

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_tag_column_geographic_role_operation_not_exists.golden.json` & `dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_set_tag_column_geographic_role_operation_not_exists.golden.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875%*

 * *Differences: {"'FieldFolders'": "{'Key': {'description': 'this is key folder'}}"}*

```diff
@@ -7,15 +7,16 @@
         "DisableUseAsDirectQuerySource": false,
         "DisableUseAsImportedSource": false
     },
     "FieldFolders": {
         "Key": {
             "columns": [
                 "ID"
-            ]
+            ],
+            "description": "this is key folder"
         }
     },
     "ImportMode": "SPICE",
     "LogicalTableMap": {
         "23456781-9abc-def0-1234-56789abcdef0": {
             "Alias": "My First DBT Model",
             "DataTransforms": [
```

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_tag_column_operation_description_exists_replace.golden.json` & `dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_set_tag_column_operation_description_exists_replace.golden.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/fixture/test_set_tag_column_operation_description_not_exists.golden.json` & `dbt_quicksight_lineage-0.3.0/tests/data/fixture/test_set_tag_column_operation_description_not_exists.golden.json`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/test_project/README.md` & `dbt_quicksight_lineage-0.3.0/tests/data/test_project/README.md`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/test_project/dbt_project.yml` & `dbt_quicksight_lineage-0.3.0/tests/data/test_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/tests/data/test_project/models/example/schema.yml` & `dbt_quicksight_lineage-0.3.0/tests/data/test_project/models/example/schema.yml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/.gitignore` & `dbt_quicksight_lineage-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/LICENSE` & `dbt_quicksight_lineage-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/README.md` & `dbt_quicksight_lineage-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/pyproject.toml` & `dbt_quicksight_lineage-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dbt_quicksight_lineage-0.2.0/PKG-INFO` & `dbt_quicksight_lineage-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-quicksight-lineage
-Version: 0.2.0
+Version: 0.3.0
 Project-URL: Documentation, https://github.com/mashiike/dbt-quicksight-lineage#readme
 Project-URL: Issues, https://github.com/mashiike/dbt-quicksight-lineage/issues
 Project-URL: Source, https://github.com/mashiike/dbt-quicksight-lineage
 Author-email: mashiike <ikeda-masashi@kayac.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

