# Comparing `tmp/mckit-0.6.23.tar.gz` & `tmp/mckit-0.6.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mckit-0.6.23.tar", max compression
+gzip compressed data, was "mckit-0.6.24.tar", max compression
```

## Comparing `mckit-0.6.23.tar` & `mckit-0.6.24.tar`

### file list

```diff
@@ -1,188 +1,189 @@
--rw-r--r--   0        0        0    35051 2023-03-13 20:34:22.709924 mckit-0.6.23/LICENSE
--rw-r--r--   0        0        0     4363 2023-03-13 20:34:22.709924 mckit-0.6.23/README.rst
--rw-r--r--   0        0        0        0 2023-03-13 20:34:22.709924 mckit-0.6.23/benchmarks/__init__.py
--rw-r--r--   0        0        0   626946 2023-03-13 20:34:22.709924 mckit-0.6.23/benchmarks/data/4M.zip
--rw-r--r--   0        0        0     1521 2023-03-13 20:34:22.709924 mckit-0.6.23/benchmarks/mckit_utils.py
--rw-r--r--   0        0        0      941 2023-03-13 20:34:22.709924 mckit-0.6.23/benchmarks/test_mcnp_reading.py
--rw-r--r--   0        0        0     5388 2023-03-13 20:34:22.709924 mckit-0.6.23/build.py
--rw-r--r--   0        0        0        0 2023-03-13 20:34:22.709924 mckit-0.6.23/building/__init__.py
--rw-r--r--   0        0        0     1834 2023-03-13 20:34:22.709924 mckit-0.6.23/building/build_nlopt.py
--rw-r--r--   0        0        0     4064 2023-03-13 20:34:22.709924 mckit-0.6.23/building/extension_geometry.py
--rw-r--r--   0        0        0     1338 2023-03-13 20:34:22.709924 mckit-0.6.23/building/extension_utils.py
--rw-r--r--   0        0        0    11087 2023-03-13 20:34:22.753925 mckit-0.6.23/pyproject.toml
--rw-r--r--   0        0        0      684 2023-03-13 20:34:22.753925 mckit-0.6.23/src/mckit/__init__.py
--rw-r--r--   0        0        0     2472 2023-03-13 20:34:22.753925 mckit-0.6.23/src/mckit/_init_dynamic_libraries.py
--rw-r--r--   0        0        0    30957 2023-03-13 20:34:22.753925 mckit-0.6.23/src/mckit/body.py
--rw-r--r--   0        0        0     1957 2023-03-13 20:34:22.753925 mckit-0.6.23/src/mckit/box.py
--rw-r--r--   0        0        0     2875 2023-03-13 20:34:22.753925 mckit-0.6.23/src/mckit/card.py
--rw-r--r--   0        0        0        0 2023-03-13 20:34:22.753925 mckit-0.6.23/src/mckit/cli/__init__.py
--rw-r--r--   0        0        0      301 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/cli/commands/__init__.py
--rw-r--r--   0        0        0     1983 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/cli/commands/check.py
--rw-r--r--   0        0        0     1226 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/cli/commands/common.py
--rw-r--r--   0        0        0     6067 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/cli/commands/compose.py
--rw-r--r--   0        0        0     4314 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/cli/commands/decompose.py
--rw-r--r--   0        0        0     3626 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/cli/commands/split.py
--rw-r--r--   0        0        0     1792 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/cli/commands/transform.py
--rw-r--r--   0        0        0     1894 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/cli/logging.py
--rw-r--r--   0        0        0     7002 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/cli/runner.py
--rw-r--r--   0        0        0      410 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/constants.py
--rw-r--r--   0        0        0     6800 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/data/isotopes.dat
--rw-r--r--   0        0        0    17098 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/fmesh.py
--rw-r--r--   0        0        0    22799 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/material.py
--rw-r--r--   0        0        0      162 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/parser/__init__.py
--rw-r--r--   0        0        0    11221 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/parser/cell_parser.py
--rw-r--r--   0        0        0     2070 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/parser/common/Lexer.py
--rw-r--r--   0        0        0      567 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/parser/common/__init__.py
--rw-r--r--   0        0        0     2203 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/parser/common/cell_index.py
--rw-r--r--   0        0        0     1802 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/parser/common/composition_index.py
--rw-r--r--   0        0        0     1264 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/parser/common/surface_index.py
--rw-r--r--   0        0        0     1208 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/parser/common/transformation_index.py
--rw-r--r--   0        0        0     2917 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/parser/common/utils.py
--rw-r--r--   0        0        0     3215 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/parser/material_parser.py
--rw-r--r--   0        0        0     8102 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/parser/mcnp_input_sly_parser.py
--rw-r--r--   0        0        0    11526 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/parser/mcnp_section_parser.py
--rw-r--r--   0        0        0     4305 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/parser/mctal_parser.py
--rw-r--r--   0        0        0    12446 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/parser/meshtal_parser.py
--rw-r--r--   0        0        0     4406 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/parser/surface_parser.py
--rw-r--r--   0        0        0     2840 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/parser/transformation_parser.py
--rw-r--r--   0        0        0     4390 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/printer.py
--rw-r--r--   0        0        0     8485 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/source.py
--rw-r--r--   0        0        0     8254 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/src/box.c
--rw-r--r--   0        0        0     3666 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/src/box.h
--rw-r--r--   0        0        0     2401 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/src/box_doc.h
--rw-r--r--   0        0        0       77 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/src/common.h
--rw-r--r--   0        0        0    46245 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/src/geometrymodule.c
--rw-r--r--   0        0        0    13249 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/src/rbtree.c
--rw-r--r--   0        0        0     1266 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/src/rbtree.h
--rw-r--r--   0        0        0    14897 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/src/shape.c
--rw-r--r--   0        0        0     4507 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/src/shape.h
--rw-r--r--   0        0        0     1208 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/src/surf_doc.h
--rw-r--r--   0        0        0    13918 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/src/surface.c
--rw-r--r--   0        0        0     3057 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/src/surface.h
--rw-r--r--   0        0        0    47237 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/surface.py
--rw-r--r--   0        0        0    11196 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/transformation.py
--rw-r--r--   0        0        0    36217 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/universe.py
--rw-r--r--   0        0        0      731 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/utils/__init__.py
--rw-r--r--   0        0        0      596 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/utils/accept.py
--rw-r--r--   0        0        0     5066 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/utils/indexes.py
--rw-r--r--   0        0        0      699 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/utils/io.py
--rw-r--r--   0        0        0     6145 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/utils/misc.py
--rw-r--r--   0        0        0      163 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/utils/named.py
--rw-r--r--   0        0        0      657 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/utils/resource.py
--rw-r--r--   0        0        0     2348 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/utils/tolerance.py
--rw-r--r--   0        0        0      583 2023-03-13 20:34:22.757926 mckit-0.6.23/src/mckit/version.py
--rw-r--r--   0        0        0      162 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/__init__.py
--rw-r--r--   0        0        0      106 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/conftest.py
--rw-r--r--   0        0        0       84 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/brick-transformations.txt
--rw-r--r--   0        0        0      246 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/brick1-rot-z90.mcnp
--rw-r--r--   0        0        0      536 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/brick1-x+10-rot-z45.mcnp
--rw-r--r--   0        0        0      315 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/brick1-x+10.mcnp
--rw-r--r--   0        0        0      206 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/brick1.mcnp
--rw-r--r--   0        0        0       31 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/concat/test_load_table_1.csv
--rw-r--r--   0        0        0       63 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/concat/test_load_table_2.csv
--rw-r--r--   0        0        0      975 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/cubes_with_fill_named_transforms.mcnp
--rw-r--r--   0        0        0      322 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/cubes_with_fill_named_transforms.universes/envelopes.i
--rw-r--r--   0        0        0      334 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/cubes_with_fill_named_transforms.universes/fill-descriptor.toml
--rw-r--r--   0        0        0      281 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/cubes_with_fill_named_transforms.universes/u1.i
--rw-r--r--   0        0        0      278 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/cubes_with_fill_named_transforms.universes/u2.i
--rw-r--r--   0        0        0      952 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/cubes_with_fill_transforms.mcnp
--rw-r--r--   0        0        0      347 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/cubes_with_fill_transforms.universes/envelopes.i
--rw-r--r--   0        0        0      252 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/cubes_with_fill_transforms.universes/fill-descriptor.toml
--rw-r--r--   0        0        0      282 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/cubes_with_fill_transforms.universes/u1.i
--rw-r--r--   0        0        0      279 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/cubes_with_fill_transforms.universes/u2.i
--rw-r--r--   0        0        0      958 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/shared_surface.mcnp
--rw-r--r--   0        0        0      312 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/shared_surface.universes/envelopes.i
--rw-r--r--   0        0        0      246 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/shared_surface.universes/fill-descriptor.toml
--rw-r--r--   0        0        0      292 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/shared_surface.universes/u1.i
--rw-r--r--   0        0        0      278 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/shared_surface.universes/u2.i
--rw-r--r--   0        0        0      927 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/simple_cubes.mcnp
--rw-r--r--   0        0        0      313 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/simple_cubes.universes/envelopes.i
--rw-r--r--   0        0        0      158 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/simple_cubes.universes/fill-descriptor.toml
--rw-r--r--   0        0        0      282 2023-03-13 20:34:22.757926 mckit-0.6.23/tests/cli/data/simple_cubes.universes/u1.i
--rw-r--r--   0        0        0      279 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/cli/data/simple_cubes.universes/u2.i
--rw-r--r--   0        0        0      937 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/cli/data/simple_cubes_with_tallies.mcnp
--rw-r--r--   0        0        0      673 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/cli/data/two_cubes_with_the_same_filler.mcnp
--rw-r--r--   0        0        0      312 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/cli/data/two_cubes_with_the_same_filler.universes/envelopes.i
--rw-r--r--   0        0        0      262 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/cli/data/two_cubes_with_the_same_filler.universes/fill-descriptor.toml
--rw-r--r--   0        0        0      281 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/cli/data/two_cubes_with_the_same_filler.universes/u1.i
--rw-r--r--   0        0        0     1164 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/cli/test_check.py
--rw-r--r--   0        0        0     4598 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/cli/test_compose.py
--rw-r--r--   0        0        0     3437 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/cli/test_concat.py
--rw-r--r--   0        0        0     8496 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/cli/test_decompose.py
--rw-r--r--   0        0        0     1193 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/cli/test_runner.py
--rw-r--r--   0        0        0     8682 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/cli/test_split.py
--rw-r--r--   0        0        0    10308 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/cli/test_transform.py
--rw-r--r--   0        0        0      297 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/conftest.py
--rw-r--r--   0        0        0     2264 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/model_test_data/geometry_replace.py
--rw-r--r--   0        0        0     1209 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/model_test_data/material_creation.py
--rw-r--r--   0        0        0      786 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/model_test_data/model1.txt
--rw-r--r--   0        0        0      814 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/model_test_data/model1_ans.txt
--rw-r--r--   0        0        0    23128 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/model_test_data/model_data.py
--rw-r--r--   0        0        0        0 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser/__init__.py
--rw-r--r--   0        0        0        0 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser/common/__init__.py
--rw-r--r--   0        0        0     2081 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser/common/test_common.py
--rw-r--r--   0        0        0     3468 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser/common/test_common_lexer.py
--rw-r--r--   0        0        0        0 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser/data/__init__.py
--rw-r--r--   0        0        0      395 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser/data/parser1.txt
--rw-r--r--   0        0        0     1210 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser/data/parser2.txt
--rw-r--r--   0        0        0     5324 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser/test_cell_parser.py
--rw-r--r--   0        0        0     3179 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser/test_material_parser.py
--rw-r--r--   0        0        0     8651 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser/test_mcnp_section_parser.py
--rw-r--r--   0        0        0    11939 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser/test_mcnp_sly_parser.py
--rw-r--r--   0        0        0   281992 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser/test_meshtal_parser.py
--rw-r--r--   0        0        0     3359 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser/test_surface_parser.py
--rw-r--r--   0        0        0     1713 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser/test_transformation_parser.py
--rw-r--r--   0        0        0    39742 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser_test_data/d1s_mesh.m
--rw-r--r--   0        0        0    61416 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser_test_data/fmesh.m
--rw-r--r--   0        0        0    16517 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser_test_data/fmesh2.m
--rw-r--r--   0        0        0    19341 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser_test_data/fmesh3.m
--rw-r--r--   0        0        0      163 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser_test_data/lex1.txt
--rw-r--r--   0        0        0      343 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser_test_data/lex2.txt
--rw-r--r--   0        0        0      345 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser_test_data/lex3.txt
--rw-r--r--   0        0        0      162 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser_test_data/lex4.txt
--rw-r--r--   0        0        0      163 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser_test_data/lex5.txt
--rw-r--r--   0        0        0      170 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser_test_data/lex6.txt
--rw-r--r--   0        0        0     6236 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser_test_data/mctal.t
--rw-r--r--   0        0        0      395 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser_test_data/parser1.txt
--rw-r--r--   0        0        0     1102 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/parser_test_data/parser2.txt
--rw-r--r--   0        0        0    82711 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/test_body.py
--rw-r--r--   0        0        0    13503 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/test_box.py
--rw-r--r--   0        0        0      753 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/test_card.py
--rw-r--r--   0        0        0    24898 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/test_fmesh.py
--rw-r--r--   0        0        0    58654 2023-03-13 20:34:22.761926 mckit-0.6.23/tests/test_material.py
--rw-r--r--   0        0        0    28762 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/test_mctal_parser.py
--rw-r--r--   0        0        0     5780 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/test_printer.py
--rw-r--r--   0        0        0     6881 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/test_source.py
--rw-r--r--   0        0        0   102321 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/test_surface.py
--rw-r--r--   0        0        0    11826 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/test_transformation.py
--rw-r--r--   0        0        0    34639 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/test_universe.py
--rw-r--r--   0        0        0      837 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/test_universe_analyser.py
--rw-r--r--   0        0        0      290 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/test_version.py
--rw-r--r--   0        0        0      888 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/universe1.i
--rw-r--r--   0        0        0   356090 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/universe_test_data/model1.txt
--rw-r--r--   0        0        0   346916 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/universe_test_data/model2.txt
--rw-r--r--   0        0        0   346916 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/universe_test_data/model3.txt
--rw-r--r--   0        0        0   346916 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/universe_test_data/model4.txt
--rw-r--r--   0        0        0   346916 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/universe_test_data/model5.txt
--rw-r--r--   0        0        0   346916 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/universe_test_data/model6.txt
--rw-r--r--   0        0        0      239 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/universe_test_data/universe1.i
--rw-r--r--   0        0        0      764 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/universe_test_data/universe1002.i
--rw-r--r--   0        0        0      868 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/universe_test_data/universe1012.i
--rw-r--r--   0        0        0      860 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/universe_test_data/universe1022.i
--rw-r--r--   0        0        0      888 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/universe_test_data/universe2.i
--rw-r--r--   0        0        0      267 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/universe_test_data/universe3.i
--rw-r--r--   0        0        0      201 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/universe_test_data/universe4.i
--rw-r--r--   0        0        0      872 2023-03-13 20:34:22.765926 mckit-0.6.23/tests/universe_test_data/universe5.i
--rw-r--r--   0        0        0    89139 2023-03-13 20:34:22.769926 mckit-0.6.23/tests/universe_test_data/volume_ans.py
--rw-r--r--   0        0        0        0 2023-03-13 20:34:22.769926 mckit-0.6.23/tests/utils/__init__.py
--rw-r--r--   0        0        0     2105 2023-03-13 20:34:22.769926 mckit-0.6.23/tests/utils/test_accept.py
--rw-r--r--   0        0        0     1237 2023-03-13 20:34:22.769926 mckit-0.6.23/tests/utils/test_index.py
--rw-r--r--   0        0        0     2631 2023-03-13 20:34:22.769926 mckit-0.6.23/tests/utils/test_index_of_named.py
--rw-r--r--   0        0        0      720 2023-03-13 20:34:22.769926 mckit-0.6.23/tests/utils/test_io.py
--rw-r--r--   0        0        0     1857 2023-03-13 20:34:22.769926 mckit-0.6.23/tests/utils/test_resource.py
--rw-r--r--   0        0        0     4124 2023-03-13 20:34:22.769926 mckit-0.6.23/tests/utils/test_rounding.py
--rw-r--r--   0        0        0      964 2023-03-13 20:34:22.769926 mckit-0.6.23/tests/utils/test_tolerance.py
--rw-r--r--   0        0        0     2836 2023-03-13 20:34:22.769926 mckit-0.6.23/tests/utils/test_utils.py
--rw-r--r--   0        0        0     6900 1970-01-01 00:00:00.000000 mckit-0.6.23/setup.py
--rw-r--r--   0        0        0     6254 1970-01-01 00:00:00.000000 mckit-0.6.23/PKG-INFO
+-rw-r--r--   0        0        0    35051 2023-07-06 13:48:53.130188 mckit-0.6.24/LICENSE
+-rw-r--r--   0        0        0     4363 2023-07-06 13:48:53.130188 mckit-0.6.24/README.rst
+-rw-r--r--   0        0        0        0 2023-07-06 13:48:53.130188 mckit-0.6.24/benchmarks/__init__.py
+-rw-r--r--   0        0        0      910 2023-07-06 13:48:53.130188 mckit-0.6.24/benchmarks/conftest.py
+-rw-r--r--   0        0        0   626946 2023-07-06 13:48:53.134188 mckit-0.6.24/benchmarks/data/4M.zip
+-rw-r--r--   0        0        0     1557 2023-07-06 13:48:53.134188 mckit-0.6.24/benchmarks/mckit_utils.py
+-rw-r--r--   0        0        0      729 2023-07-06 13:48:53.134188 mckit-0.6.24/benchmarks/test_mcnp_reading.py
+-rw-r--r--   0        0        0     5438 2023-07-06 13:48:53.134188 mckit-0.6.24/build.py
+-rw-r--r--   0        0        0        0 2023-07-06 13:48:53.134188 mckit-0.6.24/building/__init__.py
+-rwxr-xr-x   0        0        0     1957 2023-07-06 13:48:53.134188 mckit-0.6.24/building/build_nlopt.py
+-rw-r--r--   0        0        0     4039 2023-07-06 13:48:53.134188 mckit-0.6.24/building/extension_geometry.py
+-rw-r--r--   0        0        0     1318 2023-07-06 13:48:53.134188 mckit-0.6.24/building/extension_utils.py
+-rw-r--r--   0        0        0    19875 2023-07-06 13:48:53.178188 mckit-0.6.24/pyproject.toml
+-rw-r--r--   0        0        0      697 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/__init__.py
+-rw-r--r--   0        0        0     2446 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/_init_dynamic_libraries.py
+-rw-r--r--   0        0        0    30501 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/body.py
+-rw-r--r--   0        0        0     1965 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/box.py
+-rw-r--r--   0        0        0     2847 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/card.py
+-rw-r--r--   0        0        0        0 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/cli/__init__.py
+-rw-r--r--   0        0        0      336 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2018 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/cli/commands/check.py
+-rw-r--r--   0        0        0     1223 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/cli/commands/common.py
+-rw-r--r--   0        0        0     5937 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/cli/commands/compose.py
+-rw-r--r--   0        0        0     4326 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/cli/commands/decompose.py
+-rw-r--r--   0        0        0     3618 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/cli/commands/split.py
+-rw-r--r--   0        0        0     1804 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/cli/commands/transform.py
+-rw-r--r--   0        0        0     1930 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/cli/logging.py
+-rw-r--r--   0        0        0     7000 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/cli/runner.py
+-rw-r--r--   0        0        0      446 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/constants.py
+-rw-r--r--   0        0        0     6800 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/data/isotopes.dat
+-rw-r--r--   0        0        0    17003 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/fmesh.py
+-rw-r--r--   0        0        0    22942 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/material.py
+-rw-r--r--   0        0        0      198 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/parser/__init__.py
+-rw-r--r--   0        0        0    11091 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/parser/cell_parser.py
+-rw-r--r--   0        0        0     1068 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/parser/common/__init__.py
+-rw-r--r--   0        0        0     2221 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/parser/common/cell_index.py
+-rw-r--r--   0        0        0     1814 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/parser/common/composition_index.py
+-rw-r--r--   0        0        0     2056 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/parser/common/lexer.py
+-rw-r--r--   0        0        0     1282 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/parser/common/surface_index.py
+-rw-r--r--   0        0        0     1226 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/parser/common/transformation_index.py
+-rw-r--r--   0        0        0     2947 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/parser/common/utils.py
+-rw-r--r--   0        0        0     3231 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/parser/material_parser.py
+-rw-r--r--   0        0        0     8066 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/parser/mcnp_input_sly_parser.py
+-rw-r--r--   0        0        0    11449 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/parser/mcnp_section_parser.py
+-rw-r--r--   0        0        0     4341 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/parser/mctal_parser.py
+-rw-r--r--   0        0        0    12260 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/parser/meshtal_parser.py
+-rw-r--r--   0        0        0     4363 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/parser/surface_parser.py
+-rw-r--r--   0        0        0     2855 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/parser/transformation_parser.py
+-rw-r--r--   0        0        0     4309 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/printer.py
+-rw-r--r--   0        0        0     8341 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/source.py
+-rw-r--r--   0        0        0     8254 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/src/box.c
+-rw-r--r--   0        0        0     3666 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/src/box.h
+-rw-r--r--   0        0        0     2401 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/src/box_doc.h
+-rw-r--r--   0        0        0       77 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/src/common.h
+-rw-r--r--   0        0        0    46416 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/src/geometrymodule.c
+-rw-r--r--   0        0        0    13249 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/src/rbtree.c
+-rw-r--r--   0        0        0     1266 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/src/rbtree.h
+-rw-r--r--   0        0        0    14936 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/src/shape.c
+-rw-r--r--   0        0        0     4507 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/src/shape.h
+-rw-r--r--   0        0        0     1208 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/src/surf_doc.h
+-rw-r--r--   0        0        0    13918 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/src/surface.c
+-rw-r--r--   0        0        0     3057 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/src/surface.h
+-rw-r--r--   0        0        0    47833 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/surface.py
+-rw-r--r--   0        0        0    11170 2023-07-06 13:48:53.178188 mckit-0.6.24/src/mckit/transformation.py
+-rw-r--r--   0        0        0    35976 2023-07-06 13:48:53.182188 mckit-0.6.24/src/mckit/universe.py
+-rw-r--r--   0        0        0      767 2023-07-06 13:48:53.182188 mckit-0.6.24/src/mckit/utils/__init__.py
+-rw-r--r--   0        0        0      632 2023-07-06 13:48:53.182188 mckit-0.6.24/src/mckit/utils/accept.py
+-rw-r--r--   0        0        0     5050 2023-07-06 13:48:53.182188 mckit-0.6.24/src/mckit/utils/indexes.py
+-rw-r--r--   0        0        0      699 2023-07-06 13:48:53.182188 mckit-0.6.24/src/mckit/utils/io.py
+-rw-r--r--   0        0        0     6104 2023-07-06 13:48:53.182188 mckit-0.6.24/src/mckit/utils/misc.py
+-rw-r--r--   0        0        0      199 2023-07-06 13:48:53.182188 mckit-0.6.24/src/mckit/utils/named.py
+-rw-r--r--   0        0        0      768 2023-07-06 13:48:53.182188 mckit-0.6.24/src/mckit/utils/resource.py
+-rw-r--r--   0        0        0     2356 2023-07-06 13:48:53.182188 mckit-0.6.24/src/mckit/utils/tolerance.py
+-rw-r--r--   0        0        0      619 2023-07-06 13:48:53.182188 mckit-0.6.24/src/mckit/version.py
+-rw-r--r--   0        0        0      260 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/conftest.py
+-rw-r--r--   0        0        0       84 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/brick-transformations.txt
+-rw-r--r--   0        0        0      246 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/brick1-rot-z90.mcnp
+-rw-r--r--   0        0        0      536 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/brick1-x+10-rot-z45.mcnp
+-rw-r--r--   0        0        0      315 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/brick1-x+10.mcnp
+-rw-r--r--   0        0        0      206 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/brick1.mcnp
+-rw-r--r--   0        0        0       31 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/concat/test_load_table_1.csv
+-rw-r--r--   0        0        0       63 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/concat/test_load_table_2.csv
+-rw-r--r--   0        0        0      975 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/cubes_with_fill_named_transforms.mcnp
+-rw-r--r--   0        0        0      322 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/cubes_with_fill_named_transforms.universes/envelopes.i
+-rw-r--r--   0        0        0      334 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/cubes_with_fill_named_transforms.universes/fill-descriptor.toml
+-rw-r--r--   0        0        0      281 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/cubes_with_fill_named_transforms.universes/u1.i
+-rw-r--r--   0        0        0      278 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/cubes_with_fill_named_transforms.universes/u2.i
+-rw-r--r--   0        0        0      952 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/cubes_with_fill_transforms.mcnp
+-rw-r--r--   0        0        0      347 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/cubes_with_fill_transforms.universes/envelopes.i
+-rw-r--r--   0        0        0      252 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/cubes_with_fill_transforms.universes/fill-descriptor.toml
+-rw-r--r--   0        0        0      282 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/cubes_with_fill_transforms.universes/u1.i
+-rw-r--r--   0        0        0      279 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/cubes_with_fill_transforms.universes/u2.i
+-rw-r--r--   0        0        0      958 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/shared_surface.mcnp
+-rw-r--r--   0        0        0      312 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/shared_surface.universes/envelopes.i
+-rw-r--r--   0        0        0      246 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/shared_surface.universes/fill-descriptor.toml
+-rw-r--r--   0        0        0      292 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/shared_surface.universes/u1.i
+-rw-r--r--   0        0        0      278 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/shared_surface.universes/u2.i
+-rw-r--r--   0        0        0      927 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/simple_cubes.mcnp
+-rw-r--r--   0        0        0      313 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/simple_cubes.universes/envelopes.i
+-rw-r--r--   0        0        0      158 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/simple_cubes.universes/fill-descriptor.toml
+-rw-r--r--   0        0        0      282 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/simple_cubes.universes/u1.i
+-rw-r--r--   0        0        0      279 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/simple_cubes.universes/u2.i
+-rw-r--r--   0        0        0      937 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/simple_cubes_with_tallies.mcnp
+-rw-r--r--   0        0        0      673 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/two_cubes_with_the_same_filler.mcnp
+-rw-r--r--   0        0        0      312 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/two_cubes_with_the_same_filler.universes/envelopes.i
+-rw-r--r--   0        0        0      262 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/two_cubes_with_the_same_filler.universes/fill-descriptor.toml
+-rw-r--r--   0        0        0      281 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/data/two_cubes_with_the_same_filler.universes/u1.i
+-rw-r--r--   0        0        0     1209 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/test_check.py
+-rw-r--r--   0        0        0     4643 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/test_compose.py
+-rw-r--r--   0        0        0     3458 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/test_concat.py
+-rw-r--r--   0        0        0     8541 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/test_decompose.py
+-rw-r--r--   0        0        0     1229 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/test_runner.py
+-rw-r--r--   0        0        0     8635 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/test_split.py
+-rw-r--r--   0        0        0    10353 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/cli/test_transform.py
+-rw-r--r--   0        0        0      350 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/conftest.py
+-rw-r--r--   0        0        0     2300 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/model_test_data/geometry_replace.py
+-rw-r--r--   0        0        0     1245 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/model_test_data/material_creation.py
+-rw-r--r--   0        0        0      786 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/model_test_data/model1.txt
+-rw-r--r--   0        0        0      814 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/model_test_data/model1_ans.txt
+-rw-r--r--   0        0        0    23164 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/model_test_data/model_data.py
+-rw-r--r--   0        0        0        0 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/parser/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/parser/common/__init__.py
+-rw-r--r--   0        0        0     2093 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/parser/common/test_common.py
+-rw-r--r--   0        0        0     3471 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/parser/common/test_common_lexer.py
+-rw-r--r--   0        0        0        0 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/parser/data/__init__.py
+-rw-r--r--   0        0        0      395 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/parser/data/parser1.txt
+-rw-r--r--   0        0        0     1210 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/parser/data/parser2.txt
+-rw-r--r--   0        0        0     5266 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/parser/test_cell_parser.py
+-rw-r--r--   0        0        0     3182 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/parser/test_material_parser.py
+-rw-r--r--   0        0        0     8662 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/parser/test_mcnp_section_parser.py
+-rw-r--r--   0        0        0    11957 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/parser/test_mcnp_sly_parser.py
+-rw-r--r--   0        0        0   282028 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/parser/test_meshtal_parser.py
+-rw-r--r--   0        0        0     3395 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/parser/test_surface_parser.py
+-rw-r--r--   0        0        0     1742 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/parser/test_transformation_parser.py
+-rw-r--r--   0        0        0    39742 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/parser_test_data/d1s_mesh.m
+-rw-r--r--   0        0        0    61416 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/parser_test_data/fmesh.m
+-rw-r--r--   0        0        0    16517 2023-07-06 13:48:53.182188 mckit-0.6.24/tests/parser_test_data/fmesh2.m
+-rw-r--r--   0        0        0    19341 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/parser_test_data/fmesh3.m
+-rw-r--r--   0        0        0      163 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/parser_test_data/lex1.txt
+-rw-r--r--   0        0        0      343 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/parser_test_data/lex2.txt
+-rw-r--r--   0        0        0      345 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/parser_test_data/lex3.txt
+-rw-r--r--   0        0        0      162 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/parser_test_data/lex4.txt
+-rw-r--r--   0        0        0      163 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/parser_test_data/lex5.txt
+-rw-r--r--   0        0        0      170 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/parser_test_data/lex6.txt
+-rw-r--r--   0        0        0     6236 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/parser_test_data/mctal.t
+-rw-r--r--   0        0        0      395 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/parser_test_data/parser1.txt
+-rw-r--r--   0        0        0     1102 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/parser_test_data/parser2.txt
+-rw-r--r--   0        0        0    82686 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/test_body.py
+-rw-r--r--   0        0        0    13594 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/test_box.py
+-rw-r--r--   0        0        0      753 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/test_card.py
+-rw-r--r--   0        0        0    25053 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/test_fmesh.py
+-rw-r--r--   0        0        0    58769 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/test_material.py
+-rw-r--r--   0        0        0    28807 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/test_mctal_parser.py
+-rw-r--r--   0        0        0     5816 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/test_printer.py
+-rw-r--r--   0        0        0     6955 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/test_source.py
+-rw-r--r--   0        0        0   102034 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/test_surface.py
+-rw-r--r--   0        0        0    11860 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/test_transformation.py
+-rw-r--r--   0        0        0    34492 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/test_universe.py
+-rw-r--r--   0        0        0      873 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/test_universe_analyser.py
+-rw-r--r--   0        0        0      326 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/test_version.py
+-rw-r--r--   0        0        0      888 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/universe1.i
+-rw-r--r--   0        0        0   356090 2023-07-06 13:48:53.186188 mckit-0.6.24/tests/universe_test_data/model1.txt
+-rw-r--r--   0        0        0   346916 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/universe_test_data/model2.txt
+-rw-r--r--   0        0        0   346916 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/universe_test_data/model3.txt
+-rw-r--r--   0        0        0   346916 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/universe_test_data/model4.txt
+-rw-r--r--   0        0        0   346916 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/universe_test_data/model5.txt
+-rw-r--r--   0        0        0   346916 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/universe_test_data/model6.txt
+-rw-r--r--   0        0        0      239 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/universe_test_data/universe1.i
+-rw-r--r--   0        0        0      764 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/universe_test_data/universe1002.i
+-rw-r--r--   0        0        0      868 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/universe_test_data/universe1012.i
+-rw-r--r--   0        0        0      860 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/universe_test_data/universe1022.i
+-rw-r--r--   0        0        0      888 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/universe_test_data/universe2.i
+-rw-r--r--   0        0        0      267 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/universe_test_data/universe3.i
+-rw-r--r--   0        0        0      201 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/universe_test_data/universe4.i
+-rw-r--r--   0        0        0      872 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/universe_test_data/universe5.i
+-rw-r--r--   0        0        0    89175 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/universe_test_data/volume_ans.py
+-rw-r--r--   0        0        0        0 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2141 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/utils/test_accept.py
+-rw-r--r--   0        0        0     1210 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/utils/test_index.py
+-rw-r--r--   0        0        0     2597 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/utils/test_index_of_named.py
+-rw-r--r--   0        0        0      756 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/utils/test_io.py
+-rw-r--r--   0        0        0     1749 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/utils/test_resource.py
+-rw-r--r--   0        0        0     4120 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/utils/test_rounding.py
+-rw-r--r--   0        0        0     1000 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/utils/test_tolerance.py
+-rw-r--r--   0        0        0     2872 2023-07-06 13:48:53.190188 mckit-0.6.24/tests/utils/test_utils.py
+-rw-r--r--   0        0        0     6902 1970-01-01 00:00:00.000000 mckit-0.6.24/setup.py
+-rw-r--r--   0        0        0     6217 1970-01-01 00:00:00.000000 mckit-0.6.24/PKG-INFO
```

### Comparing `mckit-0.6.23/LICENSE` & `mckit-0.6.24/LICENSE`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/README.rst` & `mckit-0.6.24/README.rst`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/benchmarks/data/4M.zip` & `mckit-0.6.24/benchmarks/data/4M.zip`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/benchmarks/mckit_utils.py` & `mckit-0.6.24/benchmarks/mckit_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import numpy as np
 
 from mckit.utils import get_decades, significant_digits
 
 # def run_digits_in_fraction(a: np.ndarray) -> None:
 #     map(digits_in_fraction_for_str, a)
 #
```

### Comparing `mckit-0.6.23/build.py` & `mckit-0.6.24/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Build mckit.
 
 The `build` method from this module is called by poetry build system
 to set up proper options for actual builder.
 
 The module builds and arrange C-dependency ``nlopt`` before own build.
 """
-from typing import Any, Dict, List, Optional
+from __future__ import annotations
+
+from typing import Any
 
-# import distutils.log as log
 import shutil
 
 from pathlib import Path
 from pprint import pprint
 
 from building.build_nlopt import build_nlopt
 from building.extension_geometry import GeometryExtension
@@ -27,18 +28,18 @@
     def is_pure(self):
         return False
 
 
 def get_nlopt_lib_name() -> str:
     """Compute library name: this depends on OS and python version."""
     if MACOS:
-        return f"libnlopt.dylib"
+        return "libnlopt.dylib"
     if WIN:
-        return f"Release/nlopt.dll"
-    return f"libnlopt.so"
+        return "Release/nlopt.dll"
+    return "libnlopt.so"
 
 
 class MCKitBuilder(build_ext):
     def __init__(self, dist: Distribution, **kwargs) -> None:
         build_ext.__init__(self, dist, **kwargs)
 
     def finalize_options(self):
@@ -67,15 +68,15 @@
         # log.info(str(extension))
         # log.info("---***")
         build_ext.build_extension(self, extension)
         # log.info("---*** Search geometry:")
         # log.info(list(DIR.glob("**/*geometry*")))
 
 
-def build(setup_kwargs: Dict[str, Any]) -> None:
+def build(setup_kwargs: dict[str, Any]) -> None:
     """Set specific distribution options.
 
     This function is called with setup.py generated by pip from pyproject.toml.
     """
     update_package_data(setup_kwargs)
     update_setup_requires(setup_kwargs)
     geometry_extension = GeometryExtension()
@@ -87,50 +88,51 @@
             "long_description": Path("README.rst").read_text(encoding="utf8"),
             "src_root": str(Path(__file__).parent),
         }
     )
     save_setup_kwargs(setup_kwargs)
 
 
-def update_setup_requires(setup_kwargs: Dict[str, Any]) -> None:
+def update_setup_requires(setup_kwargs: dict[str, Any]) -> None:
     """Fix for poetry issue: it doesn't install setup requirements."""
     setup_requires = setup_kwargs.get("setup_requires")  # type: Optional[List[str]]
     assert setup_requires is None, "Poetry has created setup_requires! Check the setup-generated.py"
     setup_requires = [
-        "poetry-core>=1.0.7",
-        "setuptools>=58.1",
-        "wheel",
-        # "cmake>=3.18.4",
-        # "numpy>=1.13",
-        # "mkl-devel",
+        "poetry-core >= 1.5.2",
+        "cmake >= 3.26.3",
+        "setuptools >= 67.8.0",
+        "wheel >= 0.40.0",
+        "mkl-devel == 2023.1.0",
+        "tbb == 2021.9.0",
+        "numpy >= 1.24.3",
     ]
     setup_kwargs["setup_requires"] = setup_requires
     save_generated_setup()
 
 
