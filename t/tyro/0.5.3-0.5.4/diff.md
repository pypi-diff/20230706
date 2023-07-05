# Comparing `tmp/tyro-0.5.3.tar.gz` & `tmp/tyro-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tyro-0.5.3.tar", max compression
+gzip compressed data, was "tyro-0.5.4.tar", last modified: Wed Jul  5 23:22:33 2023, max compression
```

## Comparing `tyro-0.5.3.tar` & `tyro-0.5.4.tar`

### file list

```diff
@@ -1,28 +1,102 @@
--rw-r--r--   0        0        0     1065 2023-05-27 10:12:15.896200 tyro-0.5.3/LICENSE
--rw-r--r--   0        0        0     4445 2023-05-27 10:16:06.311375 tyro-0.5.3/README.md
--rw-r--r--   0        0        0     1866 2023-05-27 10:12:15.896200 tyro-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      406 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/__init__.py
--rw-r--r--   0        0        0    22530 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_argparse_formatter.py
--rw-r--r--   0        0        0    19335 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_arguments.py
--rw-r--r--   0        0        0     8560 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_calling.py
--rw-r--r--   0        0        0    15674 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_cli.py
--rw-r--r--   0        0        0      101 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_deprecated.py
--rw-r--r--   0        0        0    11749 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_docstrings.py
--rw-r--r--   0        0        0    30130 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_fields.py
--rw-r--r--   0        0        0    23376 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_instantiators.py
--rw-r--r--   0        0        0    21122 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_parsers.py
--rw-r--r--   0        0        0    11374 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_resolver.py
--rw-r--r--   0        0        0      383 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_singleton.py
--rw-r--r--   0        0        0     4949 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_strings.py
--rw-r--r--   0        0        0     3793 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_subcommand_matching.py
--rw-r--r--   0        0        0      764 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_typing.py
--rw-r--r--   0        0        0     1206 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/_unsafe_cache.py
--rw-r--r--   0        0        0     1083 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/conf/__init__.py
--rw-r--r--   0        0        0     1998 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/conf/_confstruct.py
--rw-r--r--   0        0        0     5805 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/conf/_markers.py
--rw-r--r--   0        0        0      579 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/extras/__init__.py
--rw-r--r--   0        0        0     2354 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/extras/_base_configs.py
--rw-r--r--   0        0        0     1258 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/extras/_choices_type.py
--rw-r--r--   0        0        0     8196 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/extras/_serialization.py
--rw-r--r--   0        0        0        0 2023-05-27 10:12:15.900200 tyro-0.5.3/tyro/py.typed
--rw-r--r--   0        0        0     5552 1970-01-01 00:00:00.000000 tyro-0.5.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.097649 tyro-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-05 23:20:00.000000 tyro-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-05 23:22:33.097649 tyro-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-05 23:22:27.000000 tyro-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.053649 tyro-0.5.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.053649 tyro-0.5.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-07-05 23:20:00.000000 tyro-0.5.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-05 23:20:00.000000 tyro-0.5.4/docs/update_example_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.053649 tyro-0.5.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.057649 tyro-0.5.4/examples/01_basics/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      587 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/01_basics/01_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/01_basics/02_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/01_basics/03_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/01_basics/04_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/01_basics/05_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/01_basics/06_literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/01_basics/07_unions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.061649 tyro-0.5.4/examples/02_nesting/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/02_nesting/01_nesting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/02_nesting/02_subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/02_nesting/03_multiple_subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/02_nesting/04_nesting_in_containers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.061649 tyro-0.5.4/examples/03_config_systems/
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/03_config_systems/01_base_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/03_config_systems/02_overriding_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.065649 tyro-0.5.4/examples/04_additional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/04_additional/01_positional_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/04_additional/02_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/04_additional/03_tuples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/04_additional/04_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/04_additional/05_generics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/04_additional/06_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/04_additional/07_flax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/04_additional/08_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/04_additional/09_attrs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      420 2023-07-05 23:20:00.000000 tyro-0.5.4/examples/_rename_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-05 23:20:00.000000 tyro-0.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 23:22:33.097649 tyro-0.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.081649 tyro-0.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_boolean_optional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24964 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17085 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_dcargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_dict_namedtuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_dynamic_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_flax_ignore_py310.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_forward_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_generics_and_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_helptext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_initvar_ignore_py37.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_is_nested_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_missing_optional_packages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_mixed_unions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26765 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_nested_in_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_new_style_annotations_above_py39.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_new_style_annotations_only_py310.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_positional_ignore_py37.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_union_from_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_unsafe_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-05 23:20:00.000000 tyro-0.5.4/tests/test_unsupported_but_should_work.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.093649 tyro-0.5.4/tyro/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22530 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_argparse_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19335 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_calling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31032 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23376 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_instantiators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21278 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_subcommand_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/_unsafe_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.093649 tyro-0.5.4/tyro/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/conf/_confstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/conf/_markers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.097649 tyro-0.5.4/tyro/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/extras/_base_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/extras/_choices_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/extras/_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 23:20:00.000000 tyro-0.5.4/tyro/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 23:22:33.093649 tyro-0.5.4/tyro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-05 23:22:33.000000 tyro-0.5.4/tyro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-05 23:22:33.000000 tyro-0.5.4/tyro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 23:22:33.000000 tyro-0.5.4/tyro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-05 23:22:33.000000 tyro-0.5.4/tyro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-05 23:22:33.000000 tyro-0.5.4/tyro.egg-info/top_level.txt
```

### Comparing `tyro-0.5.3/LICENSE` & `tyro-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tyro-0.5.3/README.md` & `tyro-0.5.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -133,10 +133,15 @@
 - [nerfstudio-project/nerfstudio](https://github.com/nerfstudio-project/nerfstudio/)
   provides a set of tools for end-to-end training, testing, and rendering of
   neural radiance fields.
 - [Sea-Snell/JAXSeq](https://github.com/Sea-Snell/JAXSeq/) is a library for
   distributed training of large language models in JAX.
 - [kevinzakka/obj2mjcf](https://github.com/kevinzakka/obj2mjcf) is an interface
   for processing composite Wavefront OBJ files for Mujoco.
-- [brentyi/tensorf-jax](https://github.com/brentyi/tensorf-jax/) is an
-  unofficial implementation of
-  [Tensorial Radiance Fields](https://apchenstu.github.io/TensoRF/) in JAX.
+- [blurgyy/jaxngp](https://github.com/blurgyy/jaxngp) is a CUDA-accelerated
+  implementation of [instant-ngp](https://nvlabs.github.io/instant-ngp/),
+  implemented in JAX.
+- [NVIDIAGameWorks/kaolin-wisp](https://github.com/NVIDIAGameWorks/kaolin-wisp)
+  is a PyTorch library for working with neural fields.
+- [openrlbenchmark/openrlbenchmark](https://github.com/openrlbenchmark/openrlbenchmark)
+  is a comprehensive collection of tracked experiments for reinforcement
+  learning.
```

### Comparing `tyro-0.5.3/tyro/_argparse_formatter.py` & `tyro-0.5.4/tyro/_argparse_formatter.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.3/tyro/_arguments.py` & `tyro-0.5.4/tyro/_arguments.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.3/tyro/_calling.py` & `tyro-0.5.4/tyro/_calling.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,25 @@
             name_maybe_prefixed = prefixed_field_name
             consumed_keywords.add(name_maybe_prefixed)
             if not arg.lowered.is_fixed():
                 value = get_value_from_arg(name_maybe_prefixed)
 
                 if value in _fields.MISSING_SINGLETONS:
                     value = arg.field.default
+
+                    # Consider a function with a positional sequence argument:
+                    #
+                    #     def f(x: tuple[int, ...], /)
+                    #
+                    # If we run this script with no arguments, we should interpret this
+                    # as empty input for x. But the argparse default will be a MISSING
+                    # value, and the field default will be inspect.Parameter.empty.
+                    if value in _fields.MISSING_SINGLETONS:
+                        assert field.is_positional() and arg.lowered.nargs in ("?", "*")
+                        value = []
                 else:
                     if arg.lowered.nargs == "?":
                         # Special case for optional positional arguments: this is the
                         # only time that arguments don't come back as a list.
                         value = [value]
 
                     try:
```

### Comparing `tyro-0.5.3/tyro/_cli.py` & `tyro-0.5.4/tyro/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,15 +284,17 @@
     # We wrap our type with a dummy dataclass if it can't be treated as a nested type.
     # For example: passing in f=int will result in a dataclass with a single field
     # typed as int.
     if not _fields.is_nested_type(cast(type, f), default_instance_internal):
         dummy_field = cast(
             dataclasses.Field,
             dataclasses.field(
-                default=default if default is not None else dataclasses.MISSING
+                default_factory=lambda: default
+                if default is not None
+                else dataclasses.MISSING
             ),
         )
         f = dataclasses.make_dataclass(
             cls_name="",
             fields=[(_strings.dummy_field_name, cast(type, f), dummy_field)],
         )
         dummy_wrapped = True
```

### Comparing `tyro-0.5.3/tyro/_docstrings.py` & `tyro-0.5.4/tyro/_docstrings.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.3/tyro/_fields.py` & `tyro-0.5.4/tyro/_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 MISSING_PROP = PropagatingMissingType()
 MISSING_NONPROP = NonpropagatingMissingType()
 
 # When total=False in a TypedDict, we exclude fields from the constructor by default.
 EXCLUDE_FROM_CALL = ExcludeFromCallType()
 
 # Note that our "public" missing API will always be the propagating missing sentinel.
-MISSING_PUBLIC: Any = MISSING_PROP
+MISSING: Any = MISSING_PROP
 """Sentinel value to mark fields as missing. Can be used to mark fields passed in as a
 `default_instance` for `tyro.cli()` as required."""
 
 
 MISSING_SINGLETONS = [
     dataclasses.MISSING,
     MISSING_PROP,
@@ -455,29 +455,51 @@
 def _field_list_from_pydantic(
     cls: TypeForm[Any], default_instance: DefaultInstance
 ) -> Union[List[FieldDefinition], UnsupportedNestedTypeMessage]:
     assert pydantic is not None
 
     # Handle pydantic models.
     field_list = []
-    for pd_field in cls.__fields__.values():  # type: ignore
-        helptext = pd_field.field_info.description
-        if helptext is None:
-            helptext = _docstrings.get_field_docstring(cls, pd_field.name)
-
-        field_list.append(
-            FieldDefinition.make(
-                name=pd_field.name,
-                typ=pd_field.outer_type_,
-                default=(
-                    MISSING_NONPROP if pd_field.required else pd_field.get_default()
-                ),
-                helptext=helptext,
+    pydantic_version = int(getattr(pydantic, "__version__", "1.0.0").partition(".")[0])
+    if pydantic_version < 2:  # pragma: no cover
+        # Pydantic 1.xx.
+        for pd_field in cls.__fields__.values():  # type: ignore
+            helptext = pd_field.field_info.description
+            if helptext is None:
+                helptext = _docstrings.get_field_docstring(cls, pd_field.name)
+
+            field_list.append(
+                FieldDefinition.make(
+                    name=pd_field.name,
+                    typ=pd_field.outer_type_,
+                    default=(
+                        MISSING_NONPROP if pd_field.required else pd_field.get_default()
+                    ),
+                    helptext=helptext,
+                )
+            )
+    else:
+        # Pydantic 2.xx.
+        for name, pd_field in cls.model_fields.items():  # type: ignore
+            helptext = pd_field.description
+            if helptext is None:
+                helptext = _docstrings.get_field_docstring(cls, name)
+
+            field_list.append(
+                FieldDefinition.make(
+                    name=name,
+                    typ=pd_field.annotation,
+                    default=(
+                        MISSING_NONPROP
+                        if pd_field.is_required()
+                        else pd_field.get_default(call_default_factory=True)
+                    ),
+                    helptext=helptext,
+                )
             )
-        )
     return field_list
 
 
 try:
     import attr
 except ImportError:
     attr = None  # type: ignore
```

### Comparing `tyro-0.5.3/tyro/_instantiators.py` & `tyro-0.5.4/tyro/_instantiators.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 NoneType = type(None)
 
 
 @dataclasses.dataclass
 class InstantiatorMetadata:
     # Unlike in vanilla argparse, we never set nargs to None. To make things simpler, we
     # instead use nargs=1.
-    nargs: Optional[Union[int, Literal["+"]]]
+    nargs: Optional[Union[int, Literal["*"]]]
     # Unlike in vanilla argparse, our metavar is always a string. We handle
     # sequences, multiple arguments, etc, manually.
     metavar: str
     choices: Optional[Tuple[str, ...]]
     action: Optional[Literal["append"]]
 
     def check_choices(self, strings: List[str]) -> None:
@@ -286,15 +286,15 @@
     type_from_typevar: Dict[TypeVar, TypeForm[Any]],
     allow_sequences: Literal["fixed_length", True, False],
     markers: FrozenSet[_markers.Marker],
 ) -> Tuple[Instantiator, InstantiatorMetadata]:
     """Thin wrapper over instantiator_from_type, with some extra asserts for catching
     errors."""
     out = instantiator_from_type(typ, type_from_typevar, markers)
-    if out[1].nargs == "+":
+    if out[1].nargs == "*":
         # We currently only use allow_sequences=False for options in Literal types,
         # which are evaluated using `type()`. It should not be possible to hit this
         # condition from polling a runtime type.
         assert allow_sequences
         if allow_sequences == "fixed_length" and not isinstance(out[1].nargs, int):
             raise UnsupportedTypeAnnotationError(
                 f"{typ} is a variable-length sequence, which is ambiguous when nested."
@@ -440,15 +440,15 @@
         options.remove(NoneType)
         options.insert(0, NoneType)
 
     # General unions, eg Union[int, bool]. We'll try to convert these from left to
     # right.
     instantiators = []
     metas = []
-    nargs: Optional[Union[int, Literal["+"]]] = 1
+    nargs: Optional[Union[int, Literal["*"]]] = 1
     first = True
     for t in options:
         a, b = _instantiator_from_type_inner(
             t, type_from_typevar, allow_sequences=True, markers=markers
         )
         instantiators.append(a)
         metas.append(b)
@@ -457,15 +457,15 @@
             # Enforce that `nargs` is the same for all child types, except for
             # NoneType.
             if first:
                 nargs = b.nargs
                 first = False
             elif nargs != b.nargs:
                 # Just be as general as possible if we see inconsistencies.
-                nargs = "+"
+                nargs = "*"
 
     metavar: str
     metavar = _join_union_metavars(map(lambda x: cast(str, x.metavar), metas))
 
     def union_instantiator(strings: List[str]) -> Any:
         metadata: InstantiatorMetadata
         errors = []
@@ -476,15 +476,15 @@
             ):
                 errors.append(
                     f"{options[i]}: {strings} does not match choices {metadata.choices}"
                 )
                 continue
 
             # Try passing input into instantiator.
-            if len(strings) == metadata.nargs or (metadata.nargs == "+"):
+            if len(strings) == metadata.nargs or (metadata.nargs == "*"):
                 try:
                     return instantiator(strings)  # type: ignore
                 except ValueError as e:
                     # Failed, try next instantiator.
                     errors.append(f"{options[i]}: {e.args[0]}")
             else:
                 errors.append(
@@ -529,15 +529,15 @@
         def append_dict_instantiator(strings: List[List[str]]) -> Any:
             out = {}
             for s in strings:
                 out[key_instantiator(s[:key_nargs])] = val_instantiator(s[key_nargs:])  # type: ignore
             return out
 
         return append_dict_instantiator, InstantiatorMetadata(
-            nargs=key_nargs + val_nargs if isinstance(val_nargs, int) else "+",
+            nargs=key_nargs + val_nargs if isinstance(val_nargs, int) else "*",
             metavar=pair_metavar,
             choices=None,
             action="append",
         )
     else:
         val_instantiator, val_meta = _instantiator_from_type_inner(
             val_type, type_from_typevar, allow_sequences="fixed_length", markers=markers
@@ -575,15 +575,15 @@
                     raise ValueError(
                         f"invalid choice: {v} (choose from {val_meta.choices}))"
                     )
                 out[key_instantiator(k)] = val_instantiator(v)  # type: ignore
             return out
 
         return dict_instantiator, InstantiatorMetadata(
-            nargs="+",
+            nargs="*",
             metavar=_strings.multi_metavar_from_single(pair_metavar),
             choices=None,
             action=None,
         )
 
 
 def _instantiator_from_sequence(
@@ -646,15 +646,15 @@
             step = inner_meta.nargs if isinstance(inner_meta.nargs, int) else 1
             for i in range(0, len(strings), step):
                 out.append(make(strings[i : i + inner_meta.nargs]))  # type: ignore
             assert container_type is not None
             return container_type(out)
 
         return sequence_instantiator, InstantiatorMetadata(
-            nargs="+",
+            nargs="*",
             metavar=_strings.multi_metavar_from_single(inner_meta.metavar),
             choices=inner_meta.choices,
             action=None,
         )
 
 
 def _instantiator_from_literal(
```

### Comparing `tyro-0.5.3/tyro/_parsers.py` & `tyro-0.5.4/tyro/_parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,112 +99,62 @@
         args = []
         helptext_from_nested_class_field_name = {}
 
         subparsers = None
         subparsers_from_prefix = {}
 
         for field in field_list:
-            if isinstance(field.typ, TypeVar):
-                raise _instantiators.UnsupportedTypeAnnotationError(
-                    f"Field {field.name} has an unbound TypeVar: {field.typ}."
-                )
-
-            if _markers.Fixed not in field.markers:
-                # (1) Handle Unions over callables; these result in subparsers.
-                subparsers_attempt = SubparsersSpecification.from_field(
-                    field,
-                    type_from_typevar=type_from_typevar,
-                    parent_classes=parent_classes,
-                    prefix=_strings.make_field_name([prefix, field.name]),
-                )
-                if subparsers_attempt is not None:
-                    if subparsers_attempt.required:
-                        has_required_args = True
-                    if (
-                        not subparsers_attempt.required
-                        and _markers.AvoidSubcommands in field.markers
-                    ):
-                        # Don't make a subparser.
-                        field = dataclasses.replace(field, typ=type(field.default))
-                    else:
-                        subparsers_from_prefix[
-                            subparsers_attempt.prefix
-                        ] = subparsers_attempt
-                        subparsers = add_subparsers_to_leaves(
-                            subparsers, subparsers_attempt
-                        )
-                        continue
-
-                # (2) Handle nested callables.
-                if _fields.is_nested_type(field.typ, field.default):
-                    field = dataclasses.replace(
-                        field,
-                        typ=_resolver.narrow_type(
-                            field.typ,
-                            field.default,
-                        ),
-                    )
-                    nested_parser = ParserSpecification.from_callable_or_type(
-                        (
-                            # Recursively apply marker types.
-                            field.typ
-                            if len(field.markers) == 0
-                            else Annotated.__class_getitem__(  # type: ignore
-                                (field.typ,) + tuple(field.markers)
-                            )
-                        ),
-                        description=None,
-                        parent_classes=parent_classes,
-                        default_instance=field.default,
-                        prefix=_strings.make_field_name([prefix, field.name]),
-                        subcommand_prefix=subcommand_prefix,
-                    )
-                    if nested_parser.has_required_args:
-                        has_required_args = True
-                    args.extend(nested_parser.args)
-
-                    # Include nested subparsers.
-                    if nested_parser.subparsers is not None:
-                        subparsers_from_prefix.update(
-                            nested_parser.subparsers_from_prefix
-                        )
-                        subparsers = add_subparsers_to_leaves(
-                            subparsers, nested_parser.subparsers
-                        )
-
-                    # Include nested strings.
-                    for (
-                        k,
-                        v,
-                    ) in nested_parser.helptext_from_nested_class_field_name.items():
-                        helptext_from_nested_class_field_name[
-                            _strings.make_field_name([field.name, k])
-                        ] = v
-
-                    if field.helptext is not None:
-                        helptext_from_nested_class_field_name[
-                            _strings.make_field_name([field.name])
-                        ] = field.helptext
-                    else:
-                        helptext_from_nested_class_field_name[
-                            _strings.make_field_name([field.name])
-                        ] = _docstrings.get_callable_description(field.typ)
-                    continue
-
-            # (3) Handle primitive or fixed types. These produce a single argument!
-            arg = _arguments.ArgumentDefinition(
-                dest_prefix=prefix,
-                name_prefix=prefix,
-                subcommand_prefix=subcommand_prefix,
-                field=field,
+            field_out = handle_field(
+                field,
                 type_from_typevar=type_from_typevar,
+                parent_classes=parent_classes,
+                prefix=prefix,
+                subcommand_prefix=subcommand_prefix,
             )
-            args.append(arg)
-            if arg.lowered.required:
-                has_required_args = True
+            if isinstance(field_out, _arguments.ArgumentDefinition):
+                # Handle single arguments.
+                args.append(field_out)
+                if field_out.lowered.required:
+                    has_required_args = True
+            elif isinstance(field_out, SubparsersSpecification):
+                # Handle subparsers.
+                subparsers_from_prefix[field_out.prefix] = field_out
+                subparsers = add_subparsers_to_leaves(subparsers, field_out)
+            elif isinstance(field_out, ParserSpecification):
+                # Handle nested parsers.
+                nested_parser = field_out
+
+                if nested_parser.has_required_args:
+                    has_required_args = True
+                args.extend(nested_parser.args)
+
+                # Include nested subparsers.
+                if nested_parser.subparsers is not None:
+                    subparsers_from_prefix.update(nested_parser.subparsers_from_prefix)
+                    subparsers = add_subparsers_to_leaves(
+                        subparsers, nested_parser.subparsers
+                    )
+
+                # Include nested strings.
+                for (
+                    k,
+                    v,
+                ) in nested_parser.helptext_from_nested_class_field_name.items():
+                    helptext_from_nested_class_field_name[
+                        _strings.make_field_name([field.name, k])
+                    ] = v
+
+                if field.helptext is not None:
+                    helptext_from_nested_class_field_name[
+                        _strings.make_field_name([field.name])
+                    ] = field.helptext
+                else:
+                    helptext_from_nested_class_field_name[
+                        _strings.make_field_name([field.name])
+                    ] = _docstrings.get_callable_description(nested_parser.f)
 
         return ParserSpecification(
             f=f,
             description=_strings.remove_single_line_breaks(
                 description
                 if description is not None
                 else _docstrings.get_callable_description(f)
@@ -302,14 +252,85 @@
             else:
                 # Suppressed argument: still need to add them, but they won't show up in
                 # the helptext so it doesn't matter which group.
                 assert arg.lowered.help is argparse.SUPPRESS
                 arg.add_argument(group_from_prefix[""])
 
 
+def handle_field(
+    field: _fields.FieldDefinition,
+    type_from_typevar: Dict[TypeVar, TypeForm[Any]],
+    parent_classes: Set[Type[Any]],
+    prefix: str,
+    subcommand_prefix: str,
+) -> Union[
+    _arguments.ArgumentDefinition,
+    ParserSpecification,
+    SubparsersSpecification,
+]:
+    """Determine what to do with a single field definition."""
+
+    if isinstance(field.typ, TypeVar):
+        raise _instantiators.UnsupportedTypeAnnotationError(
+            f"Field {field.name} has an unbound TypeVar: {field.typ}."
+        )
+
+    if _markers.Fixed not in field.markers:
+        # (1) Handle Unions over callables; these result in subparsers.
+        subparsers_attempt = SubparsersSpecification.from_field(
+            field,
+            type_from_typevar=type_from_typevar,
+            parent_classes=parent_classes,
+            prefix=_strings.make_field_name([prefix, field.name]),
+        )
+        if subparsers_attempt is not None:
+            if (
+                not subparsers_attempt.required
+                and _markers.AvoidSubcommands in field.markers
+            ):
+                # Don't make a subparser.
+                field = dataclasses.replace(field, typ=type(field.default))
+            else:
+                return subparsers_attempt
+
+        # (2) Handle nested callables.
+        if _fields.is_nested_type(field.typ, field.default):
+            field = dataclasses.replace(
+                field,
+                typ=_resolver.narrow_type(
+                    field.typ,
+                    field.default,
+                ),
+            )
+            return ParserSpecification.from_callable_or_type(
+                (
+                    # Recursively apply marker types.
+                    field.typ
+                    if len(field.markers) == 0
+                    else Annotated.__class_getitem__(  # type: ignore
+                        (field.typ,) + tuple(field.markers)
+                    )
+                ),
+                description=None,
+                parent_classes=parent_classes,
+                default_instance=field.default,
+                prefix=_strings.make_field_name([prefix, field.name]),
+                subcommand_prefix=subcommand_prefix,
+            )
+
+    # (3) Handle primitive or fixed types. These produce a single argument!
+    return _arguments.ArgumentDefinition(
+        dest_prefix=prefix,
+        name_prefix=prefix,
+        subcommand_prefix=subcommand_prefix,
+        field=field,
+        type_from_typevar=type_from_typevar,
+    )
+
+
 @dataclasses.dataclass(frozen=True)
 class SubparsersSpecification:
     """Structure for defining subparsers. Each subparser is a parser with a name."""
 
     name: str
     description: Optional[str]
     parser_from_name: Dict[str, ParserSpecification]
```

### Comparing `tyro-0.5.3/tyro/_resolver.py` & `tyro-0.5.4/tyro/_resolver.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.3/tyro/_strings.py` & `tyro-0.5.4/tyro/_strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,17 +125,17 @@
 def strip_ansi_sequences(x: str):
     return _get_ansi_pattern().sub("", x)
 
 
 def multi_metavar_from_single(single: str) -> str:
     if len(strip_ansi_sequences(single)) >= 32:
         # Shorten long metavars
-        return f"{single} [...]"
+        return f"[{single} [...]]"
     else:
-        return f"{single} [{single} ...]"
+        return f"[{single} [{single} ...]]"
 
 
 def remove_single_line_breaks(helptext: str) -> str:
     lines = helptext.split("\n")
     output_parts: List[str] = []
     for line in lines:
         # Remove trailing whitespace.
```

### Comparing `tyro-0.5.3/tyro/_subcommand_matching.py` & `tyro-0.5.4/tyro/_subcommand_matching.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.3/tyro/_typing.py` & `tyro-0.5.4/tyro/_typing.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.3/tyro/_unsafe_cache.py` & `tyro-0.5.4/tyro/_unsafe_cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 
 def clear_cache() -> None:
     for c in _cache_list:
         c.clear()
 
 
 def unsafe_cache(maxsize: int) -> Callable[[CallableType], CallableType]:
-    """Cache decorator that relies object IDs when arguments are unhashable. Assumes
-    immutability."""
+    """Cache decorator that relies object IDs when arguments are unhashable. Makes the
+    very strong assumption of not only immutability, but that unhashable types don't go
+    out of scope."""
 
     _cache_list.append({})
     local_cache = _cache_list[-1]
 
     def inner(f: CallableType) -> CallableType:
         @functools.wraps(f)
         def wrapped_f(*args, **kwargs):
```

### Comparing `tyro-0.5.3/tyro/conf/__init__.py` & `tyro-0.5.4/tyro/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.3/tyro/conf/_confstruct.py` & `tyro-0.5.4/tyro/conf/_confstruct.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.3/tyro/conf/_markers.py` & `tyro-0.5.4/tyro/conf/_markers.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.3/tyro/extras/_base_configs.py` & `tyro-0.5.4/tyro/extras/_base_configs.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.3/tyro/extras/_choices_type.py` & `tyro-0.5.4/tyro/extras/_choices_type.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.3/tyro/extras/_serialization.py` & `tyro-0.5.4/tyro/extras/_serialization.py`

 * *Files identical despite different names*

### Comparing `tyro-0.5.3/PKG-INFO` & `tyro-0.5.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 Metadata-Version: 2.1
 Name: tyro
-Version: 0.5.3
+Version: 0.5.4
 Summary: Strongly typed, zero-effort CLI interfaces
-Home-page: https://github.com/brentyi/tyro
-Author: brentyi
-Author-email: brentyi@berkeley.edu
-Requires-Python: >=3.7,<4.0
+Author-email: brentyi <brentyi@berkeley.edu>
+License: MIT
+Project-URL: GitHub, https://github.com/brentyi/tyro
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: backports.cached-property (>=1.0.2,<2.0.0) ; python_version >= "3.7" and python_version < "3.8"
-Requires-Dist: colorama (>=0.4.0,<0.5.0) ; sys_platform == "win32"
-Requires-Dist: docstring-parser (>=0.14.1,<0.15.0)
-Requires-Dist: frozendict (>=2.3.4,<3.0.0)
-Requires-Dist: rich (>=11.1.0)
-Requires-Dist: shtab (>=1.5.6,<2.0.0)
-Requires-Dist: typing-extensions (>=4.3.0,<5.0.0)
-Project-URL: Documentation, https://brentyi.github.io/tyro/
-Project-URL: Repository, https://github.com/brentyi/tyro
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
 
 <br />
 <p align="center">
     <!--
     Note that this README will be used for both GitHub and PyPI.
     We therefore:
     - Keep all image URLs absolute.
@@ -159,11 +153,15 @@
 - [nerfstudio-project/nerfstudio](https://github.com/nerfstudio-project/nerfstudio/)
   provides a set of tools for end-to-end training, testing, and rendering of
   neural radiance fields.
 - [Sea-Snell/JAXSeq](https://github.com/Sea-Snell/JAXSeq/) is a library for
   distributed training of large language models in JAX.
 - [kevinzakka/obj2mjcf](https://github.com/kevinzakka/obj2mjcf) is an interface
   for processing composite Wavefront OBJ files for Mujoco.
-- [brentyi/tensorf-jax](https://github.com/brentyi/tensorf-jax/) is an
-  unofficial implementation of
-  [Tensorial Radiance Fields](https://apchenstu.github.io/TensoRF/) in JAX.
-
+- [blurgyy/jaxngp](https://github.com/blurgyy/jaxngp) is a CUDA-accelerated
+  implementation of [instant-ngp](https://nvlabs.github.io/instant-ngp/),
+  implemented in JAX.
+- [NVIDIAGameWorks/kaolin-wisp](https://github.com/NVIDIAGameWorks/kaolin-wisp)
+  is a PyTorch library for working with neural fields.
+- [openrlbenchmark/openrlbenchmark](https://github.com/openrlbenchmark/openrlbenchmark)
+  is a comprehensive collection of tracked experiments for reinforcement
+  learning.
```