-def update_package_data(setup_kwargs: Dict[str, Any]) -> None:
+def update_package_data(setup_kwargs: dict[str, Any]) -> None:
     """Fix for poetry issue: it doesn't provide correct specification from `[tool.poetry].input` field."""
     package_data = [
         "data/isotopes.dat",
         "nlopt.dll" if WIN else "libnlopt*",
     ]
     setup_kwargs["package_data"] = {"mckit": package_data}
 
 
 def save_library(destination: Path, so: Path) -> None:
     if not so.exists():
         raise FileNotFoundError(f"Cannot find shared library {so}")
     shutil.copy(str(so), str(destination))
 
 
-def save_setup_kwargs(setup_kwargs: Dict[str, Any]) -> None:
+def save_setup_kwargs(setup_kwargs: dict[str, Any]) -> None:
     """Save resulting setup_kwargs for examining."""
     kwargs_path = Path(__file__).parent / "poetry_setup_kwargs.txt"
     with kwargs_path.open(mode="w") as fid:
-        pprint(setup_kwargs, fid, indent=4)
+        pprint(setup_kwargs, fid, indent=4)  # noqa: T203
 
 
 def save_generated_setup() -> None:
     """Save generated setup.py.
 
     Poetry ignores MANIFEST.in on command: ::
```

### Comparing `mckit-0.6.23/building/build_nlopt.py` & `mckit-0.6.24/building/build_nlopt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,33 @@
-from typing import Dict, List
+#!python
+from __future__ import annotations
 
 import os
 import sys
 
 from pathlib import Path
 from subprocess import check_call
 
-from building.extension_utils import WIN, create_directory
+sys.path.append(str(Path(__file__).parent.parent))
+print(sys.path)
+
+from building.extension_utils import WIN, create_directory  # noqa: E402
 
 
 def execute_command(
-    cmd: List[str], cwd: Path = Path.cwd(), env: Dict[str, str] = os.environ
+    cmd: list[str], cwd: Path | None = None, env: dict[str, str] = os.environ
 ) -> None:
-    print(f"--- {cwd.as_posix()}: {' '.join(cmd)}")
-    check_call(cmd, cwd=cwd, env=env)
-
+    if cwd is None:
+        cwd = Path.cwd()
+    check_call(cmd, cwd=cwd, env=env)  # noqa: S603
 
-def build_nlopt(*, install_prefix: str = None, build_dir: Path = None, clean=True) -> Path:
 
+def build_nlopt(
+    *, install_prefix: str | None = None, build_dir: Path | None = None, clean=True
+) -> Path:
     source_dir = Path(__file__).parent.parent.absolute() / "3rd-party" / "nlopt"
     if not source_dir.exists():
         execute_command(["git", "submodule", "update", "--init", "--recursive", "--depth=1"])
 
     # TODO dvp: check if something is to be done to support build isolation,
     #           use build_ext.build_temp probably?
     if build_dir is None:
```

### Comparing `mckit-0.6.23/building/extension_geometry.py` & `mckit-0.6.24/building/extension_geometry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Code to build mckit geometry C-extension."""
 from __future__ import annotations
 
-from typing import Iterable, List
+from typing import Iterable
 
 import os
 import shlex
 import sys
 
 from pathlib import Path
 
@@ -16,15 +16,15 @@
 # https://software.intel.com/content/www/us/en/develop/tools/oneapi/components/onemkl/link-line-advisor.html
 #
 # Windows (oneMKL 2021, MS-C/C++,64bit, c-32bit, shared library, no cluster):
 # mkl_intel_lp64_dll.lib mkl_tbb_thread_dll.lib mkl_core_dll.lib tbb.lib
 
 if not WIN:
 
-    def _make_full_names(lib_dir: Path, mkl_libs: Iterable[str]) -> List[str]:
+    def _make_full_names(lib_dir: Path, mkl_libs: Iterable[str]) -> list[str]:
         """Add library directory and extension to an MKL library name.
 
         According to the recommendation
         https://community.intel.com/t5/Intel-oneAPI-Math-Kernel-Library/pypi-package-for-mkl-2021-2-0-is-not-linkable-under-Linux-and/m-p/1275110?profile.language=ru
         on Linux MKL requires full path to the library.
         This method construct appropriate paths and searches the libraries.
 
@@ -40,32 +40,31 @@
         """
         # TODO dvp: implement logic for other possible suffixes in future MKL versions
         if MACOS:
             suffix = "2.dylib"
         else:
             if sys.platform != "linux":
                 msg = f"Unknown platform {sys.platform}"
-                raise EnvironmentError(msg)
+                raise OSError(msg)
             suffix = "so.2"
 
         lib_paths: list[Path] = [lib_dir / f"lib{_p}.{suffix}" for _p in mkl_libs]
 
         for p in lib_paths:
             if not p.exists():
                 msg = f"{p} is not a valid path to an MKL library."
-                raise EnvironmentError(msg)
+                raise OSError(msg)
 
         return [str(_p) for _p in lib_paths]
 
 
 class GeometryExtension(_Extension):
     """The :class:`_Extension` specialization for mckit geometry module."""
 
     def __init__(self) -> None:
-
         super().__init__(
             "mckit.geometry",
             sources=list(map(str, Path("src", "mckit", "src").glob("*.c"))),
             language="c",
         )
 
         if WIN:
```

### Comparing `mckit-0.6.23/building/extension_utils.py` & `mckit-0.6.24/building/extension_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union
+from __future__ import annotations
 
 import shutil
 import sys
 import sysconfig
 
 from pathlib import Path
 
@@ -16,15 +16,15 @@
     if WIN:
         root_prefix = root_prefix / "Library"
 
     library_dir = root_prefix / "lib"
 
     if check:
         if not library_dir.is_dir():
-            raise EnvironmentError(f"{library_dir} is not a valid directory")
+            raise OSError(f"{library_dir} is not a valid directory")
 
     return library_dir
 
 
 def create_directory(path: Path, clean: bool = True) -> Path:
     if clean and path.exists():
         shutil.rmtree(path)
@@ -33,18 +33,18 @@
 
 
 def check_directories(*directories: str) -> None:
     for directory in directories:
         if not isinstance(directory, str):
             raise TypeError(f"The value {directory} is not a string")
         if not Path(directory).is_dir():
-            raise EnvironmentError(f"The directory {directory} does not exist")
+            raise OSError(f"The directory {directory} does not exist")
 
 
-def insert_directories(destination: List[str], value: Union[str, List[str]]) -> List[str]:
+def insert_directories(destination: list[str], value: str | list[str]) -> list[str]:
     dirs = value
     if not isinstance(value, list):
         dirs = [dirs]
     for old in destination:
         if old not in dirs:
             dirs.append(old)
     return dirs
```

### Comparing `mckit-0.6.23/src/mckit/__init__.py` & `mckit-0.6.24/src/mckit/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """The mckit package code root."""
+from __future__ import annotations
+
 import mckit._init_dynamic_libraries as init_lib
 
 from mckit._init_dynamic_libraries import (
     Body,
     Cone,
     Cylinder,
     GQuadratic,
@@ -22,9 +24,7 @@
     __author__,
     __copyright__,
     __license__,
     __summary__,
     __title__,
     __version__,
 )
-
-__doc__ = __summary__
```

### Comparing `mckit-0.6.23/src/mckit/_init_dynamic_libraries.py` & `mckit-0.6.24/src/mckit/_init_dynamic_libraries.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Generator, List
+from typing import Generator
 
 import os
 import sys
 import sysconfig
 
 from ctypes import cdll
 from logging import getLogger
@@ -30,22 +30,22 @@
 
 else:  # Linux
 
     def _combine_version_and_suffix(version: int, suffix: str) -> str:
         return f"{suffix}.{version}"  # .so.2
 
 
-def _iterate_suffixes_with_version(max_version: int = 2) -> Generator["str", None, None]:
+def _iterate_suffixes_with_version(max_version: int = 2) -> Generator[str, None, None]:
     while max_version >= 0:
         yield _combine_version_and_suffix(max_version, SUFFIX)
         max_version -= 1
     yield SUFFIX
 
 
-SHARED_LIBRARY_DIRECTORIES: List[Path] = []
+SHARED_LIBRARY_DIRECTORIES: list[Path] = []
 
 if WIN:
     SHARED_LIBRARY_DIRECTORIES.append(Path(sys.prefix, "Library", "bin"))
 else:
     ld_library_path = os.environ.get("DYLD_LIBRARY_PATH" if MACOS else "LD_LIBRARY_PATH")
     if ld_library_path:
         SHARED_LIBRARY_DIRECTORIES.extend(map(Path, ld_library_path.split(":")))
@@ -58,26 +58,24 @@
     for d in SHARED_LIBRARY_DIRECTORIES:
         for s in _iterate_suffixes_with_version(max_version):
             p = Path(d, _library_base_name(lib_name)).with_suffix(s)
             if p.exists():
                 cdll.LoadLibrary(str(p))
                 _LOG.info("Found library: {}", p.absolute())
                 return
-    raise EnvironmentError(f"Cannot preload library {lib_name}")
+    raise OSError(f"Cannot preload library {lib_name}")
 
 
 def _init():
     if WIN and hasattr(os, "add_dll_directory"):  # Python 3.7 doesn't have this method
         for _dir in SHARED_LIBRARY_DIRECTORIES:
             os.add_dll_directory(str(_dir))
     _preload_library("mkl_rt", max_version=2)
     _preload_library("nlopt", max_version=0)
 
 
 _init()
 
 # We have to import these libraries here, after preloading libraries.
-
-import mckit.geometry as geometry
-
+from mckit import geometry
 from mckit.body import Body, Shape
 from mckit.surface import Cone, Cylinder, GQuadratic, Plane, Sphere, Torus, create_surface
```

### Comparing `mckit-0.6.23/src/mckit/body.py` & `mckit-0.6.24/src/mckit/body.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 import typing as tp
 
-from typing import Iterable, List, NewType, Optional, Set, Union
+from typing import Iterable, List, NewType, Union
 
 import os
 
 from copy import deepcopy
 from functools import reduce
 from itertools import groupby, permutations, product
+from logging import getLogger
 from multiprocessing import Pool
 
 import numpy as np
 
 import mckit.material as mm
 
 from click import progressbar
@@ -26,45 +27,33 @@
 from .printer import CELL_OPTION_GROUPS, print_option
 from .surface import Surface
 from .transformation import Transformation
 from .utils import filter_dict
 
 __all__ = ["Shape", "Body", "simplify", "GLOBAL_BOX", "Card", "TGeometry", "TGeometry"]
 
+_LOG = getLogger(__name__)
+
 
 # noinspection PyProtectedMember
 class Shape(_Shape):
-    """Describes shape.
+    """Shape class.
 
     Note:
         Shape is immutable object.
 
-    Args:
-        opc:
-            Operation code. Denotes operation to be applied. Possible values:
-            'I' - for intersection;
-            'U' - for union;
-            'C' - for complement;
-            'S' - (same) no operation;
-            'E' - empty set - no space occupied;
-            'R' - whole space.
-        args:
-            Geometry elements. It can be either Shape or Surface instances. But
-            no arguments must be specified for 'E' or 'R' opc. Only one argument
-            must present for 'C' or 'S' opc values.
-
     Attrs:
         opc (str):
             Operation code. It may be different from opc passed in __init__.
         invert_opc (str):
             Operation code, complement to the opc.
         args (Tuple[Shape|Surface...]):
             A tuple of shape's arguments.
 
-    Methods (inherited from native parent):
+    Methods:
         test_box(box)
             Tests if the box intersects the shape.
         volume(box, min_volume)
             Calculates the volume of the shape with desired accuracy.
         bounding_box(box, tol)
             Finds bounding box for the shape with desired accuracy.
         test_points(points)
@@ -96,15 +85,29 @@
         "U": ~hash("I"),
         "E": hash("E"),
         "R": ~hash("E"),
         "S": hash("S"),
         "C": ~hash("S"),
     }
 
-    def __init__(self, opc: str, *args: Union["Shape", "Surface"]):
+    def __init__(self, opc: str, *args: Shape | Surface):
+        """Initialize Shape object.
+
+        Args:
+            opc:  Operation code. Denotes operation to be applied. Possible values:
+                'I' - for intersection;
+                'U' - for union;
+                'C' - for complement;
+                'S' - (same) no operation;
+                'E' - empty set - no space occupied;
+                'R' - whole space.
+            args:  Geometry elements. It can be either Shape or Surface instances. But
+                no arguments must be specified for 'E' or 'R' opc. Only one argument
+                must present for 'C' or 'S' opc values.
+        """
         opc, args = _clean_args(opc, *args)
         _Shape.__init__(self, opc, *args)
         self._calculate_hash(opc, *args)
 
     def __iter__(self):
         return iter(self.args)
 
@@ -115,15 +118,15 @@
         opc, args, hash_value = state
         _Shape.__init__(self, opc, *args)
         self._hash = hash_value
 
     def __repr__(self):
         return f"Shape({self.opc}, {self.args})"
 
-    def _get_words(self, parent_opc: str = None) -> List[str]:
+    def _get_words(self, parent_opc: str = None) -> list[str]:
         """Gets list of words that describe the shape.
 
         Args:
             parent_opc:  Operation code of parent shape.
                          It is needed for proper use of parenthesis.
 
         Returns:
@@ -148,26 +151,26 @@
                 words.extend(a._get_words(self.opc))
                 words.append(sep)
             words.extend(args[-1]._get_words(self.opc))
             if need_parentheses:
                 words.append(")")
         return words
 
-    def __eq__(self, other):
+    def __eq__(self, other):  # noqa: PLR0911
         if self is other:
             return True
         if self.opc != other.opc:
             return False
         if self.opc == "E" or self.opc == "R":
             return True
         if len(self.args) != len(other.args):
             return False
         self_groups = {k: list(v) for k, v in groupby(sorted(self.args, key=hash), key=hash)}
         other_groups = {k: list(v) for k, v in groupby(sorted(other.args, key=hash), key=hash)}
-        flag = False  # TODO dvp: check is this statement doesn't break tests
+        flag: bool = False  # TODO dvp: check is this statement doesn't break tests
         for hash_value, entities in self_groups.items():
             flag = False
             if hash_value not in other_groups.keys():
                 return False
             if len(entities) != len(other_groups[hash_value]):
                 return False
             for other_entities in permutations(other_groups[hash_value]):
@@ -176,17 +179,15 @@
                         break
                 else:
                     flag = True
                     break
             if not flag:
                 return False
 
-        if flag:
-            return True
-        return False
+        return flag
 
     def __hash__(self):
         return self._hash
 
     def _calculate_hash(self, opc, *args):
         """Calculates hash value for the object.
 
@@ -200,157 +201,138 @@
             self._hash = self._opc_hash[opc]
             for a in args:
                 self._hash ^= hash(a)
 
     def complement(self):
         """Gets complement to the shape.
 
-        Returns
-        -------
-        comp_shape : Shape
+        Returns:
             Complement shape.
         """
         opc = self.opc
         args = self.args
         if opc == "S":
             return Shape("C", args[0])
-        elif opc == "C":
+        if opc == "C":
             return Shape("S", args[0])
-        elif opc == "E":
+        if opc == "E":
             return Shape("R")
-        elif opc == "R":
+        if opc == "R":
             return Shape("E")
-        else:
-            opc = self.invert_opc
-            c_args = [a.complement() for a in args]
-            return Shape(opc, *c_args)
+        opc = self.invert_opc
+        c_args = [a.complement() for a in args]
+        return Shape(opc, *c_args)
 
-    def is_complement(self, other):
+    def is_complement(self, other) -> bool:
         """Checks if this shape is complement to the other.
 
-        Returns
-        -------
-        result : bool
+        Returns:
             Test result.
         """
         if hash(self) != ~hash(other):
             return False
         if self.opc != other.invert_opc:
             return False
         if len(self.args) != len(other.args):
             return False
         if len(self.args) == 1:
             return self.args[0] == other.args[0]
-        elif len(self.args) > 1:
+        if len(self.args) > 1:
             for a in self.args:
                 for b in other.args:
                     if a.is_complement(b):
                         break
                 else:
                     return False
         return True
 
-    def intersection(self, *other: Union["Shape", "Body"]) -> "Shape":
+    def intersection(self, *other: Shape | Body) -> Shape:
         """Gets intersection with other shape.
 
         Parameters
         ----------
         other : tuple
             A list of Shape or Body objects, which must be intersected.
 
-        Returns
+        Returns:
         -------
         result : Shape
             New shape.
         """
         return Shape("I", self, *other)
 
     def union(self, *other):
         """Gets union with other shape.
 
-        Parameters
-        ----------
-        other : tuple
-            A list of Shape or Body objects, which must be joined.
+        Args:
+            other :  A list of Shape or Body objects, which must be joined.
 
-        Returns
-        -------
-        result : Shape
+        Returns:
             New shape.
         """
         return Shape("U", self, *other)
 
     def transform(self, tr):
         """Transforms the shape.
 
-        Parameters
-        ----------
-        tr : Transformation
-            Transformation to be applied.
+        Args:
+            tr : Transformation to be applied.
 
-        Returns
-        -------
-        result : Shape
+        Returns:
             New shape.
         """
         opc = self.opc
         args = []
         for a in self.args:
-            a = a.transform(tr)
+            a = a.transform(tr)  # noqa: PLW2901 - `a` is to be reassigned
             if isinstance(a, Surface):
-                a = a.apply_transformation()
+                a = a.apply_transformation()  # noqa: PLW2901 `a` is to be reassigned
                 # TODO dvp: check if call of apply_transformation() should be moved to caller site
                 #           it would be better to change only transformations instead of the surfaces
             args.append(a)
         return Shape(opc, *args)
 
     def apply_transformation(self):
         opc = self.opc
         args = []
         for a in self.args:
             if hasattr(a, "apply_transformation"):
-                a = a.apply_transformation()
-            else:
-                pass
+                a = a.apply_transformation()  # noqa: PLW2901 - `a` is to be reassigned
             args.append(a)
         return Shape(opc, *args)
 
-    def complexity(self):
+    def complexity(self) -> int:
         """Gets complexity of shape.
 
-        Returns
-        -------
-        complexity : int
+        Returns:
             The complexity of the shape description. It is the number of
             surfaces needed to describe the shape. Repeats are taken into
             account.
         """
         args = self.args
         if len(args) == 1:
             return 1
-        elif len(args) > 1:
+        if len(args) > 1:
             result = 0
             for a in args:
                 result += a.complexity()
             return result
-        else:
-            return 0
+        return 0
 
-    def get_surfaces(self) -> Set[Surface]:
+    def get_surfaces(self) -> set[Surface]:
         """Gets all the surfaces that describe the shape."""
         args = self.args
         if len(args) == 1:
             return {args[0]}
-        elif len(args) > 1:
+        if len(args) > 1:
             result = set()
             for a in args:
                 result = result.union(a.get_surfaces())
             return result
-        else:
-            return set()
+        return set()
 
     def is_empty(self):
         """Checks if the shape represents an empty set."""
         return self.opc == "E"
 
     def split_shape(self):
         shape_groups = []
@@ -381,26 +363,22 @@
                     groups[j] |= groups[index]
                     groups.pop(index)
                     break
             else:
                 break
         return groups
 
-    def get_simplest(self, trim_size=0):
+    def get_simplest(self, trim_size: int = 0) -> list[Shape]:  # noqa: PLR0911
         """Gets the simplest found description of the shape.
 
-        Parameters
-        ----------
-        trim_size : int
-            Shape variants with complexity greater than minimal one more than
-            trim_size are thrown away.
+        Args:
+            trim_size : Shape variants with complexity greater than minimal one more than
+                trim_size are thrown away.
 
-        Returns
-        -------
-        shapes : list[Shape]
+        Returns:
             A list of shapes with minimal complexity.
         """
         if self.opc != "I" and self.opc != "U":
             return [self]
         node_cases = []
         complexities = []
         stat = self.get_stat_table()
@@ -420,17 +398,17 @@
         arg_results = np.delete(stat, drop_index, axis=0)
         if arg_results.shape[0] == 0:
             if self.opc == "I":
                 return [Shape("R")]
             if self.opc == "U":
                 return [Shape("E")]
         cases = self._find_coverages(arg_results, value=val)
-        final_cases = set(tuple(c) for c in cases)
+        final_cases = {tuple(c) for c in cases}
         if len(final_cases) == 0:
-            print(self)
+            _LOG.debug(self)
             return None
         unique = reduce(set.union, map(set, final_cases))
         args = self.args
         node_variants = {i: args[i].get_simplest(trim_size) for i in unique}
         for indices in final_cases:
             variants = [node_variants[i] for i in indices]
             for args in product(*variants):
@@ -474,45 +452,40 @@
         shape is created anyway.
 
         Parameters
         ----------
         replace_dict : dict
             A dictionary of surfaces to be replaced.
 
-        Returns
+        Returns:
         -------
         shape : Shape
             New Shape object obtained by replacing certain surfaces.
         """
         if self.opc == "C" or self.opc == "S":
             arg = self.args[0]
             surf = replace_dict.get(arg, arg)
             return Shape(self.opc, surf)
-        elif self.opc == "I" or self.opc == "U":
+        if self.opc == "I" or self.opc == "U":
             args = [arg.replace_surfaces(replace_dict) for arg in self.args]
             return Shape(self.opc, *args)
-        else:
-            return self
+        return self
 
     @staticmethod
     def from_polish_notation(polish):
         """Creates Shape instance from reversed Polish notation.
 
-        Parameters
-        ----------
-        polish : list
-            List of surfaces and operations written in reversed Polish Notation.
+        Args:
+            polish:  List of surfaces and operations written in reversed Polish Notation.
 
-        Returns
-        -------
-        shape : Shape
+        Returns:
             The geometry represented by Shape instance.
         """
         operands = []
-        for i, op in enumerate(polish):
+        for op in polish:
             if isinstance(op, Surface):
                 operands.append(Shape("S", op))
             elif isinstance(op, Shape):
                 operands.append(op)
             elif op == "C":
                 operands.append(operands.pop().complement())
             else:
@@ -540,23 +513,22 @@
                 i += 1
 
         i = 0
         while i < len(args):
             a = args[i]
             if a.opc == "E" and opc == "I" or a.opc == "R" and opc == "U":
                 return a.opc, []
-            elif a.opc == "E" and opc == "U" or a.opc == "R" and opc == "I":
+            if a.opc == "E" and opc == "U" or a.opc == "R" and opc == "I":
                 args.pop(i)
                 continue
-            for j, b in enumerate(args[i + 1 :]):
+            for b in args[i + 1 :]:
                 if a.is_complement(b):
                     if opc == "I":
                         return "E", []
-                    else:
-                        return "R", []
+                    return "R", []
             i += 1
         args = list(set(args))
         args.sort(key=hash)
         if len(args) == 0:
             opc = "E" if opc == "U" else "R"
     if len(args) == 1 and isinstance(args[0], Shape):
         if opc == "S" or opc == "I" or opc == "U":
@@ -567,17 +539,17 @@
     return opc, args
 
 
 def _verify_opc(opc, *args):
     """Checks if such argument combination is valid."""
     if (opc == "E" or opc == "R") and len(args) > 0:
         raise ValueError("No arguments are expected.")
-    elif (opc == "S" or opc == "C") and len(args) != 1:
+    if (opc == "S" or opc == "C") and len(args) != 1:
         raise ValueError("Only one operand is expected.")
-    elif opc == "I" or opc == "U":
+    if opc == "I" or opc == "U":
         if len(args) == 0:
             raise ValueError("Operands are expected.")
 
 
 TOperation = NewType("TOperation", str)
 TGeometry = NewType("TGeometry", Union[List[Union[Surface, TOperation]], Shape, "Body"])
 
@@ -591,15 +563,15 @@
     ----------
     geometry : list or Shape
         Geometry expression. It is either a list of Surface instances and
         operations (reverse Polish notation is used) or Shape object.
     options :
         A set of cell's options.
 
-    Methods
+    Methods:
     -------
     intersection(other)
         Returns an intersection of this cell with the other.
     fill(universe)
         Fills this cell by universe.
     simplify(box, split_disjoint, min_volume)
         Simplifies cell description.
@@ -683,15 +655,15 @@
         return text
 
     @property
     def shape(self):
         """Gets body's shape."""
         return self._shape
 
-    def material(self) -> Optional[mm.Material]:
+    def material(self) -> mm.Material | None:
         """Gets body's Material.
 
         Returns:
             The material, if present, otherwise None
         """
         composition = self.options.get("MAT", None)
         assert composition is None or isinstance(composition, mm.Material)
@@ -704,15 +676,15 @@
         inherits all options of this one (the caller).
 
         Parameters
         ----------
         other : Cell
             Other cell.
 
-        Returns
+        Returns:
         -------
         cell : Cell
             The result.
         """
         geometry = self._shape.intersection(other)
         options = filter_dict(self.options, "original")
         return Body(geometry, **options)
@@ -723,15 +695,15 @@
         The resulting cell inherits all options of this one (the caller).
 
         Parameters
         ----------
         other : Cell
             Other cell.
 
-        Returns
+        Returns:
         -------
         cell : Cell
             The result.
         """
         geometry = self._shape.union(other)
         options = filter_dict(self.options, "original")
         return Body(geometry, **options)
@@ -757,15 +729,15 @@
         min_volume : float
             The smallest value of box's volume when the process of box splitting
             must be stopped.
         trim_size : int
             Max size of set to return. It is used to prevent unlimited growth
             of the variant set.
 
-        Returns
+        Returns:
         -------
         simple_cell : Cell
             Simplified version of this cell.
         """
         # print('Collect stage...')
         self._shape.collect_statistics(box, min_volume)
         # print('finding optimal solution...')
@@ -773,31 +745,30 @@
         # print(len(variants))
         options = filter_dict(self.options, "original")
         return Body(variants[0], **options)
 
     def split(self, box=GLOBAL_BOX, min_volume=MIN_BOX_VOLUME):
         """Splits cell into disjoint cells.
 
-        Returns
+        Returns:
         -------
         cells : list
         """
         self.shape.collect_statistics(box, min_volume)
         shape_groups = self.shape.split_shape()
-        bodies = [Body(shape, **self.options) for shape in shape_groups]
-        return bodies
+        return [Body(shape, **self.options) for shape in shape_groups]
 
     # noinspection PyShadowingNames
     def fill(
         self,
         universe=None,
         recurrent: bool = False,
         simplify: bool = False,
         **kwargs: dict[str, any],
-    ) -> list["Body"]:
+    ) -> list[Body]:
         """Fills this cell by filling universe.
 
         If this cell doesn't contain fill options and universe is not
         specified, the cell itself is returned as list of length 1. Otherwise:
         a list of cells from filling universe bounded by cell being filled is
         returned.
 
@@ -843,30 +814,30 @@
         """Applies transformation to this cell.
 
         Parameters
         ----------
         tr : Transform
             Transformation to be applied.
 
-        Returns
+        Returns:
         -------
         cell : Cell
             The result of this cell transformation.
         """
         geometry = self._shape.transform(tr)
         options = filter_dict(self.options, "original")
         cell = Body(geometry, **options)
         fill = cell.options.get("FILL", None)
         if fill:
             tr_in = fill.get("transform", Transformation())
             new_tr = tr.apply2transform(tr_in)
             fill["transform"] = new_tr
         return cell
 
-    def apply_transformation(self) -> "Body":
+    def apply_transformation(self) -> Body:
         """Actually apply transformation to this cell."""
         geometry = self._shape.apply_transformation()
         options = filter_dict(self.options, "original")
         cell = Body(geometry, **options)
         fill = cell.options.get("FILL", None)
         if fill:
             tr_in = fill.get("transform", None)
@@ -879,32 +850,29 @@
             #           one universe. Should be resolved before saving.
         return cell
 
 
 def simplify(cells: Iterable, box: Box = GLOBAL_BOX, min_volume: float = 1.0) -> tp.Generator:
     """Simplifies the cells.
 
-    Parameters
-    ----------
-
-    cells:
-        iterable over cells to simplify
-    box :
-        Box, from which simplification process starts. Default: GLOBAL_BOX.
-    min_volume : float
-        Minimal volume of the box, when splitting process terminates.
+    Args:
+        cells:
+            iterable over cells to simplify
+        box :
+            Box, from which simplification process starts. Default: GLOBAL_BOX.
+        min_volume : float
+            Minimal volume of the box, when splitting process terminates.
     """
-
     for c in cells:
         cs = c.simplify(box=box, min_volume=min_volume)
         if not cs.shape.is_empty():
             yield cs
 
 
-class Simplifier(object):
+class Simplifier:
     def __init__(self, box: Box = GLOBAL_BOX, min_volume: float = 1.0):
         self.box = box
         self.min_volume = min_volume
 
     def __call__(self, cell: Body):
         return cell.simplify(box=self.box, min_volume=self.min_volume)
 
@@ -943,25 +911,22 @@
     cells: Iterable[Body],
     box: Box = GLOBAL_BOX,
     min_volume: float = 1.0,
     chunk_size: int = 1,
 ) -> tp.Generator:
     """Simplifies the cells in multiprocessing mode with progress bar.
 
-    Parameters
-    ----------
-
-    cells:
-        iterable over cells to simplify
-    box :
-        Box, from which simplification process starts. Default: GLOBAL_BOX.
-    min_volume : float
-        Minimal volume of the box, when splitting process terminates.
-    chunk_size: size of chunks to pass to child processes
+    Args:
+        cells:
+            iterable over cells to simplify
+        box :
+            Box, from which simplification process starts. Default: GLOBAL_BOX.
+        min_volume : float
+            Minimal volume of the box, when splitting process terminates.
+        chunk_size: size of chunks to pass to child processes
     """
 
     def fmt_fun(x):
-        return "Simplifying cell #{0}".format(x.name() if x else x)
+        return f"Simplifying cell #{x.name() if x else x}"
 
     with progressbar(simplify_mp(cells, box, min_volume, chunk_size), item_show_func=fmt_fun) as pb:
-        for c in pb:
-            yield c
+        yield from pb
```

### Comparing `mckit-0.6.23/src/mckit/box.py` & `mckit-0.6.24/src/mckit/box.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+from __future__ import annotations
+
 import numpy as np
 
 # noinspection PyUnresolvedReferences,PyPackageRequirements
 from mckit.geometry import EX, EY, EZ
 from mckit.geometry import GLOBAL_BOX as _GLOBAL_BOX
 from mckit.geometry import Box as _Box
 from mckit.utils import make_hashable
 
 
 class Box(_Box):
-    __doc__ = _Box.__doc__
-
     def __init__(self, center, wx, wy, wz, ex=EX, ey=EY, ez=EZ):
         _Box.__init__(self, center, wx, wy, wz, ex=ex, ey=ey, ez=ez)
 
     @classmethod
     def from_geometry_box(cls, geometry_box: _Box):
         return cls(
             geometry_box.center,
```

### Comparing `mckit-0.6.23/src/mckit/card.py` & `mckit-0.6.24/src/mckit/card.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Features, common for all cards."""
 from __future__ import annotations
 
-from typing import Any, Dict, List, Optional, Text, cast
+from typing import Any, Optional, cast
 
 from abc import ABC, abstractmethod
 from functools import reduce
 from operator import xor
 
 from mckit.utils.named import Name
 
 from .printer import print_card
 
 
 class Card(ABC):
     """Features, common for all cards."""
 
     def __init__(self, **options):
-        self.options: Dict[str, Any] = options
+        self.options: dict[str, Any] = options
 
     def __str__(self):
         # TODO dvp: option `name` is printed twice,
         #           (second time as option)
         #           This should be explicit property of this class instance
         return f'{self.name()}: "{self.options}"'
 
@@ -31,44 +31,44 @@
 
     @property
     def has_original(self) -> bool:
         """Has original text stored in options."""
         return "original" in self.options
 
     @property
-    def original(self) -> Optional[str]:
+    def original(self) -> str | None:
         """Original text from an MCNP model."""
         return cast(Optional[str], self.options.get("original", None))
 
     @property
     def has_comment_above(self) -> bool:
         """Has comment above stored in options."""
         return "comment_above" in self.options
 
     @property
-    def comment_above(self) -> Optional[str]:
+    def comment_above(self) -> str | None:
         """Comment located above this card in an MCNP model."""
         return cast(Optional[str], self.options.get("comment_above", None))
 
     def name(
         self,
-    ) -> Optional[
-        Name
-    ]:  # TODO dvp: we'd better have special property name, don't use options for that
+    ) -> (
+        Name | None
+    ):  # TODO dvp: we'd better have special property name, don't use options for that
         """Returns card's name."""
         return self.options.get("name", None)
 
-    def rename(self, new_name) -> "Card":
+    def rename(self, new_name) -> Card:
         """Renames the card."""
         self.options["name"] = new_name
         self.drop_original()
         return self
 
     @abstractmethod
-    def mcnp_words(self, pretty=False) -> List[Text]:
+    def mcnp_words(self, pretty=False) -> list[str]:
         """Gets a list of card words."""
 
     def mcnp_repr(self, pretty: bool = False) -> str:
         """Gets str representation of the card."""
         # TODO dvp: try to use original texts, if available - this will preserve comments
         return cast(str, print_card(self.mcnp_words(pretty)))
```

### Comparing `mckit-0.6.23/src/mckit/cli/commands/check.py` & `mckit-0.6.24/src/mckit/cli/commands/check.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-# -*- coding: utf-8 -*-
 """Проверяет корректность модели и выдает статистику."""
-from typing import Any, Callable, Iterable, Optional
+from __future__ import annotations
+
+from typing import Any, Callable, Iterable
 
 from pathlib import Path
 
 from mckit import Universe
 from mckit.card import Card
 from mckit.cli.logging import logger
 from mckit.parser.mcnp_input_sly_parser import ParseResult, from_file
 from mckit.universe import collect_transformations
 
 
-def check_duplicates(
-    iterable: Optional[Iterable[Any]], label: str, key: Callable[[Any], Any]
-) -> None:
+def check_duplicates(iterable: Iterable[Any] | None, label: str, key: Callable[[Any], Any]) -> None:
     if iterable is None:
-        print(f"No {label}s are found")  # don't use logger here, should go to stdout
+        print(f"No {label}s are found")  # noqa: T201  - don't use logger here, should go to stdout
     else:
         visited = set()
         for c in iterable:
             k = key(c)
             if k in visited:
-                print(f"Duplicate of {label} {k} is found")
+                print(f"Duplicate of {label} {k} is found")  # noqa: T201
             else:
                 visited.add(k)
-        print(f"Total of {label}s: {len(visited)}")
+        print(f"Total of {label}s: {len(visited)}")  # noqa: T201
 
 
 def check(source):
     result = 0
     logger.info("Check model {}", source)
     source = Path(source)
     parse_result: ParseResult = from_file(source)
```

### Comparing `mckit-0.6.23/src/mckit/cli/commands/common.py` & `mckit-0.6.24/src/mckit/cli/commands/common.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import typing as tp
+from __future__ import annotations
 
 from io import StringIO
 from pathlib import Path
 
 import click
 
 from mckit.cli.logging import logger
 from mckit.constants import MCNP_ENCODING
 from mckit.universe import Universe, UniverseAnalyser
 
 # This is the encoding swallowing non ascii (neither unicode) symbols happening in MCNP models code
 
 
-def check_if_path_exists(path: tp.Union[str, Path], override: bool):
+def check_if_path_exists(path: str | Path, override: bool):
     if isinstance(path, str):
         path = Path(path)
     if not override and path.exists():
         errmsg = f"""\
         Cannot override existing file \"{path}\".
         Please remove the file or specify --override option"""
         logger.error(errmsg)
         raise click.UsageError(errmsg)
 
 
-def save_mcnp(model: Universe, path: tp.Union[str, Path], override: bool):
+def save_mcnp(model: Universe, path: str | Path, override: bool):
     check_if_path_exists(path, override)
     analyser = UniverseAnalyser(model)
     if analyser.we_are_all_clear():
         model.save(path, encoding=MCNP_ENCODING, check_clashes=False)
     else:
         out = StringIO()
         out.write("Duplicates found:\n")
```

### Comparing `mckit-0.6.23/src/mckit/cli/commands/compose.py` & `mckit-0.6.24/src/mckit/cli/commands/compose.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-# -*- coding: utf-8 -*-
 """Сборка модели из конвертов и входяших в них юниверсов по заданной спецификации."""
 from __future__ import annotations
 
-from typing import Dict, List, Optional, Tuple, Union
-
 from functools import reduce
 from pathlib import Path
 
 import numpy as np
 
 import mckit as mk
 
@@ -39,19 +36,19 @@
     named_transformations = load_named_transformations(fill_descriptor)
 
     comps = {}
 
     for k, v in universes.items():
         u, _ = v
         cps = u.get_compositions()
-        comps[k] = {c for c in cps}
+        comps[k] = set(cps)
 
     common = reduce(set.union, comps.values())
     envelopes.set_common_materials(common)
-    cells_index = dict((cell.name(), cell) for cell in envelopes)
+    cells_index = {cell.name(): cell for cell in envelopes}
 
     for i, spec in universes.items():
         universe, transformation = spec
         universe.set_common_materials(common)
         cell = cells_index[i]
         cell.options = filter_dict(cell.options, "original")
         cell.options["FILL"] = {"universe": universe}
@@ -87,17 +84,17 @@
                     f"Unexpected type of transformation parameter {type(transformation)}"
                 )
     save_mcnp(envelopes, output, override)
 
 
 def load_universes(
     fill_descriptor, universes_dir
-) -> Dict[int, Tuple[mk.Universe, Union[int, List[float]]]]:
-    filler_path_map: Dict[int, Tuple[Path, mk.Universe]] = dict()
-    cell_filler_map: Dict[int, Tuple[mk.Universe, Union[int, List[float]]]] = dict()
+) -> dict[int, tuple[mk.Universe, int | list[float]]]:
+    filler_path_map: dict[int, tuple[Path, mk.Universe]] = {}
+    cell_filler_map: dict[int, tuple[mk.Universe, int | list[float]]] = {}
 
     for k, v in fill_descriptor.items():
         if isinstance(v, dict) and "universe" in v:
             cell_name = int(k)
             universe_name = int(v["universe"])
             transformation = v.get("transform", None)
             universe_path = Path(v["file"])
@@ -125,15 +122,15 @@
                 filler_path_map[universe_name] = (universe_path, universe)
 
             cell_filler_map[cell_name] = (universe, transformation)
 
     return cell_filler_map
 
 
-def load_named_transformations(fill_descriptor) -> Optional[Dict[int, Transformation]]:
+def load_named_transformations(fill_descriptor) -> dict[int, Transformation] | None:
     transformations = fill_descriptor.get("named_transformations", None)
     if transformations:
         named_transformations = {}
         for k, v in transformations.items():
             name = int(k[2:])
             transform_params = np.fromiter(map(float, v), dtype=float)
             translation = transform_params[:3]
@@ -142,9 +139,8 @@
             else:
                 rotation = None
             transform = Transformation(
                 translation=translation, rotation=rotation, indegrees=True, name=name
             )
             named_transformations[name] = transform
         return named_transformations
-    else:
-        return None
+    return None
```

### Comparing `mckit-0.6.23/src/mckit/cli/commands/decompose.py` & `mckit-0.6.24/src/mckit/cli/commands/decompose.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# -*- coding: utf-8 -*-
-
 """Разложение модели на составляющие юниверсы.
 
 Читает модель, извлекает юниверсы первого уровня и сохраняет их
 в каталог universes под именем uN.i, где N - номер юниверса.
 Также сохраняет общую модель (без юниверсов) под именем envelopes.i
 Создает спецификацию для последующей сборки модели в виде TOML файла.
 """
+from __future__ import annotations
+
 from datetime import datetime
 from pathlib import Path
 
 import tomli_w as tw
 
 from mckit import Universe
 from mckit.cli.logging import logger
@@ -32,15 +32,15 @@
         comm.append(f"U={no}")
         cell.options["comment"] = comm
 
 
 def decompose(output, fill_descriptor_path, source, override):
     logger.info("Running mckit decompose")
     logger.debug("Working dir {}", Path(".").absolute())
-    logger.info(f"Processing {source}")
+    logger.info("Processing {}", source)
     logger.debug("Loading model from {}", source)
     source = Path(source)
     if output is None:
         output = get_default_output_directory(source)
     else:
         output = Path(output)
     output.mkdir(parents=True, exist_ok=True)
```

### Comparing `mckit-0.6.23/src/mckit/cli/commands/split.py` & `mckit-0.6.24/src/mckit/cli/commands/split.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# -*- coding: utf-8 -*-
-
 """Разложение текста модели на секции.
 
 Читает модель, извлекает и раскладывает в указанную директорию отедельно файлы для ячеек, поверхностей,
 материалов, трансформаций, sdef и прочие карты. Файлы соответственно: cells.txt, surfaces.txt,
 materials.txt, transformations.txt, sdef.txt, cards.txt
 """
-from typing import Iterable, Union
+from __future__ import annotations
+
+from typing import Iterable
 
 from pathlib import Path
 
 import mckit.parser.mcnp_section_parser as sp
 
 from mckit.cli.logging import logger
 
@@ -35,17 +35,15 @@
         out = output_dir / section_file_name
         check_if_path_exists(out, override)
         with out.open("w", encoding=MCNP_ENCODING) as fid:
             for card in cards:
                 print(card.text, file=fid)
 
 
-def split(
-    output_dir: Path, mcnp_file_name: Union[str, Path], override: bool, separators=False
-) -> None:
+def split(output_dir: Path, mcnp_file_name: str | Path, override: bool, separators=False) -> None:
     logger.debug("Splitting model from {}", mcnp_file_name)
     if isinstance(mcnp_file_name, str):
         mcnp_file_name = Path(mcnp_file_name)
     assert output_dir.is_dir()
     with open(mcnp_file_name, encoding=MCNP_ENCODING) as fid:
         sections: sp.InputSections = sp.parse_sections(fid)
     print_text(sections.title, output_dir, "title.txt", override)
```

### Comparing `mckit-0.6.23/src/mckit/cli/commands/transform.py` & `mckit-0.6.24/src/mckit/cli/commands/transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-# -*- coding: utf-8 -*-
 """Apply transformation to a model."""
+from __future__ import annotations
+
 from pathlib import Path
 
 from mckit.cli.logging import logger
 from mckit.parser.mcnp_input_sly_parser import ParseResult, from_file
 from mckit.parser.mcnp_section_parser import clean_mcnp_cards, split_to_cards
 from mckit.parser.transformation_parser import parse as parse_transformation
 from mckit.universe import Universe
```

### Comparing `mckit-0.6.23/src/mckit/cli/logging.py` & `mckit-0.6.24/src/mckit/cli/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Intercept log messages from the used libraries and pass them to `loguru`.
 
 See https://github.com/Delgan/loguru
 """
+from __future__ import annotations
+
 from typing import Final
 
 import logging
 import sys
 
 from os import environ
```

### Comparing `mckit-0.6.23/src/mckit/cli/runner.py` & `mckit-0.6.24/src/mckit/cli/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from __future__ import annotations
 
 import sys
 
 from contextlib import contextmanager
 from pathlib import Path
 
 import click
@@ -146,27 +146,26 @@
 def concat(output, parts_encoding, output_encoding, parts):
     """Concat text files.
 
     (will filter texts according specification in future)
     """
     override = context["OVERRIDE"]
     with resolve_output(output, exist_ok=override, encoding=output_encoding) as out_fid:
-        for f in parts:
-            f = Path(f)
+        for f in map(Path, parts):
             # TODO dvp: Add filtering of a part's text here. Implement as external scripts call.
             #           Should be configurable
             print(f.read_text(encoding=parts_encoding), file=out_fid, end="")
 
 
 # noinspection PyCompatibility
 @mckit.command()
 @click.argument(
     "sources", metavar="<source>", type=click.Path(exists=True), nargs=-1, required=True
 )
-def check(sources: List[click.Path]) -> None:
+def check(sources: list[click.Path]) -> None:
     """Read MCNP model(s) and show statistics and clashes."""
     for source in sources:
         do_check(source)
 
 
 # noinspection PyCompatibility
 @mckit.command()
```

### Comparing `mckit-0.6.23/src/mckit/data/isotopes.dat` & `mckit-0.6.24/src/mckit/data/isotopes.dat`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/src/mckit/fmesh.py` & `mckit-0.6.24/src/mckit/fmesh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: utf-8 -*-
+from __future__ import annotations
 
 import numpy as np
 
 # noinspection PyUnresolvedReferences,PyPackageRequirements
 from mckit.geometry import EX, EY, EZ, Box
 
 from .transformation import Transformation
@@ -20,15 +20,15 @@
     ----------
     xbins, ybins, zbins : array_like[float]
         Bins of mesh in every direction. The last bin value gives dimension of
         mesh in this direction.
     transform : Trnasformation
         Transformation for the mesh. Default: None.
 
-    Methods
+    Methods:
     -------
     shape() - gets the shape of mesh.
     get_voxel(i, j, k) - gets the voxel of RectMesh with indices i, j, k.
     """
 
     def __init__(self, xbins, ybins, zbins, transform: Transformation = None):
         self._xbins = np.array(xbins)
@@ -44,15 +44,15 @@
 
     def __eq__(self, other):
         return self is other
 
     def bounding_box(self):
         """Gets the bounding box of the cell.
 
-        Returns
+        Returns:
         -------
         bbox : Box
             Bounding box.
         """
         origin = [
             0.5 * (self._xbins[0] + self._xbins[-1]),
             0.5 * (self._ybins[0] + self._ybins[-1]),
@@ -85,15 +85,15 @@
         """Gets voxel.
 
         Parameters
         ----------
         i, j, k : int
             Indices of the voxel.
 
-        Returns
+        Returns:
         -------
         voxel : Box
             The box that describes the voxel.
         """
         cx = 0.5 * (self._xbins[i] + self._xbins[i + 1])
         cy = 0.5 * (self._ybins[j] + self._ybins[j + 1])
         cz = 0.5 * (self._zbins[k] + self._zbins[k + 1])
@@ -111,15 +111,15 @@
         Parameters
         ----------
         point : array_like[float]
             Coordinates of the point to be checked.
         local : bool
             If point is specified in local coordinate system.
 
-        Returns
+        Returns:
         -------
         i, j, k : int
             Indices along each dimension of voxel, where the point is located.
         """
         if self._tr and not local:
             point = self._tr.reverse().apply2point(point)
         else:
@@ -128,41 +128,38 @@
         y_proj = np.dot(point, EY)
         z_proj = np.dot(point, EZ)
         i = np.searchsorted(self._xbins, x_proj) - 1
         j = np.searchsorted(self._ybins, y_proj) - 1
         k = np.searchsorted(self._zbins, z_proj) - 1
         if len(point.shape) == 1:
             return self.check_indices(i, j, k)
-        else:
-            print("i=", i, "j=", j, "k=", k)
-            indices = []
-            for x, y, z in zip(i, j, k):
-                indices.append(self.check_indices(x, y, z))
-            return indices
+        indices = []
+        for x, y, z in zip(i, j, k):
+            indices.append(self.check_indices(x, y, z))
+        return indices
 
     def check_indices(self, i, j, k):
         """Check if the voxel with such indices really exists.
 
         Parameters
         ----------
         i, j, k : int
             Indices along x, y and z dimensions.
 
-        Returns
+        Returns:
         -------
         index_tuple : tuple(int)
             A tuple of indices if such voxel exists. None otherwise.
         """
         i = self._check_x(i)
         j = self._check_y(j)
         k = self._check_z(k)
         if i is None or j is None or k is None:
             return None
-        else:
-            return i, j, k
+        return i, j, k
 
     def _check_x(self, i):
         if i < 0 or i >= self._xbins.size - 1:
             return None
         return i
 
     def _check_y(self, j):
@@ -179,15 +176,15 @@
         """Gets index and axis of slice.
 
         Parameters
         ----------
         X, Y, Z : float
             Point of slice in local coordinate system.
 
-        Returns
+        Returns:
         -------
         axis : int
             Number of axis.
         index : int
             Index along axis.
         x, y : ndarray[float]
             Centers of bins along free axes.
@@ -267,15 +264,15 @@
         cells : list[Body]
             List of cells.
         verbose : bool
             Verbose output during calculations.
         min_volume : float
             Minimum volume for cell volume calculations
 
-        Returns
+        Returns:
         -------
         volumes : dict
             Volumes of cells for every voxel. It is dictionary cell -> vol_matrix.
             vol_matrix is SparseData instance - volume of cell for each voxel.
         """
         raise NotImplementedError
 
@@ -283,15 +280,15 @@
         """Gets voxel.
 
         Parameters
         ----------
         i, j, k : int
             Indices of the voxel.
 
-        Returns
+        Returns:
         -------
         voxel : Box
             The box that describes the voxel.
         """
         raise NotImplementedError
 
     def voxel_index(self, point, local=False):
@@ -300,41 +297,40 @@
         Parameters
         ----------
         point : array_like[float]
             Coordinates of the point to be checked.
         local : bool
             If point is specified in local coordinate system.
 
-        Returns
+        Returns:
         -------
         i, j, k : int
             Indices along each dimension of voxel, where the point is located.
         """
         raise NotImplementedError
 
     def check_indices(self, i, j, k):
         """Check if the voxel with such indices really exists.
 
         Parameters
         ----------
         i, j, k : int
             Indices along x, y and z dimensions.
 
-        Returns
+        Returns:
         -------
         index_tuple : tuple(int)
             A tuple of indices if such voxel exists. None otherwise.
         """
         i = self._check_r(i)
         j = self._check_z(j)
         k = self._check_t(k)
         if i is None or j is None or k is None:
             return None
-        else:
-            return i, j, k
+        return i, j, k
 
     def _check_r(self, i):
         if i < 0 or i >= self._rbins.size - 1:
             return None
         return i
 
     def _check_z(self, j):
@@ -351,15 +347,15 @@
         """Gets index and axis of slice.
 
         Parameters
         ----------
         R, Z, T : float
             Point of slice in local coordinate system.
 
-        Returns
+        Returns:
         -------
         axis : int
             Number of axis.
         index : int
             Index along axis.
         x, y : ndarray[float]
             Centers of bins along free axes.
@@ -397,15 +393,15 @@
     transform : Transformation
         Transformation to be applied to the spatial mesh.
     histories : int
         The number of histories run to obtain meshtal data.
     modifier : None
         Data transformation.
 
-    Methods
+    Methods:
     -------
     get_slice()
         Gets specific slice of data.
     get_spectrum(point)
         Gets energy spectrum at the specified point.
     get_spectrum_by_index(index)
         Gets energy spectrum at the specified mesh index.
@@ -447,15 +443,15 @@
         self._modifier = modifier
         if rbins is None and tbins is None:
             self._mesh = RectMesh(xbins, ybins, zbins, transform=transform)
         elif xbins is None and ybins is None:
             self._mesh = CylMesh(origin, axis, vec, rbins, zbins, tbins)
         if self._data.shape[1:] != self._mesh.shape:
             raise ValueError("Incorrect data shape")
-        elif self._error.shape[1:] != self._mesh.shape:
+        if self._error.shape[1:] != self._mesh.shape:
             raise ValueError("Incorrect error shape")
 
     @property
     def mesh(self):
         return self._mesh
 
     @property
@@ -466,15 +462,15 @@
     def histories(self):
         """The number of histories in the run."""
         return self._histories
 
     def mean_flux(self):
         """Gets average flux.
 
-        Returns
+        Returns:
         -------
         ebins : np.array[float]
             Energy bin boundaries.
         flux : np.array[float]
             Average flux in each energy bin.
         """
         return self._ebins.copy(), np.mean(self._data, axis=(1, 2, 3))
@@ -483,37 +479,37 @@
         """Gets energy spectrum at the specified point.
 
         Parameters
         ----------
         point : arraylike[float]
             Point energy spectrum must be get at.
 
-        Returns
+        Returns:
         -------
         energies: ndarray[float]
             Energy bins for the spectrum at the point - group boundaries.
         flux : ndarray[float]
             Group flux at the point.
         err : ndarray[float]
             Relative errors for flux components.
         """
         index = self._mesh.voxel_index(point)
         if index is None:
-            raise ValueError("Point {0} lies outside of the mesh.".format(point))
+            raise ValueError(f"Point {point} lies outside of the mesh.")
         return self.get_spectrum_by_index(index)
 
     def get_spectrum_by_index(self, index):
         """Gets energy spectrum in the specified voxel.
 
         Parameters
         ----------
         index : tuple[int]
             Indices of spatial mesh bins.
 
-        Returns
+        Returns:
         -------
         energies: ndarray[float]
             Energy bins for the spectrum at the point - group boundaries.
         flux : ndarray[float]
             Group flux at the point.
         err : ndarray[float]
             Relative errors for flux components.
@@ -530,15 +526,15 @@
         ----------
         E : str or float
             Energy value of interest. It specifies energy bin. If 'total' - then data
             is summed across energy axis.
         X, Y, Z : float
             Spatial point which belongs to the slice plane. Other two dimensions are free.
 
-        Returns
+        Returns:
         -------
         x, y : ndarray[float]
             Centers of spatial bins in free directions.
         data : ndarray[float]
             Data
         err : ndarray[float]
             Relative errors for data.
```

### Comparing `mckit-0.6.23/src/mckit/material.py` & `mckit-0.6.24/src/mckit/material.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Any, Dict, Iterable, Tuple, Union, cast
+from __future__ import annotations
+
+from typing import Any, Iterable, Tuple, Union, cast
 
 import math
 import os
 import sys
 
 from functools import reduce
 from operator import xor
@@ -57,15 +59,15 @@
     atomic : list
         Atomic fractions.
     weight : list
         Weight fractions.
     options : dict
         Dictionary of composition options.
 
-    Methods
+    Methods:
     -------
     molar_mass()
         Gets molar mass of the composition.
     get_atomic(isotope)
         Gets atomic fraction of the isotope.
     get_weight(isotope)
         Gets weight fraction of the isotope.
@@ -84,24 +86,24 @@
         self._composition = {}  # type Dict[Element, float]
         elem_w = []
         frac_w = []
 
         if weight:
             for elem, frac in weight:
                 if not isinstance(elem, Element):
-                    elem = Element(elem)
+                    elem = Element(elem)  # noqa: PLW2901 - elem is to be overwritten
                 elem_w.append(elem)
                 frac_w.append(frac)
 
         elem_a = []
         frac_a = []
         if atomic:
             for elem, frac in atomic:
                 if not isinstance(elem, Element):
-                    elem = Element(elem)
+                    elem = Element(elem)  # noqa: PLW2901 - elem is to be overwritten
                 elem_a.append(elem)
                 frac_a.append(frac)
 
         if len(frac_w) + len(frac_a) > 0:
             total_frac_w = np.sum(frac_w)
             total_frac_a = np.sum(frac_a)
             atoms_in_weight_spec = np.sum(np.divide(frac_w, [e.molar_mass for e in elem_w]))
@@ -163,37 +165,37 @@
 
     def __hash__(self):
         return reduce(
             xor, map(hash, self._composition.keys())
         )  # TODO dvp: check why self._hash is not used?
 
     def mcnp_words(self, pretty=False):
-        words = ["M{0} ".format(self.name())]
+        words = [f"M{self.name()} "]
         for elem, frac in self._composition.items():
             words.append(elem.mcnp_repr())
             words.append("  ")
             words.append(MATERIAL_FRACTION_FORMAT.format(frac))
             words.append("\n")
         return words
 
     def __getitem__(self, key):
         return self.options[key]
 
     def __iter__(self):
         return iter(self._composition.items())
 
-    def __contains__(self, item: Union[str, "Element"]) -> bool:
+    def __contains__(self, item: str | Element) -> bool:
         """Checks if the composition contains the item.
 
         Parameters
         ----------
         item :
             Isotope. It can be either isotope name or Element instance.
 
-        Returns
+        Returns:
         -------
         result :
             True if the composition contains the isotope, False otherwise.
         """
         if not isinstance(item, Element):
             item = Element(item)
         return item in self._composition
@@ -204,15 +206,15 @@
         Raises KeyError if the composition doesn't contain the isotope.
 
         Parameters
         ----------
         isotope : str or Element
             Isotope. It can be either isotope name or Element instance.
 
-        Returns
+        Returns:
         -------
         frac : float
             Atomic fraction of the specified isotope.
         """
         if not isinstance(isotope, Element):
             isotope = Element(isotope)
         return self._composition[isotope]
@@ -223,15 +225,15 @@
         Raises KeyError if the composition doesn't contain the isotope.
 
         Parameters
         ----------
         isotope : str or Element
             Isotope. It can be either isotope name or Element instance.
 
-        Returns
+        Returns:
         -------
         frac : float
             Weight fraction of the specified isotope.
         """
         if not isinstance(isotope, Element):
             isotope = Element(isotope)
         at = self._composition[isotope]
@@ -241,15 +243,15 @@
     def molar_mass(self):
         """Gets composition's effective molar mass [g / mol]."""
         return self._mu
 
     def expand(self):
         """Expands elements with natural abundances into detailed isotope composition.
 
-        Returns
+        Returns:
         -------
         new_comp : Composition
             New expanded composition or self.
         """
         composition = {}
         already = True
         for el, conc in self._composition.items():
@@ -257,29 +259,28 @@
                 already = False
             for isotope, frac in el.expand().items():
                 if isotope not in composition.keys():
                     composition[isotope] = 0
                 composition[isotope] += conc * frac
         if already:
             return self
-        else:
-            return Composition(atomic=composition.items(), **self.options)
+        return Composition(atomic=composition.items(), **self.options)
 
     def natural(self, tolerance=1.0e-8):
         """Tries to replace detailed isotope composition by natural elements.
 
         Modifies current object.
 
         Parameters
         ----------
         tolerance : float
             Relative tolerance to consider isotope fractions as equal.
             Default: 1.e-8
 
-        Returns
+        Returns:
         -------
         comp : Composition
             self, if composition is reduced successfully to natural. None returned if the
             composition cannot be reduced to natural.
         """
         already = True
         by_charge = {}  # type: Dict[int, Dict[int, float]]
@@ -317,23 +318,23 @@
         return Composition(atomic=cast(TFractions, composition.items()), **self.options)
 
     def elements(self):
         """Gets iterator over composition's elements."""
         return iter(self._composition.keys())
 
     @staticmethod
-    def mixture(*compositions: Tuple["Composition", float]) -> "Composition":
+    def mixture(*compositions: tuple[Composition, float]) -> Composition:
         """Makes mixture of the compositions with specific fractions.
 
         Parameters
         ----------
         compositions :
             List of pairs composition, fraction.
 
-        Returns
+        Returns:
         -------
         mix :
             Mixture.
         """
         atomics = []
         if len(compositions) == 1:
             return compositions[0][0]
@@ -374,15 +375,15 @@
     concentration : float
         Concentration of the material [atoms/cc].
     composition : Composition
         Material's composition.
     molar_mass : float
         Material's molar mass [g/mol].
 
-    Methods
+    Methods:
     -------
     correct(old_vol, new_vol)
         Correct material density - returns the corrected version of the
         material.
     mixture(*materials, fraction_type)
         Makes a mixture of specified materials in desired proportions.
     __getitem__(key)
@@ -407,15 +408,15 @@
         elif not composition and (weight or atomic):
             self._composition = Composition(atomic=atomic, weight=weight, **options)
         else:
             raise ValueError("Incorrect set of parameters.")
 
         if concentration and density or not concentration and not density:
             raise ValueError("Incorrect set of parameters.")
-        elif concentration:
+        if concentration:
             self._n = concentration
         else:
             self._n = density * AVOGADRO / self._composition.molar_mass
         self._options = options
 
     def __eq__(self, other):
         if not math.isclose(self._n, other.concentration, rel_tol=self._tolerance):
@@ -459,15 +460,15 @@
             Initial volume of the cell.
         new_vol : float
             New volume of the cell.
         factor : float
             By this factor density of material will be multiplied. If factor
             is specified, then its value will be used.
 
-        Returns
+        Returns:
         -------
         new_mat : Material
             New material that takes into account new volume of the cell.
         """
         if factor is None:
             factor = old_vol / new_vol
         return Material(
@@ -494,29 +495,38 @@
             important.
         fraction_type : str
             Indicate how fraction should be interpreted.
             'weight' - weight fractions (default);
             'volume' - volume fractions;
             'atomic' - atomic fractions.
 
-        Returns
+        Returns:
         -------
         material : Material
             New material.
         """
         if not materials:
             raise ValueError("At least one material must be specified.")
         if fraction_type == "weight":
-            fun = lambda m, f: f / m.molar_mass
+
+            def fun(m, f):
+                return f / m.molar_mass
+
             norm = sum(fun(m, f) / m.concentration for m, f in materials)
         elif fraction_type == "volume":
-            fun = lambda m, f: f * m.concentration
+
+            def fun(m, f):
+                return f * m.concentration
+
             norm = 1
         elif fraction_type == "atomic":
-            fun = lambda m, f: f
+
+            def fun(m, f):
+                return f
+
             norm = sum(fun(m, f) / m.concentration for m, f in materials)
         else:
             raise ValueError("Unknown fraction type")
         factor = sum([fun(m, f) for m, f in materials])
         compositions = [(m.composition, fun(m, f) / factor) for m, f in materials]
         new_comp = Composition.mixture(*compositions)
         return Material(composition=new_comp, concentration=factor / norm)
@@ -535,25 +545,25 @@
     comment : str, optional
         Optional comment to the element.
     lib : str
         Data library ID. Usually it is MCNP library, like '31b' for FENDL31b.
     isomer : int
         Isomer level. Default 0. Usually may appear in FISPACT output.
 
-    Methods
+    Methods:
     -------
     expand()
         Expands natural composition of this element.
     fispact_repr()
         Gets FISPACT representation of the element.
     mcnp_repr()
         Gets MCNP representation of the element.
     """
 
-    def __init__(self, _name: Union[str, int], lib=None, isomer=0, comment=None):
+    def __init__(self, _name: str | int, lib=None, isomer=0, comment=None):
         if isinstance(_name, int):
             self._charge = _name // 1000
             self._mass_number = _name % 1000
         else:
             z, a = self._split_name(_name.upper())
             if z.isalpha():
                 self._charge = _NAME_TO_CHARGE[z]
@@ -588,16 +598,15 @@
     def __eq__(self, other):
         if (
             self._charge == other.charge
             and self._mass_number == other.mass_number
             and self._isomer == other._isomer
         ):
             return True
-        else:
-            return False
+        return False
 
     def __str__(self):
         _name = _CHARGE_TO_NAME[self.charge].capitalize()
         if self._mass_number > 0:
             _name += "-" + str(self._mass_number)
             if self._isomer > 0:
                 _name += "m"
@@ -605,15 +614,15 @@
                 _name += str(self._isomer - 1)
         return _name
 
     def mcnp_repr(self):
         """Gets MCNP representation of the element."""
         _name = str(self.charge * 1000 + self.mass_number)
         if self.lib is not None:
-            _name += ".{0}".format(self.lib)
+            _name += f".{self.lib}"
         return _name
 
     def fispact_repr(self):
         """Gets FISPACT representation of the element."""
         _name = _CHARGE_TO_NAME[self.charge].capitalize()
         if self._mass_number > 0:
             _name += str(self._mass_number)
@@ -647,34 +656,34 @@
     def isomer(self):
         """Gets isomer level."""
         return self._isomer
 
     def expand(self):
         """Expands natural element into individual isotopes.
 
-        Returns
+        Returns:
         -------
         elements : dict
             A dictionary of elements that are comprised by this one.
             Keys - elements - Element instances, values - atomic fractions.
         """
         result = {}
         if self._mass_number > 0 and self._mass_number in _NATURAL_ABUNDANCE[self._charge].keys():
             result[self] = 1.0
         elif self._mass_number == 0:
             for at_num, frac in _NATURAL_ABUNDANCE[self._charge].items():
-                elem_name = "{0:d}{1:03d}".format(self._charge, at_num)
+                elem_name = f"{self._charge:d}{at_num:03d}"
                 result[Element(elem_name, lib=self._lib)] = frac
         return result
 
     @staticmethod
-    def _split_name(_name: str) -> Tuple[str, str]:
+    def _split_name(_name: str) -> tuple[str, str]:
         """Splits element's name into charge and mass number parts."""
         if _name.isnumeric():
             return _name[:-3], _name[-3:]
-        for i, l in enumerate(_name):
-            if l.isdigit():
+        for i, t in enumerate(_name):  # noqa: B007 - `i` is used below
+            if t.isdigit():
                 break
         else:
             return _name, "0"
         q = _name[: i - 1] if _name[i - 1] == "-" else _name[:i]
         return q, _name[i:]
```

### Comparing `mckit-0.6.23/src/mckit/parser/cell_parser.py` & `mckit-0.6.24/src/mckit/parser/cell_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional
+from __future__ import annotations
 
 import mckit.parser.common.utils as pu
 import sly
 
 from mckit.body import Body, Shape
 from mckit.material import Material
 from mckit.parser.common import CellStrictIndex, CompositionStrictIndex
@@ -218,16 +218,15 @@
     def attributes(self, p):
         result = p.attributes
         result.update(p.attribute)
         return result
 
     @_("attribute")
     def attributes(self, p):
-        result = p[0]
-        return result
+        return p[0]
 
     @_(
         "fill_attribute",
         "trcl_attribute",
         "imp_attribute",
         "float_attribute",
         "int_attribute",
@@ -293,43 +292,42 @@
 
     @_("translation")
     def transform_params(self, p):
         return p.translation, None, False
 
     @_("float float float")
     def translation(self, p):
-        return [f for f in p]
+        return list(p)
 
     @_("float float float float float float float float float INTEGER")
     def rotation(self, p):
         m = p[9]
         assert m == -1 or m == 1, f"Invalid value for transformation M parameter {m}"
-        return [f for f in p][:-1], m == -1
+        return list(p)[:-1], m == -1
 
     @_(
         "float float float float float float float float float",
         "float float float float float float",
         "float float float float float",
         "float float float",
     )
     def rotation(self, p):
-        return [f for f in p], False
+        return list(p), False
 
     #
     #  See MCNP, vol.I, p.3-7
     #  Example: IMP:E,P,N 1 1 0.
     #
     @_('IMP ":" particle_list float_list')
     def imp_attribute(self, p):
         number_of_particles = len(p.particle_list)
         if number_of_particles != len(p.float_list):
             while len(p.float_list) < number_of_particles:
                 p.float_list.append(p.float_list[-1])
-        result = dict(("IMP" + k, v) for k, v in zip(p.particle_list, p.float_list))
-        return result
+        return {"IMP" + k: v for k, v in zip(p.particle_list, p.float_list)}
 
     @_("float_list float")
     def float_list(self, p):
         return p.float_list + [p.float]
 
     @_("float")
     def float_list(self, p):
@@ -342,16 +340,15 @@
 
     @_("particle")
     def particle_list(self, p):
         return [p.particle]
 
     @_("N", "P", "E")
     def particle(self, p):
-        result = pu.ensure_upper(p[0])
-        return result
+        return pu.ensure_upper(p[0])
 
     @_("FLOAT_ATTR float")
     def float_attribute(self, p):
         return {intern_cell_word(p.FLOAT_ATTR): p.float}
 
     @_("INT_ATTR integer")
     def int_attribute(self, p):
@@ -368,39 +365,38 @@
     @_("INTEGER", "ZERO")
     def integer(self, p):
         return p[0]
 
 
 def parse(
     text: str,
-    cells: Optional[Index] = None,
-    surfaces: Optional[Index] = None,
-    transformations: Optional[Index] = None,
-    compositions: Optional[Index] = None,
+    cells: Index | None = None,
+    surfaces: Index | None = None,
+    transformations: Index | None = None,
+    compositions: Index | None = None,
 ) -> Body:
-    cells, surfaces, transformations, compositions = map(
-        lambda x: x[1]() if x[0] is None else x[0],
-        zip(
+    cells, surfaces, transformations, compositions = (
+        x[1]() if x[0] is None else x[0]
+        for x in zip(
             [cells, surfaces, transformations, compositions],
             [
                 CellStrictIndex,
                 SurfaceStrictIndex,
                 TransformationStrictIndex,
                 CompositionStrictIndex,
             ],
-        ),
+        )
     )
     original = text
     text = pu.drop_c_comments(text)
     text, comments, trailing_comments = pu.extract_comments(text)
     lexer = Lexer()
     parser = Parser(
         cells,
         surfaces,
         transformations,
         compositions,
         comments,
         trailing_comments,
         original,
     )
-    result = parser.parse(lexer.tokenize(text))
-    return result
+    return parser.parse(lexer.tokenize(text))
```

### Comparing `mckit-0.6.23/src/mckit/parser/common/Lexer.py` & `mckit-0.6.24/src/mckit/parser/common/lexer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import re
 
 import sly
 
 # noinspection PyProtectedMember
 from sly.lex import LexError
 
@@ -33,31 +35,29 @@
         return token
 
     @_(r"\n+")
     def ignore_newline(self, token):
         self.lineno += len(token.value)
 
     def get_start_of_line(self, token):
-        prev_cr = self.text.rfind("\n", 0, token.index)
-        return prev_cr
+        return self.text.rfind("\n", 0, token.index)
 
     def get_end_of_line(self, token):
         next_cr = self.text.find("\n", token.index)
         if next_cr < 0:
             next_cr = len(self.text)
         return next_cr
 
     @staticmethod
     def column(token, prev_cr):
         return token.index - prev_cr
 
     def find_column(self, token):
         prev_cr = self.get_start_of_line(token)
-        column = Lexer.column(token, prev_cr)
-        return column
+        return Lexer.column(token, prev_cr)
 
     def error(self, token):
         prev_cr = self.get_start_of_line(token)
         next_cr = self.get_end_of_line(token)
         column = Lexer.column(token, prev_cr)
         msg = (
             f"Illegal character '{token.value[0]}', at line {self.lineno}, column {self.find_column(token)}\n"
```

### Comparing `mckit-0.6.23/src/mckit/parser/common/cell_index.py` & `mckit-0.6.24/src/mckit/parser/common/cell_index.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Iterable, Optional
+from __future__ import annotations
+
+from typing import Iterable
 
 from mckit.body import GLOBAL_BOX, Body, Card
 from mckit.constants import MIN_BOX_VOLUME
 from mckit.utils.indexes import Index, NumberedItemNotFoundError
 
 
 class DummyCell(Body):
@@ -44,28 +46,28 @@
     def fill(self, universe=None, recurrent=False, simplify=False, **kwargs):
         raise NotImplementedError("The method is not available in dummy object")
 
     def transform(self, tr):
         raise NotImplementedError("The method is not available in dummy object")
 
 
-def raise_on_absent_cell_strategy(name: int) -> Optional[DummyCell]:
+def raise_on_absent_cell_strategy(name: int) -> DummyCell | None:
     raise CellNotFoundError(name)
 
 
-def dummy_on_absent_cell_strategy(name: int) -> Optional[DummyCell]:
+def dummy_on_absent_cell_strategy(name: int) -> DummyCell | None:
     return DummyCell(name)
 
 
 class CellStrictIndex(Index):
     def __init__(self, **kwargs):
         super().__init__(raise_on_absent_cell_strategy, **kwargs)
 
     @classmethod
-    def from_iterable(cls, items: Iterable[Body]) -> "CellStrictIndex":
+    def from_iterable(cls, items: Iterable[Body]) -> CellStrictIndex:
         index = cls()
         index.update((c.name(), c) for c in items)
         return index
 
 
 class CellDummyIndex(Index):
     def __init__(self, **kwargs):
```

### Comparing `mckit-0.6.23/src/mckit/parser/common/composition_index.py` & `mckit-0.6.24/src/mckit/parser/common/composition_index.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from typing import Iterable, Optional
+from __future__ import annotations
+
+from typing import Iterable
 
 from mckit.material import Composition, Material
 from mckit.utils.indexes import Index, NumberedItemNotFoundError
 
 
 class DummyMaterial(Material):
     def __init__(
         self,
         name: int,
         *,
-        density: Optional[float] = None,
-        concentration: Optional[float] = None,
+        density: float | None = None,
+        concentration: float | None = None,
     ) -> None:
         assert (density is None) ^ (concentration is None), "Specify only one of the parameters"
         if density is None:
             # noinspection PyTypeChecker
             super().__init__(
                 composition=DummyComposition(name), concentration=concentration * 1.0e24
             )
@@ -26,28 +28,28 @@
 class DummyComposition(Composition):
     """To substitute composition when it's not found."""
 
     def __init__(self, name: int):
         super().__init__(name=name, weight=[(1001, 1.0)], comment="dummy")
 
 
-def raise_on_absent_composition_strategy(name: int) -> Optional[DummyComposition]:
+def raise_on_absent_composition_strategy(name: int) -> DummyComposition | None:
     raise CompositionNotFoundError(name)
 
 
-def dummy_on_absent_composition_strategy(name: int) -> Optional[DummyComposition]:
+def dummy_on_absent_composition_strategy(name: int) -> DummyComposition | None:
     return DummyComposition(name)
 
 
 class CompositionStrictIndex(Index):
     def __init__(self, **kwargs):
         super().__init__(raise_on_absent_composition_strategy, **kwargs)
 
     @classmethod
-    def from_iterable(cls, items: Iterable[Composition]) -> "CompositionStrictIndex":
+    def from_iterable(cls, items: Iterable[Composition]) -> CompositionStrictIndex:
         index = cls()
         index.update((c.name(), c) for c in items)
         return index
 
 
 class CompositionDummyIndex(Index):
     def __init__(self, **kwargs):
```

### Comparing `mckit-0.6.23/src/mckit/parser/common/surface_index.py` & `mckit-0.6.24/src/mckit/parser/common/surface_index.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Iterable, Optional
+from __future__ import annotations
+
+from typing import Iterable
 
 from mckit.surface import EX, Plane, Surface
 from mckit.utils.indexes import Index, NumberedItemNotFoundError
 
 
 class DummySurface(Plane):
     """Dummy surface to substitute surface when it's not found in a ``IgnoringIndex``."""
@@ -13,28 +15,28 @@
     def __str__(self) -> str:
         return str(self.name())
 
     def __repr__(self):
         return f"DummySurface({self.name()})"
 
 
-def raise_on_absent_surface_strategy(name: int) -> Optional[DummySurface]:
+def raise_on_absent_surface_strategy(name: int) -> DummySurface | None:
     raise SurfaceNotFoundError(name)
 
 
-def dummy_on_absent_surface_strategy(name: int) -> Optional[DummySurface]:
+def dummy_on_absent_surface_strategy(name: int) -> DummySurface | None:
     return DummySurface(name)
 
 
 class SurfaceStrictIndex(Index):
     def __init__(self, **kwargs):
         super().__init__(raise_on_absent_surface_strategy, **kwargs)
 
     @classmethod
-    def from_iterable(cls, items: Iterable[Surface]) -> "SurfaceStrictIndex":
+    def from_iterable(cls, items: Iterable[Surface]) -> SurfaceStrictIndex:
         index = cls()
         index.update((c.name(), c) for c in items)
         return index
 
 
 class SurfaceDummyIndex(Index):
     def __init__(self, **kwargs):
```

### Comparing `mckit-0.6.23/src/mckit/parser/common/transformation_index.py` & `mckit-0.6.24/src/mckit/parser/common/transformation_index.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from typing import Iterable, Optional
+from __future__ import annotations
+
+from typing import Iterable
 
 from mckit.transformation import Transformation
 from mckit.utils.indexes import Index, NumberedItemNotFoundError
 
 
 class DummyTransformation(Transformation):
     """To substitute transformation when it's not found."""
 
     def __init__(self, name: int):
         super().__init__(name=name, comment="dummy")
 
 
-def raise_on_absent_transformation_strategy(name: int) -> Optional[DummyTransformation]:
+def raise_on_absent_transformation_strategy(name: int) -> DummyTransformation | None:
     raise TransformationNotFoundError(name)
 
 
-def dummy_on_absent_transformation_strategy(name: int) -> Optional[DummyTransformation]:
+def dummy_on_absent_transformation_strategy(name: int) -> DummyTransformation | None:
     return DummyTransformation(name)
 
 
 class TransformationStrictIndex(Index):
     def __init__(self, **kwargs):
         super().__init__(raise_on_absent_transformation_strategy, **kwargs)
 
     @classmethod
-    def from_iterable(cls, items: Iterable[Transformation]) -> "TransformationStrictIndex":
+    def from_iterable(cls, items: Iterable[Transformation]) -> TransformationStrictIndex:
         index = cls()
         index.update((c.name(), c) for c in items)
         return index
 
 
 class TransformationDummyIndex(Index):
     def __init__(self, **kwargs):
```

### Comparing `mckit-0.6.23/src/mckit/parser/common/utils.py` & `mckit-0.6.24/src/mckit/parser/common/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Iterable
 
 import re
 
 C_COMMENT = r"(^|(?<=\n))\s{0,5}[cC]([ ][^\n]*)?\n?"
 RE_C_COMMENT = re.compile(C_COMMENT, re.MULTILINE)
 EOL_COMMENT = r"\$.*[^\n]*"
@@ -12,34 +14,34 @@
 FLOAT = r"[+-]?((\d+\.?\d*)|(\.\d+))(?:[ed][-+]?\d+)?"
 INTEGER = r"\d+"
 RE_EMPTY_LINE = re.compile(r"\s*")
 
 
 def ensure_lower(text: str):
     if not text.islower():
-        text = text.lower()
+        return text.lower()
     return text
 
 
 def ensure_upper(text: str):
     if not text.isupper():
-        text = text.upper()
+        return text.upper()
     return text
 
 
 def drop_c_comments(text: str) -> str:
     has_comments = RE_C_COMMENT.search(text)
     if has_comments:
-        text = RE_C_COMMENT.sub("", text)
+        return RE_C_COMMENT.sub("", text)
     return text
 
 
 def drop_eol_comments(text):
     if RE_EOL_COMMENT.search(text) is not None:
-        text = RE_EOL_COMMENT.sub("", text)
+        return RE_EOL_COMMENT.sub("", text)
     return text
 
 
 def drop_comments(text):
     return drop_eol_comments(drop_c_comments(text))
 
 
@@ -75,15 +77,15 @@
             else:
                 assert c is not None, "If there's no text, then at least comment should present"
                 trailing_comment.append(c)
 
     assert cleaned_text, "There should be some  text in a card"
 
     if comments:
-        comments = dict((k, tuple(v)) for k, v in comments)
+        comments = {k: tuple(v) for k, v in comments}
     else:
         comments = None
 
     if not trailing_comment:
         trailing_comment = None
 
     return "\n".join(cleaned_text), comments, trailing_comment
```

### Comparing `mckit-0.6.23/src/mckit/parser/material_parser.py` & `mckit-0.6.24/src/mckit/parser/material_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from __future__ import annotations
+
 import mckit.parser.common.utils as cmn
 import sly
 
 from mckit.material import Composition, Element
-from mckit.parser.common.Lexer import Lexer as LexerBase
+from mckit.parser.common.lexer import Lexer as LexerBase
 from mckit.parser.common.utils import drop_comments
 
 
 # noinspection PyPep8Naming,PyUnboundLocalVariable,PyUnresolvedReferences,SpellCheckingInspection
 class Lexer(LexerBase):
     tokens = {NAME, FRACTION, OPTION}
     ignore = " \t="
@@ -108,9 +110,8 @@
         return option, value
 
 
 def parse(text):
     text = drop_comments(text)
     lexer = Lexer()
     parser = Parser()
-    result = parser.parse(lexer.tokenize(text))
-    return result
+    return parser.parse(lexer.tokenize(text))
```

### Comparing `mckit-0.6.23/src/mckit/parser/mcnp_input_sly_parser.py` & `mckit-0.6.24/src/mckit/parser/mcnp_input_sly_parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# -*- coding: utf-8 -*-
 """
  Read and parse MCNP file text.
 """
-from typing import Any, Callable, Generator, Iterable, List, NewType, Optional, TextIO, Tuple, Union
+from __future__ import annotations
+
+from typing import Any, Callable, Generator, Iterable, NewType, TextIO, Tuple, Union
 
 from itertools import repeat
 from pathlib import Path
 
 from attr import attrib, attrs
 from mckit.card import Card
 from mckit.constants import MCNP_ENCODING
@@ -38,30 +39,30 @@
 Pair = NewType("Pair", Tuple[T1, T2])
 YieldGenerator = NewType("YieldGenerator", Generator[T, None, None])
 
 
 @attrs
 class ParseResult:
     universe: Universe = attrib()
-    cells: List[Body] = attrib()
+    cells: list[Body] = attrib()
     cells_index: CellStrictIndex = attrib()
-    surfaces: List[Surface] = attrib()
+    surfaces: list[Surface] = attrib()
     surfaces_index: SurfaceStrictIndex = attrib()
-    compositions: Optional[List[Composition]] = attrib()
-    compositions_index: Optional[CompositionStrictIndex] = attrib()
-    transformations: Optional[List[Transformation]] = attrib()
-    transformations_index: Optional[TransformationStrictIndex] = attrib()
+    compositions: list[Composition] | None = attrib()
+    compositions_index: CompositionStrictIndex | None = attrib()
+    transformations: list[Transformation] | None = attrib()
+    transformations_index: TransformationStrictIndex | None = attrib()
     sections: InputSections = attrib()
 
     @property
     def title(self):
         return self.sections.title
 
 
-def from_file(path: Union[str, Path]) -> ParseResult:
+def from_file(path: str | Path) -> ParseResult:
     if isinstance(path, str):
         path = Path(path)
     with path.open("r", encoding=MCNP_ENCODING) as fid:
         return from_stream(fid)
 
 
 def from_stream(stream: TextIO) -> ParseResult:
@@ -113,15 +114,15 @@
     "TSectionGenerator",
     Generator[Union[Transformation, Composition, Surface], None, None],
 )
 
 
 def join_comments(text_cards: Iterable[TextCard]):
     def _iter():
-        comment: Optional[str] = None
+        comment: str | None = None
         for card in text_cards:
             if card.is_comment:
                 assert comment is None, f"Comment is already set {comment[:70]}"
                 comment = card.text
             else:
                 assert (
                     not card.is_comment
@@ -148,51 +149,51 @@
                 card.options["comment_above"] = comment
             # card.options['original'] = text_card.text
             yield card
 
     return iterator()
 
 
-def parse_transformations(text_cards: Iterable[TextCard]) -> List[Transformation]:
+def parse_transformations(text_cards: Iterable[TextCard]) -> list[Transformation]:
     return list(parse_section(text_cards, Kind.TRANSFORMATION, parse_transformation))
 
 
-def parse_compositions(text_cards: Iterable[TextCard]) -> List[Composition]:
+def parse_compositions(text_cards: Iterable[TextCard]) -> list[Composition]:
     return list(parse_section(text_cards, Kind.MATERIAL, parse_composition))
 
 
-def parse_surfaces(text_cards: Iterable[TextCard], transformations: Index) -> List[Surface]:
+def parse_surfaces(text_cards: Iterable[TextCard], transformations: Index) -> list[Surface]:
     def parser(text: str):
         return parse_surface(text, transformations=transformations)
 
     return list(parse_section(text_cards, Kind.SURFACE, parser))
 
 
 def extract_number(text_card: TextCard):
     return int(text_card.text.split(maxsplit=1)[0])
 
 
 class MissedCellsError(RuntimeError):
-    def __init__(self, missed_cells: List[int]):
+    def __init__(self, missed_cells: list[int]):
         self.missed_cells = missed_cells
         msg = f"Not found cells: {missed_cells}"
         super().__init__(msg)
 
     @classmethod
     def from_text_cards(cls, missed_cells: Iterable[TextCard]):
-        missed_cells_numbers: List[int] = list(map(extract_number, missed_cells))
+        missed_cells_numbers: list[int] = list(map(extract_number, missed_cells))
         return cls(missed_cells_numbers)
 
 
 def parse_cells(
-    text_cards: List[TextCard],
+    text_cards: list[TextCard],
     surfaces: Index,
     compositions: Index,
     transformations: Index,
-) -> Tuple[List[Body], CellStrictIndex]:
+) -> tuple[list[Body], CellStrictIndex]:
     text_cards_with_comments = join_comments(text_cards)
     size = len(text_cards_with_comments)
     cells_index = CellStrictIndex()
     cells_to_process = list(range(size))
     cells = list(repeat(None, size))
 
     def parser(text: str):
@@ -218,15 +219,15 @@
                 continue
             if comment:
                 card.options["comment_above"] = comment
             card.options["original"] = text_card.text
             cells[i] = card
             cells_index[card.name()] = card
         if cells_to_process_length == len(new_cells_to_process):
-            missed_cells_cards = list(text_cards[i] for i in new_cells_to_process)
+            missed_cells_cards = [text_cards[i] for i in new_cells_to_process]
             raise MissedCellsError.from_text_cards(missed_cells_cards)
         cells_to_process = new_cells_to_process
 
-    if any(map(lambda c: c is None, cells)):
+    if any(c is None for c in cells):
         cells = list(filter(lambda c: c is not None, cells))
 
     return cells, cells_index
```

### Comparing `mckit-0.6.23/src/mckit/parser/mcnp_section_parser.py` & `mckit-0.6.24/src/mckit/parser/mcnp_section_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Generator, Iterable, List, Optional, TextIO, Tuple
+from __future__ import annotations
+
+from typing import Generator, Iterable, TextIO
 
 import re
 import sys
 
 from enum import IntEnum
 
 from attr import attrib, attrs
@@ -10,14 +12,15 @@
 BLANK_LINE_PATTERN = re.compile(r"\n\s*\n", flags=re.MULTILINE)
 COMMENT_LINE_PATTERN = re.compile(r"^\s{,5}[cC]( .*)?\s*$")
 # pattern to remove comments from a card text
 REMOVE_COMMENT_PATTERN = re.compile(
     r"(\s*\$.*$)|(^\s{0,5}c\s.*\n?)", flags=re.MULTILINE | re.IGNORECASE
 )
 # pattern to split section text to optional "comment" and subsequent MCNP card pairs
+# noinspection RegExpUnexpectedAnchor
 CARD_PATTERN = re.compile(
     r"(?P<comment>((^\s{,5}c( .*)?\s*$)\n?)+)?(?P<card>^\s{,5}(\*|\+|\w).*(\n((^\s{,5}c.*\n?)*^\s{5,}\S.*\n?)*)?)?",
     flags=re.MULTILINE | re.IGNORECASE,
 )
 
 # pattern to replace subsequent spaces with a single one
 SPACE_PATTERN = re.compile(r"\s+", flags=re.MULTILINE)
@@ -56,24 +59,24 @@
             return Kind.TALLY
         if is_comment(text):
             return Kind.COMMENT
         return Kind.GENERIC
 
 
 @attrs(str=False)
-class Card(object):
+class Card:
     """
     Generic MCNP card raw text item
 
     The card kind is defined either from parsing context (for cells and surfaces) or
     from card label
     """
 
     text: str = attrib()
-    kind: Optional[Kind] = attrib(default=None)
+    kind: Kind | None = attrib(default=None)
 
     # noinspection PyUnusedLocal,PyUnresolvedReferences
     @kind.validator
     def check(self, attribute, value) -> None:
         if self.kind is None:
             self.kind = Kind.from_card_text(self.text)
 
@@ -120,36 +123,35 @@
     def number(self) -> int:
         name = self.name
         if self.is_cell:
             return int(name)
         if self.is_surface:
             if name.isdigit():
                 return int(name)
-            else:
-                assert name[0] in "%*", "Expected reflecting, white surface"
-                return int(name[1:])
+            assert name[0] in "%*", "Expected reflecting, white surface"
+            return int(name[1:])
         if self.is_material:
             return int(name[1:])
         if self.is_transformation:
             i = 0
             if name[0] == "*":
                 i = 1
             if name[i] in "tT" and name[i + 1] in "rR" and name[i + 2 :].isdigit():
                 return int(name[i + 2 :])
         raise NotImplementedError(f"Cannot define number for {self.kind} card '{name}'")
 
 
 @attrs
-class InputSections(object):
-    title: Optional[str] = attrib(default=None)
-    cell_cards: Optional[List[Card]] = attrib(default=None)
-    surface_cards: Optional[List[Card]] = attrib(default=None)
-    data_cards: Optional[List[Card]] = attrib(default=None)
-    message: Optional[str] = attrib(default=None)
-    remainder: Optional[str] = attrib(default=None)
+class InputSections:
+    title: str | None = attrib(default=None)
+    cell_cards: list[Card] | None = attrib(default=None)
+    surface_cards: list[Card] | None = attrib(default=None)
+    data_cards: list[Card] | None = attrib(default=None)
+    message: str | None = attrib(default=None)
+    remainder: str | None = attrib(default=None)
     is_continue: bool = attrib(default=False)
 
     # noinspection PyUnusedLocal,PyUnresolvedReferences
     @is_continue.validator
     def check(self, attribute, value) -> None:
         if self.is_continue:
             if self.cell_cards or self.surface_cards:
@@ -244,15 +246,15 @@
     cell_cards = None
     surface_cards = None
     data_cards = None
     remainder = None
 
     sections = BLANK_LINE_PATTERN.split(text, 5)
 
-    # The first line can be message or title.
+    # The first line can be a message or a title.
     kw = sections[0][: len("message:")].lower()
 
     i = 0
 
     if "message:" == kw:
         message = sections[0]
         i += 1
@@ -310,45 +312,43 @@
 
 
 def is_comment(text: str) -> bool:
     assert isinstance(text, str), "The parameter 'line' should be text"
     if "\n" in text:
         res = next((line for line in text.split("\n") if not is_comment_line(line)), False)
         return not res
-    else:
-        return is_comment_line(text, skip_asserts=True)
+    return is_comment_line(text, skip_asserts=True)
 
 
 def is_comment_line(line: str, skip_asserts=False) -> bool:
     if not skip_asserts:
         assert isinstance(line, str), "The parameter 'line' should be text"
         assert "\n" not in line, "The parameter 'line' should be the single text line"
     return COMMENT_LINE_PATTERN.match(line) is not None
 
 
 def get_clean_text(text: str) -> str:
     without_comments = REMOVE_COMMENT_PATTERN.sub("", text)
-    with_spaces_normalized = SPACE_PATTERN.sub(" ", without_comments)
-    return with_spaces_normalized
+    return SPACE_PATTERN.sub(" ", without_comments)
 
 
 def clean_mcnp_cards(iterable: Iterable[Card]) -> Generator[Card, None, None]:
     for x in iterable:
         if x.kind is not Kind.COMMENT:
             clean_text = x.get_clean_text()
             t = Card(clean_text, kind=x.kind)
             yield t
 
 
 def distribute_cards(
     cards: Iterable[Card],
-) -> Tuple[List[Card], List[Card], List[Card], List[Card], List[Card]]:
-    comment: Optional[Card] = None
+) -> tuple[list[Card], list[Card], list[Card], list[Card], list[Card]]:
+    comment: Card | None = None
 
-    def append(_cards: List[Card], _card: Card) -> None:
+    def append(_cards: list[Card], _card: Card) -> None:
         nonlocal comment
         if comment:
             _cards.append(comment)
             comment = None
         _cards.append(_card)
 
     # fmt: off
```

### Comparing `mckit-0.6.23/src/mckit/parser/mctal_parser.py` & `mckit-0.6.24/src/mckit/parser/mctal_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import re
 
 from collections import deque
 from itertools import product
 
 import numpy as np
```

### Comparing `mckit-0.6.23/src/mckit/parser/meshtal_parser.py` & `mckit-0.6.24/src/mckit/parser/meshtal_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,16 @@
 
 import re
 
 from pathlib import Path
 
 import numpy as np
 
-import ply.lex as lex
-import ply.yacc as yacc
-
 from mckit.fmesh import FMesh
+from ply import lex, yacc
 
 literals = ["+", "-", ":", "/"]
 
 KEYWORDS = [
     "MCNP",
     "VERSION",
     "LD",
@@ -176,14 +174,15 @@
         meshtal_lexer.lineno = 1
         t.lineno = 1
         t.lexer.last_pos = 1
     if value in KEYWORDS:
         t.type = value
         t.value = value
         return t
+    return None
 
 
 @lex.TOKEN(KEYWORD)
 def t_norm_tally_keyword(t):
     value = t.value.upper()
     if value == "TIMES":
         value = "TIME"
@@ -193,22 +192,21 @@
         elif value == "ERRORS":
             value = "ERROR"
         elif value == "TH":
             value = "THETA"
         t.type = value
         t.value = value
         return t
+    return None
 
 
 # noinspection PyPep8Naming
 def t_ANY_error(t):
     column = t.lexer.lexpos - t.lexer.last_pos + 1
-    msg = r"Illegal character '{0}' at line {1} column {2}".format(
-        t.value[0], t.lexer.lineno, column
-    )
+    msg = f"Illegal character {t.value[0]!r} at line {t.lexer.lineno} column {column}"
     raise ValueError(msg, t.value[0], t.lexer.lineno, column)
 
 
 @lex.TOKEN(FLT_NUMBER)
 def t_norm_tally_flt_number(t):
     t.value = float(t.value)
     return t
@@ -233,16 +231,16 @@
     }
 
 
 def p_header(p):
     """header : MCNP VERSION stamp LD stamp PROBID stamp stamp
     | MCNP VERSION stamp MPI LD stamp PROBID stamp stamp
     """
-    l = len(p)
-    p[0] = {"PROBID": p[l - 2] + p[l - 1], "VERSION": p[3]}
+    t = len(p)
+    p[0] = {"PROBID": p[t - 2] + p[t - 1], "VERSION": p[3]}
 
 
 # noinspection GrazieInspection
 def p_tallies(p):
     """tallies : tallies tally
     | tallies tally separator
     | tally separator
@@ -471,17 +469,17 @@
         p[0] = order, p[1][1], p[1][2]
 
 
 def p_energy_bin(p):
     """energy_bin : ENERGY ':' float '-' float newline separator spatial_bins
     | TIME ':' float newline separator spatial_bins
     """
-    l = len(p) - 1
-    order = [p[1]] + p[l][0]
-    p[0] = order, p[l][1], p[l][2]
+    t = len(p) - 1
+    order = [p[1]] + p[t][0]
+    p[0] = order, p[t][1], p[t][2]
 
 
 def p_total_energy_bin(p):
     """total_energy_bin : TOTAL ENERGY newline separator spatial_bins separator"""
     order = [p[1]] + p[5][0]
     p[0] = order, p[5][1], p[5][2]
 
@@ -507,19 +505,15 @@
     errors = [line[1:] for line in p[18][1:]]
     p[0] = order, results, errors
 
 
 def p_error(p):
     if p:
         column = p.lexer.lexpos - p.lexer.last_pos + 1
-        print(
-            "Syntax error at token {0} {3}, line {1}, column {2}".format(
-                p.type, p.lexer.lineno, column, p.value
-            )
-        )
+        print(f"Syntax error at token {p.type} {p.value}, line {p.lexer.lineno}, column {column}")
     else:
         print("Syntax error at EOF")
 
 
 meshtal_parser = yacc.yacc(tabmodule="meshtal_tab", debug=True)
 
 
@@ -533,24 +527,19 @@
     "TIME": "dtbins",
 }
 
 
 def read_meshtal(filename: str | Path) -> dict[int, FMesh]:
     """Reads MCNP meshtal file.
 
-    Parameters
-    ----------
-    filename : str
-        File that contains MCNP meshtally data.
-
-    Returns
-    -------
-    tallies : dict
-        Dictionary of mesh tallies contained in the file. It is
-        tally_name -> Fmesh pairs.
+    Args:
+        filename: File that contains MCNP meshtally data.
+
+    Returns:
+        tallies Index of mesh tallies contained in the file.
     """
     with open(filename) as f:
         text = f.read() + "\n"
     meshtal_lexer.begin("INITIAL")
     meshtal_data = meshtal_parser.parse(text, lexer=meshtal_lexer)
     histories = meshtal_data["histories"]
     tallies = {}
```

### Comparing `mckit-0.6.23/src/mckit/parser/surface_parser.py` & `mckit-0.6.24/src/mckit/parser/surface_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Tuple
+from __future__ import annotations
 
 import mckit.parser.common.utils as pu  # parse utils
 import sly
 
 from mckit.parser.common import Lexer as LexerBase
 from mckit.parser.common import TransformationStrictIndex
 from mckit.parser.common.utils import drop_c_comments, extract_comments
@@ -85,25 +85,24 @@
         self._transformations = transformations
 
     @property
     def transformations(self):
         return self._transformations
 
     def build_surface(
-        self, name: int, kind: str, params: List[float], transform, modifier
+        self, name: int, kind: str, params: list[float], transform, modifier
     ) -> Surface:
         options = {"name": name}
         if transform is not None:
             transformation = self.transformations[transform]
             if transformation:
                 options["transform"] = transformation
         if modifier is not None:
             options["modifier"] = modifier
-        _surface = create_surface(kind, *params, **options)
-        return _surface
+        return create_surface(kind, *params, **options)
 
     @_("MODIFIER  name surface_description")
     def surface(self, p):
         (
             kind,
             params,
             transform,
@@ -120,45 +119,45 @@
         return self.build_surface(p.name, kind, params, transform, None)
 
     @_("INTEGER")
     def name(self, p):
         return p.INTEGER
 
     @_("transform SURFACE_TYPE surface_params")
-    def surface_description(self, p) -> Tuple[str, List[float], Optional[int]]:
+    def surface_description(self, p) -> tuple[str, list[float], int | None]:
         return p.SURFACE_TYPE, p.surface_params, p.transform
 
     @_("SURFACE_TYPE surface_params")
-    def surface_description(self, p) -> Tuple[str, List[float], Optional[int]]:
+    def surface_description(self, p) -> tuple[str, list[float], int | None]:
         return p.SURFACE_TYPE, p.surface_params, None
 
     @_("INTEGER")
     def transform(self, p):
         return p.INTEGER
 
     @_("surface_params float")
-    def surface_params(self, p) -> List[float]:
-        surface_params: List[float] = p.surface_params
+    def surface_params(self, p) -> list[float]:
+        surface_params: list[float] = p.surface_params
         surface_params.append(p.float)
         return surface_params
 
     @_("float")
-    def surface_params(self, p) -> List[float]:
+    def surface_params(self, p) -> list[float]:
         return [p.float]
 
     @_("FLOAT")
     def float(self, p):
         return p.FLOAT
 
     @_("INTEGER")
     def float(self, p) -> float:
         return float(p.INTEGER)
 
 
-def parse(text: str, transformations: Optional[Index] = None) -> Surface:
+def parse(text: str, transformations: Index | None = None) -> Surface:
     if transformations is None:
         transformations = TransformationStrictIndex()
     else:
         assert isinstance(transformations, Index)
     text = drop_c_comments(text)
     text, comments, trailing_comments = extract_comments(text)
     lexer = Lexer()
```

### Comparing `mckit-0.6.23/src/mckit/parser/transformation_parser.py` & `mckit-0.6.24/src/mckit/parser/transformation_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import mckit.parser.common.utils as cmn
 import sly
 
 from mckit.parser.common import Lexer as LexerBase
 from mckit.parser.common.utils import drop_c_comments, extract_comments
 from mckit.transformation import Transformation
 
@@ -57,32 +59,32 @@
 
     @_("translation")
     def transform_params(self, p):
         return p.translation, None, False
 
     @_("float float float")
     def translation(self, p):
-        return [f for f in p]
+        return list(p)
 
     # TODO dvp: check what to do, if transformation is specified with default values using the MCNP J shortcuts?
 
     @_("float float float float float float float float float INTEGER")
     def rotation(self, p):
         m = p[9]
         assert m == -1 or m == 1, f"Invalid M option value {m}"
-        return [f for f in p][:-1], m == -1
+        return list(p)[:-1], m == -1
 
     @_(
         "float float float float float float float float float",
         "float float float float float float",
         "float float float float float",
         "float float float",
     )
     def rotation(self, p):
-        return [f for f in p], False
+        return list(p), False
 
     @_("FLOAT")
     def float(self, p):
         return p.FLOAT
 
     @_("INTEGER")
     def float(self, p):
```

### Comparing `mckit-0.6.23/src/mckit/printer.py` & `mckit-0.6.24/src/mckit/printer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 """Functions for MCNP model text printing."""
-from typing import Any, List
+from __future__ import annotations
 
-import warnings
+from typing import Any
 
-import mckit.constants as constants
+from logging import getLogger
 
+from mckit import constants
 from mckit.utils import get_decades, prettify_float, significant_digits
 
 IMPORTANCE_FORMAT = "{0:.3f}"
 
+_LOG = getLogger(__name__)
 
-def print_card(tokens: List[str], offset: int = 8, max_column: int = 80, sep: str = "\n") -> str:
+
+def print_card(tokens: list[str], offset: int = 8, max_column: int = 80, sep: str = "\n") -> str:
     """Produce string in MCNP card format.
 
-    Parameters
-    ----------
-    tokens :
-        List of words to be printed.
-    offset :
-        The number of spaces to make continuation of line. Minimum 5.
-    max_column :
-        The maximum length of card line. Maximum 80.
-    sep :
-        Separator symbol. This symbol marks positions where newline character
-        should be inserted even if max_column position not reached.
-
-    Returns
-    -------
-    text :
+    Args:
+        tokens :
+            List of words to be printed.
+        offset :
+            The number of spaces to make continuation of line. Minimum 5.
+        max_column :
+            The maximum length of card line. Maximum 80.
+        sep :
+            Separator symbol. This symbol marks positions where newline character
+            should be inserted even if max_column position not reached.
+
+    Returns:
         MCNP code of a card.
     """
     if offset < 5:
         offset = 5
-        warnings.warn("offset must not be less than 5. offset is set to be 5.")
+        _LOG.warning("offset must not be less than 5. offset is set to be 5.")
     if max_column > 80:
         max_column = 80
-        warnings.warn("max_column must not be greater than 80. It is set to be 80.")
+        _LOG.warning("max_column must not be greater than 80. It is set to be 80.")
 
     length = 0  # current length.
     words = []  # a list of individual words.
     line_sep = "\n" + " " * offset  # separator between lines.
     i = 0
     while i < len(tokens):
         if length + len(tokens[i]) > max_column or tokens[i] == sep:
@@ -52,99 +52,93 @@
                     return "".join(words)
         words.append(tokens[i])
         length += len(tokens[i])
         i += 1
     return "".join(words)
 
 
-def separate(tokens: List[str], sep: str = " ") -> List[str]:
+def separate(tokens: list[str], sep: str = " ") -> list[str]:
     """Adds separation symbols between tokens.
 
-    Parameters
-    ----------
-    tokens :
-        A list of strings.
-    sep :
-        Separator to be inserted between tokens. Default: single space.
-
-    Returns
-    -------
-    sep_tokens :
+    Args:
+        tokens :
+            A list of strings.
+        sep :
+            Separator to be inserted between tokens. Default: single space.
+
+    Returns:
         List of separated tokens.
     """
     sep_tokens = []
     for t in tokens[:-1]:
         sep_tokens.append(t)
         sep_tokens.append(sep)
     sep_tokens.append(tokens[-1])
     return sep_tokens
 
 
-def print_option(option: str, value: Any) -> List[str]:
+def print_option(option: str, value: Any) -> list[str]:
     name = option[:3]
     par = option[3:]
     if name == "IMP" and (par == "N" or par == "P" or par == "E"):
-        return ["IMP:{0}={1}".format(par, IMPORTANCE_FORMAT.format(value))]
-    elif option == "VOL":
-        return ["VOL={0}".format(value)]
-    elif option == "U":
-        return ["U={0}".format(value.name())]
-    elif option == "FILL":
+        return [f"IMP:{par}={IMPORTANCE_FORMAT.format(value)}"]
+    if option == "VOL":
+        return [f"VOL={value}"]
+    if option == "U":
+        return [f"U={value.name()}"]
+    if option == "FILL":
         universe = value["universe"]
         tr = value.get("transform", None)
-        words = ["FILL={0}".format(universe.name())]
+        words = [f"FILL={universe.name()}"]
         if tr:
             tr_name = tr.name()
             if not tr_name:
                 words[0] = "*" + words[0]
                 words.append("(")
                 words.extend(tr.get_words())
                 words.append(")")
             else:
                 words.append("(")
                 words.append(str(tr_name))
                 words.append(")")
         return words
-    else:
-        raise ValueError("Incorrect option name: {0}".format(option))
+    raise ValueError(f"Incorrect option name: {option}")
 
 
 def pretty_float(value: float, frac_digits: int = None) -> str:
     """Pretty print of the float number.
 
-    Parameters
-    ----------
-    value :
-        Value to be printed.
-    frac_digits :
-        The number of digits after decimal point.
+    Args:
+        value :
+            Value to be printed.
+        frac_digits :
+            The number of digits after decimal point.
     """
     if frac_digits is None:
         frac_digits = significant_digits(
             value, constants.FLOAT_TOLERANCE, resolution=constants.FLOAT_TOLERANCE
         )
     if value == abs(value):
         value = abs(value)
     decades = get_decades(value)
-    format_f = "{{0:.{0}f}}".format(max(frac_digits, 0))
-    format_e = "{{0:.{0}e}}".format(max(frac_digits + decades, 0))
+    format_f = f"{{0:.{max(frac_digits, 0)}f}}"
+    format_e = f"{{0:.{max(frac_digits + decades, 0)}e}}"
     text_f = format_f.format(round(value, frac_digits))
     text_e = format_e.format(value)
     if len(text_f) <= len(text_e):
         return text_f
-    else:
-        return text_e
+    return text_e
 
 
 CELL_OPTION_GROUPS = (
     ("IMPN", "IMPP", "IMPE", "VOL"),  # Importance options
     ("TRCL",),  # Transformation options
     ("U", "FILL"),  # Universe and fill options
 )
 
 
-def add_float(words: List[str], v: float, pretty: bool) -> None:
+def add_float(words: list[str], v: float, pretty: bool) -> None:
     words.append(" ")
     if pretty:
         words.append(pretty_float(v))
     else:
         words.append(prettify_float(v))
```

### Comparing `mckit-0.6.23/src/mckit/source.py` & `mckit-0.6.24/src/mckit/source.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 """Code to load source distribution and print corresponding MCNP SDEF."""
 from __future__ import annotations
 
-from typing import Dict, Optional, Set, Tuple, Union
-
 import numpy as np
 
 from numpy.typing import ArrayLike
 
 from .printer import print_card, separate
 
 
@@ -35,26 +33,26 @@
         _probs: probabilities or distributions for bins
         _is_pdf: is this PDF or more complicated distribution?
     """
 
     def __init__(
         self,
         name: int,
-        values: Union[ArrayLike, list["Distribution"]],
-        probs: Union[ArrayLike, "Distribution"],
-        distribution_variable: Optional[str] = None,
+        values: ArrayLike | list[Distribution],
+        probs: ArrayLike | Distribution,
+        distribution_variable: str | None = None,
         is_discrete: bool = False,
     ) -> None:
         self._name = name
         self._var = distribution_variable
         Distribution.check_distr(values, len(probs), is_discrete)
         self._is_discrete = is_discrete
         self._values = np.asarray(values)
         if isinstance(probs, Distribution):
-            self._probs: Union[ArrayLike, "Distribution"] = probs
+            self._probs: ArrayLike | Distribution = probs
         else:
             self._probs = np.asarray(probs)
         self._is_pdf = (
             isinstance(self._probs, np.ndarray)
             and len(self._probs) == len(values)
             and not is_discrete
             and not isinstance(self._values[0], Distribution)
@@ -71,26 +69,26 @@
 
         Returns:
             The number of probability values.
         """
         return len(self._probs)
 
     @property
-    def variable(self) -> Optional[str]:
+    def variable(self) -> str | None:
         """Gets distribution's source variable name."""
         return self._var
 
     @property
     def has_nested_distributions(self) -> bool:
         """Are there nested (inner) distributions?"""
         return isinstance(self._values[0], Distribution)
 
     @staticmethod
     def check_distr(
-        bins_or_distrs: [Union[ArrayLike, list["Distribution"]]],
+        bins_or_distrs: [ArrayLike | list[Distribution]],
         size: int,
         is_discrete: bool,
     ) -> None:
         """Checks if the distribution is correct.
 
         Args:
             bins_or_distrs: List of variable values.
@@ -115,43 +113,41 @@
         card = print_card(separate(bin_tokens))
 
         if prob_tokens:
             card += "\n" + print_card(separate(prob_tokens))
 
         return card
 
-    def get_inner(self) -> Set["Distribution"]:
+    def get_inner(self) -> set[Distribution]:
         """Gets nested distributions this one depends on.
 
         If values of this distribution are distributions themselves,
         then they are returned.
 
         Returns:
             Set:  A set of nested distributions, if any, empty set otherwise.
         """
         return set(self._values) if self.has_nested_distributions else set()
 
-    def depends_on(self) -> Optional["Distribution"]:
+    def depends_on(self) -> Distribution | None:
         """Gets distribution this one depends on.
 
         Returns:
             Distribution|None:  Distribution this one depends on, if any. None otherwise.
         """
         if isinstance(self._probs, Distribution):
             return self._probs
-        else:
-            return None
+        return None
 
     def _mcnp_distribution_tag(self):
         if self._is_discrete:
             return "L"
-        elif self._is_pdf:
+        if self._is_pdf:
             return "A"
-        else:
-            return "H"
+        return "H"
 
     def _prob_tokens_repr(self, bin_tokens):
         if isinstance(self._probs, Distribution):
             bin_tokens.insert(0, f"DS{self._name}")
             prob_tokens = None
         else:
             bin_tokens.insert(0, f"SI{self._name}")
@@ -191,15 +187,15 @@
     expect_distributions = isinstance(bins_or_distrs[0], Distribution)
     if not all(expect_distributions == isinstance(x, Distribution) for x in bins_or_distrs):
         raise TypeError("Distribution bins should be either all Distributions or all not")
 
 
 def create_bin_distributions(
     bins: list[float], start_name: int = 1
-) -> Tuple[int, list["Distribution"]]:
+) -> tuple[int, list[Distribution]]:
     """Creates bin distributions for specified bins.
 
     A list of distributions created. Index in the list corresponds to the  index of bin.
 
     Args:
         bins:   A list of bin boundaries.
         start_name:  Starting name for distributions.
@@ -220,15 +216,15 @@
 
     Args:
         variables:
             A dictionary of source variables. var_name -> var_value. The value
             can be either float (int) value or Distribution instance.
     """
 
-    def __init__(self, **variables: Dict[int, Union[int, float, Distribution]]) -> None:
+    def __init__(self, **variables: dict[int, int | float | Distribution]) -> None:
         self._variables = variables
 
     def mcnp_repr(self) -> str:
         """Gets a string representation of corresponding MCNP card."""
         tokens = ["SDEF"]
         cards = []
         extra_cards = []
```

### Comparing `mckit-0.6.23/src/mckit/src/box.c` & `mckit-0.6.24/src/mckit/src/box.c`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/src/mckit/src/box.h` & `mckit-0.6.24/src/mckit/src/box.h`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/src/mckit/src/box_doc.h` & `mckit-0.6.24/src/mckit/src/box_doc.h`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/src/mckit/src/geometrymodule.c` & `mckit-0.6.24/src/mckit/src/geometrymodule.c`

 * *Files 0% similar despite different names*

```diff
@@ -1206,14 +1206,15 @@
 }
 
 static PyObject *
 shapeobj_bounding_box(ShapeObject * self, PyObject * args, PyObject * kwds)
 {
     PyObject * start_box = NULL;
     double tol = 100.0;
+    int status = SHAPE_FAILURE;
 
     static char * kwlist[] = {"tol", "box", NULL};
 
     if (! PyArg_ParseTupleAndKeywords(args, kwds, "|dO", kwlist, &tol, &start_box)) return NULL;
 
     if (start_box == NULL) start_box = GET_NAME(GLOBAL_BOX);
 
@@ -1221,44 +1222,57 @@
         PyErr_SetString(PyExc_ValueError, "Box instance is expected");
         return NULL;
     }
 
     BoxObject * box = (BoxObject *) boxobj_copy((BoxObject *) start_box);
     if (box == NULL) return NULL;
 
+
+//    Py_BEGIN_ALLOW_THREADS
+
     shape_reset_cache(&self->shape);
-    int status = shape_bounding_box(&self->shape, &box->box, tol);
+    status = shape_bounding_box(&self->shape, &box->box, tol);
 
-    if (status == SHAPE_SUCCESS) return (PyObject *) box;
+//    Py_END_ALLOW_THREADS
+
+    if (status == SHAPE_SUCCESS)
+        return (PyObject *) box;
     else {
         Py_DECREF(box);
         // TODO: Probably some exception should be raised.
         return NULL;
     }
 }
 
 static PyObject *
 shapeobj_volume(ShapeObject * self, PyObject * args, PyObject * kwds)
 {
     PyObject * box = NULL;
     double min_vol = MIN_VOLUME;
+    double vol = -1.0;
 
     static char * kwlist[] = {"box", "min_volume", NULL};
 
     if (! PyArg_ParseTupleAndKeywords(args, kwds, "|Od", kwlist, &box, &min_vol)) return NULL;
 
     if (box == NULL) box = GET_NAME(GLOBAL_BOX);
 
     if (! PyObject_TypeCheck(box, &BoxType)) {
         PyErr_SetString(PyExc_ValueError, "Box instance is expected");
         return NULL;
     }
 
+
+//    Py_BEGIN_ALLOW_THREADS
+
     shape_reset_cache(&self->shape);
-    double vol = shape_volume(&self->shape, &((BoxObject *) box)->box, min_vol);
+    vol = shape_volume(&self->shape, &((BoxObject *) box)->box, min_vol);
+
+//    Py_END_ALLOW_THREADS
+
     return Py_BuildValue("d", vol);
 }
 
 /*
 static PyObject *
 shapeobj_contour(ShapeObject * self, PyObject * args, PyObject * kwds)
 {
```

### Comparing `mckit-0.6.23/src/mckit/src/rbtree.c` & `mckit-0.6.24/src/mckit/src/rbtree.c`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/src/mckit/src/rbtree.h` & `mckit-0.6.24/src/mckit/src/rbtree.h`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/src/mckit/src/shape.c` & `mckit-0.6.24/src/mckit/src/shape.c`

 * *Files 1% similar despite different names*

```diff
@@ -29,25 +29,32 @@
     for (i = 0; i < n; ++i) {
         if (a->arr[i] < b->arr[i]) return 1;
         else if (a->arr[i] > b->arr[i]) return -1;
     }
     return 0;
 }
 
-// Initializes shape struct
+/**
+ * Initializes Shape struct.
+ *
+ * @param shape Pointer to struct to be initialized
+ * @param opc   Operation code
+ * @param alen  Length of arguments
+ * @param args  A surface or an array of Shapes
+ */
 int shape_init(
-        Shape * shape,          // Pointer to struct to be initialized
-        char opc,               // Operation code
-        size_t alen,            // Length of arguments
-        const void * args       // Argument array.
+        Shape * shape,
+        char opc,
+        size_t alen,
+        const void * args
 )
 {
     shape->opc = opc;
     shape->alen = alen;
-    shape->stats = rbtree_create(stat_compare);;
+    shape->stats = rbtree_create(stat_compare);
     shape->last_box = 0;
     shape->last_box_result = 0;
     if (is_final(opc)) {
         shape->args.surface = (Surface *) args;
     } else if (is_void(opc)) {
         shape->args.surface = NULL;
     } else {
```

### Comparing `mckit-0.6.23/src/mckit/src/shape.h` & `mckit-0.6.24/src/mckit/src/shape.h`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/src/mckit/src/surf_doc.h` & `mckit-0.6.24/src/mckit/src/surf_doc.h`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/src/mckit/src/surface.c` & `mckit-0.6.24/src/mckit/src/surface.c`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/src/mckit/src/surface.h` & `mckit-0.6.24/src/mckit/src/surface.h`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/src/mckit/surface.py` & `mckit-0.6.24/src/mckit/surface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Surface methods."""
 from __future__ import annotations
 
-from typing import Any, Callable, Dict, List, Optional, Sequence, Set, Text, Tuple, Union
+from typing import Any, Callable, List, Sequence, Union
 
 from abc import abstractmethod
 
 import numpy as np
 
 from mckit.box import GLOBAL_BOX
 
@@ -60,15 +60,15 @@
 ]
 
 
 VectorLike = Union[np.ndarray, List[float]]
 
 
 # noinspection PyPep8Naming
-def create_surface(kind: str, *params: float, **options) -> "Surface":
+def create_surface(kind: str, *params: float, **options) -> Surface:
     """Creates new surface.
 
     Args:
         kind: Surface kind designator. See MCNP manual.
         params: List of surface parameters.
         options: Dictionary of surface's options.
                 In particular, transform  - transformation instance
@@ -91,123 +91,170 @@
         assume_normalized = True
     elif kind[-1] == "Z":
         axis = EZ
         assume_normalized = True
     else:
         axis = None
         assume_normalized = False
+    surface = _create_surface_by_spec(assume_normalized, axis, kind, options, params)
+
+    if surface:
+        return surface
+
+    # ---------- Axis-symmetric surface defined by points ------
+    if len(params) == 2:
+        return Plane(axis, -params[0], **options)
+    if len(params) == 4:
+        # TODO: Use special classes instead of GQ
+        h1, r1, h2, r2 = params
+        if abs(h2 - h1) < constants.RESOLUTION * max(abs(h1), abs(h2)):
+            return Plane(axis, -0.5 * (h1 + h2), **options)
+        if abs(r2 - r1) < constants.RESOLUTION * max(abs(r2), abs(r1)):
+            R = 0.5 * (abs(r1) + abs(r2))
+            return Cylinder([0, 0, 0], axis, R, **options)
+        if r1 * r2 < 0:
+            raise ValueError("Points must belong to the one sheet.")
+        h0 = (abs(r1) * h2 - abs(r2) * h1) / (abs(r1) - abs(r2))
+        t2 = ((r1 - r2) / (h1 - h2)) ** 2
+        s = int(
+            round((h1 - h0) / abs(h1 - h0))
+        )  # TODO: dvp check this conversion: was without int()
+        return Cone(axis * h0, axis, t2, sheet=s, **options)
+    # TODO: Implement creation of surface by 3 points.
+    raise NotImplementedError()
+
+
+def _create_surface_by_spec(  # noqa: PLR0911
+    assume_normalized, axis, kind, options, params
+) -> Surface | None:
     # -------- Plane -------------------
     if kind[0] == "P":
-        if len(kind) == 2:
-            return Plane(axis, -params[0], assume_normalized=assume_normalized, **options)
-        else:
-            return Plane(
-                params[:3],
-                -params[3],
-                assume_normalized=assume_normalized,
-                **options,
-            )
+        return _create_plane(assume_normalized, axis, kind, options, params)
     # -------- SQ -------------------
-    elif kind == "SQ":
-        A, B, C, D, E, F, G, x0, y0, z0 = params
-        m = np.diag([A, B, C])
-        v = 2 * np.array([D - A * x0, E - B * y0, F - C * z0])
-        k = A * x0**2 + B * y0**2 + C * z0**2 - 2 * (D * x0 + E * y0 + F * z0) + G
-        return GQuadratic(m, v, k, **options)
+    if kind == "SQ":
+        return _create_sq(options, params)
     # -------- Sphere ------------------
-    elif kind[0] == "S":
-        if kind == "S":
-            r0 = np.array(params[:3])
-        elif kind == "SO":
-            r0 = ORIGIN
-        else:
-            r0 = axis * params[0]
-        R = params[-1]
-        return Sphere(r0, R, **options)
+    if kind[0] == "S":
+        return _create_sphere(axis, kind, options, params)
     # -------- Cylinder ----------------
-    elif kind[0] == "C":
-        A = 1 - axis
-        if kind[1] == "/":
-            Ax, Az = np.dot(A, EX), np.dot(A, EZ)
-            r0 = params[0] * (Ax * EX + (1 - Ax) * EY) + params[1] * ((1 - Az) * EY + Az * EZ)
-        else:
-            r0 = ORIGIN
-        R = params[-1]
-        return Cylinder(r0, axis, R, assume_normalized=assume_normalized, **options)
+    if kind[0] == "C":
+        return _create_cylinder(assume_normalized, axis, kind, options, params)
     # -------- Cone ---------------
-    elif kind[0] == "K":
-        if kind[1] == "/":
-            r0 = np.array(params[:3], dtype=float)
-            ta = params[3]
-        else:
-            r0 = params[0] * axis
-            ta = params[1]
-        sheet = 0 if len(params) % 2 == 0 else int(params[-1])
-        return Cone(r0, axis, ta, sheet, assume_normalized=assume_normalized, **options)
+    if kind[0] == "K":
+        return _create_cone(assume_normalized, axis, kind, options, params)
     # ---------- GQ -----------------
-    elif kind == "GQ":
-        A, B, C, D, E, F, G, H, J, k = params
-        m = np.array([[A, 0.5 * D, 0.5 * F], [0.5 * D, B, 0.5 * E], [0.5 * F, 0.5 * E, C]])
-        v = np.array([G, H, J])
-        return GQuadratic(m, v, k, **options)
+    if kind == "GQ":
+        return _create_gquadratic(options, params)
     # ---------- Torus ---------------------
-    elif kind[0] == "T":
-        x0, y0, z0, R, a, b = params
-        return Torus([x0, y0, z0], axis, R, a, b, **options)
+    if kind[0] == "T":
+        return _create_torus(axis, options, params)
     # ---------- Macrobodies ---------------
-    elif kind == "RPP":
-        x_min, x_max, y_min, y_max, z_min, z_max = params
-        center = [x_min, y_min, z_min]
-        dir_x = [x_max - x_min, 0, 0]
-        dir_y = [0, y_max - y_min, 0]
-        dir_z = [0, 0, z_max - z_min]
-        return BOX(center, dir_x, dir_y, dir_z, **options)
-    elif kind == "BOX":
-        center = params[:3]
-        dir_x = params[3:6]
-        dir_y = params[6:9]
-        dir_z = params[9:]
-        return BOX(center, dir_x, dir_y, dir_z, **options)
-    elif kind == "RCC":
-        center = params[:3]
-        axis = params[3:6]
-        radius = params[6]
-        return RCC(center, axis, radius, **options)
-    # ---------- Axis-symmetric surface defined by points ------
+    if kind == "RPP":
+        return _create_rpp(options, params)
+    if kind == "BOX":
+        return _create_box(options, params)
+    if kind == "RCC":
+        return _create_rcc(options, params)
+    return None
+
+
+def _create_rcc(options, params):
+    center = params[:3]
+    axis = params[3:6]
+    radius = params[6]
+    return RCC(center, axis, radius, **options)
+
+
+def _create_box(options, params):
+    center = params[:3]
+    dir_x = params[3:6]
+    dir_y = params[6:9]
+    dir_z = params[9:]
+    return BOX(center, dir_x, dir_y, dir_z, **options)
+
+
+def _create_rpp(options, params):
+    x_min, x_max, y_min, y_max, z_min, z_max = params
+    center = [x_min, y_min, z_min]
+    dir_x = [x_max - x_min, 0, 0]
+    dir_y = [0, y_max - y_min, 0]
+    dir_z = [0, 0, z_max - z_min]
+    return BOX(center, dir_x, dir_y, dir_z, **options)
+
+
+def _create_torus(axis, options, params):
+    x0, y0, z0, R, a, b = params
+    return Torus([x0, y0, z0], axis, R, a, b, **options)
+
+
+def _create_gquadratic(options, params):
+    A, B, C, D, E, F, G, H, J, k = params
+    m = np.array([[A, 0.5 * D, 0.5 * F], [0.5 * D, B, 0.5 * E], [0.5 * F, 0.5 * E, C]])
+    v = np.array([G, H, J])
+    return GQuadratic(m, v, k, **options)
+
+
+def _create_cone(assume_normalized, axis, kind, options, params):
+    if kind[1] == "/":
+        r0 = np.array(params[:3], dtype=float)
+        ta = params[3]
     else:
-        if len(params) == 2:
-            return Plane(axis, -params[0], **options)
-        elif len(params) == 4:
-            # TODO: Use special classes instead of GQ
-            h1, r1, h2, r2 = params
-            if abs(h2 - h1) < constants.RESOLUTION * max(abs(h1), abs(h2)):
-                return Plane(axis, -0.5 * (h1 + h2), **options)
-            elif abs(r2 - r1) < constants.RESOLUTION * max(abs(r2), abs(r1)):
-                R = 0.5 * (abs(r1) + abs(r2))
-                return Cylinder([0, 0, 0], axis, R, **options)
-            else:
-                if r1 * r2 < 0:
-                    raise ValueError("Points must belong to the one sheet.")
-                h0 = (abs(r1) * h2 - abs(r2) * h1) / (abs(r1) - abs(r2))
-                t2 = ((r1 - r2) / (h1 - h2)) ** 2
-                s = int(
-                    round((h1 - h0) / abs(h1 - h0))
-                )  # TODO: dvp check this conversion: was without int()
-                return Cone(axis * h0, axis, t2, sheet=s, **options)
-        elif len(params) == 6:
-            # TODO: Implement creation of surface by 3 points.
-            raise NotImplementedError
+        r0 = params[0] * axis
+        ta = params[1]
+    sheet = 0 if len(params) % 2 == 0 else int(params[-1])
+    return Cone(r0, axis, ta, sheet, assume_normalized=assume_normalized, **options)
+
+
+def _create_cylinder(assume_normalized, axis, kind, options, params):
+    A = 1 - axis
+    if kind[1] == "/":
+        Ax, Az = np.dot(A, EX), np.dot(A, EZ)
+        r0 = params[0] * (Ax * EX + (1 - Ax) * EY) + params[1] * ((1 - Az) * EY + Az * EZ)
+    else:
+        r0 = ORIGIN
+    R = params[-1]
+    return Cylinder(r0, axis, R, assume_normalized=assume_normalized, **options)
+
+
+def _create_sphere(axis, kind, options, params):
+    if kind == "S":
+        r0 = np.array(params[:3])
+    elif kind == "SO":
+        r0 = ORIGIN
+    else:
+        r0 = axis * params[0]
+    R = params[-1]
+    return Sphere(r0, R, **options)
+
+
+def _create_sq(options, params):
+    A, B, C, D, E, F, G, x0, y0, z0 = params
+    m = np.diag([A, B, C])
+    v = 2 * np.array([D - A * x0, E - B * y0, F - C * z0])
+    k = A * x0**2 + B * y0**2 + C * z0**2 - 2 * (D * x0 + E * y0 + F * z0) + G
+    return GQuadratic(m, v, k, **options)
+
+
+def _create_plane(assume_normalized, axis, kind, options, params):
+    if len(kind) == 2:
+        return Plane(axis, -params[0], assume_normalized=assume_normalized, **options)
+    return Plane(
+        params[:3],
+        -params[3],
+        assume_normalized=assume_normalized,
+        **options,
+    )
 
 
 def create_replace_dictionary(
-    surfaces: Set["Surface"],
-    unique: Optional[set["Surface"]] = None,
+    surfaces: set[Surface],
+    unique: set[Surface] | None = None,
     box=GLOBAL_BOX,
     tol: float = 1.0e-10,
-) -> dict["Surface", tuple["Surface", int]]:
+) -> dict[Surface, tuple[Surface, int]]:
     """Creates surface replace dictionary for equal surfaces removing.
 
     Args:
         surfaces : A set of surfaces to be checked.
         unique:  A set of surfaces that are assumed to be unique. If not None, then
                 `surfaces` are checked for coincidence with one of them.
         box : Box
@@ -228,112 +275,109 @@
                 replace[s] = (us, t)
                 break
         else:
             unique_surfaces.add(s)
     return replace
 
 
-def _drop_empty_transformation(options: Dict[str, Any]) -> None:
+def _drop_empty_transformation(options: dict[str, Any]) -> None:
     if "transform" in options and not options["transform"]:  # empty transformation option
         del options["transform"]
 
 
 class Surface(Card, MaybeClose):
     """Base class for all surface classes.
 
-    Methods
-    -------
-    equals(other, box, tol)
-        Checks if this surface and surf are equal inside the box.
-    test_point(p)
-        Checks the sense of point p with respect to this surface.
-    test_box(box)
-        Checks whether this surface crosses the box.
-    projection(p)
-        Gets projection of point p on the surface.
+    Methods:
+        equals(other, box, tol)
+            Checks if this surface and surf are equal inside the box.
+        test_point(p)
+            Checks the sense of point p with respect to this surface.
+        test_box(box)
+            Checks whether this surface crosses the box.
+        projection(p)
+            Gets projection of point p on the surface.
     """
 
     def __init__(self, **options) -> None:
         """Create :class:`Surface` with the options.
 
         Args:
             options: kwargs - properties for the `Surface` card.
         """
         _drop_empty_transformation(options)
         Card.__init__(self, **options)
 
     @abstractmethod
-    def copy(self) -> "Surface":
+    def copy(self) -> Surface:
         pass
 
     @property
-    def transformation(self) -> Optional[Transformation]:
+    def transformation(self) -> Transformation | None:
         return self.options.get("transform", None)
 
     @abstractmethod
-    def apply_transformation(self) -> "Surface":
+    def apply_transformation(self) -> Surface:
         """Applies transformation specified for the surface.
 
-        Returns
-        -------
-        A 1new surface with transformed parameters, If there's specified transformation,
-        otherwise returns self.
+        Returns:
+            A new surface with transformed parameters, if there's specified transformation,
+            otherwise returns self.
         """
 
     def combine_transformations(self, tr: Transformation) -> Transformation:
         my_transformation: Transformation = self.transformation
         if my_transformation:
-            tr = tr.apply2transform(my_transformation)
+            return tr.apply2transform(my_transformation)
         return tr
 
     @abstractmethod
-    def transform(self, tr: Transformation) -> "Surface":
+    def transform(self, tr: Transformation) -> Surface:
         """Applies transformation to this surface.
 
         Args:
             tr: Transformation to be applied.
 
         Returns:
             The result of this surface transformation.
         """
 
     @abstractmethod
     def is_close_to(
         self,
-        other: "Surface",
+        other: Surface,
         estimator: Callable[[Any, Any], bool] = DEFAULT_TOLERANCE_ESTIMATOR,
     ) -> bool:
         """Checks if this surface is close to other one with the given tolerance values."""
 
     @abstractmethod
-    def round(self) -> "Surface":
+    def round(self) -> Surface:  # noqa: A003
         """Returns rounded version of self."""
 
     def mcnp_words(self, pretty: bool = False) -> list[str]:
         words = []
         mod = self.options.get("modifier", None)
         if mod:
             words.append(mod)
         words.append(str(self.name()))
         words.append(" ")
         # TODO dvp: add transformations processing in Universe.
         return words
 
-    def clean_options(self) -> Dict[Text, Any]:
-        result: Dict[Text, Any] = filter_dict(self.options, DROP_OPTIONS)
+    def clean_options(self) -> dict[str, Any]:
+        result: dict[str, Any] = filter_dict(self.options, DROP_OPTIONS)
         return result
 
     def compare_transformations(self, tr: Transformation) -> bool:
         my_transformation = self.transformation
         if my_transformation is not None:
             if tr is None:
                 return False
             return my_transformation == tr
-        else:
-            return tr is None
+        return tr is None
 
     def has_close_transformations(
         self, tr: Transformation, estimator: Callable[[Any, Any], bool]
     ) -> bool:
         my_transformation = self.transformation
         if my_transformation is None:
             return tr is None
@@ -344,20 +388,20 @@
     def __getstate__(self):
         return self.options
 
     def __setstate__(self, state):
         self.options = state
 
 
-def internalize_ort(v: np.ndarray) -> Tuple[np.ndarray, bool]:
+def internalize_ort(v: np.ndarray) -> tuple[np.ndarray, bool]:
     if v is EX or np.array_equal(v, EX):
         return EX, True
-    elif v is EY or np.array_equal(v, EY):
+    if v is EY or np.array_equal(v, EY):
         return EY, True
-    elif v is EZ or np.array_equal(v, EZ):
+    if v is EZ or np.array_equal(v, EZ):
         return EZ, True
     return v, False
 
 
 class RCC(Surface, _RCC):
     def __init__(self, center, direction, radius, **options):
         center = np.array(center)
@@ -374,25 +418,22 @@
         opt_surf["name"] = 3
         plane3 = Plane(-norm, offset3, **opt_surf).apply_transformation()
         _RCC.__init__(self, cyl, plane2, plane3)
         options.pop("transform", None)
         Surface.__init__(self, **options)
         self._hash = hash(cyl) ^ hash(plane2) ^ hash(plane3)
 
-    def surface(self, number):
+    def surface(self, number: int):
         args = self.surfaces
         if 1 <= number <= len(args):
             return args[number - 1]
-        else:
-            raise ValueError(f"There is no such surface in macrobody: {number}")
+        raise ValueError(f"There is no such surface in macrobody: {number}")
 
     def get_params(self):
         args = self.surfaces
-        for a in args:
-            print(a.mcnp_repr())
         center = args[0]._pt - args[2]._k * args[0]._axis * np.dot(args[0]._axis, args[2]._v)
         direction = -(args[1]._k + args[2]._k) * args[1]._v
         radius = args[0]._radius
         return center, direction, radius
 
     def mcnp_words(self, pretty: bool = False) -> list[str]:
         words = Surface.mcnp_words(self, pretty)
@@ -406,37 +447,35 @@
             fd = significant_digits(
                 v, constants.FLOAT_TOLERANCE, resolution=constants.FLOAT_TOLERANCE
             )
             words.append(pretty_float(v, fd))
             words.append(" ")
         return words
 
-    def transform(self, tr: Transformation) -> "RCC":
+    def transform(self, tr: Transformation) -> RCC:
         """Transforms the shape.
 
         Args:
             tr:  Transformation to be applied.
 
         Returns:
             New RCC shape with the transformation stored in options.
         """
         center, direction, radius = self.get_params()
         # TODO(dvp): What if `self` already has transformation?
         #            Should we apply the both transformation on new one?
         return RCC(center, direction, radius, transform=tr)
 
-    def __hash__(self):
+    def __hash__(self) -> int:
         return self._hash
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:
         if not isinstance(other, RCC):
             return False
-        args_this = self.surfaces
-        args_other = other.surfaces
-        return args_this == args_other
+        return self.surfaces == other.surfaces
 
     def __getstate__(self):
         surf_state = Surface.__getstate__(self)
         args = self.surfaces
         return args, self._hash, surf_state
 
     def __setstate__(self, state):
@@ -491,20 +530,19 @@
         _BOX.__init__(self, surf1, surf2, surf3, surf4, surf5, surf6)
         options.pop("transform", None)
         Surface.__init__(self, **options)
         self._hash = (
             hash(surf1) ^ hash(surf2) ^ hash(surf3) ^ hash(surf4) ^ hash(surf5) ^ hash(surf6)
         )
 
-    def surface(self, number):
+    def surface(self, number: int):
         args = self.surfaces
         if 1 <= number <= len(args):
             return args[number - 1]
-        else:
-            raise ValueError(f"There is no such surface in macrobody: {number}")
+        raise ValueError(f"There is no such surface in macrobody: {number}")
 
     def __hash__(self):
         return self._hash
 
     def __eq__(self, other):
         if not isinstance(other, BOX):
             return False
@@ -547,25 +585,21 @@
             fd = significant_digits(
                 v, constants.FLOAT_TOLERANCE, resolution=constants.FLOAT_TOLERANCE
             )
             words.append(pretty_float(v, fd))
             words.append(" ")
         return words
 
-    def transform(self, tr):
+    def transform(self, tr: Transformation):
         """Transforms the shape.
 
-        Parameters
-        ----------
-        tr : Transformation
-            Transformation to be applied.
-
-        Returns
-        -------
-        result : Shape
+        Args:
+            tr:  Transformation to be applied.
+
+        Returns:
             New shape.
         """
         center, dir_x, dir_y, dir_z = self.get_params()
         return BOX(center, dir_x, dir_y, dir_z, transform=tr)
 
     def __getstate__(self):
         surf_state = Surface.__getstate__(self)
@@ -608,54 +642,53 @@
                 v = v / length
                 k /= length
         Surface.__init__(self, **options)
         _Plane.__init__(self, v, k)
         self._hash = compute_hash(self._k, self._v, self.transformation)
 
     # noinspection PyTypeChecker
-    def round(self):
+    def round(self):  # noqa: A003
         result = self.apply_transformation()
         k_digits = significant_digits(
             result._k, constants.FLOAT_TOLERANCE, constants.FLOAT_TOLERANCE
         )
         v_digits = significant_array(
             result._v, constants.FLOAT_TOLERANCE, constants.FLOAT_TOLERANCE
         )
         k = round_scalar(result._k, k_digits)
         v = round_array(result._v, v_digits)
         return Plane(v, k, transform=None, assume_normalized=True, **result.options)
 
     def copy(self):
         options = filter_dict(self.options)
-        instance = Plane(self._v, self._k, assume_normalized=True, **options)
-        return instance
+        return Plane(self._v, self._k, assume_normalized=True, **options)
 
     __deepcopy__ = copy
 
-    def apply_transformation(self) -> "Plane":
+    def apply_transformation(self) -> Plane:
         tr = self.transformation
         if tr is None:
             return self
         v, k = tr.apply2plane(self._v, self._k)
         options = self.clean_options()
         return Plane(v, k, transform=None, assume_normalized=True, **options)
 
-    def transform(self, tr: Transformation) -> "Plane":
+    def transform(self, tr: Transformation) -> Plane:
         if tr is None:
             return self
         tr = self.combine_transformations(tr)
         options = self.clean_options()
         return Plane(self._v, self._k, transform=tr, assume_normalized=True, **options)
 
     def reverse(self):
         """Gets the surface with reversed normal."""
         options = self.clean_options()
         return Plane(-self._v, -self._k, assume_normalized=True, **options)
 
-    def mcnp_words(self, pretty: bool = False) -> List[str]:
+    def mcnp_words(self, pretty: bool = False) -> list[str]:
         words = Surface.mcnp_words(self, pretty)
         if np.array_equal(self._v, EX):
             words.append("PX")
         elif np.array_equal(self._v, EY):
             words.append("PY")
         elif np.array_equal(self._v, EZ):
             words.append("PZ")
@@ -666,15 +699,15 @@
         add_float(
             words, -self._k, pretty
         )  # TODO dvp: check why is offset negated in create_surface()?
         return words
 
     def is_close_to(
         self,
-        other: "Surface",
+        other: Surface,
         estimator: Callable[[Any, Any], bool] = DEFAULT_TOLERANCE_ESTIMATOR,
     ) -> bool:
         if self is other:
             return True
         if not isinstance(other, Plane):
             return False
         return estimator(
@@ -718,15 +751,15 @@
         The radius of the sphere.
     options : dict
         Dictionary of surface's options. Possible values:
             transform = tr - transformation to be applied to the sphere being
                              created. Transformation instance.
     """
 
-    def __init__(self, center: Union[Sequence[float], np.ndarray], radius: float, **options: Any):
+    def __init__(self, center: Sequence[float] | np.ndarray, radius: float, **options: Any):
         center = np.asarray(center, dtype=float)
         radius = float(radius)
         Surface.__init__(self, **options)
         _Sphere.__init__(self, center, radius)
         self._hash = compute_hash(self._radius, self._center, self.transformation)
 
     def __getstate__(self):
@@ -755,27 +788,27 @@
         return are_equal(
             (self._radius, self._center, self.transformation),
             (other._radius, other._center, other.transformation),
         )
 
     def is_close_to(
         self,
-        other: "Sphere",
+        other: Sphere,
         estimator: Callable[[Any, Any], bool] = DEFAULT_TOLERANCE_ESTIMATOR,
     ) -> bool:
         if self is other:
             return True
         if not isinstance(other, Sphere):
             return False
         return estimator(
             (self._radius, self._center, self.transformation),
             (other._radius, other._center, other.transformation),
         )
 
-    def round(self) -> "Surface":
+    def round(self) -> Surface:  # noqa: A003
         temp = self.apply_transformation()
         center_digits = significant_array(
             temp._center,
             constants.FLOAT_TOLERANCE,
             resolution=constants.FLOAT_TOLERANCE,
         )
         center = round_array(temp._center, center_digits)
@@ -784,30 +817,30 @@
             constants.FLOAT_TOLERANCE,
             resolution=constants.FLOAT_TOLERANCE,
         )
         radius = round_scalar(temp._radius, radius_digits)
         options = temp.clean_options()
         return Sphere(center, radius, transform=None, **options)
 
-    def apply_transformation(self) -> "Sphere":
+    def apply_transformation(self) -> Sphere:
         tr = self.transformation
         if tr is None:
             return self
         center = tr.apply2point(self._center)
         options = self.clean_options()
         return Sphere(center, self._radius, transform=None, **options)
 
-    def transform(self, tr: Transformation) -> "Sphere":
+    def transform(self, tr: Transformation) -> Sphere:
         if tr is None:
             return self
         tr = self.combine_transformations(tr)
         options = self.clean_options()
         return Sphere(self._center, self._radius, transform=tr, **options)
 
-    def mcnp_words(self, pretty: bool = False) -> List[str]:
+    def mcnp_words(self, pretty: bool = False) -> list[str]:
         words = Surface.mcnp_words(self, pretty)
         c = self._center
         if np.array_equal(self._center, ORIGIN):
             words.append("SO")
         elif c[0] == 0.0 and c[1] == 0.0:
             words.append("SZ")
             add_float(words, c[2], pretty)
@@ -881,27 +914,27 @@
         return are_equal(
             (self._radius, self._pt, self._axis, self.transformation),
             (other._radius, other._pt, other._axis, other.transformation),
         )
 
     def is_close_to(
         self,
-        other: "Cylinder",
+        other: Cylinder,
         estimator: Callable[[Any, Any], bool] = DEFAULT_TOLERANCE_ESTIMATOR,
     ) -> bool:
         if self is other:
             return True
         if not isinstance(other, Cone):
             return False
         return estimator(
             (self._radius, self._pt, self._axis, self.transformation),
             (other._radius, other._pt, other._axis, other.transformation),
         )
 
-    def round(self):
+    def round(self):  # noqa: A003
         temp = self.apply_transformation()
         pt = round_array(temp._pt)
         axis = round_array(temp._axis)
         radius = round_scalar(temp._radius)
         options = self.clean_options()
         return Cylinder(pt, axis, radius, transform=None, **options)
 
@@ -911,15 +944,15 @@
             return self
         pt = tr.apply2point(self._pt)
         axis = tr.apply2vector(self._axis)
         options = self.clean_options()
         # TODO dvp: actually may create Generic Quadratic. Should we use __new__() for this?
         return Cylinder(pt, axis, self._radius, assume_normalized=True, **options)
 
-    def transform(self, tr: Transformation) -> "Cylinder":
+    def transform(self, tr: Transformation) -> Cylinder:
         if tr is None:
             return self
         tr = self.combine_transformations(tr)
         options = self.clean_options()
         return Cylinder(
             self._pt,
             self._axis,
@@ -1028,15 +1061,15 @@
             return self
         apex = tr.apply2point(self._apex)
         axis = tr.apply2vector(self._axis)
         sheet = self._sheet
         options = self.clean_options()
         return Cone(apex, axis, self._t2, sheet, assume_normalized=True, **options)
 
-    def round(self) -> Surface:
+    def round(self) -> Surface:  # noqa: A003
         res = self.apply_transformation()
         apex = round_array(res._apex)
         axis = round_array(res._axis)
         t2 = round_scalar(self._t2)
         sheet = self._sheet
         options = self.clean_options()
         # TODO dvp: what if Generic Quadratic is to be returned?
@@ -1062,50 +1095,48 @@
         apex, axis, t2, sheet, options = state
         self.__init__(apex, axis, t2, sheet, **options)
 
     def __hash__(self):
         return self._hash
 
     def __eq__(self, other):
-
         # noinspection DuplicatedCode
         if self is other:
             return True
 
         if not isinstance(other, Cone):
             return False
 
         return are_equal(
             (self._t2, self._sheet, self._apex, self._axis, self.transformation),
             (other._t2, other._sheet, other._apex, other._axis, self.transformation),
         )
 
     def is_close_to(
         self,
-        other: "Surface",
+        other: Surface,
         estimator: Callable[[Any, Any], bool] = DEFAULT_TOLERANCE_ESTIMATOR,
     ) -> bool:
         if self is other:
             return True
         if not isinstance(other, Cone):
             return False
         return estimator(
             (self._apex, self._axis, self._t2, self.transformation),
             (other._apex, other._axis, other._t2, other.transformation),
         )
 
-    def transform(self, tr: Transformation) -> "Surface":
+    def transform(self, tr: Transformation) -> Surface:
         if tr is None:
             return self
         tr = self.combine_transformations(tr)
         options = self.clean_options()
-        cone = Cone(self._apex, self._axis, self._t2, sheet=self._sheet, transform=tr, **options)
-        return cone
+        return Cone(self._apex, self._axis, self._t2, sheet=self._sheet, transform=tr, **options)
 
-    def mcnp_words(self, pretty: bool = False) -> List[str]:
+    def mcnp_words(self, pretty: bool = False) -> list[str]:
         words = Surface.mcnp_words(self)
         axis = self._axis
         apex = self._apex
         if np.array_equal(axis, EX):
             if apex[1] == 0.0 and apex[2] == 0.0:
                 words.append("KX")
                 add_float(words, apex[0], pretty)
@@ -1182,29 +1213,29 @@
         tr = self.transformation
         if tr is None:
             return self
         m, v, k = tr.apply2gq(self._m, self._v, self._k)
         options = self.clean_options()
         return GQuadratic(m, v, k, **options)
 
-    def round(self) -> Surface:
+    def round(self) -> Surface:  # noqa: A003
         temp: Surface = self.apply_transformation()
         m, v = map(round_array, [temp._m, temp._v])
         k = round_scalar(temp._k)
         # TODO dvp: handle cases when the surface can be represented with specialized quadratic surface: Cone etc.
         return GQuadratic(m, v, k, **self.clean_options())
 
     def __getstate__(self):
         return self._m, self._v, self._k, self._factor, Surface.__getstate__(self)
 
     def __setstate__(self, state):
         m, v, k, factor, options = state
         self.__init__(m, v, k, factor, **options)
 
-    def copy(self) -> "GQuadratic":
+    def copy(self) -> GQuadratic:
         options = deepcopy(self.options)
         return GQuadratic(self._m, self._v, self._k, self._factor, **options)
 
     def __repr__(self):
         options = str(self.options) if self.options else ""
         return f"GQuadratic({self._m}, {self._v}, {self._k}, {self._factor}, {options})"
 
@@ -1240,15 +1271,15 @@
     def transform(self, tr):
         if tr is None:
             return self
         tr = self.combine_transformations(tr)
         options = self.clean_options()
         return GQuadratic(self._m, self._v, self._k, transform=tr, **options)
 
-    def mcnp_words(self, pretty: bool = False) -> List[str]:
+    def mcnp_words(self, pretty: bool = False) -> list[str]:
         words = Surface.mcnp_words(self)
         words.append("GQ")
         m = self._m
         a, b, c = np.diag(m)
         d = m[0, 1] + m[1, 0]
         e = m[1, 2] + m[2, 1]
         f = m[0, 2] + m[2, 0]
@@ -1291,26 +1322,26 @@
         maxdir = np.argmax(np.abs(axis))
         if axis[maxdir] < 0:
             axis *= -1
         Surface.__init__(self, **options)
         _Torus.__init__(self, center, axis, r, a, b)
         self._hash = compute_hash(self._center, self._axis, self._R, self._a, self._b)
 
-    def round(self) -> "Surface":
+    def round(self) -> Surface:  # noqa: A003
         temp = self.apply_transformation()
         center, axis = map(round_array, [temp._center, temp._axis])
 
         def r(x):
             return round_scalar(x, significant_digits(x, FLOAT_TOLERANCE))
 
         r, a, b = map(r, [temp._R, temp._a, temp._b])
         options = temp.clean_options()
         return Torus(center, axis, r, a, b, assume_normalized=True, **options)
 
-    def apply_transformation(self) -> "Surface":
+    def apply_transformation(self) -> Surface:
         tr = self.transformation
         if tr is None:
             return self
         center = tr.apply2point(self._center)
         axis = tr.apply2vector(self._axis)
         # TODO dvp: should we check the transformation and result? The axis is to be along EX, EY, EZ.
         return Torus(
@@ -1347,15 +1378,15 @@
             assume_normalized=True,
             **deepcopy(self.options),
         )
 
     def __hash__(self):
         return self._hash
 
-    def __eq__(self, other: "Torus"):
+    def __eq__(self, other: Torus):
         if self is other:
             return True
         if not isinstance(other, Torus):
             return False
         return are_equal(
             (self._center, self._axis, self._R, self._a, self._b, self.transformation),
             (
@@ -1366,15 +1397,15 @@
                 other._b,
                 other.transformation,
             ),
         )
 
     def is_close_to(
         self,
-        other: "Torus",
+        other: Torus,
         estimator: Callable[[Any, Any], bool] = DEFAULT_TOLERANCE_ESTIMATOR,
     ) -> bool:
         if self is other:
             return True
         if not isinstance(other, Torus):
             return False
         return estimator(
@@ -1392,15 +1423,15 @@
     def transform(self, tr):
         if tr is None:
             return self
         tr = self.combine_transformations(tr)
         options = self.clean_options()
         return Torus(self._center, self._axis, self._R, self._a, self._b, transform=tr, **options)
 
-    def mcnp_words(self, pretty: bool = False) -> List[str]:
+    def mcnp_words(self, pretty: bool = False) -> list[str]:
         words = Surface.mcnp_words(self)
         estimator = DEFAULT_TOLERANCE_ESTIMATOR
         if estimator(self._axis, EX):
             words.append("TX")
         elif estimator(self._axis, EY):
             words.append("TY")
         elif estimator(self._axis, EZ):
```

### Comparing `mckit-0.6.23/src/mckit/transformation.py` & `mckit-0.6.24/src/mckit/transformation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Code for transformations."""
 from __future__ import annotations
 
-from typing import Any, Optional, Tuple
+from typing import Any
 
 import numpy as np
 
 from numpy.typing import ArrayLike
 
 # noinspection PyUnresolvedReferences,PyPackageRequirements
 from mckit.geometry import ORIGIN
@@ -47,15 +47,15 @@
         How translation vector should be interpreted. If True - it is the origin
         of local coordinate system defined in the global one. Otherwise - the
         origin of global coordinate system defined in the local one.
         Default: False
     options : dict
         Other options, like name, comment, etc.
 
-    Methods
+    Methods:
     -------
     apply2gq(m, v, k)
         Gets parameters of generic quadratic surface in the main coordinate
         system.
     apply2plane(v, k)
         Gets parameters of plane in the main coordinate system.
     apply2point(p)
@@ -72,15 +72,14 @@
         self,
         translation=ORIGIN,
         rotation=None,
         indegrees=False,
         inverted=False,
         **options: dict[str, Any],
     ):
-
         Card.__init__(self, **options)
 
         if translation is not ORIGIN:
             translation = np.asarray(translation, dtype=float)
             if translation.shape != (3,):
                 raise ValueError(f"Transaction #{self.name()}: wrong length of translation vector.")
 
@@ -121,15 +120,15 @@
                 words.append(" ")
                 _value = np.arccos(v) * 180 / np.pi
                 words.append(f"{_value:.10g}")
         return words
 
     def apply2gq(
         self, m1: ArrayLike, v1: ArrayLike, k1: float
-    ) -> Tuple[ArrayLike, ArrayLike, float]:
+    ) -> tuple[ArrayLike, ArrayLike, float]:
         """Gets parameters of generic quadratic surface in the main CS.
 
         Args:
             m1 : array_like[float]
                 A 3x3 matrix which defines coefficients of quadratic terms of
                 generic quadratic surface equation in the auxiliary coordinate
                 system.
@@ -152,15 +151,15 @@
                 Free term of GQ surface equation in the main coordinate system.
         """
         m = np.dot(np.dot(self._u, m1), np.transpose(self._u))
         v = np.dot(self._u, v1) - 2 * np.dot(m, self._t)
         k = k1 - np.dot(v, self._t) - np.dot(self._t, np.dot(m, self._t))
         return m, v, k
 
-    def apply2plane(self, v1: ArrayLike, k1: float) -> Tuple[ArrayLike, float]:
+    def apply2plane(self, v1: ArrayLike, k1: float) -> tuple[ArrayLike, float]:
         """Gets parameters of plane surface in the main coordinate system.
 
         Args:
             v1: A vector of size 3 which defines vector, normal to the plane in
                 the auxiliary coordinate system.
             k1: Free term of plane equation in the auxiliary coordinate
                 system.
@@ -198,15 +197,15 @@
 
         Returns:
             Coordinates of the vector(s) in the main coordinate system.
         """
         # In contrast with apply2point - no translation is needed.
         return np.dot(v1, np.transpose(self._u))
 
-    def apply2transform(self, tr: "Transformation") -> "Transformation":
+    def apply2transform(self, tr: Transformation) -> Transformation:
         """Gets new transformation.
 
         Suppose there are three coordinate systems r, r1, r2. Transformation
         tr: r2 -> r1; and this transformation: r1 -> r. Thus the resulting
         transformation: r2 -> r. In other words the result is a sequence of
         two transformations: `tr` and this. The `tr` is applied first.
 
@@ -216,15 +215,15 @@
         Returns:
             New transformation - the result.
         """
         rot = np.dot(self._u, tr._u)
         trans = self.apply2point(tr._t)
         return Transformation(translation=trans, rotation=rot)
 
-    def reverse(self) -> "Transformation":
+    def reverse(self) -> Transformation:
         """Reverses this transformation.
 
         Gets new transformation which is complement to this one.
 
         Returns:
             Reversed version of this transformation.
         """
@@ -238,15 +237,15 @@
         """Check if this transformation is almost equal to `other` one."""
         if self is other:
             return True
         if not isinstance(other, Transformation):
             return False
         return estimator((self._t, self._u), (other._t, other._u))
 
-    def _setup_rotation_matrix(self, u: Optional[ArrayLike]) -> ArrayLike:
+    def _setup_rotation_matrix(self, u: ArrayLike | None) -> ArrayLike:
         zero_cosines_idx = np.abs(u) < ZERO_COS_TOLERANCE
         u[zero_cosines_idx] = 0.0
         # TODO: Implement creation from reduced rotation parameter set.
         if u.shape == (9,):
             u = u.reshape((3, 3), order="F")
         if u.shape != (3, 3):
             raise ValueError(
```

### Comparing `mckit-0.6.23/src/mckit/universe.py` & `mckit-0.6.24/src/mckit/universe.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-from typing import Any, Callable, Dict, Iterable, List, Optional, Set, Tuple, Union, cast
+from __future__ import annotations
+
+from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, cast
 
 import operator
 import sys
 
 from collections import defaultdict
 from contextlib import contextmanager
 from functools import reduce
 from io import StringIO
+from logging import getLogger
 from pathlib import Path
 
 import numpy as np
 
 from attr import attrib, attrs
 from click import progressbar
 from mckit.constants import MCNP_ENCODING
@@ -33,17 +36,19 @@
     "collect_transformations",
     "UniverseAnalyser",
 ]
 
 from .utils.indexes import IndexOfNamed, StatisticsCollector
 from .utils.named import Name
 
+_LOG = getLogger(__name__)
+
 
 class NameClashError(ValueError):
-    def __init__(self, result: Union[str, Dict[str, Dict[int, Set["Universe"]]]]) -> None:
+    def __init__(self, result: str | dict[str, dict[int, set[Universe]]]) -> None:
         if isinstance(result, str):
             ValueError.__init__(self, result)
         else:
             msg = StringIO()
             msg.write("\n")
             for kind, index in result.items():
                 for i, u in index.items():
@@ -56,42 +61,41 @@
     """Produces cell selector function for specific cell names.
 
     Parameters
     ----------
     cell_names : int or iterable
         Names of cells to be selected.
 
-    Returns
+    Returns:
     -------
     selector : func
         Selector function.
     """
     if isinstance(cell_names, int):
         cell_names = {cell_names}
     else:
         cell_names = set(cell_names)
 
     def selector(cell):
         if cell.name() in cell_names:
             return [cell]
-        else:
-            return []
+        return []
 
     return selector
 
 
 def surface_selector(surface_names):
     """Produces surface selector function for specific surface names.
 
     Parameters
     ----------
     surface_names : int or iterable
         Names of surfaces to be selected.
 
-    Returns
+    Returns:
     -------
     selector : func
         Selector function
     """
     if isinstance(surface_names, int):
         surface_names = {surface_names}
     else:
@@ -121,15 +125,15 @@
         Optional verbose name. This name also can be used to retrieve inner
         universe.
     comment : list[str] or str
         String or list of strings that describes the universe.
     common_materials : set
         A set of common materials. Default: None.
 
-    Methods
+    Methods:
     -------
     add_cells(cell)
         Adds new cell to the universe.
     apply_fill(cell, universe)
         Applies fill operations to all or selected cells or universes.
     bounding_box(tol, box)
         Gets bounding box of the universe.
@@ -172,15 +176,15 @@
     def __init__(
         self,
         cells,
         name: Name = 0,
         verbose_name: str = None,
         comment: str = None,
         name_rule: str = "keep",
-        common_materials: Set[Composition] = None,
+        common_materials: set[Composition] = None,
     ):
         self._name = name
         self._comment = comment
         self._verbose_name = verbose_name
         self._cells = []
         if common_materials is None:
             common_materials = set()
@@ -259,16 +263,16 @@
             if mat:
                 new_comp = Universe._update_replace_dict(
                     mat.composition, comp_replace, comp_names, name_rule, "Material"
                 )
                 new_cell.options["MAT"] = Material(composition=new_comp, density=mat.density)
 
             if name_rule == "keep" and cell.name() in cell_names:
-                raise NameClashError("Cell name clash: {0}".format(cell.name()))
-            elif name_rule == "new" or name_rule == "clash" and cell.name() in cell_names:
+                raise NameClashError(f"Cell name clash: {cell.name()}")
+            if name_rule == "new" or name_rule == "clash" and cell.name() in cell_names:
                 new_name = max(cell_names, default=0) + 1
                 new_cell.rename(new_name)
             cell_names.add(new_cell.name())
             new_cell.options["U"] = self
             self._cells.append(new_cell)
 
     def set_common_materials(self, common_materials):
@@ -317,57 +321,55 @@
         return cell.shape.replace_surfaces(replace_dict)
 
     @staticmethod
     def _update_replace_dict(entity, replace, names, rule, err_desc):
         if entity not in replace.keys():
             new_entity = entity.copy()
             if rule == "keep" and new_entity.name() in names:
-                print(entity.mcnp_repr())
+                _LOG.debug(entity.mcnp_repr())
                 for c in replace.keys():
-                    print(c.mcnp_repr())
-                raise NameClashError("{0} name clash: {1}".format(err_desc, entity.name()))
-            elif rule == "new" or rule == "clash" and new_entity.name() in names:
+                    _LOG.debug(c.mcnp_repr())
+                raise NameClashError(f"{err_desc} name clash: {entity.name()}")
+            if rule == "new" or rule == "clash" and new_entity.name() in names:
                 new_name = max(names, default=0) + 1
                 new_entity.rename(new_name)
                 names.add(new_name)
             replace[new_entity] = new_entity
             names.add(new_entity.name())
             return new_entity
-        else:
-            return replace[entity]
+        return replace[entity]
 
     @staticmethod
     def _fill_check(predicate):
         def _predicate(cell):
             fill = cell.options.get("FILL", None)
             if fill:
                 return predicate(cell)
-            else:
-                return False
+            return False
 
         return _predicate
 
     def alone(self):
         """Gets this universe alone, without inner universes.
 
-        Returns
+        Returns:
         -------
         u : Universe
             A copy of the universe with FILL cards removed.
         """
         cells = []
         for c in self:
             options = {k: v for k, v in c.options.items() if k != "FILL"}
             cells.append(Body(c.shape, **options))
         return Universe(cells)
 
     def apply_fill(
         self,
-        cell: Union[Body, int] = None,
-        universe: Union["Universe", int] = None,
+        cell: Body | int = None,
+        universe: Universe | int = None,
         predicate: Callable[[Body], bool] = None,
         name_rule: str = "new",
     ):
         """Applies fill operations to all or selected cells or universes.
 
         Modifies current universe.
 
@@ -427,15 +429,15 @@
             this value. Default: 100 cm.
         box : Box
             Starting box for the search. The user must be sure that box covers
             all geometry, because cells, that already contains corners of the
             box will be considered as infinite and will be excluded from
             analysis.
 
-        Returns
+        Returns:
         -------
         bbox : Box
             Universe bounding box.
         """
         boxes = []
         for c in self._cells:
             test = c.shape.test_points(box.corners)
@@ -460,38 +462,31 @@
             comment=self._comment,
             common_materials=self._common_materials,
         )
 
     def find_common_materials(self):
         """Finds common materials among universes included.
 
-        Returns
-        -------
-        common_mats : set
+        Returns:
             A set of common materials.
         """
         comp_count = defaultdict(lambda: 0)
         for u in self.get_universes():
             for c in u.get_compositions():
                 comp_count[c] += 1
-        common_mats = {c for c, cnt in comp_count.items() if cnt > 1}
-        return common_mats
+        return {c for c, cnt in comp_count.items() if cnt > 1}
 
-    def get_surfaces(self, inner: bool = False) -> Set[Surface]:
+    def get_surfaces(self, inner: bool = False) -> set[Surface]:
         """Gets all surfaces of the universe.
 
-        Parameters
-        ----------
-        inner : bool
-            Whether to take surfaces of inner universes. Default: False -
-            return surfaces of this universe only.
+        Args:
+            inner:  Whether to take surfaces of inner universes. Default: False -
+                    return surfaces of this universe only.
 
-        Returns
-        -------
-        surfs : set
+        Returns:
             A set of surfaces that belong to the universe.
         """
         surfs = set()
         for c in self:
             surfs.update(c.shape.get_surfaces())
             if inner and "FILL" in c.options.keys():
                 surfs.update(c.options["FILL"]["universe"].get_surfaces(inner))
@@ -502,40 +497,40 @@
             surfaces_list.extend(cell.shape.get_surfaces())
             if inner and "FILL" in cell.options:
                 surfaces_list.extend(cell.options["FILL"]["universe"].get_surfaces_list(inner))
             return surfaces_list
 
         return reduce(reducer, self, [])
 
-    def get_compositions(self, exclude_common: bool = False) -> Set[Composition]:
+    def get_compositions(self, exclude_common: bool = False) -> set[Composition]:
         """Gets all compositions of the universe.
 
         Parameters
         ----------
         exclude_common : bool
             Exclude common compositions from the result. Default: False.
 
-        Returns
+        Returns:
         -------
         comps : set
             A set of Composition objects.
         """
         compositions = set()
         for c in self:
             material = c.material()
             if material:
                 compositions.add(material.composition)
         if exclude_common:
             compositions.difference_update(self._common_materials)
         return compositions
 
-    def get_universes(self) -> Set["Universe"]:
+    def get_universes(self) -> set[Universe]:
         """Gets all inner universes.
 
-        Returns
+        Returns:
         -------
         universes : set
             A set of universes.
         """
         universes = {self}
         for c in self:
             if "FILL" in c.options:
@@ -543,18 +538,18 @@
                 universes.update(u.get_universes())
         return universes
 
     def name(self) -> Name:
         """Gets numeric name of the universe."""
         return self._name
 
-    def name_clashes(self) -> Dict[str, Dict[int, Set["Universe"]]]:
+    def name_clashes(self) -> dict[str, dict[int, set[Universe]]]:
         """Checks, if there is name clashes.
 
-        Returns
+        Returns:
         -------
         stat : dict
             Description of found clashes. If no clashes - the dictionary is empty.
         """
         universes = self.get_universes()
         universe_to_cell_name_map = {u: list(map(Card.name, u)) for u in universes}
         universe_to_surface_name_map = {
@@ -577,23 +572,23 @@
         ustat = Universe._produce_stat(univs)
         if ustat:
             stat["universe"] = ustat
         # TODO dvp: handle transformations here
         return stat
 
     @staticmethod
-    def _produce_stat(names: Dict["Universe", Iterable[int]]) -> Dict[int, Set["Universe"]]:
+    def _produce_stat(names: dict[Universe, Iterable[int]]) -> dict[int, set[Universe]]:
         stat = defaultdict(list)
         for u, u_names in names.items():
             for name in u_names:
                 stat[name].append(u)
         return Universe._clean_stat_dict(stat)
 
     @staticmethod
-    def _clean_stat_dict(stat) -> Dict[int, Set["Universe"]]:
+    def _clean_stat_dict(stat) -> dict[int, set[Universe]]:
         new_stat = {}
         for k, v in stat.items():
             if len(v) > 1:
                 new_stat[k] = set(v)
         return new_stat
 
     def rename(
@@ -647,15 +642,15 @@
     def check_clashes(self) -> None:
         result = self.name_clashes()
         if result:
             raise NameClashError(result)
 
     def save(
         self,
-        filename: Union[str, Path],
+        filename: str | Path,
         encoding: str = MCNP_ENCODING,
         check_clashes: bool = True,
     ):
         """Saves the universe into file."""
         # NOTE dvp: Don't try to resolve names here, the object shouldn't change on save() function.
         # self.check_clashes()
         if check_clashes:
@@ -668,15 +663,15 @@
 
         transformations = collect_transformations(self)
         if transformations:
             transformations = sorted(transformations, key=Card.name)
         universes = self.get_universes()
         cells = []
         surfaces = []
-        materials = list(sorted(self._common_materials, key=Card.name))
+        materials = sorted(self._common_materials, key=Card.name)
         for u in sorted(universes, key=Universe.name):
             cells.extend(sorted(u, key=Card.name))
             surfaces.extend(sorted(u.get_surfaces(), key=Card.name))
             materials.extend(sorted(u.get_compositions(True), key=Card.name))
         cards = [self.verbose_name]
         cards.extend(map(Card.mcnp_repr, cells))
         cards.append("")
@@ -698,15 +693,15 @@
         selector : func
             A function that accepts 1 argument, Body instance, and returns
             selected entities.
         inner : bool
             Whether to consider inner universes. Default: False - only this
             universe will be taken into account.
 
-        Returns
+        Returns:
         -------
         items : list
             List of selected items.
         """
         items = []
         taken_ids = set()
         for c in self:
@@ -737,68 +732,67 @@
         verbose : bool
             Turns on verbose output. Default: True.
         """
         new_cells = []
         if verbose:
 
             def fmt_fun(x):
-                return "Simplifying cell #{0}".format(x.name() if x else x)
+                return f"Simplifying cell #{x.name() if x else x}"
 
             uiter = progressbar(self, item_show_func=fmt_fun).__enter__()
         else:
             uiter = self
 
         for c in uiter:
             cs = c.simplify(box=box, min_volume=min_volume)
             if not cs.shape.is_empty():
                 new_cells.append(cs)
 
-        if verbose:
-            print("Universe {0} simplification has been finished.".format(self.name()))
-            print("{0} empty cells were deleted.".format(len(self._cells) - len(new_cells)))
+        _LOG.info(f"Universe {self.name()} simplification has been finished.")
+        _LOG.info(f"{len(self._cells) - len(new_cells)} empty cells were deleted.")
 
         self._cells = new_cells
 
     def test_points(self, points):
         """Finds cell to which each point belongs to.
 
         Parameters
         ----------
         points : array_like[float]
             An array of point coordinates. If there is only one point it has
             shape (3,); if there are n points, it has shape (n, 3).
 
-        Returns
+        Returns:
         -------
         result : np.ndarray[int]
             An array of cell indices to which a particular point belongs to.
             Its length equals to the number of points.
         """
         points = np.array(points)
         result = np.empty(points.size // 3)
         for i, c in enumerate(self._cells):
             test = c.shape.test_points(points)
             result[test == +1] = i
         return result
 
-    def transform(self, tr: Transformation) -> "Universe":
+    def transform(self, tr: Transformation) -> Universe:
         """Applies transformation tr to this universe.
 
         Returns a new universe.
         """
         new_cells = [c.transform(tr) for c in self]
         return Universe(
             new_cells,
             name=self._name,
             name_rule="clash",
             verbose_name=self._verbose_name,
             comment=self._comment,
         )
 
-    def apply_transformation(self) -> "Universe":
+    def apply_transformation(self) -> Universe:
         """Applies transformations specified in cells.
 
         Returns a new universe.
         """
         new_cells = [c.apply_transformation() for c in self]
         return Universe(
             new_cells,
@@ -817,91 +811,91 @@
     def comment(self):
         return self._comment
 
 
 @attrs
 class _UniverseCellsGroup:
     universe: Universe = attrib()
-    cells: List[Body] = attrib()
+    cells: list[Body] = attrib()
 
 
 def produce_universes(cells: Iterable[Body]) -> Universe:
     """Creates groups from cells.
 
     The function groups all the cells by 'universe' option value,
     and creates corresponding groups.
 
     Parameters
     ----------
     cells : Iterable[Body]
         Cells to process.
 
-    Returns
+    Returns:
     -------
     universe : Universe
         The top level universe with name = 0.
     """
-    groups: Dict[Name, _UniverseCellsGroup] = {}
+    groups: dict[Name, _UniverseCellsGroup] = {}
     for c in cells:
         universe_no: Name = c.options.get("U", 0)
         if universe_no in groups:
             groups[universe_no].cells.append(c)
         else:
             new_group = _UniverseCellsGroup(universe=Universe([], universe_no), cells=[c])
             groups[universe_no] = new_group
     for c in cells:
-        fill: Dict[str, Any] = c.options.get("FILL", None)
+        fill: dict[str, Any] = c.options.get("FILL", None)
         if fill is not None:
             fill_universe_no = fill["universe"]
             fill["universe"] = groups[fill_universe_no].universe
     for group in groups.values():
         group.universe.add_cells(group.cells, name_rule="keep")
     top_universe = groups[0].universe
     top_universe.set_common_materials(top_universe.find_common_materials())
     return top_universe
 
 
-def collect_transformations(universe: Universe, recursive=True) -> Set[Transformation]:
-    def add_surface_transformation(aggregator: Set[Transformation], surface: Surface) -> None:
+def collect_transformations(universe: Universe, recursive=True) -> set[Transformation]:
+    def add_surface_transformation(aggregator: set[Transformation], surface: Surface) -> None:
         transformation = surface.transformation
         if transformation and transformation.name():
             aggregator.add(transformation)
 
-    def at_surface(aggregator: Set[Transformation], s: Union[Surface, Shape, Body]):
+    def at_surface(aggregator: set[Transformation], s: Surface | Shape | Body):
         if isinstance(s, Surface):
             add_surface_transformation(aggregator, s)
         elif isinstance(s, Shape):
             aggregator.update(accept(s, visit_shape))
         else:
             assert isinstance(s, Body)
             aggregator.update(accept(s, visit_body))
         return aggregator
 
     @contextmanager
-    def visit_shape(s: Union[Surface, Body, Shape]):
+    def visit_shape(s: Surface | Body | Shape):
         if isinstance(s, (Surface, Body, Shape)):
             yield at_surface, set()
         else:
             on_unknown_acceptor(s)
 
-    def at_shape(aggregator: Set[Transformation], s: Union[Surface, Body, Shape]):
+    def at_shape(aggregator: set[Transformation], s: Surface | Body | Shape):
         if isinstance(s, Surface):
             add_surface_transformation(aggregator, s)
             return aggregator
         aggregator.update(accept(s, visit_shape))
         return aggregator
 
     @contextmanager
     def visit_body(b: Body):
         if isinstance(b, Body):
             yield at_shape, set()
         else:
             on_unknown_acceptor(b)
 
-    def at_body(aggregator: Set[Transformation], b: Body) -> Set[Transformation]:
+    def at_body(aggregator: set[Transformation], b: Body) -> set[Transformation]:
         body_transformation = b.transformation
         if body_transformation and body_transformation.name():
             aggregator.add(body_transformation)
         if recursive:
             fill = b.options.get("FILL", None)
             if fill:
                 fill_universe = fill["universe"]
@@ -909,15 +903,15 @@
                 if fill_transformation and fill_transformation.name():
                     aggregator.add(fill_transformation)
                 aggregator.update(collect_transformations(fill_universe))
         aggregator.update(accept(b, visit_body))
         return aggregator
 
     @contextmanager
-    def visit_universe(u: Universe) -> Set[Transformation]:
+    def visit_universe(u: Universe) -> set[Transformation]:
         if isinstance(u, Universe):
             yield at_body, set()
             # TODO dvp:  set() is not a valid choice as aggregator considering
             #        cases when names differ but transformations are equal by values
         else:
             on_unknown_acceptor(u)
 
@@ -968,15 +962,15 @@
 def transformations_to_universe_mapper(universe: Universe) -> IU:
     return (
         list(map(Transformation.name, collect_transformations(universe, recursive=False))),
         universe.name(),
     )
 
 
-def is_shared_between_universes(item: Tuple[Name, Dict[Name, int]]) -> bool:
+def is_shared_between_universes(item: tuple[Name, dict[Name, int]]) -> bool:
     entity, universes_counts = item
     return 1 < len(universes_counts.keys())
 
 
 def make_universe_counter_map():
     return defaultdict(int)
 
@@ -1002,15 +996,15 @@
         universes = self.universe.get_universes()
         self.universe_duplicates = StatisticsCollector(ignore_equal=True)
         self.universes_index = IndexOfNamed.from_iterable(
             universes,
             on_duplicate=self.universe_duplicates,
         )
         self.cell_duplicates = StatisticsCollector()
-        cells: List[Body] = reduce(operator.add, map(list, universes), [])
+        cells: list[Body] = reduce(operator.add, map(list, universes), [])
         self.cell_index = IndexOfNamed[Name, Body].from_iterable(
             cells,
             on_duplicate=self.cell_duplicates,
         )
         self.cell_to_universe_map = collect_shared_entities(cells_to_universe_mapper, universes)
         self.surface_duplicates = StatisticsCollector(ignore_equal=True)
         self.surface_index = IndexOfNamed[Name, Surface].from_iterable(
@@ -1053,20 +1047,20 @@
             self.transformations_to_universe_map,
         )
 
     def we_are_all_clear(self) -> bool:
         return not any(self.duplicates())
 
     def print_duplicates_map(self, stream=sys.stdout):
-        def printer(_, item: Tuple[str, E2U]):
+        def printer(_, item: tuple[str, E2U]):
             tag, info = item
-            entities = sorted(list(info.keys()))
+            entities = sorted(info.keys())
             for e in entities:
                 universes_count_map = info[e]
-                universes = sorted(list(universes_count_map.keys()))
+                universes = sorted(universes_count_map.keys())
                 print(f"{tag} {e} occurs", file=stream)
                 for u in universes:
                     print(
                         f"   in universe {u} {universes_count_map[u]} times",
                         file=stream,
                     )
```

### Comparing `mckit-0.6.23/src/mckit/utils/__init__.py` & `mckit-0.6.24/src/mckit/utils/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Utility code to use in all other modules."""
+from __future__ import annotations
+
 from mckit.utils.accept import TVisitor, accept, on_unknown_acceptor
 from mckit.utils.io import MCNP_ENCODING
 from mckit.utils.misc import (
     MAX_DIGITS,
     are_equal,
     compute_hash,
     deepcopy,
```

### Comparing `mckit-0.6.23/src/mckit/utils/accept.py` & `mckit-0.6.24/src/mckit/utils/accept.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """The interfaces to facilitate adding new functionality to an hierarchy of classes (Visitor pattern)."""
+from __future__ import annotations
+
 from typing import Any, Callable, ContextManager, NoReturn
 
 from functools import reduce
 
 TVisitor = Callable[..., ContextManager]
```

### Comparing `mckit-0.6.23/src/mckit/utils/indexes.py` & `mckit-0.6.24/src/mckit/utils/indexes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Classes to index MCNP objects on model file parsing."""
 from __future__ import annotations
 
-from typing import Callable, Dict, Iterable, NoReturn, Optional, Type, TypeVar, cast
+from typing import Callable, Dict, Iterable, NoReturn, Optional, TypeVar, cast
 
 from functools import reduce
 
 from mckit.utils.named import Name, default_name_key
 
 Key = TypeVar("Key")
 Item = TypeVar("Item")
@@ -21,15 +21,15 @@
         _default_factory (FactoryMethodWithKey):
             Same as in Args.
     """
 
     def __init__(
         self,
         default_factory: FactoryMethodWithKey = None,
-        **kwargs: Dict[Key, Item],
+        **kwargs: dict[Key, Item],
     ) -> None:
         """Create `Index`.
 
         Args:
             default_factory: factory method accepting `key` as the only positional argument.
             kwargs: keyword arguments to pass to base class, if any
         """
@@ -37,36 +37,36 @@
         self._default_factory = default_factory
 
     @property
     def default_factory(self) -> FactoryMethodWithKey:
         """Public accessor to `self._default_factory`."""
         return self._default_factory
 
-    def __missing__(self, key: Key) -> Optional[Item]:
+    def __missing__(self, key: Key) -> Item | None:
         """Calls default factory with the key as argument."""
         if self._default_factory:
             return self._default_factory(key)
 
         raise NumberedItemNotFoundError(key)
 
 
 # noinspection PyUnusedLocal
-def ignore(_: Key) -> Optional[Item]:
+def ignore(_: Key) -> Item | None:
     """Default factory for `IgnoringIndex`.
 
     Returns:
         None - always.
     """
     return None
 
 
 class IgnoringIndex(Index[Key, Item]):
     """Index ignoring absence of a key in the dictionary."""
 
-    def __init__(self, **kwargs: Dict[Key, Item]) -> None:
+    def __init__(self, **kwargs: dict[Key, Item]) -> None:
         Index.__init__(self, ignore, **kwargs)
 
 
 class NumberedItemNotFoundError(KeyError):
     """Error to raise, when an item is not found in an `Index`."""
 
     kind: str = ""
@@ -147,21 +147,21 @@
 
 
 class IndexOfNamed(Index[Key, Item]):
     """Index of items from a key can be extracted."""
 
     @classmethod
     def from_iterable(
-        cls: Type["IndexOfNamed[Key, Item]"],
+        cls: type[IndexOfNamed[Key, Item]],
         items: Iterable[Item],
         *,
         key: Callable[[Item], Name] = default_name_key,
         default_factory: Callable[[Key], Item] = None,
         on_duplicate: Callable[[Key, Item, Item], None] = None,
-    ) -> "IndexOfNamed":
+    ) -> IndexOfNamed:
         """Construct `IndexOfNamed` from `items`."""
         index = cls(default_factory)
 
         def _reducer(a, b):
             name = key(b)
             if on_duplicate is not None and name in a:
                 on_duplicate(name, a[name], b)
```

### Comparing `mckit-0.6.23/src/mckit/utils/io.py` & `mckit-0.6.24/src/mckit/utils/io.py`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/src/mckit/utils/misc.py` & `mckit-0.6.24/src/mckit/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Generic utility methods."""
 from __future__ import annotations
 
-from typing import Any, Dict, Tuple, cast
+from typing import Any, cast
 
 import collections
 import collections.abc
 import functools
 import itertools
 
 from copy import deepcopy
@@ -45,16 +45,15 @@
         if abs(value - v) > reltol * d:
             low = p
         else:
             high = p
     v = round(value, low)
     if abs(value - v) < reltol * d:
         return low
-    else:
-        return high
+    return high
 
 
 def get_decades(value: int | float) -> int:
     """Compute number of digits needed to represent integer part of 'value' in fixed format.
 
     Args:
         value: ... to check
@@ -163,17 +162,17 @@
 
 @is_in.register
 def _(where: collections.abc.Container, x) -> bool:
     return x in where
 
 
 def filter_dict(
-    a: Dict[Any, Any],
+    a: dict[Any, Any],
     *drop_items,
-) -> Dict[Any, Any]:
+) -> dict[Any, Any]:
     """Create copy of a dictionary omitting some keys."""
     res = {}
     for k, v in a.items():
         if drop_items and is_in(drop_items, k):
             pass
         else:
             if isinstance(v, dict):
@@ -198,20 +197,20 @@
 
 @make_hashable.register
 def _(x: str):
     return x
 
 
 @make_hashable.register
-def _(x: collections.abc.Mapping) -> Tuple:
+def _(x: collections.abc.Mapping) -> tuple:
     return tuple((k, make_hashable(v)) for k, v in x.items())
 
 
 @make_hashable.register
-def _(x: collections.abc.Iterable) -> Tuple:
+def _(x: collections.abc.Iterable) -> tuple:
     return tuple(map(make_hashable, x))
 
 
 def compute_hash(*items) -> int:
     """Compute hash for a sequence of potentially formally not hashable objects.
 
     Note:
@@ -233,9 +232,8 @@
     return result
 
 
 def prettify_float(x: float, fmt: str = "{:.13g}") -> str:
     """Format float in uniform way."""
     if x.is_integer():
         return str(int(x))
-    else:
-        return fmt.format(x)
+    return fmt.format(x)
```

### Comparing `mckit-0.6.23/src/mckit/utils/tolerance.py` & `mckit-0.6.24/src/mckit/utils/tolerance.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Code to estimate "closeness" of various objects."""
+from __future__ import annotations
+
 from typing import Callable, Iterable, Optional, Union
 
 import itertools
 import math
 
 from abc import ABC, abstractmethod
 
@@ -13,15 +15,15 @@
 from mckit.constants import FLOAT_TOLERANCE
 
 
 class MaybeClose(ABC):
     """Interface to be implemented by objects supporting the "closeness" estimation."""
 
     @abstractmethod
-    def is_close_to(self, other: object, estimator: "EstimatorType") -> bool:
+    def is_close_to(self, other: object, estimator: EstimatorType) -> bool:
         """Objects can be estimated as close with some estimator."""
 
 
 ComparableType = Optional[Union[Iterable, ndarray, float, int, MaybeClose]]
 EstimatorType = Callable[[ComparableType, ComparableType], bool]
 
 
@@ -39,24 +41,23 @@
     Returns:
         EstimatorType: estimator
     """
 
     def _estimate(a: ComparableType, b: ComparableType) -> bool:
         if isinstance(a, float) and isinstance(b, float):
             return math.isclose(a, b, rel_tol=rtol, abs_tol=atol)
-        elif isinstance(a, ndarray) and isinstance(b, ndarray):
+        if isinstance(a, ndarray) and isinstance(b, ndarray):
             return np.allclose(a, b, rtol, atol, equal_nan)
-        elif issubclass(type(a), Iterable) and issubclass(type(b), Iterable):
+        if issubclass(type(a), Iterable) and issubclass(type(b), Iterable):
             return all(_call(ai, bi) for ai, bi in itertools.zip_longest(a, b))
-        elif isinstance(a, int) and isinstance(b, int):
+        if isinstance(a, int) and isinstance(b, int):
             return a == b
-        elif isinstance(a, MaybeClose) and isinstance(b, MaybeClose):
+        if isinstance(a, MaybeClose) and isinstance(b, MaybeClose):
             return a.is_close_to(b, _call)
-        else:
-            raise TypeError(f"Not implemented for {type(a).__name__} and {type(b).__name__}")
+        raise TypeError(f"Not implemented for {type(a).__name__} and {type(b).__name__}")
 
     def _call(a: ComparableType, b: ComparableType) -> bool:
         if a is b:
             return True
         if a is None:
             return False  # `a` is None, but `b` is not None here
         if b is None:
```

### Comparing `mckit-0.6.23/src/mckit/version.py` & `mckit-0.6.24/src/mckit/version.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Provide package version and other meta information."""
+from __future__ import annotations
+
 try:
     import importlib_metadata as meta
 except ImportError:
     import importlib.metadata as meta  # type: ignore
 
 __title__ = "mckit"
 __distribution__ = meta.distribution(__title__)
```

### Comparing `mckit-0.6.23/tests/cli/data/brick1-x+10-rot-z45.mcnp` & `mckit-0.6.24/tests/cli/data/brick1-x+10-rot-z45.mcnp`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/cli/data/cubes_with_fill_named_transforms.mcnp` & `mckit-0.6.24/tests/cli/data/cubes_with_fill_named_transforms.mcnp`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/cli/data/cubes_with_fill_transforms.mcnp` & `mckit-0.6.24/tests/cli/data/cubes_with_fill_transforms.mcnp`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/cli/data/shared_surface.mcnp` & `mckit-0.6.24/tests/cli/data/shared_surface.mcnp`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/cli/data/simple_cubes.mcnp` & `mckit-0.6.24/tests/cli/data/simple_cubes.mcnp`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/cli/data/simple_cubes_with_tallies.mcnp` & `mckit-0.6.24/tests/cli/data/simple_cubes_with_tallies.mcnp`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/cli/data/two_cubes_with_the_same_filler.mcnp` & `mckit-0.6.24/tests/cli/data/two_cubes_with_the_same_filler.mcnp`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/cli/test_check.py` & `mckit-0.6.24/tests/cli/test_check.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+from __future__ import annotations
+
 import pytest
 
 from mckit.cli.runner import mckit
 from mckit.utils.resource import path_resolver
 
 data_path_resolver = path_resolver("tests")
-data_filename_resolver = lambda x: str(data_path_resolver(x))
+
+
+def data_filename_resolver(x):
+    return str(data_path_resolver(x))
 
 
 def test_when_there_is_no_args(runner):
     with runner.isolated_filesystem():
         result = runner.invoke(mckit, args=["check"], catch_exceptions=False)
         assert result.exit_code != 0, "Should fail when no arguments provided"
         assert "Usage:" in result.output
```

### Comparing `mckit-0.6.23/tests/cli/test_compose.py` & `mckit-0.6.24/tests/cli/test_compose.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,23 @@
+from __future__ import annotations
+
 from pathlib import Path
 
 import pytest
 
 from mckit.cli.runner import mckit
 from mckit.parser import from_file
 from mckit.universe import collect_transformations
 from mckit.utils.resource import path_resolver
 
 data_path_resolver = path_resolver("tests.cli")
-data_filename_resolver = lambda x: str(data_path_resolver(x))
+
+
+def data_filename_resolver(x):
+    return str(data_path_resolver(x))
 
 
 def test_help_compose(runner):
     result = runner.invoke(mckit, args=["compose", "--help"], catch_exceptions=False)
     assert result.exit_code == 0, result.output
     assert "Usage: mckit compose" in result.output
```

### Comparing `mckit-0.6.23/tests/cli/test_concat.py` & `mckit-0.6.24/tests/cli/test_concat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-# -*- coding: utf-8 -*-
+from __future__ import annotations
+
 from pathlib import Path
 
 from mckit.cli.runner import mckit
 from mckit.utils.resource import path_resolver
 
 data_path_resolver = path_resolver("tests.cli")
-data_filename_resolver = lambda x: str(data_path_resolver(x))
+
+
+def data_filename_resolver(x):
+    return str(data_path_resolver(x))
 
 
 def test_when_there_is_no_args(runner):
     with runner.isolated_filesystem():
         result = runner.invoke(mckit, args=["concat"], catch_exceptions=False)
         assert result.exit_code != 0, "Should fail when no arguments provided"
         assert "Usage:" in result.output
```

### Comparing `mckit-0.6.23/tests/cli/test_decompose.py` & `mckit-0.6.24/tests/cli/test_decompose.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import sys
 
 from pathlib import Path
 
 import numpy as np
 
 import pytest
@@ -15,15 +17,18 @@
 
 from mckit.cli.commands.decompose import get_default_output_directory
 from mckit.cli.runner import mckit
 from mckit.parser import from_file
 from mckit.utils.resource import path_resolver
 
 data_path_resolver = path_resolver("tests")
-data_filename_resolver = lambda x: str(data_path_resolver(x))
+
+
+def data_filename_resolver(x):
+    return str(data_path_resolver(x))
 
 
 @pytest.mark.parametrize(
     "path, expected_cells",
     [
         ("cli/data/simple_cubes.mcnp", 3),
         ("cli/data/simple_cubes.universes/envelopes.i", 3),
```

### Comparing `mckit-0.6.23/tests/cli/test_runner.py` & `mckit-0.6.24/tests/cli/test_runner.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from io import StringIO
 
 import pytest
 
 from mckit.cli.logging import logger
 from mckit.cli.runner import VERSION, mckit, meta
```

### Comparing `mckit-0.6.23/tests/cli/test_split.py` & `mckit-0.6.24/tests/cli/test_split.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
+from __future__ import annotations
+
 from pathlib import Path
 
 import pytest
 
-from click.testing import CliRunner
 from mckit.cli.commands.common import get_default_output_directory
 from mckit.cli.runner import mckit
 from mckit.parser.mcnp_section_parser import is_comment
 from mckit.utils.io import MCNP_ENCODING
 from mckit.utils.resource import path_resolver
 
-
-@pytest.fixture
-def runner():
-    return CliRunner()
+data_path_resolver = path_resolver("tests")
 
 
-data_path_resolver = path_resolver("tests")
-data_filename_resolver = lambda x: str(data_path_resolver(x))
+def data_filename_resolver(x):
+    return str(data_path_resolver(x))
 
 
 def test_when_there_is_no_args(runner):
     with runner.isolated_filesystem():
         result = runner.invoke(mckit, args=["split"], catch_exceptions=False)
         assert result.exit_code != 0, "Should fail when no arguments provided"
         assert "Usage:" in result.output
```

### Comparing `mckit-0.6.23/tests/cli/test_transform.py` & `mckit-0.6.24/tests/cli/test_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,22 @@
+from __future__ import annotations
+
 from pathlib import Path
 
 import pytest
 
 from mckit.cli.runner import mckit
 from mckit.parser import from_file
 from mckit.utils.resource import path_resolver
 
 data_path_resolver = path_resolver("tests.cli")
-data_filename_resolver = lambda x: str(data_path_resolver(x))
+
+
+def data_filename_resolver(x):
+    return str(data_path_resolver(x))
 
 
 def test_when_there_is_no_args(runner):
     with runner.isolated_filesystem():
         result = runner.invoke(mckit, args=["transform"], catch_exceptions=False)
         assert result.exit_code != 0, "Should fail when no arguments provided"
         assert "Usage:" in result.output
```

### Comparing `mckit-0.6.23/tests/model_test_data/geometry_replace.py` & `mckit-0.6.24/tests/model_test_data/geometry_replace.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # This is not real surface objects. They need only to test function.
 # String object utilizing here is acceptable.
+from __future__ import annotations
+
 surf_obj = {
     1: "S1",
     2: "S2",
     3: "S3",
     4: "S4",
     5: "S5",
     6: "S6",
```

### Comparing `mckit-0.6.23/tests/model_test_data/material_creation.py` & `mckit-0.6.24/tests/model_test_data/material_creation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from mckit.material import Material
 
 # for testing _get_material function purposes
 materials = [
     Material(atomic=[(1000, 2), (8000, 1)], density=0.9982),
     Material(atomic=[(1000, 2), (8000, 1)], density=0.1),
 ]
```

### Comparing `mckit-0.6.23/tests/model_test_data/model1.txt` & `mckit-0.6.24/tests/model_test_data/model1.txt`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/model_test_data/model1_ans.txt` & `mckit-0.6.24/tests/model_test_data/model1_ans.txt`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/model_test_data/model_data.py` & `mckit-0.6.24/tests/model_test_data/model_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 case_names = ["model1"]
 
 
 get_universe_dependencies_ans = {"model1": {0: {2, 3}, 1: set(), 2: {1}, 3: {4}, 4: {1}}}
 
 get_contained_cells_ans = {
     "model1": {
```

### Comparing `mckit-0.6.23/tests/parser/common/test_common.py` & `mckit-0.6.24/tests/parser/common/test_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# -*- coding: utf-8 -*-
+from __future__ import annotations
+
 import re
 
 import mckit.parser.common.utils as m
 import pytest
 
 
 @pytest.mark.parametrize(
```

### Comparing `mckit-0.6.23/tests/parser/common/test_common_lexer.py` & `mckit-0.6.24/tests/parser/common/test_common_lexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from __future__ import annotations
+
 import re
 
 import mckit.parser.common as cmn
 import pytest
 import sly
 
-from mckit.parser.common.Lexer import Lexer as LexerBase
-from mckit.parser.common.Lexer import LexError
+from mckit.parser.common.lexer import Lexer as LexerBase
+from mckit.parser.common.lexer import LexError
 
 
 # noinspection PyUnboundLocalVariable,PyPep8Naming,PyUnresolvedReferences
 class DerivedLexer(LexerBase):
     tokens = {FRACTION, FLOAT, INTEGER, ZERO}
 
     FRACTION = r"\d+(?:\.\d+[a-z])"
@@ -32,17 +34,17 @@
         ("3.14 3.14c", ["FLOAT", "FRACTION"], [3.14, "3.14c"]),
         ("1 0 1e-4", ["INTEGER", "ZERO", "FLOAT"], [1, 0, 1e-4]),
     ],
 )
 def test_derived_lexer(text, expected_types, expected_values):
     lexer = DerivedLexer()
     tokens = list(lexer.tokenize(text))
-    result = list(t.type for t in tokens)
+    result = [t.type for t in tokens]
     assert result == expected_types
-    result = list(t.value for t in tokens)
+    result = [t.value for t in tokens]
     assert result == expected_values
 
 
 @pytest.mark.parametrize(
     "text, msg_contains",
     [
         ("1~ 0 3.14", "column 2"),
@@ -51,16 +53,15 @@
         ("\n1 0 3.14 0~", r"\s{10}\^"),
         ("~", "column 1\n~\n\\^"),
     ],
 )
 def test_bad_path(text, msg_contains):
     lexer = DerivedLexer()
     with pytest.raises(LexError, match=msg_contains):
-        for _ in lexer.tokenize(text):
-            pass
+        _ = list(lexer.tokenize(text))
 
 
 # noinspection PyUnboundLocalVariable,PyPep8Naming,PyUnresolvedReferences
 class MyLexer(LexerBase):
     literals = {":", "(", ")"}
     ignore = " \t"
     reflags = re.IGNORECASE | re.MULTILINE
@@ -86,17 +87,17 @@
         ("AAA 1 0 3.14", ["NAME", "INTEGER", "ZERO", "FLOAT"], ["AAA", 1, 0, 3.14]),
         ("1B 1 0 3.14", ["NAME", "INTEGER", "ZERO", "FLOAT"], ["1B", 1, 0, 3.14]),
     ],
 )
 def test_good_path(text, expected_types, expected_values):
     lexer = MyLexer()
     tokens = list(lexer.tokenize(text))
-    result = list(t.type for t in tokens)
+    result = [t.type for t in tokens]
     assert result == expected_types
-    result = list(t.value for t in tokens)
+    result = [t.value for t in tokens]
     assert result == expected_values
 
 
 # noinspection PyUnresolvedReferences
 class MyParser(sly.Parser):
     tokens = MyLexer.tokens
```

### Comparing `mckit-0.6.23/tests/parser/data/parser2.txt` & `mckit-0.6.24/tests/parser/data/parser2.txt`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/parser/test_cell_parser.py` & `mckit-0.6.24/tests/parser/test_cell_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Set output for parser debugging before importing Parser classes.
 # from sly import Parser as SlyParser
 # SlyParser.debugfile = "sly-debug.out"
-from typing import List, Optional
+from __future__ import annotations
 
 import mckit.parser.cell_parser as clp
 import pytest
 
 from mckit.body import Body
 from mckit.material import Material
 from mckit.parser.common import (
@@ -20,21 +20,21 @@
 )
 from mckit.transformation import Transformation
 from mckit.utils.indexes import Index
 
 
 def create_cell(
     cell_no: int,
-    geometry: List,
-    material: Optional[Material] = None,
-    transformation: Optional[Transformation] = None,
+    geometry: list,
+    material: Material | None = None,
+    transformation: Transformation | None = None,
     **options,
 ):
     if not options:
-        options = dict()
+        options = {}
     options["name"] = cell_no
 
     def convert_integers_to_surfaces(_geometry):
         for i, e in enumerate(_geometry):
             if isinstance(e, int):
                 _geometry[i] = DummySurface(e)
             elif isinstance(e, list):
@@ -56,16 +56,16 @@
         ("1 0", ["INTEGER", "ZERO"], [1, 0]),
         ("1 1 -0.083", ["INTEGER", "INTEGER", "FLOAT"], [1, 1, -0.083]),
     ],
 )
 def test_cell_lexer(text, expected_types, expected_values):
     lexer = clp.Lexer()
     tokens = list(lexer.tokenize(text))
-    actual_types = list(f.type for f in tokens)
-    actual_values = list(f.value for f in tokens)
+    actual_types = [f.type for f in tokens]
+    actual_values = [f.value for f in tokens]
     assert actual_types == expected_types
     assert actual_values == expected_values
 
 
 @pytest.mark.parametrize(
     "text,expected,surfaces",
     [
@@ -113,34 +113,34 @@
     expected.options["original"] = text
     assert actual == expected
 
 
 @pytest.mark.parametrize(
     "text,expected,surfaces",
     [
-        ("1 0 1 IMP:n=1.0", create_cell(1, [1], **{"IMPN": 1.0}), [1]),
-        ("1 0 1 vol 1.0", create_cell(1, [1], **{"VOL": 1.0}), [1]),
-        ("1 0 1 U=200 PMT=0", create_cell(1, [1], **{"U": 200, "PMT": 0}), [1]),
+        ("1 0 1 IMP:n=1.0", create_cell(1, [1], IMPN=1.0), [1]),
+        ("1 0 1 vol 1.0", create_cell(1, [1], VOL=1.0), [1]),
+        ("1 0 1 U=200 PMT=0", create_cell(1, [1], U=200, PMT=0), [1]),
     ],
 )
 def test_parser_with_attributes(text, expected, surfaces):
     surfaces_index = create_dummy_surface_index(surfaces)
     actual = clp.parse(text, surfaces=surfaces_index)
     expected.options["original"] = text
     assert actual == expected
 
 
 @pytest.mark.parametrize(
     "text,expected,surfaces,cells",
     [
         (
             "2 like 1 but imp:p=2.0",
-            create_cell(2, [1], **{"IMPN": 1.0, "IMPP": 2.0}),
+            create_cell(2, [1], IMPN=1.0, IMPP=2.0),
             [1],
-            [create_cell(1, [1], **{"IMPN": 1.0})],
+            [create_cell(1, [1], IMPN=1.0)],
         )
     ],
 )
 def test_parser_with_like_spec(text, expected, surfaces, cells):
     surfaces_index = create_dummy_surface_index(surfaces)
     cells_index = CellStrictIndex.from_iterable(cells)
     actual = clp.parse(text, cells=cells_index, surfaces=surfaces_index)
@@ -168,17 +168,17 @@
     surfaces_index = SurfaceDummyIndex()
     cells_index = CellDummyIndex()
     actual = clp.parse(text, cells=cells_index, surfaces=surfaces_index)
     assert actual is not None
     assert actual.name() == expected
 
 
-def create_dummy_surface_index(surfaces: List[int]) -> Index:
+def create_dummy_surface_index(surfaces: list[int]) -> Index:
     return SurfaceStrictIndex.from_iterable(map(DummySurface, surfaces))
 
 
-def create_dummy_composition_index(compositions: List[int]) -> Index:
+def create_dummy_composition_index(compositions: list[int]) -> Index:
     return CompositionStrictIndex.from_iterable(map(DummyComposition, compositions))
 
 
 if __name__ == "__main__":
     pytest.main()
```

### Comparing `mckit-0.6.23/tests/parser/test_material_parser.py` & `mckit-0.6.24/tests/parser/test_material_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# -*- coding: utf-8 -*-
+from __future__ import annotations
 
 import mckit.parser.material_parser as mp
 import pytest
 
 from mckit.material import Composition, Element
 
 
@@ -18,17 +18,17 @@
         ),
         ("M17    18000.70c 1.", ["NAME", "FRACTION"], [17, (18000, "70c", 1.0)]),
     ],
 )
 def test_composition_lexer(text, expected_types, expected_values):
     lexer = mp.Lexer()
     tokens = list(lexer.tokenize(text))
-    result = list(t.type for t in tokens)
+    result = [t.type for t in tokens]
     assert result == expected_types
-    result = list(t.value for t in tokens)
+    result = [t.value for t in tokens]
     assert result == expected_values
 
 
 # M17    18000.70c 1. $Ar 00 weight(%)  100
 
 
 @pytest.mark.parametrize(
```

### Comparing `mckit-0.6.23/tests/parser/test_mcnp_section_parser.py` & `mckit-0.6.24/tests/parser/test_mcnp_section_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from __future__ import annotations
 
 from io import StringIO
 
 import mckit.parser.mcnp_section_parser as sp
 import pytest
 
 from mckit.parser.mcnp_section_parser import Card, Kind
@@ -12,15 +12,15 @@
     "text,expected",
     [
         ("aaa\n\nbbb", ["aaa", "bbb"]),
         ("aaa\n   \nbbb", ["aaa", "bbb"]),
         ("aaa\nbbb", ["aaa\nbbb"]),
     ],
 )
-def test_blank_line_pattern(text: str, expected: List[str]) -> None:
+def test_blank_line_pattern(text: str, expected: list[str]) -> None:
     actual = sp.BLANK_LINE_PATTERN.split(text)
     assert actual == expected
 
 
 @pytest.mark.parametrize(
     "text,expected",
     [
```

### Comparing `mckit-0.6.23/tests/parser/test_mcnp_sly_parser.py` & `mckit-0.6.24/tests/parser/test_mcnp_sly_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from typing import List, NamedTuple
+from __future__ import annotations
+
+from typing import NamedTuple
 
 import pytest
 
 from mckit.parser.mcnp_input_sly_parser import ParseResult, from_file, from_text
 from mckit.utils import path_resolver
 
 file_resolver = path_resolver("tests.parser")
 
 
 class TExpected(NamedTuple):
     title: str
-    cells: List[int]
-    surfaces: List[int]
+    cells: list[int]
+    surfaces: list[int]
 
 
 @pytest.mark.parametrize(
     "text, expected",
     [
         (
             """test 1
@@ -27,19 +29,19 @@
             TExpected("test 1", [1, 2], [1]),
         )
     ],
 )
 def test_parser_basic_functionality(text: str, expected: TExpected):
     result: ParseResult = from_text(text)
     assert expected.title == result.title
-    actual_cells = list(c.name() for c in result.cells)
+    actual_cells = [c.name() for c in result.cells]
     assert expected.cells == actual_cells
-    actual_cells = list(c.name() for c in result.universe.cells)
+    actual_cells = [c.name() for c in result.universe.cells]
     assert expected.cells == actual_cells
-    actual_surfaces = list(s.name() for s in result.surfaces)
+    actual_surfaces = [s.name() for s in result.surfaces]
     assert expected.surfaces == actual_surfaces
 
 
 # noinspection DuplicatedCode
 @pytest.mark.parametrize(
     "parse_file, expected",
     [
```

### Comparing `mckit-0.6.23/tests/parser/test_meshtal_parser.py` & `mckit-0.6.24/tests/parser/test_meshtal_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import numpy as np
 
 import pytest
 
 from mckit.parser.meshtal_parser import meshtal_lexer, meshtal_parser
 from mckit.utils import path_resolver
```

### Comparing `mckit-0.6.23/tests/parser/test_surface_parser.py` & `mckit-0.6.24/tests/parser/test_surface_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import mckit.parser.common.transformation_index as ti
 import mckit.parser.surface_parser as srp
 import pytest
 
 from mckit.surface import create_surface
 from mckit.utils.indexes import IgnoringIndex
```

### Comparing `mckit-0.6.23/tests/parser/test_transformation_parser.py` & `mckit-0.6.24/tests/parser/test_transformation_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import mckit.parser.transformation_parser as trp
 import pytest
 
 from mckit.transformation import Transformation
 
 
 @pytest.mark.parametrize(
@@ -17,15 +19,15 @@
             ["NAME", "INTEGER", "INTEGER", "FLOAT"],
             [(1, True), 0, 0, 1.0],
         ),
     ],
 )
 def test_transformation_lexer(text, expected_types, expected_values):
     lexer = trp.Lexer()
-    tokens = [t for t in lexer.tokenize(text)]
+    tokens = list(lexer.tokenize(text))
     actual_types = [t.type for t in tokens]
     assert actual_types == expected_types
     actual_values = [t.value for t in tokens]
     assert actual_values == expected_values
 
 
 # noinspection PyTypeChecker
```

### Comparing `mckit-0.6.23/tests/parser_test_data/d1s_mesh.m` & `mckit-0.6.24/tests/parser_test_data/d1s_mesh.m`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/parser_test_data/fmesh.m` & `mckit-0.6.24/tests/parser_test_data/fmesh.m`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/parser_test_data/fmesh2.m` & `mckit-0.6.24/tests/parser_test_data/fmesh2.m`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/parser_test_data/fmesh3.m` & `mckit-0.6.24/tests/parser_test_data/fmesh3.m`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/parser_test_data/mctal.t` & `mckit-0.6.24/tests/parser_test_data/mctal.t`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/parser_test_data/parser2.txt` & `mckit-0.6.24/tests/parser_test_data/parser2.txt`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/test_body.py` & `mckit-0.6.24/tests/test_body.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import typing as tp
+from __future__ import annotations
 
 import numpy as np
 
 import pytest
 
 from mckit.body import Body, Shape
 from mckit.box import Box
@@ -35,18 +35,18 @@
     return surfs
 
 
 def create_node(kind, args, surfs):
     new_args = []
     for g in args:
         if isinstance(g, tuple):
-            g = create_node(g[0], g[1], surfs)
+            _g = create_node(g[0], g[1], surfs)
         else:
-            g = surfs[g]
-        new_args.append(g)
+            _g = surfs[g]
+        new_args.append(_g)
     return Shape(kind, *new_args)
 
 
 basic_geoms = [
     ("U", [("I", [("C", [2]), ("S", [3]), ("S", [1]), ("C", [5])]), ("C", [4])]),
     ("I", [("C", [6]), ("C", [1])]),
     ("U", [("C", [6]), ("C", [1])]),
@@ -98,27 +98,25 @@
     ("U", [("I", [("C", [2]), ("S", [11])]), ("I", [("C", [2]), ("S", [12])])]),
     ("I", [("C", [13]), ("C", [12])]),
 ]
 
 
 @pytest.fixture(scope="class")
 def geometry(surfaces):
-    geoms = [create_node(g[0], g[1], surfaces) for g in basic_geoms]
-    return geoms
+    return [create_node(g[0], g[1], surfaces) for g in basic_geoms]
 
 
 class TestShape:
     @staticmethod
     def filter_arg(arg, surfs):
         if isinstance(arg, int):
             return surfs[arg]
-        elif isinstance(arg, tuple):
+        if isinstance(arg, tuple):
             return create_node(arg[0], arg[1], surfs)
-        else:
-            return arg
+        return arg
 
     @pytest.mark.parametrize(
         "opc, args, ans_opc, ans_args",
         [
             ("S", [1], "S", [1]),
             ("C", [1], "C", [1]),
             ("E", [], "E", []),
@@ -190,15 +188,15 @@
             ("C", [("C", [1]), ("S", [2])]),
             ("I", []),
             ("U", []),
         ],
     )
     def test_create_failure(self, surfaces, opc, args):
         args = [self.filter_arg(a, surfaces) for a in args]
-        with pytest.raises(ValueError):
+        with pytest.raises(ValueError, match="expected"):
             Shape(opc, *args)
 
     polish_cases = [
         [2, "C", 3, "I", 1, "I", ("C", [5]), "I", 4, "C", "U"],
         [6, "C", 1, "C", "I"],
         [6, "C", 1, "C", "U"],
         [
@@ -1904,27 +1902,26 @@
         [[1.25, 1.75, 1.5], 2.5, 3.5, 3],
         [[-3.25, -1.5, 1.5], 2.5, 3, 3],
         [[5.5, -0.75, 0.75], 2, 1.5, 1.5],
     ]
 
     @pytest.fixture(scope="class")
     def box(self):
-        boxes = [Box(*b) for b in self.box_data]
-        return boxes
+        return [Box(*b) for b in self.box_data]
 
     @pytest.mark.parametrize("box_no", range(len(box_data)))
     @pytest.mark.parametrize(
         "case_no, expected",
         enumerate([(0, 0, -1), (-1, -1, 0), (0, -1, 0), (0, 0, -1), (0, 0, 0), (0, 0, 0)]),
     )
-    def test_box(self, geometry, box, box_no: int, case_no: int, expected: tp.Tuple[int]):
+    def test_box(self, geometry, box, box_no: int, case_no: int, expected: tuple[int]):
         result = geometry[case_no].test_box(box[box_no])
         assert result == expected[box_no]
 
-    @pytest.mark.slow
+    @pytest.mark.slow()
     @pytest.mark.parametrize("tol", [0.2, None])
     @pytest.mark.parametrize(
         "case_no, expected",
         enumerate(
             [
                 [[-4, 4], [-2, 2], [-2, 2]],
                 [[3, 5], [-1, 1], [-1, 1]],
@@ -1948,15 +1945,15 @@
         for j, (low, high) in enumerate(expected):
             bbd_halves_of_dimensions = 0.5 * bb.dimensions[j]
             assert bb.center[j] - bbd_halves_of_dimensions <= low
             assert bb.center[j] - bbd_halves_of_dimensions >= low - tol
             assert bb.center[j] + bbd_halves_of_dimensions >= high
             assert bb.center[j] + bbd_halves_of_dimensions <= high + tol
 
-    @pytest.mark.slow
+    @pytest.mark.slow()
     @pytest.mark.parametrize("box_no", range(len(box_data)))
     @pytest.mark.parametrize(
         "case_no, expected",
         enumerate(
             [
                 [7.4940, 3.6652, 0],
                 [0, 0, 0.1636],
@@ -1987,15 +1984,15 @@
                 [1, 6],
                 [2, 11, 12],
                 [13, 12],
             ]
         ),
     )
     def test_get_surface(self, geometry, surfaces, case_no, expected):
-        expected = set(surfaces[s] for s in expected)
+        expected = {surfaces[s] for s in expected}
         surfs = geometry[case_no].get_surfaces()
         assert surfs == expected
 
     @pytest.mark.parametrize("case_no, polish", enumerate(polish_cases))
     def test_pickle(self, surfaces, case_no, polish):
         polish = [self.filter_arg(a, surfaces) for a in polish]
         g = Shape.from_polish_notation(polish)
@@ -2096,15 +2093,15 @@
         body1 = Body(geometry[no1], **kwargs)
         body2 = Body(geometry[no2], name="1001")
         body = body1.union(body2)
         assert body.shape == body1.shape.union(body2.shape)
         for k, v in kwargs.items():
             assert body.options[k] == v
 
-    @pytest.mark.slow
+    @pytest.mark.slow()
     @pytest.mark.parametrize("kwarg", kwarg_data)
     @pytest.mark.parametrize(
         "case_no, expected",
         [
             (0, [2, "C", 3, "I", 1, "I", 5, "C", "I", 4, "C", "U"]),
             (1, [6, "C"]),
             (2, [1, "C"]),
@@ -2148,15 +2145,15 @@
         7: create_surface("PX", 1, name=7),
         8: create_surface("PX", 1.2, name=8),
         9: create_surface("PX", 3, name=9),
         10: create_surface("CX", 10, name=10),
         11: create_surface("CX", 1, name=11),
     }
 
-    @pytest.mark.slow
+    @pytest.mark.slow()
     @pytest.mark.parametrize("kwarg", kwarg_data)
     @pytest.mark.parametrize(
         "case_no, geometry, ans_geometry",
         [
             (0, [1, "C", 2, "C", "U"], [[1, "C"], [2, "C"]]),
             (1, [1, "C", 3, "C", "U"], [[1, "C", 3, "C", "U"]]),
             (2, [1, "C"], [[1, "C"]]),
@@ -2198,15 +2195,15 @@
             expected.add(
                 Shape.from_polish_notation(
                     [TestShape.filter_arg(a, self.split_surfaces) for a in ans]
                 )
             )
         gb = Box([0, 0, 0], 100, 100, 100)
         split_bodies = body.split(min_volume=0.001, box=gb)
-        print(body.shape.get_stat_table())
+        body.shape.get_stat_table()
         assert len(split_bodies) == len(expected)
         split_shapes = {b.shape for b in split_bodies}
         assert split_shapes == expected
         for b in split_bodies:
             for k, v in kwarg.items():
                 assert b.options[k] == v
             assert b.material() == kwarg.get("MAT", None)
@@ -2281,14 +2278,14 @@
             points2 = new_body.options["FILL"]["transform"].apply2point(points)
         else:
             points2 = tr.apply2point(points)
         new_results = new_body.shape.test_points(points2)
         # TODO: Check testing of FILL without 'transform' case
         np.testing.assert_array_equal(results, new_results)
 
-    @pytest.mark.skip
+    @pytest.mark.skip()
     def test_print(self):
         raise NotImplementedError
 
-    @pytest.mark.skip
+    @pytest.mark.skip()
     def test_fill(self):
         raise NotImplementedError
```

### Comparing `mckit-0.6.23/tests/test_box.py` & `mckit-0.6.24/tests/test_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import io
 import pickle
 
 import numpy as np
 
 import pytest
 
@@ -9,16 +11,15 @@
 
 # noinspection PyUnresolvedReferences,PyPackageRequirements
 from mckit.geometry import EX, EY, EZ
 
 
 @pytest.fixture(scope="module")
 def box():
-    boxes = [Box([0.5, 1, 1.5], 1, 2, 3), Box([0.5, -1, 1.5], 3, 2, 1)]
-    return boxes
+    return [Box([0.5, 1, 1.5], 1, 2, 3), Box([0.5, -1, 1.5], 3, 2, 1)]
 
 
 @pytest.mark.parametrize(
     "point_no, point",
     enumerate(
         [
             [0.1, 0.1, 0.1],
@@ -469,15 +470,16 @@
     assert vol == expected
 
 
 @pytest.mark.parametrize("case_no", range(2))
 def test_random_points(box, case_no):
     points = box[case_no].generate_random_points(100)
     pt = box[case_no].test_points(points)
-    assert np.all(pt) == True
+    if not np.all(pt):
+        pytest.fail(f"Some points are not in the box #{case_no}")
 
 
 boxes = [
     Box([0, 0, 0], 1, 1, 1),
     Box([2, 0, 0], 0.5, 4, 2),
     Box([0, 0, 2], 0.5, 4, 2),
     Box([0, 0, 2], 0.2, 0.2, 10),
@@ -526,9 +528,9 @@
     "center, wx, wy, wz, ex, ey, ez", [([0.0, 0.0, 0.0], 1.0, 2.0, 3.0, EX, EY, EZ)]
 )
 def test_pickle(center, wx, wy, wz, ex, ey, ez):
     box = Box(center, wx, wy, wz, ex, ey, ez)
     with io.BytesIO() as f:
         pickle.dump(box, f)
         f.seek(0)
-        box_unpickled = pickle.load(f)
+        box_unpickled = pickle.load(f)  # noqa: S301
     assert box == box_unpickled
```

### Comparing `mckit-0.6.23/tests/test_card.py` & `mckit-0.6.24/tests/test_card.py`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/test_fmesh.py` & `mckit-0.6.24/tests/test_fmesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from itertools import product
 
 import numpy as np
 
 import pytest
 
 from mckit import read_meshtal
@@ -198,17 +200,14 @@
 
     @pytest.mark.parametrize("mi, ti", product(range(len(bins)), range(len(transforms))))
     def test_get_voxel(self, mi: int, ti: int):
         tr = transforms[ti]
         _bin = bins[mi]
         mesh = create_rmesh(_bin, tr)
         shape = mesh.shape
-        ex = EX
-        ey = EY
-        ez = EZ
         for i, j, k in product(range(shape[0]), range(shape[1]), range(shape[2])):
             vox = mesh.get_voxel(i, j, k)
             corners = []
             for pr in product(
                 _bin["xbins"][i : i + 2],
                 _bin["ybins"][j : j + 2],
                 _bin["zbins"][k : k + 2],
@@ -239,32 +238,31 @@
 
     @pytest.mark.parametrize(
         "mi, ti, pi, local",
         product(range(len(bins)), range(len(transforms)), range(len(points)), [False, True]),
     )
     def test_voxel_index(self, mi: int, ti: int, pi: int, local: bool):
         tr = transforms[ti]
-        bin = bins[mi]
-        mesh = create_rmesh(bin, tr)
+        _bin = bins[mi]
+        mesh = create_rmesh(_bin, tr)
         pt = self.points[pi]
         result = mesh.voxel_index(pt, local=local)
         if local is False and tr is not None:
             pt = tr.reverse().apply2point(pt)
 
         def check_one(r, pt):
             if r is not None:
-                print(r)
                 i, j, k = r
-                assert bin["xbins"][i] <= pt[0] <= bin["xbins"][i + 1]
-                assert bin["ybins"][j] <= pt[1] <= bin["ybins"][j + 1]
-                assert bin["zbins"][k] <= pt[2] <= bin["zbins"][k + 1]
+                assert _bin["xbins"][i] <= pt[0] <= _bin["xbins"][i + 1]
+                assert _bin["ybins"][j] <= pt[1] <= _bin["ybins"][j + 1]
+                assert _bin["zbins"][k] <= pt[2] <= _bin["zbins"][k + 1]
             else:
-                px = pt[0] <= bin["xbins"][0] or pt[0] >= bin["xbins"][-1]
-                py = pt[1] <= bin["ybins"][0] or pt[1] >= bin["ybins"][-1]
-                pz = pt[2] <= bin["zbins"][0] or pt[2] >= bin["zbins"][-1]
+                px = pt[0] <= _bin["xbins"][0] or pt[0] >= _bin["xbins"][-1]
+                py = pt[1] <= _bin["ybins"][0] or pt[1] >= _bin["ybins"][-1]
+                pz = pt[2] <= _bin["zbins"][0] or pt[2] >= _bin["zbins"][-1]
                 assert px or py or pz
 
         if np.array(pt).shape == (3,):
             check_one(result, pt)
         else:
             for r, p in zip(result, pt):
                 check_one(r, p)
@@ -334,33 +332,36 @@
                 {"axis": 2, "index": 0, "x": [-2.0, 0.0], "y": [-1.5, -0.5, 0.5]},
             ),
             (0, {"X": 5}, {"axis": 0, "index": 3, "x": [1.0, 3.5], "y": [0.0, 2.0]}),
         ],
     )
     def test_slice_index(self, ti: int, mi: int, args, expected):
         tr = transforms[ti]
-        bin = bins[mi]
-        mesh = create_rmesh(bin, tr)
+        _bin = bins[mi]
+        mesh = create_rmesh(_bin, tr)
         if expected is None:
-            with pytest.raises(ValueError):
+            with pytest.raises(
+                ValueError,
+                match="Wrong number of fixed spatial variables|Specified point lies outside of the mesh",
+            ):
                 mesh.slice_axis_index(**args)
         else:
             axis, index, x, y = mesh.slice_axis_index(**args)
             assert axis == expected["axis"]
             assert index == expected["index"]
             np.testing.assert_array_almost_equal(x, expected["x"])
             np.testing.assert_array_almost_equal(y, expected["y"])
 
 
 parser_test_data = path_resolver("tests")
 # dvp: On Linux access to package should be organized with resource name resolver.
 
 
 class TestFMesh:
-    @pytest.fixture
+    @pytest.fixture()
     def tallies(self):
         file_name = parser_test_data("parser_test_data/fmesh.m")
         return read_meshtal(file_name)
 
     @pytest.mark.parametrize(
         "name, particle, histories, meshclass",
         [
@@ -376,15 +377,15 @@
     def test_creation(self, tallies, name, particle, histories, meshclass):
         assert tallies[name]._name == name
         assert tallies[name].particle == particle
         assert tallies[name].histories == histories
         assert tallies[name].mesh.__class__ == meshclass
 
     @pytest.mark.parametrize(
-        "name, E, dir, value, x_ans, y_ans, data_ans, max_err",
+        "name, E, _dir, value, x_ans, y_ans, data_ans, max_err",
         [
             (
                 34,
                 "total",
                 "X",
                 0.5,
                 np.array([-2.0, 0.0, 2.0, 4.0]),
@@ -609,16 +610,16 @@
                         [0.00000000e00, 0.00000000e00, 0.00000000e00, 0.00000000e00],
                     ]
                 ),
                 np.array([[0.0, 0.0, 0.0, 0.0], [0.0, 0.0, 0.0, 1.0], [0.0, 0.0, 0.0, 0.0]]),
             ),
         ],
     )
-    def test_slice(self, tallies, name, E, dir, value, x_ans, y_ans, data_ans, max_err):
-        x, y, data, err = tallies[name].get_slice(E=E, **{dir: value})
+    def test_slice(self, tallies, name, E, _dir, value, x_ans, y_ans, data_ans, max_err):
+        x, y, data, err = tallies[name].get_slice(E=E, **{_dir: value})
         np.testing.assert_array_almost_equal(x, x_ans)
         np.testing.assert_array_almost_equal(y, y_ans)
         np.testing.assert_array_almost_equal(data, data_ans)
         if E == "total":
             assert np.all(err <= max_err)
         else:
             np.testing.assert_array_almost_equal(err, max_err)
@@ -651,15 +652,15 @@
                 np.array([0.04113, 1.00000, 1.00000]),
             ),
             # TODO: Add tests for cylindrical mesh.
         ],
     )
     def test_spectrum(self, tallies, name, point, ebins, flux, err):
         if ebins is None:
-            with pytest.raises(ValueError):
+            with pytest.raises(ValueError, match="lies outside of the mesh"):
                 tallies[name].get_spectrum(point)
         else:
             eb, fl, er = tallies[name].get_spectrum(point)
             assert np.all(eb == ebins)
             assert np.all(fl == flux)
             assert np.all(er == err)
```

### Comparing `mckit-0.6.23/tests/test_material.py` & `mckit-0.6.24/tests/test_material.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Any, Dict
+from __future__ import annotations
+
+from typing import Any
 
 from copy import deepcopy
 
 import pytest
 
 from mckit.material import Composition, Element, Material
 
@@ -609,16 +611,15 @@
     def test_hash_equal(self, compositions, case1: int, case2: int):
         comp1 = compositions[case1]
         comp2 = compositions[case2]
         assert (hash(comp1) == hash(comp2)) == bool(self.hash_eq_matrix[case1][case2])
 
     @pytest.fixture(scope="class")
     def compositions(self):
-        comp = [Composition(**params) for params in self.cases]
-        return comp
+        return [Composition(**params) for params in self.cases]
 
     @pytest.mark.parametrize("case_no", range(len(cases)))
     def test_name(self, case_no: int):
         comp = Composition(**self.cases[case_no])
         assert comp.name() == case_no + 1
 
     @pytest.mark.parametrize(
@@ -680,15 +681,15 @@
         comp2 = Composition(**inp2)
         assert comp2._composition == ans
 
     @pytest.mark.parametrize(
         "_input", [{"atomic": [], "weight": []}, {"atomic": []}, {"weight": []}, {}]
     )
     def test_create_failure(self, _input):
-        with pytest.raises(ValueError):
+        with pytest.raises(ValueError, match="Incorrect set of parameters."):
             Composition(**_input)
 
     @pytest.mark.parametrize(
         "case_no, expected",
         enumerate(
             [
                 1.0079,
@@ -1065,14 +1066,15 @@
     )
     def test_atomic(self, compositions, case_no, expected):
         comp = compositions[case_no]
         for k, v in expected.items():
             if v == 0:
                 with pytest.raises(KeyError):
                     comp.get_atomic(k)
+                with pytest.raises(KeyError):
                     comp.get_atomic(Element(k))
             else:
                 assert comp.get_atomic(k) == pytest.approx(v, rel=1.0e-3)
                 assert comp.get_atomic(Element(k)) == pytest.approx(v, rel=1.0e-3)
 
     @pytest.mark.parametrize(
         "case_no, expected",
@@ -1248,14 +1250,15 @@
     )
     def test_weight(self, compositions, case_no, expected):
         comp = compositions[case_no]
         for k, v in expected.items():
             if v == 0:
                 with pytest.raises(KeyError):
                     comp.get_weight(k)
+                with pytest.raises(KeyError):
                     comp.get_weight(Element(k))
             else:
                 assert comp.get_weight(k) == pytest.approx(v, rel=1.0e-3)
                 assert comp.get_weight(Element(k)) == pytest.approx(v, rel=1.0e-3)
 
     @pytest.mark.parametrize(
         "case_no, expected",
@@ -1444,15 +1447,14 @@
             (10, 11, {"lib": "21c"}),
             (11, 12, {"lib": "21c"}),
             (12, 13, {"lib": "21c"}),
         ],
     )
     def test_get_option(self, compositions, case_no, name, expected_kw):
         comp = compositions[case_no]
-        print(comp.name(), name)
         assert comp.name() == name
         for key, value in expected_kw.items():
             assert comp[key] == value
 
     @pytest.mark.parametrize(
         "mix_components, ans_index",
         [
@@ -1502,16 +1504,15 @@
         {"atomic": [("N", 1)], "density": 1.251e-3},
         {"atomic": [("O", 1)], "density": 1.42897e-3},
         {"atomic": [("Ar", 1)], "density": 1.784e-3},
     ]
 
     @pytest.fixture(scope="class")
     def materials(self):
-        mats = [Material(**c) for c in self.cases]
-        return mats
+        return [Material(**c) for c in self.cases]
 
     @pytest.mark.parametrize(
         "data",
         [
             {},
             {"atomic": [("N", 1)]},
             {"weight": [("N", 1)]},
@@ -1565,33 +1566,33 @@
                 "concentration": 7.8,
                 "composition": {"atomic": [("N", 1)]},
                 "atomic": [("N", 1)],
                 "weight": [("N", 1)],
             },
         ],
     )
-    def test_creation_failure(self, data: Dict[str, Any]):
+    def test_creation_failure(self, data: dict[str, Any]):
         data = deepcopy(data)  # this fixes pytest strange behavior (see below)"
         if "composition" in data.keys():
             composition_params = data.pop("composition")
             assert not isinstance(
                 composition_params, Composition
             ), "Check some strange behavior on 'pytest test/*.py': arriving params are already Composition"
             composition = Composition(**composition_params)
         else:
             composition = None
-        with pytest.raises(ValueError):
+        with pytest.raises(ValueError, match="Incorrect set of parameters."):
             Material(**data, composition=composition)
 
     @pytest.mark.parametrize("case", cases)
     def test_creation(self, case):
         mat1 = Material(**case)
         data = case.copy()
-        atomic = data.pop("atomic", tuple())
-        weight = data.pop("weight", tuple())
+        atomic = data.pop("atomic", ())
+        weight = data.pop("weight", ())
         comp = Composition(atomic=atomic, weight=weight)
         mat2 = Material(composition=comp, **data)
         assert mat1.composition == comp
         assert mat2.composition == comp
         if "density" in data.keys():
             d = pytest.approx(data["density"], rel=1.0e-5)
             assert mat1.density == d
```

### Comparing `mckit-0.6.23/tests/test_mctal_parser.py` & `mckit-0.6.24/tests/test_mctal_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+from __future__ import annotations
+
 import numpy as np
 
 import pytest
 
 from mckit.parser.mctal_parser import read_mctal
 from mckit.utils import path_resolver
 
 data_path_resolver = path_resolver("tests")
-file_resolver = lambda x: str(data_path_resolver(x))
+
+
+def file_resolver(x):
+    return str(data_path_resolver(x))
 
 
 @pytest.mark.parametrize(
     "mctal_file, expected",
     [
         (
             "parser_test_data/mctal.t",
```

### Comparing `mckit-0.6.23/tests/test_printer.py` & `mckit-0.6.24/tests/test_printer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 
 from mckit.printer import pretty_float, print_card, separate
 
 
 @pytest.mark.parametrize(
     "tokens, sep, expected",
```

### Comparing `mckit-0.6.23/tests/test_source.py` & `mckit-0.6.24/tests/test_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pytest
 
 from mckit.source import Distribution, Source, create_bin_distributions
 
 
 class TestDistribution:
     @pytest.mark.parametrize(
@@ -10,15 +12,15 @@
             (1, [1, 2, 3], [1, 2, 3, 4, 5]),
             (2, [1, 2, 3], [1, 2, 3, 4]),
             (3, [1, 2, 3, 4], [1, 2]),
             (4, [1, 2, 3, 4], Distribution(1, [1, 2], [1, 2])),
         ],
     )
     def test_create_failure(self, name, values, probs):
-        with pytest.raises(ValueError):
+        with pytest.raises(ValueError, match="Inconsistent size of values."):
             Distribution(name, values, probs)
 
     @pytest.mark.parametrize(
         "name, values, probs, var",
         [
             (1, [1, 2, 3], [1, 2, 3], "X"),
             (2, [1, 2, 3, 4], [1, 2, 3], "Y"),
```

### Comparing `mckit-0.6.23/tests/test_surface.py` & `mckit-0.6.24/tests/test_surface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import sys
+from __future__ import annotations
 
 import numpy as np
 
 import pytest
 
 from mckit.box import Box
 from mckit.surface import BOX, RCC, Cone, Cylinder, GQuadratic, Plane, Sphere, Torus, create_surface
@@ -1061,16 +1061,14 @@
                 "3 C/Z 1 -2 3",
                 "3 C/Z 1 -2 3",
             ],
         ),
     )
     def test_mcnp_prety_repr(self, surface, answer):
         desc = surface.round().mcnp_repr(True)
-        print(surface.mcnp_repr())
-        print("{0:.15e}".format(surface._pt[0]))
         assert desc == answer
 
     @pytest.mark.parametrize(
         "surface, answer",
         zip(
             surfs,
             [
@@ -1093,16 +1091,14 @@
                 "3 GQ 1 1 0 5e-27 1e-13 -1e-13 -2 4 3e-13 -4",
                 "3 GQ 1 1 0 1.999999999999e-26 -2e-13 2e-13 -2.000000000001 4.000000000001 -6.000000000001e-13 -3.999999999997",
             ],
         ),
     )
     def test_mcnp_repr(self, surface, answer):
         desc = surface.mcnp_repr()
-        print(surface.mcnp_repr())
-        print("{0:.15e}".format(surface._pt[0]))
         if "\n" in desc:
             assert desc.split() == answer.split()
         else:
             assert desc == answer
 
 
 class TestCone:
@@ -3068,16 +3064,14 @@
         [0, 0, 0, 0, 0, 1],
     ]
 
     @pytest.mark.parametrize("i1, s1", enumerate(surfs))
     @pytest.mark.parametrize("i2, s2", enumerate(surfs))
     def test_eq(self, i1, s1, i2, s2):
         result = s1 == s2
-        print(s1.get_params())
-        print(s2.get_params())
         assert result == bool(self.eq_matrix[i1][i2])
 
     @pytest.mark.parametrize("i1, s1", enumerate(surfs))
     @pytest.mark.parametrize("i2, s2", enumerate(surfs))
     def test_hash(self, i1, s1, i2, s2):
         if self.eq_matrix[i1][i2]:
             assert hash(s1) == hash(s2)
@@ -3127,16 +3121,14 @@
         ],
     )
     def test_init(self, transform, center, axis, radius):
         surf = RCC(center, axis, radius, transform=transform)
         c = transform.apply2point(center)
         a = transform.apply2vector(axis)
         ac, axc, rc = surf.get_params()
-        print(c, ac)
-        print(a, axc)
         np.testing.assert_array_almost_equal(c, ac)
         np.testing.assert_array_almost_equal(a, axc)
         np.testing.assert_almost_equal(radius, rc)
 
     @pytest.mark.parametrize(
         "point, expected",
         [
@@ -3164,26 +3156,26 @@
         surf = RCC([1, 0, -1], [0, 0, 2], 3)
         result = surf.test_points(point)
         np.testing.assert_array_equal(result, expected)
 
     @pytest.mark.parametrize(
         "center, axis, rad, ans",
         [
-            pytest.param(
-                [-2, 0, 0],
-                [4, 0, 0],
-                0.5,
-                0,
-                marks=pytest.mark.skipif(
-                    sys.platform == "darwin"
-                    or sys.platform == "linux"
-                    and sys.version_info[0:2] < (3, 9),
-                    reason="Fails on MacOS and Linux with python 3.8",
-                ),
-            ),
+            # pytest.param(
+            #     [-2, 0, 0],
+            #     [4, 0, 0],
+            #     0.5,
+            #     0,
+            #     marks=pytest.mark.skipif(
+            #         sys.platform == "darwin"
+            #         or sys.platform == "linux"
+            #         and sys.version_info[0:2] < (3, 9),
+            #         reason="Fails on MacOS and Linux with python 3.8",
+            #     ),
+            # ),
             ([-2, 0, 0], [4, 0, 0], 3, -1),
             pytest.param(
                 [-0.75, 0, 0],
                 [1.5, 0, 0],
                 0.75,
                 0,
                 marks=pytest.mark.skip(
@@ -3251,16 +3243,14 @@
         [0, 0, 0, 0, 0, 1],
     ]
 
     @pytest.mark.parametrize("i1, s1", enumerate(surfs))
     @pytest.mark.parametrize("i2, s2", enumerate(surfs))
     def test_eq(self, i1, s1, i2, s2):
         result = s1 == s2
-        print(s1.get_params())
-        print(s2.get_params())
         assert result == bool(self.eq_matrix[i1][i2])
 
     @pytest.mark.parametrize("i1, s1", enumerate(surfs))
     @pytest.mark.parametrize("i2, s2", enumerate(surfs))
     def test_hash(self, i1, s1, i2, s2):
         if self.eq_matrix[i1][i2]:
             assert hash(s1) == hash(s2)
```

### Comparing `mckit-0.6.23/tests/test_transformation.py` & `mckit-0.6.24/tests/test_transformation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import numpy as np
 
 import pytest
 
 from mckit.geometry import ORIGIN
 from mckit.transformation import IDENTITY_ROTATION, Transformation
 
@@ -96,15 +98,15 @@
         {
             "rotation": [30, 60, 90, 120, 30, 90, 89.942, 89.942, 0.058],
             "indegrees": True,
         },
     ],
 )
 def test_creation_failure(args):
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="wrong|is greater"):
         Transformation(**args)
 
 
 @pytest.mark.parametrize(
     "args, answer",
     [
         (
@@ -298,18 +300,17 @@
         "translation": [-2, 5, 3],
         "rotation": [30, 90, 60, 90, 0, 90, 120, 90, 30],
         "indegrees": True,
     },
 ]
 
 
-@pytest.fixture(scope="function")
+@pytest.fixture()
 def trtr():
-    tr = [Transformation(**tdata) for tdata in tr_tr_cases]
-    return tr
+    return [Transformation(**tdata) for tdata in tr_tr_cases]
 
 
 @pytest.mark.parametrize("tr1_no", range(len(tr_tr_cases)))
 @pytest.mark.parametrize("tr2_no", range(len(tr_tr_cases)))
 @pytest.mark.parametrize(
     "point",
     [
```

### Comparing `mckit-0.6.23/tests/test_universe.py` & `mckit-0.6.24/tests/test_universe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Dict, List, Set, Union
 
 import tempfile
 import textwrap
 
 from copy import deepcopy
 
@@ -21,15 +23,19 @@
     cell_selector,
     collect_transformations,
     surface_selector,
 )
 from mckit.utils.resource import path_resolver
 
 data_path_resolver = path_resolver("tests")
-data_filename_resolver = lambda x: str(data_path_resolver(x))
+
+
+def data_filename_resolver(x):
+    return str(data_path_resolver(x))
+
 
 TStatItem = Dict[
     int, Union[List[int], Set[Universe]]
 ]  # TODO dvp: cool but isn't this too much freedom?
 TStat = Dict[str, TStatItem]
 
 
@@ -605,15 +611,15 @@
     copy_surfaces_idx = {s.name(): s for s in uc.get_surfaces()}
     assert surfaces_idx == copy_surfaces_idx
     for k, v in surfaces_idx.items():
         assert copy_surfaces_idx[k] is not v
         assert copy_surfaces_idx[k] == v
 
 
-@pytest.mark.slow
+@pytest.mark.slow()
 @pytest.mark.parametrize("tol", [0.2, None])
 @pytest.mark.parametrize("case, expected", [(1, [[-10, 10], [-10, 10], [-6.5, 13.5]])])
 def test_bounding_box(universe, tol, case, expected):
     u = universe(case)
     base = [0, 0, 0]
     dims = [30, 30, 30]
     gb = Box(base, dims[0], dims[1], dims[2])
@@ -701,21 +707,21 @@
         (3, {}, {}),
         (4, {}, {}),
     ],
 )
 def test_name_clashes(
     universe,
     case: int,
-    rename: Dict[int, Dict[str, int]],
+    rename: dict[int, dict[str, int]],
     stat: TStat,
 ):
     rename = deepcopy(rename)
     stat = deepcopy(stat)
     u: Universe = universe(case)
-    universes_index: Dict[int, Universe] = {x.name(): x for x in u.get_universes()}
+    universes_index: dict[int, Universe] = {x.name(): x for x in u.get_universes()}
     for uname, ren_dict in rename.items():
         universes_index[uname].rename(**ren_dict)
     for stat_item in stat.values():
         for kind, universe_names in stat_item.items():
             stat_item[kind] = {universes_index[uname] for uname in universe_names}
     s = u.name_clashes()
     assert s == stat
@@ -785,31 +791,25 @@
             {"material": {10: [1, None], 11: [1, None]}},
         ),
     ],
 )
 def test_name_clashes_with_common_materials(
     universe,
     case: int,
-    common_mat: Set[Composition],
+    common_mat: set[Composition],
     stat: TStat,
 ):
     stat = deepcopy(stat)
     u = universe(case)
     universes_idx = {x.name(): x for x in u.get_universes()}
     u.set_common_materials(common_mat)
     for stat_item in stat.values():
         for kind, universes_names in stat_item.items():
             stat_item[kind] = {universes_idx[uname] if uname else None for uname in universes_names}
     s = u.name_clashes()
-    for c in u._common_materials:
-        print(c.mcnp_repr())
-    for name, un in universes_idx.items():
-        print(name)
-        for c in un.get_compositions():
-            print(c.mcnp_repr())
     assert s == stat
 
 
 @pytest.mark.parametrize(
     "case, common_mat",
     [
         (2, {Composition(atomic=[("6012", 1)], name=1)}),
@@ -853,15 +853,15 @@
             mat = c.material()
             if mat:
                 comp = mat.composition
                 if comp in common_mat:
                     assert comp is cm[comp]
 
 
-@pytest.mark.slow
+@pytest.mark.slow()
 @pytest.mark.parametrize(
     "case, condition, answer_case, box",
     [
         (2, {}, 1002, Box([0, 0, 0], 20, 20, 20)),
         (2, {"cell": 1}, 1012, Box([0, 0, 0], 20, 20, 20)),
         (2, {"cell": 2}, 1022, Box([0, 0, 0], 20, 20, 20)),
         (2, {"universe": 1}, 1022, Box([0, 0, 0], 20, 20, 20)),
@@ -1041,15 +1041,15 @@
 def test_rename_when_common_mat(universe, case, common, start, answer):
     u = Universe(universe(case), common_materials=common)
     u.rename(start_mat=start)
     composition_names = sorted(m.name() for m in u.get_compositions())
     assert composition_names == answer
 
 
-@pytest.mark.slow
+@pytest.mark.slow()
 @pytest.mark.parametrize("verbose", [False, True])
 @pytest.mark.parametrize(
     "case, complexities", [(1, {1: 1, 2: 3, 3: 5, 4: 1}), (3, {1: 1, 2: 3, 4: 5, 5: 1})]
 )
 def test_simplify(universe, case, complexities, verbose):
     u = universe(case)
     u.simplify(min_volume=0.1, verbose=verbose)
@@ -1174,12 +1174,12 @@
             TR2 -1 -1 -1
             TR3  0 1 0
             """,
             [1, 2, 3],
         ),
     ],
 )
-def test_collect_transformations(case: str, expected: List[int]) -> None:
+def test_collect_transformations(case: str, expected: list[int]) -> None:
     case = textwrap.dedent(case)
     u = from_text(case).universe
     actual = sorted(map(int, map(Card.name, collect_transformations(u))))
     assert actual == expected
```

### Comparing `mckit-0.6.23/tests/test_universe_analyser.py` & `mckit-0.6.24/tests/test_universe_analyser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from io import StringIO
 
 from mckit.parser import from_file
 from mckit.universe import UniverseAnalyser
 from mckit.utils import path_resolver
 
 cli_data = path_resolver("tests.cli")
```

### Comparing `mckit-0.6.23/tests/universe1.i` & `mckit-0.6.24/tests/universe1.i`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/universe_test_data/model1.txt` & `mckit-0.6.24/tests/universe_test_data/model1.txt`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/universe_test_data/model2.txt` & `mckit-0.6.24/tests/universe_test_data/model2.txt`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/universe_test_data/model3.txt` & `mckit-0.6.24/tests/universe_test_data/model3.txt`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/universe_test_data/model4.txt` & `mckit-0.6.24/tests/universe_test_data/model4.txt`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/universe_test_data/model5.txt` & `mckit-0.6.24/tests/universe_test_data/model5.txt`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/universe_test_data/model6.txt` & `mckit-0.6.24/tests/universe_test_data/model6.txt`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/universe_test_data/universe1002.i` & `mckit-0.6.24/tests/universe_test_data/universe1002.i`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/universe_test_data/universe1012.i` & `mckit-0.6.24/tests/universe_test_data/universe1012.i`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/universe_test_data/universe1022.i` & `mckit-0.6.24/tests/universe_test_data/universe1022.i`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/universe_test_data/universe2.i` & `mckit-0.6.24/tests/universe_test_data/universe2.i`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/universe_test_data/universe5.i` & `mckit-0.6.24/tests/universe_test_data/universe5.i`

 * *Files identical despite different names*

### Comparing `mckit-0.6.23/tests/universe_test_data/volume_ans.py` & `mckit-0.6.24/tests/universe_test_data/volume_ans.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import numpy as np
 
 case_names = ["model1"]
 
 volume_ans = {
     "model1": {
         ((650, 700), (0, 50), (400, 450)): (
```

### Comparing `mckit-0.6.23/tests/utils/test_accept.py` & `mckit-0.6.24/tests/utils/test_accept.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import Any
 
 from contextlib import contextmanager
 
 from mckit.utils.accept import accept, on_unknown_acceptor
```

### Comparing `mckit-0.6.23/tests/utils/test_index.py` & `mckit-0.6.24/tests/utils/test_index.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# -*- coding: utf-8 -*-
-from typing import Dict, List, NoReturn
+from __future__ import annotations
+
+from typing import NoReturn
 
 import pytest
 
 from mckit.utils.indexes import Index
 
 
 def dummy_strategy(c: int) -> int:
     return c * c
 
 
 @pytest.mark.parametrize("inp", [{1: 1, 2: 4}, {}])
-def test_index_with_dummy_strategy(inp: Dict[int, int]) -> None:
+def test_index_with_dummy_strategy(inp: dict[int, int]) -> None:
     dictionary = Index(dummy_strategy)
     dictionary.update(inp)
     for k in range(5):
         v = dictionary[k]
         expected = k * k
         assert expected == v
 
@@ -35,18 +36,17 @@
 
 
 @pytest.mark.parametrize(
     "inp,keys,success",
     [({1: 1, 2: 4}, [1, 2, 3], [True, True, False]), ({}, [1], [False])],
 )
 def test_index_with_strict_strategy(
-    inp: Dict[int, int], keys: List[int], success: List[bool]
+    inp: dict[int, int], keys: list[int], success: list[bool]
 ) -> None:
     dictionary = Index(strict_strategy)
     dictionary.update(inp)
     for k, s in zip(keys, success):
-        try:
-            _ = dictionary[k]
-            assert s is True
-        except MyKeyError as ex:
-            assert ex.key == k
-            assert s is False
+        if s:
+            assert dictionary[k]
+        else:
+            with pytest.raises(MyKeyError):
+                _ = dictionary[k]
```

### Comparing `mckit-0.6.23/tests/utils/test_index_of_named.py` & `mckit-0.6.24/tests/utils/test_index_of_named.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from typing import NamedTuple
 
 import mckit.utils.named as nm
 import pytest
 
 from mckit.utils.indexes import (
     IndexOfNamed,
@@ -35,18 +37,17 @@
     "entities",
     [
         (list(map(Something, [1, 1]))),
     ],
 )
 def test_clashes(entities):
     with pytest.raises(NumberedItemDuplicateError, match="Something"):
-        actual = IndexOfNamed.from_iterable(
+        IndexOfNamed.from_iterable(
             entities, key=lambda x: x.name, on_duplicate=raise_on_duplicate_strategy
         )
-        assert not actual
 
 
 @pytest.mark.parametrize(
     "entities, expected",
     [
         (list(map(Something, [1, 1])), {1: Something(1)}),
     ],
@@ -67,18 +68,17 @@
     "entities",
     [
         [Something2(1, 1), Something2(1, 2)],
     ],
 )
 def test_clashes_on_non_equal_items(entities):
     with pytest.raises(NumberedItemDuplicateError, match="Something2"):
-        actual = IndexOfNamed.from_iterable(
+        IndexOfNamed.from_iterable(
             entities, key=lambda x: x.name, on_duplicate=raise_on_duplicate_strategy
         )
-        assert not actual
 
 
 @pytest.mark.parametrize(
     "entities, expected, expected_collected",
     [
         ([Something2(1, 1), Something2(1, 2)], {1: Something2(1, 2)}, {1: 2}),
         (
```

### Comparing `mckit-0.6.23/tests/utils/test_io.py` & `mckit-0.6.24/tests/utils/test_io.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from pathlib import Path
 
 import pytest
 
 from mckit.utils.io import check_if_all_paths_exist, check_if_path_exists, make_dirs
 
 TEST_VAR = "TEST_GET_ROOT_DIR_VAR"
```

### Comparing `mckit-0.6.23/tests/utils/test_resource.py` & `mckit-0.6.24/tests/utils/test_resource.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,48 @@
+from __future__ import annotations
+
 from pathlib import Path
 
 import pytest
 
 from mckit.utils.resource import path_resolver
 
 THIS_FILENAME = Path(__file__).name
 
 
 # noinspection PyCompatibility
 @pytest.mark.parametrize(
-    "package, resource, expected",
+    "package,resource,expected",
     [
         ("tests", "cli/data/simple_cubes.mcnp", "/cli/data/simple_cubes.mcnp"),
     ],
 )
 def test_path_resolver(package, resource, expected) -> None:
     resolver = path_resolver(package)
     actual = resolver(resource)
     assert str(actual).replace("\\", "/").endswith(expected), "Failed to compute resource file name"
     assert Path(actual).exists(), f"The resource {resource!r} is not available"
 
 
-# noinspection PyCompatibility
 @pytest.mark.parametrize(
-    "package, resource, expected",
+    "package,resource",
     [
-        ("tests", "data/fispact/not_existing", "tests/data/fispact/not_existing"),
-        ("mckit", "data/not_existing", "mckit/data/not_existing"),
+        ("tests", "data/fispact/not_existing"),
+        ("mckit", "data/not_existing"),
     ],
 )
-def test_path_resolver_when_resource_doesnt_exist(package, resource, expected) -> None:
+def test_path_resolver_when_resource_doesnt_exist(package, resource) -> None:
     resolver = path_resolver(package)
     actual = resolver(resource)
     assert not Path(actual).exists(), f"The resource {resource!r} should not be available"
 
 
 def test_path_resolver_when_package_doesnt_exist() -> None:
     with pytest.raises(ModuleNotFoundError):
-        resolver = path_resolver("not_existing")
-        resolver("something.txt")
+        path_resolver("not_existing")("something.txt")
 
 
 def test_path_resolver_local() -> None:
     resolver = path_resolver("tests")
     actual = resolver("utils/" + THIS_FILENAME)
     assert isinstance(actual, Path)
     assert actual.name == THIS_FILENAME
```

### Comparing `mckit-0.6.23/tests/utils/test_rounding.py` & `mckit-0.6.24/tests/utils/test_rounding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import numpy as np
 
 import pytest
 
 from mckit.utils import round_array, round_scalar, significant_array, significant_digits
 
 
@@ -32,15 +34,14 @@
     approx = round(value, precision)
     if res and abs(value) < res:
         assert approx == 0
     elif value != approx:
         rel = abs(value - approx) / max(abs(value), abs(approx))
         assert rel <= tol
         wrong = round(value, precision - 1)
-        print(approx, wrong, precision)
         rel = abs(value - wrong) / max(abs(value), abs(wrong))
         assert rel > tol
 
 
 @pytest.mark.parametrize(
     "value, reltol, resolution, answer",
     [
```

### Comparing `mckit-0.6.23/tests/utils/test_tolerance.py` & `mckit-0.6.24/tests/utils/test_tolerance.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import numpy as np
 
 import pytest
 
 from mckit.utils.tolerance import DEFAULT_TOLERANCE_ESTIMATOR
 
 SOME_ARRAY = np.arange(3, dtype=float)
```

### Comparing `mckit-0.6.23/tests/utils/test_utils.py` & `mckit-0.6.24/tests/utils/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import numpy as np
 
 import pytest
 
 from mckit.utils import (
     FLOAT_TOLERANCE,
     are_equal,
```

### Comparing `mckit-0.6.23/setup.py` & `mckit-0.6.24/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,46 +48,46 @@
 install_requires = \
 ['DateTime>=4.3',
  'atomicwrites>=1.4.0',
  'attrs>=21.2.0',
  'click>=8.0.1',
  'colorama>=0.4.4',
  'loguru>=0.6.0',
- 'mkl-devel==2022.2.1',
- 'numpy>=1.24.2',
+ 'mkl-devel==2023.1.0',
+ 'numpy>=1.24.3',
  'ply>=3.11',
  'python-dotenv>=0.20.0',
  'scipy>=1.10.1',
  'sly>=0.4',
- 'tbb==2021.7.1',
+ 'tbb==2021.9.0',
  'tomli-w>=1.0.0',
  'tqdm>=4.55.1']
 
 extras_require = \
 {':python_version < "3.11"': ['tomli>=2.0.1'],
  ':python_version == "3.8"': ['importlib-resources>=5.12.0']}
 
 entry_points = \
 {'console_scripts': ['mckit = mckit.cli.runner:mckit']}
 
 setup_kwargs = {
     'name': 'mckit',
-    'version': '0.6.23',
+    'version': '0.6.24',
     'description': 'Tools to process MCNP models and results',
     'long_description': '.. image:: https://img.shields.io/badge/Maintained%3F-yes-green.svg\n   :target: https://github.com/MC-kit/mckit/graphs/commit-activity\n\n.. image:: https://github.com/MC-kit/mckit/workflows/Tests/badge.svg\n   :target: https://github.com/MC-kit/mckit/actions\n\n.. image:: https://codecov.io/gh/MC-kit/mckit/branch/devel/graph/badge.svg?token=05OFBQS3RX\n   :target: https://codecov.io/gh/MC-kit/mckit\n\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n\n.. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336\n    :target: https://pycqa.github.io/isort/\n\n.. image:: https://img.shields.io/github/license/MC-kit/mckit\n   :target: https://github.com/MC-kit/mckit\n\n\nMCKIT: MCNP model and results processing utilities\n==================================================\n\nThe mckit package provides a programming framework and command line tools to manipulate complex MCNP models.\nWhen a model is rather complex and its description occupies thousands of text lines it becomes hard to modify it and integrate several model manually.\nThe package automates integration process.\n\n.. TODO The complete documentation is available in the following languages:\n\n.. * `English documentation`_\n.. * `Russian documentation`_\n\n.. .. _English documentation: https://mckit.readthedocs.io/en/latest/\n.. .. _Russian documentation: https://mckit.readthedocs.io/ru/latest/\n\n.. contents:: Table of contents\n\nUsage\n-----\n\nCommand line interface\n~~~~~~~~~~~~~~~~~~~~~~\n\n.. code-block:: bash\n\n    Usage: mckit [OPTIONS] COMMAND [ARGS]...\n\n      Tools to process MCNP models and results\n\n    Options:\n      --override / --no-override\n      --version                   Show the version and exit.\n      -v, --verbose               Log debugging info to stderr.  [default: False]\n      -q, --quiet                 Suppress info to stderr.  [default: False]\n      --logfile / --no-logfile    Log to file.  [default: True]\n      --profile_mem               Profile peak memory use.  [default: False]\n      --help                      Show this message and exit.\n\n    Commands:\n      check      Read MCNP model(s) and show statistics and clashes.\n      compose    Merge universes and envelopes into MCNP model using merge...\n      concat     Concat text files.\n      decompose  Separate an MCNP model to envelopes and filling universes\n      split      Splits MCNP model to text portions (opposite to concat)\n      transform  Transform MCNP model(s) with one of specified transformation.\n\n\nLibrary\n~~~~~~~\n\nThe library allows subtraction and merging models, renaming objects (cells, surfaces, compositions, universes),\nsimplification of cell expressions (removing redundant surfaces), homogenization, computation of cell volumes and\nmaterial masses, and more.\n\n.. code-block:: python\n\n    LOG.info("Loading c-model envelopes")\n    envelopes = load_model(str(CMODEL_ROOT / "c-model.universes/envelopes.i"))\n\n    cells_to_fill = [11, 14, 75]\n    cells_to_fill_indexes = [c - 1 for c in cells_to_fill]\n\n    LOG.info("Attaching bounding boxes to c-model envelopes %s", cells_to_fill)\n    attach_bounding_boxes(\n        [envelopes[i] for i in cells_to_fill_indexes], tolerance=5.0, chunk_size=1\n    )\n    LOG.info("Backing up original envelopes")\n    envelopes_original = envelopes.copy()\n\n    antenna_envelop.rename(start_cell=200000, start_surf=200000)\n\n    LOG.info("Subtracting antenna envelop from c-model envelopes %s", cells_to_fill)\n    envelopes = subtract_model_from_model(\n        envelopes, antenna_envelop, cells_filter=lambda c: c in cells_to_fill\n    )\n    LOG.info("Adding antenna envelop to c-model envelopes")\n    envelopes.add_cells(antenna_envelop, name_rule="clash")\n    envelopes_path = "envelopes+antenna-envelop.i"\n    envelopes.save(envelopes_path)\n    LOG.info("The model of HFSR in envelopes is saved to %s", envelopes_path)\n\n\n\nInstallation\n------------\n\nInstalling from pypi:\n\n.. code-block:: bash\n\n    pip3 install mckit\n\n\nInstalling from github.com:\n\n.. code-block:: bash\n\n    pip3 install git+https://github.com/MC-kit/mckit.git\n\n\nVersioning\n----------\n\nThis software follows `Semantic Versioning`_\n\n.. _Semantic Versioning: http://semver.org/\n\n\nContributors\n------------\n\n* `Roman Rodionov <mailto:r.rodionov@iterrf.ru>`_\n* `Dmitri Portnov <mailto:dmitri_portnov@yahoo.com>`_\n',
     'author': 'rrn',
     'author_email': 'r.rodionov@iterrf.ru',
     'maintainer': 'dpv2015',
     'maintainer_email': 'dmitri_portnov@yahoo.com',
     'url': 'https://github.com/MC-kit/mckit',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
     'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.12',
+    'python_requires': '>=3.8.1,<3.12',
 }
 from build import *
 build(setup_kwargs)
 
 setup(**setup_kwargs)
```

### Comparing `mckit-0.6.23/PKG-INFO` & `mckit-0.6.24/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 Metadata-Version: 2.1
 Name: mckit
-Version: 0.6.23
+Version: 0.6.24
 Summary: Tools to process MCNP models and results
 Home-page: https://github.com/MC-kit/mckit
 License: GPL3
 Keywords: mckit,MCNP
 Author: rrn
 Author-email: r.rodionov@iterrf.ru
 Maintainer: dpv2015
 Maintainer-email: dmitri_portnov@yahoo.com
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8.1,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Dist: DateTime (>=4.3)
 Requires-Dist: atomicwrites (>=1.4.0)
 Requires-Dist: attrs (>=21.2.0)
 Requires-Dist: click (>=8.0.1)
 Requires-Dist: colorama (>=0.4.4)
 Requires-Dist: importlib-resources (>=5.12.0) ; python_version == "3.8"
 Requires-Dist: loguru (>=0.6.0)
-Requires-Dist: mkl-devel (==2022.2.1)
-Requires-Dist: numpy (>=1.24.2)
+Requires-Dist: mkl-devel (==2023.1.0)
+Requires-Dist: numpy (>=1.24.3)
 Requires-Dist: ply (>=3.11)
 Requires-Dist: python-dotenv (>=0.20.0)
 Requires-Dist: scipy (>=1.10.1)
 Requires-Dist: sly (>=0.4)
-Requires-Dist: tbb (==2021.7.1)
+Requires-Dist: tbb (==2021.9.0)
 Requires-Dist: tomli (>=2.0.1) ; python_version < "3.11"
 Requires-Dist: tomli-w (>=1.0.0)
 Requires-Dist: tqdm (>=4.55.1)
 Project-URL: Bug Tracker, https://github.com/MC-kit/mckit/issues
 Project-URL: Documentation, https://mckit.readthedocs.io
 Project-URL: Repository, https://github.com/MC-kit/mckit
 Description-Content-Type: text/x-rst
```

