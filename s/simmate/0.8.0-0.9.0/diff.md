# Comparing `tmp/simmate-0.8.0.tar.gz` & `tmp/simmate-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simmate-0.8.0.tar", last modified: Thu Aug 11 21:23:48 2022, max compression
+gzip compressed data, was "simmate-0.9.0.tar", last modified: Wed Aug 17 16:40:39 2022, max compression
```

## Comparing `simmate-0.8.0.tar` & `simmate-0.9.0.tar`

### file list

```diff
@@ -1,653 +1,664 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.373717 simmate-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-08-11 21:23:38.000000 simmate-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-08-11 21:23:48.373717 simmate-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12777 2022-08-11 21:23:38.000000 simmate-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     8375 2022-08-11 21:23:38.000000 simmate-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-11 21:23:48.373717 simmate-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.317716 simmate-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.321716 simmate-0.8.0/src/simmate/
--rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.325716 simmate-0.8.0/src/simmate/calculators/
--rw-r--r--   0 runner    (1001) docker     (121)     1767 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.325716 simmate-0.8.0/src/simmate/calculators/bader/
--rw-r--r--   0 runner    (1001) docker     (121)     1657 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/bader/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/bader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/bader/inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.325716 simmate-0.8.0/src/simmate/calculators/bader/outputs/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/bader/outputs/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/bader/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1701 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/bader/outputs/acf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.325716 simmate-0.8.0/src/simmate/calculators/bader/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/bader/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1670 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/bader/workflows/badelf.py
--rw-r--r--   0 runner    (1001) docker     (121)     5079 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/bader/workflows/bader.py
--rw-r--r--   0 runner    (1001) docker     (121)      724 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/bader/workflows/combine_chgcars.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.325716 simmate-0.8.0/src/simmate/calculators/deepmd/
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/deepmd/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/deepmd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.325716 simmate-0.8.0/src/simmate/calculators/deepmd/inputs/
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/deepmd/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1851 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/deepmd/inputs/parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     9611 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/deepmd/inputs/type_and_set.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.325716 simmate-0.8.0/src/simmate/calculators/vasp/
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5441 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/configuration.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.329716 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/brions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5768 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/brmix.py
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/edddav.py
--rw-r--r--   0 runner    (1001) docker     (121)     2922 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/eddrmm.py
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/edwav.py
--rw-r--r--   0 runner    (1001) docker     (121)      706 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/elf_kpar.py
--rw-r--r--   0 runner    (1001) docker     (121)     3755 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/frozen.py
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/incorrect_shift.py
--rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/incorrect_smearing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1566 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/insufficient_bands.py
--rw-r--r--   0 runner    (1001) docker     (121)     4102 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/large_sigma.py
--rw-r--r--   0 runner    (1001) docker     (121)      877 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/long_vector.py
--rw-r--r--   0 runner    (1001) docker     (121)     3673 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/mesh_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (121)     5919 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/nonconverging.py
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/point_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     3699 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/positive_energy.py
--rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/posmap.py
--rw-r--r--   0 runner    (1001) docker     (121)     3200 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/potim.py
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/pricel.py
--rw-r--r--   0 runner    (1001) docker     (121)      808 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/pssyevx.py
--rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/real_optlay.py
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/rhosyg.py
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/rotation_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/rotation_matrix_nonint.py
--rw-r--r--   0 runner    (1001) docker     (121)     2232 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/subspace_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/symprec_noise.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.329716 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/
--rw-r--r--   0 runner    (1001) docker     (121)     2695 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_brmix.py
--rw-r--r--   0 runner    (1001) docker     (121)     3409 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_eddrmm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_frozen.py
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_incorrect_smearing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1696 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_large_sigma.py
--rw-r--r--   0 runner    (1001) docker     (121)     1540 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_mesh_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (121)     2621 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_nonconverging.py
--rw-r--r--   0 runner    (1001) docker     (121)     1598 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_positive_energy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_potim.py
--rw-r--r--   0 runner    (1001) docker     (121)     1436 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_tetrahedron_mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_unconverged.py
--rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_zpotrf.py
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/tetirr.py
--rw-r--r--   0 runner    (1001) docker     (121)     2121 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/tetrahedron_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.329716 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/to_do/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/to_do/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     4662 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/to_do/aliasing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/to_do/drift.py
--rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/to_do/lrf_commutor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/to_do/scan_metal.py
--rw-r--r--   0 runner    (1001) docker     (121)     2625 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/to_do/standard_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/triple_product.py
--rw-r--r--   0 runner    (1001) docker     (121)     5462 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/unconverged.py
--rw-r--r--   0 runner    (1001) docker     (121)     9530 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/walltime.py
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/zbrent.py
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/zheev.py
--rw-r--r--   0 runner    (1001) docker     (121)     3278 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/zpotrf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.329716 simmate-0.8.0/src/simmate/calculators/vasp/inputs/
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/inputs/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16534 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/inputs/dev_notes.md
--rw-r--r--   0 runner    (1001) docker     (121)    20736 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/inputs/incar.py
--rw-r--r--   0 runner    (1001) docker     (121)    10336 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/inputs/incar_modifiers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4412 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/inputs/kpoints.py
--rw-r--r--   0 runner    (1001) docker     (121)    15442 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/inputs/poscar.py
--rw-r--r--   0 runner    (1001) docker     (121)     3358 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/inputs/potcar.py
--rw-r--r--   0 runner    (1001) docker     (121)     6187 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/inputs/potcar_mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.333716 simmate-0.8.0/src/simmate/calculators/vasp/inputs/test/
--rw-r--r--   0 runner    (1001) docker     (121)     8195 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/inputs/test/test_incar.py
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/inputs/test/test_poscar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.333716 simmate-0.8.0/src/simmate/calculators/vasp/outputs/
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/outputs/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10369 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/outputs/oszicar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.333716 simmate-0.8.0/src/simmate/calculators/vasp/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1474 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/all.py
--rw-r--r--   0 runner    (1001) docker     (121)    13840 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4107 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/customized.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.333716 simmate-0.8.0/src/simmate/calculators/vasp/workflows/diffusion/
--rw-r--r--   0 runner    (1001) docker     (121)     2689 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/diffusion/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/diffusion/all.py
--rw-r--r--   0 runner    (1001) docker     (121)     9402 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/diffusion/neb_all_paths_mit.py
--rw-r--r--   0 runner    (1001) docker     (121)     5394 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/diffusion/neb_from_endpoints_mit.py
--rw-r--r--   0 runner    (1001) docker     (121)    14463 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/diffusion/neb_from_images_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/diffusion/neb_from_images_mit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/diffusion/neb_from_images_mvl_ci.py
--rw-r--r--   0 runner    (1001) docker     (121)     4616 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/diffusion/neb_single_path_mit.py
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/diffusion/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.333716 simmate-0.8.0/src/simmate/calculators/vasp/workflows/dynamics/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/dynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/dynamics/all.py
--rw-r--r--   0 runner    (1001) docker     (121)     1905 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/dynamics/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2904 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/dynamics/matproj.py
--rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/dynamics/mit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/dynamics/mvl_npt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.333716 simmate-0.8.0/src/simmate/calculators/vasp/workflows/elastic/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/elastic/mvl.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.333716 simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/all.py
--rw-r--r--   0 runner    (1001) docker     (121)     3836 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/base_band_structure.py
--rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/base_density_of_states.py
--rw-r--r--   0 runner    (1001) docker     (121)     2387 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/base_full.py
--rw-r--r--   0 runner    (1001) docker     (121)      895 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_band_structure.py
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_band_structure_hse.py
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_density_of_states.py
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_density_of_states_hse.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_full.py
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_hse_full.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.333716 simmate-0.8.0/src/simmate/calculators/vasp/workflows/nuclear_magnetic_resonance/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/nuclear_magnetic_resonance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/nuclear_magnetic_resonance/all.py
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/nuclear_magnetic_resonance/matproj_chemical_shifts.py
--rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/nuclear_magnetic_resonance/matproj_field_gradient.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.337716 simmate-0.8.0/src/simmate/calculators/vasp/workflows/population_analysis/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/population_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/population_analysis/all.py
--rw-r--r--   0 runner    (1001) docker     (121)     6687 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/population_analysis/badelf.py
--rw-r--r--   0 runner    (1001) docker     (121)     3323 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/population_analysis/bader.py
--rw-r--r--   0 runner    (1001) docker     (121)     5312 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/population_analysis/elf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.337716 simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/all.py
--rw-r--r--   0 runner    (1001) docker     (121)     4933 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/matproj.py
--rw-r--r--   0 runner    (1001) docker     (121)     3280 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/matproj_hse.py
--rw-r--r--   0 runner    (1001) docker     (121)      723 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/matproj_metal.py
--rw-r--r--   0 runner    (1001) docker     (121)     3735 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/matproj_scan.py
--rw-r--r--   0 runner    (1001) docker     (121)     5889 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/mit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/mvl_grainboundary.py
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/mvl_neb_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/mvl_slab.py
--rw-r--r--   0 runner    (1001) docker     (121)     2068 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/quality00.py
--rw-r--r--   0 runner    (1001) docker     (121)     2070 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/quality01.py
--rw-r--r--   0 runner    (1001) docker     (121)     2105 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/quality02.py
--rw-r--r--   0 runner    (1001) docker     (121)     2050 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/quality03.py
--rw-r--r--   0 runner    (1001) docker     (121)     2248 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/quality04.py
--rw-r--r--   0 runner    (1001) docker     (121)     3128 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/staged.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.337716 simmate-0.8.0/src/simmate/calculators/vasp/workflows/static_energy/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/static_energy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/static_energy/all.py
--rw-r--r--   0 runner    (1001) docker     (121)      916 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/static_energy/matproj.py
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/static_energy/matproj_hse.py
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/static_energy/matproj_scan.py
--rw-r--r--   0 runner    (1001) docker     (121)      808 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/static_energy/mit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/static_energy/mvl_neb_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     1656 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/static_energy/quality04.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.337716 simmate-0.8.0/src/simmate/calculators/vasp/workflows/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1538 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/test/test_all_paths.py
--rw-r--r--   0 runner    (1001) docker     (121)     1824 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/test/test_band_structure.py
--rw-r--r--   0 runner    (1001) docker     (121)     2378 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)      738 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/test/test_density_of_states.py
--rw-r--r--   0 runner    (1001) docker     (121)     2364 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/test/test_nudged_elastic_band.py
--rw-r--r--   0 runner    (1001) docker     (121)     8256 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/calculators/vasp/workflows/test/test_pymatgen_sets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.337716 simmate-0.8.0/src/simmate/command_line/
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/command_line/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/command_line/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1368 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/command_line/base_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     5169 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/command_line/database.py
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/command_line/run_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     2205 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/command_line/start_project.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.341716 simmate-0.8.0/src/simmate/command_line/test/
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/command_line/test/test_base_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/command_line/test/test_database_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/command_line/test/test_worker_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     7472 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/command_line/test/test_workflows_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2414 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/command_line/workflow_engine.py
--rw-r--r--   0 runner    (1001) docker     (121)     5645 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/command_line/workflow_engine_prefect.py
--rw-r--r--   0 runner    (1001) docker     (121)    12040 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/command_line/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.341716 simmate-0.8.0/src/simmate/configuration/
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.341716 simmate-0.8.0/src/simmate/configuration/dask/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/dask/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/dask/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4938 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/dask/connect_to_database.py
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/dask/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2546 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/dask/setup_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/dask/submit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.341716 simmate-0.8.0/src/simmate/configuration/django/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/django/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17982 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/django/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/django/settings_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1626 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/django/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.341716 simmate-0.8.0/src/simmate/configuration/example_configs/
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/example_configs/applications.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/example_configs/dask_cluster.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      639 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/example_configs/database.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/example_configs/executor.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/example_configs/prefect_agent.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.341716 simmate-0.8.0/src/simmate/configuration/example_configs/sqlite-prebuilds/
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/example_configs/sqlite-prebuilds/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.317716 simmate-0.8.0/src/simmate/configuration/example_configs/vasp/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.341716 simmate-0.8.0/src/simmate/configuration/example_configs/vasp/Potentials/
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/example_configs/vasp/Potentials/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.341716 simmate-0.8.0/src/simmate/configuration/example_project/
--rw-r--r--   0 runner    (1001) docker     (121)     2874 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/example_project/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.341716 simmate-0.8.0/src/simmate/configuration/example_project/example_app/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/example_project/example_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/example_project/example_app/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/example_project/example_app/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/example_project/example_app/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/example_project/example_app/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/example_project/example_app/views.py
--rw-r--r--   0 runner    (1001) docker     (121)     4553 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/example_project/example_app/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.341716 simmate-0.8.0/src/simmate/configuration/prefect/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/prefect/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/prefect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/configuration/prefect/connect_to_dask.py
--rw-r--r--   0 runner    (1001) docker     (121)     8137 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.341716 simmate-0.8.0/src/simmate/database/
--rw-r--r--   0 runner    (1001) docker     (121)     5807 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.345716 simmate-0.8.0/src/simmate/database/base_data_types/
--rw-r--r--   0 runner    (1001) docker     (121)     4883 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      848 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6458 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/_to_do.md
--rw-r--r--   0 runner    (1001) docker     (121)     6675 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/band_structure.py
--rw-r--r--   0 runner    (1001) docker     (121)    34874 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7526 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/calculation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2062 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/calculation_customized.py
--rw-r--r--   0 runner    (1001) docker     (121)     4882 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/calculation_nested.py
--rw-r--r--   0 runner    (1001) docker     (121)     6374 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/density_of_states.py
--rw-r--r--   0 runner    (1001) docker     (121)     5651 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (121)     3056 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/forces.py
--rw-r--r--   0 runner    (1001) docker     (121)    16788 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/nudged_elastic_band.py
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/population_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)    14544 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/relaxation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4704 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/static_energy.py
--rw-r--r--   0 runner    (1001) docker     (121)     7601 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/structure.py
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/symmetry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.345716 simmate-0.8.0/src/simmate/database/base_data_types/test/
--rw-r--r--   0 runner    (1001) docker     (121)     2436 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/test/test_base_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/test/test_calculation_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     1382 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/test/test_dynamics_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     1434 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/test/test_forces_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/test/test_relaxation_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     1703 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/test/test_static_energy_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/test/test_structure_db.py
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/test/test_symmetry_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     1237 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/test/test_thermodynamics_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     6818 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/base_data_types/thermodynamics.py
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/connect.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.345716 simmate-0.8.0/src/simmate/database/third_parties/
--rw-r--r--   0 runner    (1001) docker     (121)     3672 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/third_parties/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/third_parties/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.345716 simmate-0.8.0/src/simmate/database/third_parties/aflow/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/third_parties/aflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3081 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/third_parties/aflow/prototypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1446 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/third_parties/aflow/structures.py
--rw-r--r--   0 runner    (1001) docker     (121)     2426 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/third_parties/cod.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.345716 simmate-0.8.0/src/simmate/database/third_parties/for_providers/
--rw-r--r--   0 runner    (1001) docker     (121)    18615 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/third_parties/for_providers/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/third_parties/for_providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.349717 simmate-0.8.0/src/simmate/database/third_parties/for_providers/_todo/
--rw-r--r--   0 runner    (1001) docker     (121)      939 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/third_parties/for_providers/_todo/materials_cloud.py
--rw-r--r--   0 runner    (1001) docker     (121)     2207 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/third_parties/for_providers/_todo/mpds.py
--rw-r--r--   0 runner    (1001) docker     (121)     3935 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/third_parties/for_providers/aflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     1807 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/third_parties/for_providers/aflow_prototypes.py
--rw-r--r--   0 runner    (1001) docker     (121)    26060 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/third_parties/for_providers/cod.py
--rw-r--r--   0 runner    (1001) docker     (121)     2588 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/third_parties/for_providers/jarvis.py
--rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/third_parties/for_providers/materials_project.py
--rw-r--r--   0 runner    (1001) docker     (121)     6324 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/third_parties/for_providers/oqmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/third_parties/jarvis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/third_parties/materials_project.py
--rw-r--r--   0 runner    (1001) docker     (121)     1499 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/third_parties/oqmd.py
--rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/third_parties/utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)     4397 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.349717 simmate-0.8.0/src/simmate/database/workflow_results/
--rw-r--r--   0 runner    (1001) docker     (121)     1661 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/workflow_results/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/database/workflow_results/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.349717 simmate-0.8.0/src/simmate/file_converters/
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/file_converters/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/file_converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.349717 simmate-0.8.0/src/simmate/file_converters/molecule/
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/file_converters/molecule/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/file_converters/molecule/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.349717 simmate-0.8.0/src/simmate/file_converters/structure/
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/file_converters/structure/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/file_converters/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/file_converters/structure/ase.py
--rw-r--r--   0 runner    (1001) docker     (121)      842 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/file_converters/structure/cif.py
--rw-r--r--   0 runner    (1001) docker     (121)     7570 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/file_converters/structure/database.py
--rw-r--r--   0 runner    (1001) docker     (121)      757 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/file_converters/structure/jarvis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1392 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/file_converters/structure/pymatgen.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.349717 simmate-0.8.0/src/simmate/file_converters/voxeldata/
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/file_converters/voxeldata/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/file_converters/voxeldata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.349717 simmate-0.8.0/src/simmate/toolkit/
--rw-r--r--   0 runner    (1001) docker     (121)     1983 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.349717 simmate-0.8.0/src/simmate/toolkit/base_data_types/
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/base_data_types/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/base_data_types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.349717 simmate-0.8.0/src/simmate/toolkit/base_data_types/_to_do/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/base_data_types/_to_do/README.md
--rw-r--r--   0 runner    (1001) docker     (121)   182930 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/base_data_types/_to_do/element_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    11660 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/base_data_types/_to_do/elements.py
--rw-r--r--   0 runner    (1001) docker     (121)     5080 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/base_data_types/_to_do/lattice.py
--rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/base_data_types/_to_do/species.py
--rw-r--r--   0 runner    (1001) docker     (121)     9382 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/base_data_types/composition.py
--rw-r--r--   0 runner    (1001) docker     (121)     6195 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/base_data_types/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.349717 simmate-0.8.0/src/simmate/toolkit/base_data_types/test/
--rw-r--r--   0 runner    (1001) docker     (121)     2427 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/base_data_types/test/test_composition.py
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/base_data_types/test/test_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.349717 simmate-0.8.0/src/simmate/toolkit/creators/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14387 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/lattice.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.349717 simmate-0.8.0/src/simmate/toolkit/creators/sites/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1777 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/sites/random.py
--rw-r--r--   0 runner    (1001) docker     (121)    11305 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/sites/random_wyckoff.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.349717 simmate-0.8.0/src/simmate/toolkit/creators/structure/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/structure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.353716 simmate-0.8.0/src/simmate/toolkit/creators/structure/_todo/
--rw-r--r--   0 runner    (1001) docker     (121)     9654 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/structure/_todo/random_symmetry_walk.py
--rw-r--r--   0 runner    (1001) docker     (121)     4441 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/structure/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    14600 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/structure/prototypes.py
--rw-r--r--   0 runner    (1001) docker     (121)    14350 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/structure/random_symmetry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.353716 simmate-0.8.0/src/simmate/toolkit/creators/structure/third_party/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/structure/third_party/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.353716 simmate-0.8.0/src/simmate/toolkit/creators/structure/third_party/_to_do/
--rw-r--r--   0 runner    (1001) docker     (121)     4676 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/structure/third_party/_to_do/airss.py
--rw-r--r--   0 runner    (1001) docker     (121)     4998 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/structure/third_party/_to_do/ase.py
--rw-r--r--   0 runner    (1001) docker     (121)    10766 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/structure/third_party/_to_do/calypso.py
--rw-r--r--   0 runner    (1001) docker     (121)     4496 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/structure/third_party/_to_do/gasp.py
--rw-r--r--   0 runner    (1001) docker     (121)    13086 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/structure/third_party/_to_do/uspex.py
--rw-r--r--   0 runner    (1001) docker     (121)     6001 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/structure/third_party/_to_do/xtalopt.py
--rw-r--r--   0 runner    (1001) docker     (121)     4643 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/structure/third_party/pyxtal.py
--rw-r--r--   0 runner    (1001) docker     (121)     6266 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.353716 simmate-0.8.0/src/simmate/toolkit/creators/vector/
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2808 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/vector/normal_distribution.py
--rw-r--r--   0 runner    (1001) docker     (121)     2140 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/creators/vector/uniform_distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.353716 simmate-0.8.0/src/simmate/toolkit/diffusion/
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/diffusion/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4645 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/diffusion/migration_hop.py
--rw-r--r--   0 runner    (1001) docker     (121)    12254 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/diffusion/migration_images.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.353716 simmate-0.8.0/src/simmate/toolkit/structure_prediction/
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/structure_prediction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.353716 simmate-0.8.0/src/simmate/toolkit/structure_prediction/evolution/
--rw-r--r--   0 runner    (1001) docker     (121)     1948 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/structure_prediction/evolution/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/structure_prediction/evolution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12746 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/structure_prediction/evolution/database.py
--rw-r--r--   0 runner    (1001) docker     (121)    27312 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/structure_prediction/evolution/search_engine.py
--rw-r--r--   0 runner    (1001) docker     (121)     2564 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/structure_prediction/evolution/selectors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2093 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/structure_prediction/evolution/stop_conditions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4736 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/structure_prediction/evolution/triggered_actions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/structure_prediction/known.py
--rw-r--r--   0 runner    (1001) docker     (121)     1142 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/structure_prediction/prototypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     7012 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/structure_prediction/substitution.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.353716 simmate-0.8.0/src/simmate/toolkit/symmetry/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/symmetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16344 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/symmetry/asymdata.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.353716 simmate-0.8.0/src/simmate/toolkit/symmetry/webscraper/
--rw-r--r--   0 runner    (1001) docker     (121)     2589 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/symmetry/webscraper/aflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     6166 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/symmetry/webscraper/bilbao_wyckoff.py
--rw-r--r--   0 runner    (1001) docker     (121)    12837 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/symmetry/webscraper/itc_datascrape.py
--rw-r--r--   0 runner    (1001) docker     (121)    11897 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/symmetry/wyckoff.py
--rw-r--r--   0 runner    (1001) docker     (121)    44585 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/symmetry/wyckoffdata.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.353716 simmate-0.8.0/src/simmate/toolkit/transformations/
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/transformations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4186 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/transformations/atomic_permutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2619 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/transformations/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/transformations/coordinate_perturation_ordered.py
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/transformations/coordinate_perturbation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.357717 simmate-0.8.0/src/simmate/toolkit/transformations/from_ase/
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/transformations/from_ase/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/transformations/from_ase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2984 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/transformations/from_ase/atomic_permutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2702 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/transformations/from_ase/coordinate_perturbation.py
--rw-r--r--   0 runner    (1001) docker     (121)     5549 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/transformations/from_ase/heredity_mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2898 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/transformations/from_ase/lattice_strain.py
--rw-r--r--   0 runner    (1001) docker     (121)     2804 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/transformations/from_ase/mirror_mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2880 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/transformations/from_ase/rotational_mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4658 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/transformations/from_ase/soft_mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2834 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/transformations/lattice_strain.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.357717 simmate-0.8.0/src/simmate/toolkit/validators/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/validators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.357717 simmate-0.8.0/src/simmate/toolkit/validators/fingerprint/
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/validators/fingerprint/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/validators/fingerprint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.357717 simmate-0.8.0/src/simmate/toolkit/validators/fingerprint/_to_do/
--rw-r--r--   0 runner    (1001) docker     (121)     6654 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/validators/fingerprint/_to_do/ase.py
--rw-r--r--   0 runner    (1001) docker     (121)     4217 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/validators/fingerprint/_to_do/crystalnn.py
--rw-r--r--   0 runner    (1001) docker     (121)     5004 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/validators/fingerprint/_to_do/prdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4377 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/validators/fingerprint/_to_do/rdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     7132 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/validators/fingerprint/pcrystalnn.py
--rw-r--r--   0 runner    (1001) docker     (121)     5668 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/toolkit/validators/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.357717 simmate-0.8.0/src/simmate/utilities/
--rw-r--r--   0 runner    (1001) docker     (121)      363 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/utilities/async_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)    10343 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/utilities/files.py
--rw-r--r--   0 runner    (1001) docker     (121)     4015 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/utilities/other.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.357717 simmate-0.8.0/src/simmate/utilities/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/utilities/test/test_files.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.357717 simmate-0.8.0/src/simmate/visualization/
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/visualization/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.357717 simmate-0.8.0/src/simmate/visualization/structure/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/visualization/structure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.357717 simmate-0.8.0/src/simmate/visualization/structure/blender/
--rw-r--r--   0 runner    (1001) docker     (121)     4432 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/visualization/structure/blender/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/visualization/structure/blender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6189 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/visualization/structure/blender/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6437 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/visualization/structure/blender/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.357717 simmate-0.8.0/src/simmate/visualization/structure/blender/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)    12054 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/visualization/structure/blender/scripts/make_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.357717 simmate-0.8.0/src/simmate/visualization/structure/blender/test/
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/visualization/structure/blender/test/test_blender.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.357717 simmate-0.8.0/src/simmate/website/
--rw-r--r--   0 runner    (1001) docker     (121)    10246 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.357717 simmate-0.8.0/src/simmate/website/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.357717 simmate-0.8.0/src/simmate/website/core/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core/test/test_core_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     4693 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core/views.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.361717 simmate-0.8.0/src/simmate/website/core_components/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     9375 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/base_api_view.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.361717 simmate-0.8.0/src/simmate/website/core_components/filters/
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/filters/band_structure.py
--rw-r--r--   0 runner    (1001) docker     (121)     5109 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/filters/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/filters/calculation.py
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/filters/density_of_states.py
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/filters/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/filters/forces.py
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/filters/nudged_elastic_band.py
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/filters/relaxation.py
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/filters/static_energy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3502 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/filters/structure.py
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/filters/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/filters/thermodynamics.py
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.361717 simmate-0.8.0/src/simmate/website/core_components/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/templatetags/chemical_formula_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)      997 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/templatetags/markdown_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/templatetags/matplotlib_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1796 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/templatetags/structure_serialize_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.361717 simmate-0.8.0/src/simmate/website/core_components/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/test/test_cc_views.py
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     4383 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/core_components/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.321716 simmate-0.8.0/src/simmate/website/static_files/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.361717 simmate-0.8.0/src/simmate/website/static_files/images/
--rw-r--r--   0 runner    (1001) docker     (121)     5171 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/static_files/images/dask-icon.svg
--rw-r--r--   0 runner    (1001) docker     (121)     6785 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/static_files/images/dask-logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1781 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/static_files/images/digitalocean-icon.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3776 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/static_files/images/digitalocean-logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/static_files/images/django-icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.361717 simmate-0.8.0/src/simmate/website/static_files/images/geometry_templates/
--rw-r--r--   0 runner    (1001) docker     (121)     2732 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/static_files/images/geometry_templates/cube.svg
--rw-r--r--   0 runner    (1001) docker     (121)     5373 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/static_files/images/geometry_templates/octahedron.svg
--rw-r--r--   0 runner    (1001) docker     (121)     5257 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/static_files/images/geometry_templates/tetrahedron.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2069 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/static_files/images/github-icon.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3999 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/static_files/images/prefect-icon.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2866 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/static_files/images/prefect-logo.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7157 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/static_files/images/simmate-geometries.svg
--rw-r--r--   0 runner    (1001) docker     (121)     3012 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/static_files/images/simmate-icon.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7818 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/static_files/images/simmate-logo-dark.svg
--rw-r--r--   0 runner    (1001) docker     (121)    20638 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/static_files/images/simmate-logo-other-ideas.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7777 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/static_files/images/simmate-logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.361717 simmate-0.8.0/src/simmate/website/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     1344 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (121)     1439 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/500.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.361717 simmate-0.8.0/src/simmate/website/templates/account/
--rw-r--r--   0 runner    (1001) docker     (121)     4408 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/account/login.html
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/account/loginstatus.html
--rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/account/logout.html
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/account/profile.html
--rw-r--r--   0 runner    (1001) docker     (121)     2298 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/account/signup.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.365717 simmate-0.8.0/src/simmate/website/templates/core_components/
--rw-r--r--   0 runner    (1001) docker     (121)     6580 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/about.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.365717 simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/band-structure-calc.html
--rw-r--r--   0 runner    (1001) docker     (121)      791 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/band-structure.html
--rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/calculation.html
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/density-of-states-calc.html
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/density-of-states.html
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/diffusion-analysis.html
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/dynamics-run.html
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/forces.html
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/relaxation.html
--rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/static-energy.html
--rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/structure.html
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/thermodynamics.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.365717 simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/band-structure-calc.html
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/band-structure.html
--rw-r--r--   0 runner    (1001) docker     (121)      778 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/calculation.html
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/density-of-states-calc.html
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/density-of-states.html
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/diffusion-analysis.html
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/dynamics-run.html
--rw-r--r--   0 runner    (1001) docker     (121)      853 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/forces.html
--rw-r--r--   0 runner    (1001) docker     (121)     1845 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/relaxation.html
--rw-r--r--   0 runner    (1001) docker     (121)     1388 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/static-energy.html
--rw-r--r--   0 runner    (1001) docker     (121)     3421 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/structure.html
--rw-r--r--   0 runner    (1001) docker     (121)      939 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/thermodynamics.html
--rw-r--r--   0 runner    (1001) docker     (121)     4072 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/contact.html
--rw-r--r--   0 runner    (1001) docker     (121)     4123 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/datatable.html
--rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/extras.html
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/footer.html
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/footerbar.html
--rw-r--r--   0 runner    (1001) docker     (121)     7893 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/navbar.html
--rw-r--r--   0 runner    (1001) docker     (121)    36678 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/periodic_table.html
--rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/search_form.html
--rw-r--r--   0 runner    (1001) docker     (121)     2133 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/search_results_pagination.html
--rw-r--r--   0 runner    (1001) docker     (121)     3183 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/sidebar.html
--rw-r--r--   0 runner    (1001) docker     (121)     2724 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/site_base.html
--rw-r--r--   0 runner    (1001) docker     (121)     5580 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/structure_viewer.html
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/table_entry.html
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/core_components/test.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.365717 simmate-0.8.0/src/simmate/website/templates/home/
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/home/home.html
--rw-r--r--   0 runner    (1001) docker     (121)     3861 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/home/search-form.html
--rw-r--r--   0 runner    (1001) docker     (121)     3946 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/home/search-results.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.369717 simmate-0.8.0/src/simmate/website/templates/third_parties/
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/third_parties/entry_detail.html
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/third_parties/provider.html
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/third_parties/providers_all.html
--rw-r--r--   0 runner    (1001) docker     (121)     2227 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/third_parties/search_results.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.369717 simmate-0.8.0/src/simmate/website/templates/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/workflows/all.html
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/workflows/by_type.html
--rw-r--r--   0 runner    (1001) docker     (121)     1960 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/workflows/detail.html
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/workflows/detail_run.html
--rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/workflows/search_results.html
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/templates/workflows/submit.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.369717 simmate-0.8.0/src/simmate/website/test_app/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/test_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/test_app/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/test_app/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.369717 simmate-0.8.0/src/simmate/website/third_parties/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/third_parties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/third_parties/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     3200 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/third_parties/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/third_parties/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.369717 simmate-0.8.0/src/simmate/website/third_parties/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/third_parties/test/test_third_parties_views.py
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/third_parties/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/third_parties/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.369717 simmate-0.8.0/src/simmate/website/workflow_engine/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/workflow_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/workflow_engine/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/workflow_engine/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.369717 simmate-0.8.0/src/simmate/website/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/workflows/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     8024 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/workflows/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/workflows/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.369717 simmate-0.8.0/src/simmate/website/workflows/test/
--rw-r--r--   0 runner    (1001) docker     (121)     3769 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/workflows/test/test_workflows_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/workflows/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     5671 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/website/workflows/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.369717 simmate-0.8.0/src/simmate/workflow_engine/
--rw-r--r--   0 runner    (1001) docker     (121)     4499 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflow_engine/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflow_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8378 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflow_engine/error_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.369717 simmate-0.8.0/src/simmate/workflow_engine/execution/
--rw-r--r--   0 runner    (1001) docker     (121)     1411 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflow_engine/execution/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflow_engine/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3026 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflow_engine/execution/database.py
--rw-r--r--   0 runner    (1001) docker     (121)     6676 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflow_engine/execution/executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     4939 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflow_engine/execution/future.py
--rw-r--r--   0 runner    (1001) docker     (121)     8009 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflow_engine/execution/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.369717 simmate-0.8.0/src/simmate/workflow_engine/execution_prefect/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflow_engine/execution_prefect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9865 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflow_engine/execution_prefect/worker.py
--rw-r--r--   0 runner    (1001) docker     (121)     9608 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflow_engine/execution_prefect/workflow.py
--rw-r--r--   0 runner    (1001) docker     (121)    33964 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflow_engine/s3_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.373717 simmate-0.8.0/src/simmate/workflow_engine/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflow_engine/test/test_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     7377 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflow_engine/test/test_s3_workflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     3858 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflow_engine/test/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     2982 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflow_engine/utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    45870 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflow_engine/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.373717 simmate-0.8.0/src/simmate/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     3361 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflows/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflows/customized.py
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflows/diffusion.py
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflows/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflows/electronic_structure.py
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflows/population_analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflows/relaxation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2311 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflows/restart.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflows/static_energy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.373717 simmate-0.8.0/src/simmate/workflows/test/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.373717 simmate-0.8.0/src/simmate/workflows/test/simmate-task-ERROR/
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflows/test/simmate-task-ERROR/simmate_metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4772 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflows/test/test_all_workflow_runs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3773 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflows/test/test_workflows_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    10347 2022-08-11 21:23:38.000000 simmate-0.8.0/src/simmate/workflows/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 21:23:48.325716 simmate-0.8.0/src/simmate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      868 2022-08-11 21:23:48.000000 simmate-0.8.0/src/simmate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    30020 2022-08-11 21:23:48.000000 simmate-0.8.0/src/simmate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-11 21:23:48.000000 simmate-0.8.0/src/simmate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-08-11 21:23:48.000000 simmate-0.8.0/src/simmate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-08-11 21:23:48.000000 simmate-0.8.0/src/simmate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-11 21:23:48.000000 simmate-0.8.0/src/simmate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.631188 simmate-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-08-17 16:40:21.000000 simmate-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      868 2022-08-17 16:40:39.631188 simmate-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    12777 2022-08-17 16:40:21.000000 simmate-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     8698 2022-08-17 16:40:21.000000 simmate-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-17 16:40:39.631188 simmate-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.575188 simmate-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.583187 simmate-0.9.0/src/simmate/
+-rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      845 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.583187 simmate-0.9.0/src/simmate/calculators/
+-rw-r--r--   0 runner    (1001) docker     (121)     1767 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.583187 simmate-0.9.0/src/simmate/calculators/bader/
+-rw-r--r--   0 runner    (1001) docker     (121)     1657 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/bader/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/bader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/bader/inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.583187 simmate-0.9.0/src/simmate/calculators/bader/outputs/
+-rw-r--r--   0 runner    (1001) docker     (121)      112 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/bader/outputs/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      138 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/bader/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1701 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/bader/outputs/acf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.583187 simmate-0.9.0/src/simmate/calculators/bader/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/bader/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1670 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/bader/workflows/badelf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5079 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/bader/workflows/bader.py
+-rw-r--r--   0 runner    (1001) docker     (121)      724 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/bader/workflows/combine_chgcars.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.583187 simmate-0.9.0/src/simmate/calculators/deepmd/
+-rw-r--r--   0 runner    (1001) docker     (121)      611 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/deepmd/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/deepmd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.583187 simmate-0.9.0/src/simmate/calculators/deepmd/inputs/
+-rw-r--r--   0 runner    (1001) docker     (121)       65 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/deepmd/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1851 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/deepmd/inputs/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9610 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/deepmd/inputs/type_and_set.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.583187 simmate-0.9.0/src/simmate/calculators/vasp/
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5441 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/configuration.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.587187 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1434 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      925 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/brions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5768 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/brmix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/edddav.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2922 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/eddrmm.py
+-rw-r--r--   0 runner    (1001) docker     (121)      984 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/edwav.py
+-rw-r--r--   0 runner    (1001) docker     (121)      706 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/elf_kpar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3755 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/frozen.py
+-rw-r--r--   0 runner    (1001) docker     (121)      840 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/incorrect_shift.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/incorrect_smearing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1566 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/insufficient_bands.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4102 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/large_sigma.py
+-rw-r--r--   0 runner    (1001) docker     (121)      877 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/long_vector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3673 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/mesh_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5919 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/nonconverging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/point_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3699 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/positive_energy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/posmap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3200 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/potim.py
+-rw-r--r--   0 runner    (1001) docker     (121)      844 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/pricel.py
+-rw-r--r--   0 runner    (1001) docker     (121)      808 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/pssyevx.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/real_optlay.py
+-rw-r--r--   0 runner    (1001) docker     (121)      920 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/rhosyg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      938 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/rotation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/rotation_matrix_nonint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2232 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/subspace_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/symprec_noise.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.587187 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     2695 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_brmix.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3409 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_eddrmm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_frozen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_incorrect_smearing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1696 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_large_sigma.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1540 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_mesh_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2621 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_nonconverging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1598 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_positive_energy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1443 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_potim.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1436 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_tetrahedron_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_unconverged.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_zpotrf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      778 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/tetirr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2121 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/tetrahedron_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.587187 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/to_do/
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/to_do/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     4662 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/to_do/aliasing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/to_do/drift.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/to_do/lrf_commutor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/to_do/scan_metal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2625 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/to_do/standard_error.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/triple_product.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5462 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/unconverged.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9577 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/walltime.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/zbrent.py
+-rw-r--r--   0 runner    (1001) docker     (121)      821 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/zheev.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3278 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/zpotrf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.591188 simmate-0.9.0/src/simmate/calculators/vasp/inputs/
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/inputs/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16534 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/inputs/dev_notes.md
+-rw-r--r--   0 runner    (1001) docker     (121)    20707 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/inputs/incar.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10336 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/inputs/incar_modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4412 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/inputs/kpoints.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15441 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/inputs/poscar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3355 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/inputs/potcar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6187 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/inputs/potcar_mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.591188 simmate-0.9.0/src/simmate/calculators/vasp/inputs/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     8195 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/inputs/test/test_incar.py
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/inputs/test/test_poscar.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.591188 simmate-0.9.0/src/simmate/calculators/vasp/outputs/
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/outputs/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10369 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/outputs/oszicar.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.591188 simmate-0.9.0/src/simmate/calculators/vasp/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      747 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1468 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/all.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13842 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4128 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/customized.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.591188 simmate-0.9.0/src/simmate/calculators/vasp/workflows/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (121)     2689 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/diffusion/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      367 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/diffusion/all.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9378 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/diffusion/neb_all_paths_mit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5412 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/diffusion/neb_from_endpoints_mit.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14466 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/diffusion/neb_from_images_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/diffusion/neb_from_images_mit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1284 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/diffusion/neb_from_images_mvl_ci.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4634 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/diffusion/neb_single_path_mit.py
+-rw-r--r--   0 runner    (1001) docker     (121)      795 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/diffusion/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.591188 simmate-0.9.0/src/simmate/calculators/vasp/workflows/dynamics/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/dynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      151 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/dynamics/all.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1905 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/dynamics/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2904 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/dynamics/matproj.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/dynamics/mit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/dynamics/mvl_npt.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.591188 simmate-0.9.0/src/simmate/calculators/vasp/workflows/elastic/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      616 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/elastic/mvl.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.595188 simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      293 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/all.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3836 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/base_band_structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/base_density_of_states.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2405 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/base_full.py
+-rw-r--r--   0 runner    (1001) docker     (121)      895 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_band_structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)      817 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_band_structure_hse.py
+-rw-r--r--   0 runner    (1001) docker     (121)      908 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_density_of_states.py
+-rw-r--r--   0 runner    (1001) docker     (121)      829 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_density_of_states_hse.py
+-rw-r--r--   0 runner    (1001) docker     (121)      909 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_full.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_hse_full.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.595188 simmate-0.9.0/src/simmate/calculators/vasp/workflows/nuclear_magnetic_resonance/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/nuclear_magnetic_resonance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/nuclear_magnetic_resonance/all.py
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/nuclear_magnetic_resonance/matproj_chemical_shifts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/nuclear_magnetic_resonance/matproj_field_gradient.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.595188 simmate-0.9.0/src/simmate/calculators/vasp/workflows/population_analysis/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/population_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      297 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/population_analysis/all.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6705 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/population_analysis/badelf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3341 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/population_analysis/bader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5312 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/population_analysis/elf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.595188 simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      756 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/all.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4924 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/matproj.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3271 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/matproj_hse.py
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/matproj_metal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3726 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/matproj_scan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5889 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/mit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/mvl_grainboundary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/mvl_neb_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)      682 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/mvl_slab.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2068 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/quality00.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2070 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/quality01.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2105 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/quality02.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2050 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/quality03.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2248 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/quality04.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6108 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/staged.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.595188 simmate-0.9.0/src/simmate/calculators/vasp/workflows/static_energy/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/static_energy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/static_energy/all.py
+-rw-r--r--   0 runner    (1001) docker     (121)      916 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/static_energy/matproj.py
+-rw-r--r--   0 runner    (1001) docker     (121)      935 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/static_energy/matproj_hse.py
+-rw-r--r--   0 runner    (1001) docker     (121)      643 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/static_energy/matproj_scan.py
+-rw-r--r--   0 runner    (1001) docker     (121)      808 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/static_energy/mit.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/static_energy/mvl_neb_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1656 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/static_energy/quality04.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.595188 simmate-0.9.0/src/simmate/calculators/vasp/workflows/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1539 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/test/test_all_paths.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1824 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/test/test_band_structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2378 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/test/test_density_of_states.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2362 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/test/test_nudged_elastic_band.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8277 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/calculators/vasp/workflows/test/test_pymatgen_sets.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.599187 simmate-0.9.0/src/simmate/command_line/
+-rw-r--r--   0 runner    (1001) docker     (121)      926 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/command_line/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/command_line/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1452 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/command_line/base_command.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4963 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/command_line/database.py
+-rw-r--r--   0 runner    (1001) docker     (121)      620 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/command_line/run_server.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2207 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/command_line/start_project.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.599187 simmate-0.9.0/src/simmate/command_line/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/command_line/test/test_base_command.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/command_line/test/test_database_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/command_line/test/test_worker_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7471 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/command_line/test/test_workflows_cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/command_line/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3012 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/command_line/workflow_engine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5628 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/command_line/workflow_engine_prefect.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12016 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/command_line/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.599187 simmate-0.9.0/src/simmate/configuration/
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.599187 simmate-0.9.0/src/simmate/configuration/dask/
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/dask/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/dask/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4938 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/dask/connect_to_database.py
+-rw-r--r--   0 runner    (1001) docker     (121)      644 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/dask/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2545 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/dask/setup_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/dask/submit.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.599187 simmate-0.9.0/src/simmate/configuration/django/
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/django/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17982 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/django/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      750 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/django/settings_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/django/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.599187 simmate-0.9.0/src/simmate/configuration/example_configs/
+-rw-r--r--   0 runner    (1001) docker     (121)      373 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/example_configs/applications.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/example_configs/dask_cluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      639 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/example_configs/database.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      330 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/example_configs/executor.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/example_configs/prefect_agent.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.599187 simmate-0.9.0/src/simmate/configuration/example_configs/sqlite-prebuilds/
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/example_configs/sqlite-prebuilds/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.575188 simmate-0.9.0/src/simmate/configuration/example_configs/vasp/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.599187 simmate-0.9.0/src/simmate/configuration/example_configs/vasp/Potentials/
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/example_configs/vasp/Potentials/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.599187 simmate-0.9.0/src/simmate/configuration/example_project/
+-rw-r--r--   0 runner    (1001) docker     (121)     2874 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/example_project/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.599187 simmate-0.9.0/src/simmate/configuration/example_project/example_app/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/example_project/example_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      280 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/example_project/example_app/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/example_project/example_app/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      563 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/example_project/example_app/tests.py
+-rw-r--r--   0 runner    (1001) docker     (121)      904 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/example_project/example_app/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1237 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/example_project/example_app/views.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4560 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/example_project/example_app/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.599187 simmate-0.9.0/src/simmate/configuration/prefect/
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/prefect/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/prefect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1364 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/configuration/prefect/connect_to_dask.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8137 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.599187 simmate-0.9.0/src/simmate/database/
+-rw-r--r--   0 runner    (1001) docker     (121)     5807 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.603187 simmate-0.9.0/src/simmate/database/base_data_types/
+-rw-r--r--   0 runner    (1001) docker     (121)     4883 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6458 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/_to_do.md
+-rw-r--r--   0 runner    (1001) docker     (121)     6675 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/band_structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34834 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7526 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/calculation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/calculation_customized.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4857 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/calculation_nested.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6374 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/density_of_states.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5639 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3056 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/forces.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16772 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/nudged_elastic_band.py
+-rw-r--r--   0 runner    (1001) docker     (121)      592 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/population_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14519 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/relaxation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4704 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/static_energy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7584 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2337 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/symmetry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.603187 simmate-0.9.0/src/simmate/database/base_data_types/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     2436 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/test/test_base_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/test/test_calculation_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/test/test_dynamics_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1434 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/test/test_forces_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1357 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/test/test_relaxation_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1702 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/test/test_static_energy_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1295 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/test/test_structure_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)      195 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/test/test_symmetry_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1237 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/test/test_thermodynamics_db.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6775 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/base_data_types/thermodynamics.py
+-rw-r--r--   0 runner    (1001) docker     (121)      534 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/connect.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.603187 simmate-0.9.0/src/simmate/database/third_parties/
+-rw-r--r--   0 runner    (1001) docker     (121)     3672 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/third_parties/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      385 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/third_parties/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.603187 simmate-0.9.0/src/simmate/database/third_parties/aflow/
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/third_parties/aflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3081 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/third_parties/aflow/prototypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1446 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/third_parties/aflow/structures.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2426 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/third_parties/cod.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.603187 simmate-0.9.0/src/simmate/database/third_parties/for_providers/
+-rw-r--r--   0 runner    (1001) docker     (121)    18615 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/third_parties/for_providers/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/third_parties/for_providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.603187 simmate-0.9.0/src/simmate/database/third_parties/for_providers/_todo/
+-rw-r--r--   0 runner    (1001) docker     (121)      939 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/third_parties/for_providers/_todo/materials_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2205 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/third_parties/for_providers/_todo/mpds.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3935 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/third_parties/for_providers/aflow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1806 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/third_parties/for_providers/aflow_prototypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26060 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/third_parties/for_providers/cod.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2587 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/third_parties/for_providers/jarvis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3882 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/third_parties/for_providers/materials_project.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6324 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/third_parties/for_providers/oqmd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1620 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/third_parties/jarvis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/third_parties/materials_project.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1499 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/third_parties/oqmd.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3358 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/third_parties/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4718 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.607187 simmate-0.9.0/src/simmate/database/workflow_results/
+-rw-r--r--   0 runner    (1001) docker     (121)     1661 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/workflow_results/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/database/workflow_results/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.607187 simmate-0.9.0/src/simmate/file_converters/
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/file_converters/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/file_converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.607187 simmate-0.9.0/src/simmate/file_converters/molecule/
+-rw-r--r--   0 runner    (1001) docker     (121)      309 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/file_converters/molecule/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/file_converters/molecule/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.607187 simmate-0.9.0/src/simmate/file_converters/structure/
+-rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/file_converters/structure/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/file_converters/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      719 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/file_converters/structure/ase.py
+-rw-r--r--   0 runner    (1001) docker     (121)      842 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/file_converters/structure/cif.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7570 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/file_converters/structure/database.py
+-rw-r--r--   0 runner    (1001) docker     (121)      757 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/file_converters/structure/jarvis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1393 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/file_converters/structure/pymatgen.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.607187 simmate-0.9.0/src/simmate/file_converters/voxeldata/
+-rw-r--r--   0 runner    (1001) docker     (121)      314 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/file_converters/voxeldata/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/file_converters/voxeldata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.607187 simmate-0.9.0/src/simmate/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (121)     1983 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.607187 simmate-0.9.0/src/simmate/toolkit/base_data_types/
+-rw-r--r--   0 runner    (1001) docker     (121)      454 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/base_data_types/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/base_data_types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.607187 simmate-0.9.0/src/simmate/toolkit/base_data_types/_to_do/
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/base_data_types/_to_do/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)   182930 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/base_data_types/_to_do/element_data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11660 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/base_data_types/_to_do/elements.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5080 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/base_data_types/_to_do/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/base_data_types/_to_do/species.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10049 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/base_data_types/composition.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6195 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/base_data_types/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.607187 simmate-0.9.0/src/simmate/toolkit/base_data_types/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     2427 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/base_data_types/test/test_composition.py
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/base_data_types/test/test_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.607187 simmate-0.9.0/src/simmate/toolkit/creators/
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14387 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/lattice.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.607187 simmate-0.9.0/src/simmate/toolkit/creators/sites/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1777 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/sites/random.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14384 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/sites/random_wyckoff.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.607187 simmate-0.9.0/src/simmate/toolkit/creators/structure/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/structure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.607187 simmate-0.9.0/src/simmate/toolkit/creators/structure/_todo/
+-rw-r--r--   0 runner    (1001) docker     (121)     9655 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/structure/_todo/random_symmetry_walk.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6680 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/structure/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14600 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/structure/prototypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15113 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/structure/random_symmetry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.611188 simmate-0.9.0/src/simmate/toolkit/creators/structure/third_party/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/structure/third_party/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.611188 simmate-0.9.0/src/simmate/toolkit/creators/structure/third_party/_to_do/
+-rw-r--r--   0 runner    (1001) docker     (121)     4676 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/structure/third_party/_to_do/airss.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4997 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/structure/third_party/_to_do/ase.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10766 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/structure/third_party/_to_do/calypso.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4496 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/structure/third_party/_to_do/gasp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13086 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/structure/third_party/_to_do/uspex.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6002 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/structure/third_party/_to_do/xtalopt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4643 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/structure/third_party/pyxtal.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6266 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.611188 simmate-0.9.0/src/simmate/toolkit/creators/vector/
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2808 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/vector/normal_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2140 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/creators/vector/uniform_distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.611188 simmate-0.9.0/src/simmate/toolkit/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/diffusion/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4652 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/diffusion/migration_hop.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12274 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/diffusion/migration_images.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.611188 simmate-0.9.0/src/simmate/toolkit/structure_prediction/
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/structure_prediction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.611188 simmate-0.9.0/src/simmate/toolkit/structure_prediction/evolution/
+-rw-r--r--   0 runner    (1001) docker     (121)     1948 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/structure_prediction/evolution/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/structure_prediction/evolution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.611188 simmate-0.9.0/src/simmate/toolkit/structure_prediction/evolution/database/
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/structure_prediction/evolution/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32966 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/structure_prediction/evolution/database/evolutionary_search.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6365 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/structure_prediction/evolution/database/structure_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4463 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/structure_prediction/evolution/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2093 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/structure_prediction/evolution/stop_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4736 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/structure_prediction/evolution/triggered_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.611188 simmate-0.9.0/src/simmate/toolkit/structure_prediction/evolution/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/structure_prediction/evolution/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      173 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/structure_prediction/evolution/workflows/all.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9191 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/structure_prediction/evolution/workflows/fixed_composition.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/structure_prediction/evolution/workflows/new_individual.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1446 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/structure_prediction/known.py
+-rw-r--r--   0 runner    (1001) docker     (121)      682 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/structure_prediction/prototypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7695 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/structure_prediction/substitution.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.611188 simmate-0.9.0/src/simmate/toolkit/symmetry/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/symmetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16344 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/symmetry/asymdata.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.611188 simmate-0.9.0/src/simmate/toolkit/symmetry/webscraper/
+-rw-r--r--   0 runner    (1001) docker     (121)     2589 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/symmetry/webscraper/aflow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6166 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/symmetry/webscraper/bilbao_wyckoff.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12837 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/symmetry/webscraper/itc_datascrape.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11898 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/symmetry/wyckoff.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44585 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/symmetry/wyckoffdata.csv
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.615188 simmate-0.9.0/src/simmate/toolkit/transformations/
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/transformations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4185 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/transformations/atomic_permutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6154 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/transformations/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      854 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/transformations/coordinate_perturation_ordered.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/transformations/coordinate_perturbation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.615188 simmate-0.9.0/src/simmate/toolkit/transformations/from_ase/
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/transformations/from_ase/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/transformations/from_ase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2984 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/transformations/from_ase/atomic_permutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2702 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/transformations/from_ase/coordinate_perturbation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5547 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/transformations/from_ase/heredity_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2898 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/transformations/from_ase/lattice_strain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2804 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/transformations/from_ase/mirror_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2880 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/transformations/from_ase/rotational_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4658 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/transformations/from_ase/soft_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2834 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/transformations/lattice_strain.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.615188 simmate-0.9.0/src/simmate/toolkit/validators/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/validators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.615188 simmate-0.9.0/src/simmate/toolkit/validators/fingerprint/
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/validators/fingerprint/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/validators/fingerprint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.615188 simmate-0.9.0/src/simmate/toolkit/validators/fingerprint/_to_do/
+-rw-r--r--   0 runner    (1001) docker     (121)     6652 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/validators/fingerprint/_to_do/ase.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4216 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/validators/fingerprint/_to_do/crystalnn.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5004 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/validators/fingerprint/_to_do/prdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4377 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/validators/fingerprint/_to_do/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7135 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/validators/fingerprint/pcrystalnn.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5669 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/toolkit/validators/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.615188 simmate-0.9.0/src/simmate/utilities/
+-rw-r--r--   0 runner    (1001) docker     (121)      363 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      451 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/utilities/_dev_logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/utilities/async_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10306 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/utilities/files.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4019 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/utilities/other.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.615188 simmate-0.9.0/src/simmate/utilities/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/utilities/test/test_files.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.615188 simmate-0.9.0/src/simmate/visualization/
+-rw-r--r--   0 runner    (1001) docker     (121)      551 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/visualization/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.615188 simmate-0.9.0/src/simmate/visualization/structure/
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/visualization/structure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.615188 simmate-0.9.0/src/simmate/visualization/structure/blender/
+-rw-r--r--   0 runner    (1001) docker     (121)     4432 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/visualization/structure/blender/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/visualization/structure/blender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6189 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/visualization/structure/blender/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6437 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/visualization/structure/blender/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.615188 simmate-0.9.0/src/simmate/visualization/structure/blender/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)    12053 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/visualization/structure/blender/scripts/make_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.615188 simmate-0.9.0/src/simmate/visualization/structure/blender/test/
+-rw-r--r--   0 runner    (1001) docker     (121)      701 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/visualization/structure/blender/test/test_blender.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.615188 simmate-0.9.0/src/simmate/website/
+-rw-r--r--   0 runner    (1001) docker     (121)    10246 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.615188 simmate-0.9.0/src/simmate/website/core/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.615188 simmate-0.9.0/src/simmate/website/core/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1059 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core/test/test_core_views.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2041 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4693 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core/views.py
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.619187 simmate-0.9.0/src/simmate/website/core_components/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9374 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/base_api_view.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.619187 simmate-0.9.0/src/simmate/website/core_components/filters/
+-rw-r--r--   0 runner    (1001) docker     (121)      695 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/filters/band_structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5109 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/filters/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/filters/calculation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      908 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/filters/density_of_states.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/filters/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/filters/forces.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/filters/nudged_elastic_band.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/filters/relaxation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      748 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/filters/static_energy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3502 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/filters/structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)      416 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/filters/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (121)      522 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/filters/thermodynamics.py
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.619187 simmate-0.9.0/src/simmate/website/core_components/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/templatetags/chemical_formula_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)      995 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/templatetags/markdown_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/templatetags/matplotlib_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1796 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/templatetags/structure_serialize_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.619187 simmate-0.9.0/src/simmate/website/core_components/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/test/test_cc_views.py
+-rw-r--r--   0 runner    (1001) docker     (121)      924 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4383 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/core_components/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.579187 simmate-0.9.0/src/simmate/website/static_files/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.619187 simmate-0.9.0/src/simmate/website/static_files/images/
+-rw-r--r--   0 runner    (1001) docker     (121)     5171 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/static_files/images/dask-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     6785 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/static_files/images/dask-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1781 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/static_files/images/digitalocean-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     3776 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/static_files/images/digitalocean-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      762 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/static_files/images/django-icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.619187 simmate-0.9.0/src/simmate/website/static_files/images/geometry_templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     2732 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/static_files/images/geometry_templates/cube.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     5373 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/static_files/images/geometry_templates/octahedron.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     5257 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/static_files/images/geometry_templates/tetrahedron.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     2069 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/static_files/images/github-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     3999 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/static_files/images/prefect-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     2866 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/static_files/images/prefect-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     7157 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/static_files/images/simmate-geometries.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     3012 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/static_files/images/simmate-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     7818 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/static_files/images/simmate-logo-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    20638 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/static_files/images/simmate-logo-other-ideas.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     7777 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/static_files/images/simmate-logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.623187 simmate-0.9.0/src/simmate/website/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     1344 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1439 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/500.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.623187 simmate-0.9.0/src/simmate/website/templates/account/
+-rw-r--r--   0 runner    (1001) docker     (121)     4408 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/account/login.html
+-rw-r--r--   0 runner    (1001) docker     (121)      648 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/account/loginstatus.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2002 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/account/logout.html
+-rw-r--r--   0 runner    (1001) docker     (121)      698 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/account/profile.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2298 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/account/signup.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.623187 simmate-0.9.0/src/simmate/website/templates/core_components/
+-rw-r--r--   0 runner    (1001) docker     (121)     6580 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/about.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.623187 simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/band-structure-calc.html
+-rw-r--r--   0 runner    (1001) docker     (121)      791 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/band-structure.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/calculation.html
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/density-of-states-calc.html
+-rw-r--r--   0 runner    (1001) docker     (121)      523 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/density-of-states.html
+-rw-r--r--   0 runner    (1001) docker     (121)      235 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/diffusion-analysis.html
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/dynamics-run.html
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/forces.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/relaxation.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/static-energy.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/structure.html
+-rw-r--r--   0 runner    (1001) docker     (121)      809 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/thermodynamics.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.627187 simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/band-structure-calc.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/band-structure.html
+-rw-r--r--   0 runner    (1001) docker     (121)      778 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/calculation.html
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/density-of-states-calc.html
+-rw-r--r--   0 runner    (1001) docker     (121)      847 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/density-of-states.html
+-rw-r--r--   0 runner    (1001) docker     (121)      975 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/diffusion-analysis.html
+-rw-r--r--   0 runner    (1001) docker     (121)      967 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/dynamics-run.html
+-rw-r--r--   0 runner    (1001) docker     (121)      853 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/forces.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1845 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/relaxation.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1388 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/static-energy.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3421 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/structure.html
+-rw-r--r--   0 runner    (1001) docker     (121)      939 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/thermodynamics.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4072 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/contact.html
+-rw-r--r--   0 runner    (1001) docker     (121)     4123 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/datatable.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1907 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/extras.html
+-rw-r--r--   0 runner    (1001) docker     (121)      912 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/footer.html
+-rw-r--r--   0 runner    (1001) docker     (121)      528 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/footerbar.html
+-rw-r--r--   0 runner    (1001) docker     (121)     7893 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/navbar.html
+-rw-r--r--   0 runner    (1001) docker     (121)    36678 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/periodic_table.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/search_form.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2133 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/search_results_pagination.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3712 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/sidebar.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2724 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/site_base.html
+-rw-r--r--   0 runner    (1001) docker     (121)     5580 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/structure_viewer.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/table_entry.html
+-rw-r--r--   0 runner    (1001) docker     (121)      653 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/core_components/test.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.627187 simmate-0.9.0/src/simmate/website/templates/home/
+-rw-r--r--   0 runner    (1001) docker     (121)      291 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/home/home.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3861 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/home/search-form.html
+-rw-r--r--   0 runner    (1001) docker     (121)     3946 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/home/search-results.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.627187 simmate-0.9.0/src/simmate/website/templates/third_parties/
+-rw-r--r--   0 runner    (1001) docker     (121)      924 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/third_parties/entry_detail.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/third_parties/provider.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/third_parties/providers_all.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2227 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/third_parties/search_results.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.627187 simmate-0.9.0/src/simmate/website/templates/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/workflows/all.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/workflows/by_type.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1960 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/workflows/detail.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/workflows/detail_run.html
+-rw-r--r--   0 runner    (1001) docker     (121)     2750 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/workflows/search_results.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1272 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/templates/workflows/submit.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.627187 simmate-0.9.0/src/simmate/website/test_app/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/test_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/test_app/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      718 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/test_app/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.627187 simmate-0.9.0/src/simmate/website/third_parties/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/third_parties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/third_parties/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3200 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/third_parties/forms.py
+-rw-r--r--   0 runner    (1001) docker     (121)      435 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/third_parties/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.627187 simmate-0.9.0/src/simmate/website/third_parties/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1266 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/third_parties/test/test_third_parties_views.py
+-rw-r--r--   0 runner    (1001) docker     (121)      491 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/third_parties/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/third_parties/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.627187 simmate-0.9.0/src/simmate/website/workflow_engine/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/workflow_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/workflow_engine/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)      332 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/workflow_engine/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.627187 simmate-0.9.0/src/simmate/website/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      180 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/workflows/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8042 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/workflows/forms.py
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/workflows/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.627187 simmate-0.9.0/src/simmate/website/workflows/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     3920 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/workflows/test/test_workflows_views.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/workflows/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5668 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/website/workflows/views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.627187 simmate-0.9.0/src/simmate/workflow_engine/
+-rw-r--r--   0 runner    (1001) docker     (121)     4499 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflow_engine/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflow_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8378 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflow_engine/error_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.627187 simmate-0.9.0/src/simmate/workflow_engine/execution/
+-rw-r--r--   0 runner    (1001) docker     (121)     1411 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflow_engine/execution/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflow_engine/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3492 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflow_engine/execution/database.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6816 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflow_engine/execution/executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5001 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflow_engine/execution/future.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2309 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflow_engine/execution/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11761 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflow_engine/execution/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.631188 simmate-0.9.0/src/simmate/workflow_engine/execution_prefect/
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflow_engine/execution_prefect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9865 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflow_engine/execution_prefect/worker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9608 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflow_engine/execution_prefect/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34431 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflow_engine/s3_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.631188 simmate-0.9.0/src/simmate/workflow_engine/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflow_engine/test/test_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7214 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflow_engine/test/test_s3_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4442 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflow_engine/test/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2982 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflow_engine/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)    52504 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflow_engine/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.631188 simmate-0.9.0/src/simmate/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     3361 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflows/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflows/customized.py
+-rw-r--r--   0 runner    (1001) docker     (121)      312 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflows/diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      355 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflows/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (121)      423 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflows/electronic_structure.py
+-rw-r--r--   0 runner    (1001) docker     (121)      420 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflows/population_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflows/relaxation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2322 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflows/restart.py
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflows/static_energy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflows/structure_prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.631188 simmate-0.9.0/src/simmate/workflows/test/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.631188 simmate-0.9.0/src/simmate/workflows/test/simmate-task-ERROR/
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflows/test/simmate-task-ERROR/simmate_metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     4759 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflows/test/test_all_workflow_runs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4390 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflows/test/test_workflows_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10314 2022-08-17 16:40:21.000000 simmate-0.9.0/src/simmate/workflows/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 16:40:39.583187 simmate-0.9.0/src/simmate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      868 2022-08-17 16:40:39.000000 simmate-0.9.0/src/simmate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    30599 2022-08-17 16:40:39.000000 simmate-0.9.0/src/simmate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-17 16:40:39.000000 simmate-0.9.0/src/simmate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-08-17 16:40:39.000000 simmate-0.9.0/src/simmate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2022-08-17 16:40:39.000000 simmate-0.9.0/src/simmate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-17 16:40:39.000000 simmate-0.9.0/src/simmate.egg-info/top_level.txt
```

### Comparing `simmate-0.8.0/LICENSE` & `simmate-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/PKG-INFO` & `simmate-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simmate
-Version: 0.8.0
+Version: 0.9.0
 Summary: Simmate is a toolbox for computational materials research.
 Author-email: "Jack D. Sundberg" <jacksund@live.unc.edu>
 License: BSD 3-Clause License
 Project-URL: homepage, https://simmate.org/
 Project-URL: repository, https://github.com/jacksund/simmate
 Project-URL: documentation, https://jacksund.github.io/simmate/simmate.html
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `simmate-0.8.0/README.md` & `simmate-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/pyproject.toml` & `simmate-0.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 # published name for pip install to use
 name="simmate"
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 # https://semver.org/
-version="0.8.0"
+version="0.9.0"
 
 # Maintainer info
 authors = [{name = "Jack D. Sundberg", email = "jacksund@live.unc.edu"}]
 
 # a quick summary and then README
 # NOTE: instead of our main README, I tell users to move directly to github
 description="Simmate is a toolbox for computational materials research."
@@ -70,14 +70,15 @@
     # For development and testing
     "pytest >=6.2.5, <7.1",  # BUG: see issue #162 for limiting <7.1
     "pytest-django >=4.5.2, <=4.5.2",
     "pytest-mock >=3.7.0, <=3.8.2",
     "pytest-xdist >=2.5.0, <=2.5.0",
     "black >=22.1.0, <=22.6.0",
     "coverage >=6.2, <=6.4.3",
+    "isort >=5.10.1, <=5.10.1",
     #
     # These are from the MP stack and I want to phase them out over time
     "pymatgen >=2022.1.9, <=2022.7.25",
     "pymatgen-analysis-diffusion >=2021.4.29, <=2022.7.21",  # pymatgen-diffusion on conda
     "matminer >=0.7.6, <=0.7.8",
     #
     # These are packages that I commonly use alongside simmate. I plan to
@@ -166,15 +167,15 @@
 
 # By default, we only want to run unmarked tests. The simplest way to do this
 # without adding extra files is to just list "not <marker1> and not <marker2" 
 # for all of them. We also want migrations to be built from scratch, not past 
 # migration folders.
 # I manually remove -m when testing coverage, but am unsure if there's a better
 # way to do this.
-addopts = "--no-migrations -m 'not blender and not vasp'"
+addopts = "--no-migrations --durations=15 -m 'not blender and not vasp'"
 
 # There are a number of warnings that are expected when running our tests.
 # We remove these from our output for clarity.
 filterwarnings = [
     "ignore:cannot collect test class*:Warning",
     "ignore:Issues encountered while parsing CIF*:Warning",
     "ignore:No POTCAR file with matching TITEL fields*:Warning",
@@ -196,7 +197,15 @@
 # when testing coverage, we want to ignore the test files themselves.
 omit = ["*/test_*", "*/conftest.py", "*/*_test.py"]
 
 # consider adding for coverage of templates
 # plugins = django_coverage_plugin  
 
 # -----------------------------------------------------------------------------
+
+# isort is a tool for organizing imports at the top of python files. By default,
+# it conflicts with the black formatter we use, so we need to configure it here.
+
+[tool.isort]
+profile = "black"
+
+# -----------------------------------------------------------------------------
```

### Comparing `simmate-0.8.0/src/simmate/README.md` & `simmate-0.9.0/src/simmate/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/__init__.py` & `simmate-0.9.0/src/simmate/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # -*- coding: utf-8 -*-
 
-import logging
 import importlib.metadata
-
+import logging
 
 __version__ = importlib.metadata.version("simmate")
 
 # Some of these utilities use the __version__ above, so this import must come after
-from simmate.utilities import get_doc_from_readme, check_if_using_latest_version
+from simmate.utilities import check_if_using_latest_version, get_doc_from_readme
 
 __doc__ = get_doc_from_readme(__file__)
 
 
 # Configure our logger to output timestamps and "SIMMATE" with logs
 # Also changes the logging level to info
 logging.basicConfig(
-    format="[SIMMATE-%(levelname)-s %(asctime)-s] %(message)s",
+    format="[SIMMATE-%(levelname)-s | %(asctime)-s] %(message)s",
     level=logging.INFO,
     datefmt="%Y-%m-%d %H:%M:%S",
 )
 
 
 # Check if there is a newer Simmate version available, and if the current
 # installation is out of date, print a message for the user.
 try:
     check_if_using_latest_version()
 except:
-    logging.warn("Unable to check if using the latest Simmate version.")
+    logging.warning("Unable to check if using the latest Simmate version.")
```

### Comparing `simmate-0.8.0/src/simmate/calculators/README.md` & `simmate-0.9.0/src/simmate/calculators/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/bader/README.md` & `simmate-0.9.0/src/simmate/calculators/bader/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/bader/outputs/acf.py` & `simmate-0.9.0/src/simmate/calculators/bader/outputs/acf.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/bader/workflows/badelf.py` & `simmate-0.9.0/src/simmate/calculators/bader/workflows/badelf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from pymatgen.io.vasp.outputs import Elfcar, Chgcar
+from pymatgen.io.vasp.outputs import Chgcar, Elfcar
 
 from simmate.toolkit import Structure
 
 from .bader import PopulationAnalysis__Bader__Bader
 
 
 class PopulationAnalysis__Bader__Badelf(PopulationAnalysis__Bader__Bader):
```

### Comparing `simmate-0.8.0/src/simmate/calculators/bader/workflows/bader.py` & `simmate-0.9.0/src/simmate/calculators/bader/workflows/bader.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 
-import yaml
 from pathlib import Path
-from pandas import DataFrame
 
-from pymatgen.io.vasp.outputs import Chgcar
+import yaml
+from pandas import DataFrame
 from pymatgen.io.vasp import Potcar
+from pymatgen.io.vasp.outputs import Chgcar
 
-from simmate.workflow_engine import S3Workflow
 from simmate.calculators.bader.outputs import ACF
+from simmate.workflow_engine import S3Workflow
 
 
 class PopulationAnalysis__Bader__Bader(S3Workflow):
 
     command = "bader CHGCAR -ref CHGCAR_sum -b weight > bader.out"
     """
     The command to call the executable, which is typically bader. Note we
```

### Comparing `simmate-0.8.0/src/simmate/calculators/bader/workflows/combine_chgcars.py` & `simmate-0.9.0/src/simmate/calculators/bader/workflows/combine_chgcars.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/deepmd/README.md` & `simmate-0.9.0/src/simmate/calculators/deepmd/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/deepmd/inputs/parameters.py` & `simmate-0.9.0/src/simmate/calculators/deepmd/inputs/parameters.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/deepmd/inputs/type_and_set.py` & `simmate-0.9.0/src/simmate/calculators/deepmd/inputs/type_and_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
 import numpy
-
-from sklearn.model_selection import train_test_split
 from django_pandas.io import read_frame
+from sklearn.model_selection import train_test_split
 
-from simmate.toolkit import Structure, Composition
+from simmate.toolkit import Composition, Structure
 from simmate.utilities import get_directory
 
 
 class DeepmdDataset:
     """
     This class works simply as a converter. You provide it a list of
     IonicStepStructures that have forces and energies, and it will create a
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/configuration.md` & `simmate-0.9.0/src/simmate/calculators/vasp/configuration.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/README.md` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/__init__.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 # -*- coding: utf-8 -*-
 
 from simmate.utilities import get_doc_from_readme
 
 __doc__ = get_doc_from_readme(__file__)
 
+from .brions import Brions
+from .brmix import Brmix
+from .edddav import Edddav
+from .eddrmm import Eddrmm
+from .edwav import Edwav
+from .elf_kpar import ElfKpar
+from .frozen import Frozen
+from .incorrect_shift import IncorrectShift
 from .incorrect_smearing import IncorrectSmearing
+from .insufficient_bands import InsufficientBands
+from .large_sigma import LargeSigma
+from .long_vector import LongVector
 from .mesh_symmetry import MeshSymmetry
-from .unconverged import Unconverged
 from .nonconverging import NonConverging
-from .potim import Potim
+from .point_group import PointGroup
 from .positive_energy import PositiveEnergy
-from .frozen import Frozen
-from .large_sigma import LargeSigma
-
-from .tetrahedron_mesh import TetrahedronMesh
-from .rotation_matrix import RotationMatrix
-from .brmix import Brmix
-from .zpotrf import Zpotrf
-from .subspace_matrix import SubspaceMatrix
-from .incorrect_shift import IncorrectShift
-from .real_optlay import RealOptlay
-from .tetirr import Tetirr
-from .rotation_matrix_nonint import RotationNonIntMatrix
-from .long_vector import LongVector
-from .triple_product import TripleProduct
+from .posmap import Posmap
+from .potim import Potim
 from .pricel import Pricel
-from .brions import Brions
-from .zbrent import Zbrent
-from .insufficient_bands import InsufficientBands
 from .pssyevx import Pssyevx
-from .eddrmm import Eddrmm
-from .edddav import Edddav
-from .edwav import Edwav
-from .zheev import Zheev
-from .elf_kpar import ElfKpar
+from .real_optlay import RealOptlay
 from .rhosyg import Rhosyg
-from .posmap import Posmap
-from .point_group import PointGroup
+from .rotation_matrix import RotationMatrix
+from .rotation_matrix_nonint import RotationNonIntMatrix
+from .subspace_matrix import SubspaceMatrix
 from .symprec_noise import SymprecNoise
+from .tetrahedron_mesh import TetrahedronMesh
+from .triple_product import TripleProduct
+from .unconverged import Unconverged
 from .walltime import Walltime
+from .zbrent import Zbrent
+from .zheev import Zheev
+from .zpotrf import Zpotrf
+
+# These handlers depend on other handlers above. So we make sure they are
+# imported last and disable isort for them.
+# isort: split
+from .tetirr import Tetirr
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/brions.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/brions.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class Brions(ErrorHandler):
     """
     This fixes an internal VASP error by increasing POTIM.
     """
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/brmix.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/brmix.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 
-from pathlib import Path
 import json
+from pathlib import Path
 
 from pymatgen.io.vasp.outputs import Outcar
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class Brmix(ErrorHandler):
     """
     This handler addresses changes in charge density during a SCF loop. There are
     a series of fixes that depend on the type and state of the calculation being
     ran, so be sure to read the stages below.
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/edddav.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/edddav.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class Edddav(ErrorHandler):
     """
     When the gradient is not orthogonal, we make a fix depending on what IMSEAR
     is set to.
     """
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/eddrmm.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/eddrmm.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class Eddrmm(ErrorHandler):
     """
     This is an error caused by failed call to LAPCK.
 
     This could be caused by a number of things, such as instability of the
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/edwav.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/edwav.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class Edwav(ErrorHandler):
     """
     When the gradient is not orthogonal, we make a fix depending on what IMSEAR
     is set to.
     """
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/elf_kpar.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/elf_kpar.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class ElfKpar(ErrorHandler):
 
     is_monitor = True
     filename_to_check = "vasp.out"
     possible_error_messages = ["ELF: KPAR>1 not implemented"]
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/frozen.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/frozen.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
-from pathlib import Path
 import time
+from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class Frozen(ErrorHandler):
     """
     Checks when the output file has last been editted. If the job has been sitting
     for a long time (i.e. 1 hour), we consider it frozen and want to change the
     ALGO from Normal to Fast or alternatively reduce SYMPREC.
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/incorrect_shift.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/incorrect_shift.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class IncorrectShift(ErrorHandler):
     """
     This handler addresses issues in the K-point mesh that can be fixed by switching
     to a gamma-centered mesh.
     """
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/incorrect_smearing.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/incorrect_smearing.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
 from pymatgen.io.vasp.outputs import Vasprun
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class IncorrectSmearing(ErrorHandler):
     """
     This checks if a calculation is a metal (zero bandgap), has been run with
     ISMEAR=-5, and is not a static calculation. This type of smearing is only
     appropriate for the relaxation of semiconductors and insulators -- not
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/insufficient_bands.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/insufficient_bands.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class InsufficientBands(ErrorHandler):
     """
     If the calculation has too few bands, we increase the number of bands by
     10% and try again.
     """
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/large_sigma.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/large_sigma.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
+from simmate.calculators.vasp.inputs import Incar
 from simmate.toolkit import Structure
 from simmate.workflow_engine import ErrorHandler
-from simmate.calculators.vasp.inputs import Incar
 
 
 class LargeSigma(ErrorHandler):
     """
     When ISMEAR >= 0 (Gaussian or Methfessel-Paxton), we need to monitor the
     magnitude of the entropy term T*S. If the entropy term is larger than
     1 meV/atom, then we reduce value of SIGMA. See VASP documentation for ISMEAR.
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/long_vector.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/long_vector.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class LongVector(ErrorHandler):
     """
     This a simple error handler that is active when VASP finds an issue with the
     rotation matrix.
     """
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/mesh_symmetry.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/mesh_symmetry.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from pymatgen.io.vasp.outputs import Vasprun
 from pymatgen.io.vasp.inputs import Kpoints
+from pymatgen.io.vasp.outputs import Vasprun
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class MeshSymmetry(ErrorHandler):
     """
     Corrects the mesh symmetry error in VASP. This error is sometimes
     non-fatal and the job can complete successfully. So this error handler
     only checks at the end of the run, and if the run has converged, no error
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/nonconverging.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/nonconverging.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/point_group.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/point_group.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class PointGroup(ErrorHandler):
     """
     Fixes an error where VASP does not have the symmetry group operations
     available. To fix this, we simply need to turn symmetry off.
     """
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/positive_energy.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/positive_energy.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/posmap.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/posmap.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
-from pathlib import Path
 import json
+from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class Posmap(ErrorHandler):
 
     is_monitor = True
     filename_to_check = "vasp.out"
     possible_error_messages = ["POSMAP"]
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/potim.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/potim.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.toolkit import Structure
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
 from simmate.calculators.vasp.outputs import Oszicar
+from simmate.toolkit import Structure
+from simmate.workflow_engine import ErrorHandler
 
 
 class Potim(ErrorHandler):
     """
     This handler checks if a run has excessively large positive energy changes,
     where it's typically caused by too large of a POTIM. Runs will end up crashing
     with some other error (e.g. BRMIX) as the geometry gets progressively worse.
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/pricel.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/pricel.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class Pricel(ErrorHandler):
     """
     This fixes an internal VASP error by turning off symmetry.
     """
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/pssyevx.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/pssyevx.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class Pssyevx(ErrorHandler):
     """
     This fixes subspace rotation error by switching ALGO to Normal
     """
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/real_optlay.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/real_optlay.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import json
 from pathlib import Path
 
+from simmate.calculators.vasp.inputs import Incar
 from simmate.toolkit import Structure
 from simmate.workflow_engine import ErrorHandler
-from simmate.calculators.vasp.inputs import Incar
 
 
 class RealOptlay(ErrorHandler):
     """
     This handler addresses a series of warning messages that each have the same
     attempted fixes. There are a series of fixes that can be attempted, so we
     keep a running log of how many times this handler is called.
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/rhosyg.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/rhosyg.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class Rhosyg(ErrorHandler):
 
     is_monitor = True
     filename_to_check = "vasp.out"
     possible_error_messages = ["RHOSYG"]
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/rotation_matrix.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/rotation_matrix.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class RotationMatrix(ErrorHandler):
     """
     This a simple error handler that is active when VASP struggles to find the
     rotation matrix. VASP gives us the suggested fix directly, which is to
     simply increase the symmetry precision.
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/rotation_matrix_nonint.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/rotation_matrix_nonint.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
-from pathlib import Path
 import json
+from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class RotationNonIntMatrix(ErrorHandler):
     """
     This a simple error handler that is active when VASP finds an issue with the
     rotation matrix.
     """
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/subspace_matrix.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/subspace_matrix.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
-from pathlib import Path
 import json
+from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class SubspaceMatrix(ErrorHandler):
     """
     This handler fixes when the sub-space-matrix is not hermitian. On the first
     attempt, we switch evaluation of projection operators to reciprocal space.
     If that doesn't work, the calculation precision is switched to "Accurate".
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/symprec_noise.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/symprec_noise.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class SymprecNoise(ErrorHandler):
     """
     Fixes determination of symmetry in problematic structures.
     """
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_brmix.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_brmix.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
-from simmate.conftest import copy_test_files, make_dummy_files
-from simmate.calculators.vasp.inputs import Incar
 from simmate.calculators.vasp.error_handlers import Brmix
+from simmate.calculators.vasp.inputs import Incar
+from simmate.conftest import copy_test_files, make_dummy_files
 
 
 def test_brmix(tmp_path):
     copy_test_files(
         tmp_path,
         test_directory=__file__,
         test_folder="brmix.zip",
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_eddrmm.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_eddrmm.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
-from simmate.conftest import copy_test_files, make_dummy_files
-from simmate.calculators.vasp.inputs import Incar
 from simmate.calculators.vasp.error_handlers import Eddrmm
+from simmate.calculators.vasp.inputs import Incar
+from simmate.conftest import copy_test_files, make_dummy_files
 
 
 def test_eddrmm(tmp_path):
     copy_test_files(
         tmp_path,
         test_directory=__file__,
         test_folder="eddrmm",
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_frozen.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_frozen.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import pytest
 
-from simmate.conftest import copy_test_files, make_dummy_files
-from simmate.calculators.vasp.inputs import Incar
 from simmate.calculators.vasp.error_handlers import Frozen
+from simmate.calculators.vasp.inputs import Incar
+from simmate.conftest import copy_test_files, make_dummy_files
 
 
 def test_frozen(tmp_path):
     copy_test_files(
         tmp_path,
         test_directory=__file__,
         test_folder="frozen",
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_incorrect_smearing.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_incorrect_smearing.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
-from simmate.conftest import copy_test_files
-from simmate.calculators.vasp.inputs import Incar
 from simmate.calculators.vasp.error_handlers import IncorrectSmearing
+from simmate.calculators.vasp.inputs import Incar
+from simmate.conftest import copy_test_files
 
 
 def test_incorrect_smearing(tmp_path):
     copy_test_files(
         tmp_path,
         test_directory=__file__,
         test_folder="incorrect_smearing.zip",
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_large_sigma.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_large_sigma.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import pytest
 
-from simmate.conftest import copy_test_files
-from simmate.calculators.vasp.inputs import Incar
 from simmate.calculators.vasp.error_handlers import LargeSigma
+from simmate.calculators.vasp.inputs import Incar
+from simmate.conftest import copy_test_files
 
 
 def test_large_sigma(tmp_path):
     copy_test_files(
         tmp_path,
         test_directory=__file__,
         test_folder="large_sigma.zip",
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_mesh_symmetry.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_mesh_symmetry.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import pytest
 
-from simmate.conftest import copy_test_files
-from simmate.calculators.vasp.inputs import Incar
 from simmate.calculators.vasp.error_handlers import MeshSymmetry
+from simmate.calculators.vasp.inputs import Incar
+from simmate.conftest import copy_test_files
 
 
 def test_mesh_symmetry(tmp_path):
     copy_test_files(
         tmp_path,
         test_directory=__file__,
         test_folder="mesh_symmetry.zip",
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_nonconverging.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_nonconverging.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import pytest
 
-from simmate.conftest import copy_test_files
-from simmate.calculators.vasp.inputs import Incar
 from simmate.calculators.vasp.error_handlers import NonConverging
+from simmate.calculators.vasp.inputs import Incar
+from simmate.conftest import copy_test_files
 
 
 def test_nonconverging(tmp_path):
     copy_test_files(
         tmp_path,
         test_directory=__file__,
         test_folder="nonconverging",
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_positive_energy.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_positive_energy.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
-from simmate.conftest import copy_test_files
-from simmate.calculators.vasp.inputs import Incar
 from simmate.calculators.vasp.error_handlers import PositiveEnergy
+from simmate.calculators.vasp.inputs import Incar
+from simmate.conftest import copy_test_files
 
 
 def test_positive_energy(tmp_path):
     copy_test_files(
         tmp_path,
         test_directory=__file__,
         test_folder="positive_energy",
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_potim.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_potim.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
-from simmate.conftest import copy_test_files
-from simmate.calculators.vasp.inputs import Incar
 from simmate.calculators.vasp.error_handlers import Potim
+from simmate.calculators.vasp.inputs import Incar
+from simmate.conftest import copy_test_files
 
 
 def test_potim(tmp_path):
     copy_test_files(
         tmp_path,
         test_directory=__file__,
         test_folder="potim",
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_tetrahedron_mesh.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_tetrahedron_mesh.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
-from simmate.conftest import copy_test_files
-from simmate.calculators.vasp.inputs import Incar
 from simmate.calculators.vasp.error_handlers import TetrahedronMesh
+from simmate.calculators.vasp.inputs import Incar
+from simmate.conftest import copy_test_files
 
 
 def test_tetrahedron_mesh(tmp_path):
     copy_test_files(
         tmp_path,
         test_directory=__file__,
         test_folder="tetrahedron_mesh",
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_unconverged.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_unconverged.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
-from simmate.conftest import copy_test_files
-from simmate.calculators.vasp.inputs import Incar
 from simmate.calculators.vasp.error_handlers import Unconverged
+from simmate.calculators.vasp.inputs import Incar
+from simmate.conftest import copy_test_files
 
 
 def test_unconverged_electronic(tmp_path):
     copy_test_files(
         tmp_path,
         test_directory=__file__,
         test_folder="unconverged_electronic.zip",
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/test/test_zpotrf.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/test/test_zpotrf.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
-from simmate.conftest import copy_test_files, make_dummy_files
-from simmate.calculators.vasp.inputs import Incar
 from simmate.calculators.vasp.error_handlers import Zpotrf
+from simmate.calculators.vasp.inputs import Incar
+from simmate.conftest import copy_test_files, make_dummy_files
 
 
 def test_eddrmm(tmp_path):
     copy_test_files(
         tmp_path,
         test_directory=__file__,
         test_folder="zpotrf",
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/tetirr.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/tetirr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
+from simmate.calculators.vasp.error_handlers import IncorrectShift, TetrahedronMesh
 from simmate.workflow_engine import ErrorHandler
-from simmate.calculators.vasp.error_handlers import TetrahedronMesh, IncorrectShift
 
 
 class Tetirr(ErrorHandler):
     """
     This handler addresses an issue that is a combination of the TetrahedronMesh
     and IncorrectShift errors.
     """
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/tetrahedron_mesh.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/tetrahedron_mesh.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class TetrahedronMesh(ErrorHandler):
     """
     This handler addresses a series of error messages that are all caused by
     having incompatible tetrahedral mesh. In some cases, increasing the k-point
     mesh will fix the issue, and in other cases, we'll simply turn off the
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/to_do/aliasing.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/to_do/aliasing.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class Aliasing(ErrorHandler):
     """
     Aliasing errors occur when there are issues with the NGX, NGY, and NGZ grid
     in VASP. Typically the fix is to just remove user defined settings for these
     values, delete the CHGCAR and WAVECAR, and then restart the calculation. In
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/to_do/drift.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/to_do/drift.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/to_do/lrf_commutor.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/to_do/lrf_commutor.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/to_do/scan_metal.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/to_do/scan_metal.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/to_do/standard_error.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/to_do/standard_error.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/triple_product.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/triple_product.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
+from simmate.calculators.vasp.inputs import Incar
 from simmate.toolkit import Structure
 from simmate.workflow_engine import ErrorHandler
-from simmate.calculators.vasp.inputs import Incar
 
 
 class TripleProduct(ErrorHandler):
     """
     This error handler swaps the b and c lattice vectors when VASP fails to handle
     its basis vectors properly.
     """
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/unconverged.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/unconverged.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 
-from pathlib import Path
 import shutil
+from pathlib import Path
 
 from pymatgen.io.vasp.outputs import Vasprun
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class Unconverged(ErrorHandler):
     """
     Check if a calculation converged successfully. If not, the fix depends on
     whether its the ionic steps or electronic steps are struggling to converge.
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/walltime.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/walltime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 
-import os
-from pathlib import Path
-import time
 import datetime
-import subprocess
 import logging
+import os
+import subprocess
+import time
+from pathlib import Path
 
 import numpy
 from pymatgen.io.vasp.outputs import Outcar
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.error_handlers import Unconverged
+from simmate.workflow_engine import ErrorHandler
 
 
 class Walltime(ErrorHandler):
     """
     Checks if a run is nearing the walltime of a SLURM job that it's
     running in. If so, VASP can be stopped by writing a STOPCAR with
     LSTOP or LABORT = True.
@@ -139,15 +139,17 @@
             # simmate_metadata.yaml.
             # If there is no simmate_metadata.yaml (meaning the S3task
             # was ran outside of a Workflow), then we say that wall_time cannot
             # be determined. (checking files like INCAR won't work bc of other
             # handlers updating them)
             filename = directory / "simmate_metadata.yaml"
             if not filename.exists():
-                logging.warn("Unable to detect the time remaining. Ignoring Timeout.")
+                logging.warning(
+                    "Unable to detect the time remaining. Ignoring Timeout."
+                )
                 return
                 # !!! What if I looked at the creation time of the current directory?
 
             time_since_creation = time.time() - filename.lstat().st_mtime
 
             remaining_time = self.wall_time - time_since_creation
 
@@ -160,28 +162,28 @@
                 "squeue -h -O TimeLeft -j $SLURM_JOBID",
                 shell=True,
                 capture_output=True,
                 text=True,
             ).stdout.strip()
             # parse the output into a time
             if output == "INVALID":
-                logging.warn(
+                logging.warning(
                     "SLURM node improperly configured. " "Cannot detect TimeLeft"
                 )
                 return
             elif output == "UNLIMITED":
                 return
             else:
                 # OPTIMIZE: this section could benefit from regex.
 
                 # Converts a string like "199-21:58:12" to ['199', '21', '58', '12']
                 try:
                     output = [int(i) for i in output.replace("-", ":").split(":")]
                 except:
-                    logging.warn(
+                    logging.warning(
                         "Failed to parse SLURM output. Please report this to the"
                         f"Simmate team. Output was {output}"
                     )
                     return
                 # this funky format is because we don't know how long our list
                 # will be.
                 time_inputs = {}
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/zbrent.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/zbrent.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
-from pathlib import Path
 import shutil
+from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class Zbrent(ErrorHandler):
     """
     Calculation is simply restarted using the most recent structure (CONTCAR)
     """
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/zheev.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/zheev.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
+from simmate.workflow_engine import ErrorHandler
 
 
 class Zheev(ErrorHandler):
 
     is_monitor = True
     filename_to_check = "vasp.out"
     possible_error_messages = ["ERROR EDDIAG: Call to routine ZHEEV failed!"]
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/error_handlers/zpotrf.py` & `simmate-0.9.0/src/simmate/calculators/vasp/error_handlers/zpotrf.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.toolkit import Structure
-from simmate.workflow_engine import ErrorHandler
 from simmate.calculators.vasp.inputs import Incar
 from simmate.calculators.vasp.outputs import Oszicar
+from simmate.toolkit import Structure
+from simmate.workflow_engine import ErrorHandler
 
 
 class Zpotrf(ErrorHandler):
     """
     This handler attempts to fix a routine failure associated with LAPACK. The
     fix depends on the state of the calculation, so we check the OSZICAR to
     decide what to do.
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/inputs/dev_notes.md` & `simmate-0.9.0/src/simmate/calculators/vasp/inputs/dev_notes.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/inputs/incar.py` & `simmate-0.9.0/src/simmate/calculators/vasp/inputs/incar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # -*- coding: utf-8 -*-
 
-from typing import Callable
-
 from simmate.calculators.vasp.inputs.incar_modifiers import (
     keyword_modifier_density,
     keyword_modifier_density_a,
     keyword_modifier_density_b,
     keyword_modifier_density_c,
     keyword_modifier_per_atom,
-    keyword_modifier_smart_magmom,
-    keyword_modifier_smart_lmaxmix,
-    keyword_modifier_smart_ldau,
     keyword_modifier_smart_ismear,
+    keyword_modifier_smart_ldau,
+    keyword_modifier_smart_lmaxmix,
+    keyword_modifier_smart_magmom,
 )
 
 
 class Incar(dict):
     """
     INCAR object for reading and writing INCAR files. This behaves exactly like
     a python dictionary, but has a few extra checks and methods attached to it.
@@ -461,15 +459,15 @@
             else:
                 new_parameters[parameter] = value
 
         # now return the new Incar
         return Incar(**new_parameters)
 
     @classmethod
-    def add_keyword_modifier(cls, keyword_modifier: Callable):
+    def add_keyword_modifier(cls, keyword_modifier: callable):
         """
         Dynamically sets a keyword_modifier function to the Incar class. When
         loaded onto the Incar class, you can then use the modifiers name to
         set a parameter based on the input structure.
 
         Names of modifiers MUST start with "keyword_modifier_" and
         have unique endings (i.e. you can't have 2 "per_atom" modifiers).
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/inputs/incar_modifiers.py` & `simmate-0.9.0/src/simmate/calculators/vasp/inputs/incar_modifiers.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/inputs/kpoints.py` & `simmate-0.9.0/src/simmate/calculators/vasp/inputs/kpoints.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/inputs/poscar.py` & `simmate-0.9.0/src/simmate/calculators/vasp/inputs/poscar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import numpy
+from pymatgen.core.lattice import Lattice  # BUG -- this is only for a bug-fix
 
 from simmate.toolkit import Structure
 
-from pymatgen.core.lattice import Lattice  # BUG -- this is only for a bug-fix
-
 
 class Poscar:
     """
     This is format converter class for loading and writing POSCAR or CONTCAR
     files, which are VASP's version of structure files (as oppossed to a cif
     file for example). When you initialize this class, you're only setting generic
     settings. You will either load a POSCAR file by doing...
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/inputs/potcar.py` & `simmate-0.9.0/src/simmate/calculators/vasp/inputs/potcar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # -*- coding: utf-8 -*-
 
 # These are dictionaries that tell us which POTCARs we should grab based on
 # the type of calculation as well as where to find them
-from simmate.calculators.vasp.inputs.potcar_mappings import (
+from simmate.calculators.vasp.inputs.potcar_mappings import (  # TODO: LDA_ELEMENT_MAPPINGS
     FOLDER_MAPPINGS,
     PBE_ELEMENT_MAPPINGS,
     PBE_GW_ELEMENT_MAPPINGS,
-    # TODO: LDA_ELEMENT_MAPPINGS
 )
 
 
 class Potcar:
     @staticmethod
     def to_file_from_type(
         elements,
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/inputs/potcar_mappings.py` & `simmate-0.9.0/src/simmate/calculators/vasp/inputs/potcar_mappings.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/inputs/test/test_incar.py` & `simmate-0.9.0/src/simmate/calculators/vasp/inputs/test/test_incar.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/outputs/oszicar.py` & `simmate-0.9.0/src/simmate/calculators/vasp/outputs/oszicar.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/README.md` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/all.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/all.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,48 @@
 # -*- coding: utf-8 -*-
 
+from .customized import Customized__Vasp__UserConfig
 from .diffusion.all import (
     Diffusion__Vasp__NebAllPathsMit,
-    Diffusion__Vasp__NebSinglePathMit,
     Diffusion__Vasp__NebFromEndpointsMit,
     Diffusion__Vasp__NebFromImagesMit,
     Diffusion__Vasp__NebFromImagesMvlCi,
+    Diffusion__Vasp__NebSinglePathMit,
+)
+from .dynamics.all import (
+    Dynamics__Vasp__Matproj,
+    Dynamics__Vasp__Mit,
+    Dynamics__Vasp__MvlNpt,
 )
-
 from .electronic_structure.all import (
     ElectronicStructure__Vasp__MatprojFull,
     ElectronicStructure__Vasp__MatprojHseFull,
 )
-
 from .population_analysis.all import (
+    PopulationAnalysis__Vasp__BadelfMatproj,
     PopulationAnalysis__Vasp__BaderMatproj,
     PopulationAnalysis__Vasp__ElfMatproj,
-    PopulationAnalysis__Vasp__BadelfMatproj,
-)
-
-from .static_energy.all import (
-    StaticEnergy__Vasp__Matproj,
-    StaticEnergy__Vasp__MatprojHse,
-    StaticEnergy__Vasp__MatprojScan,
-    StaticEnergy__Vasp__Mit,
-    StaticEnergy__Vasp__Quality04,
-    StaticEnergy__Vasp__MvlNebEndpoint,
 )
-
 from .relaxation.all import (
     Relaxation__Vasp__Matproj,
     Relaxation__Vasp__MatprojHse,
-    Relaxation__Vasp__MatprojScan,
     Relaxation__Vasp__MatprojMetal,
+    Relaxation__Vasp__MatprojScan,
     Relaxation__Vasp__Mit,
     Relaxation__Vasp__MvlGrainboundary,
-    Relaxation__Vasp__MvlSlab,
     Relaxation__Vasp__MvlNebEndpoint,
+    Relaxation__Vasp__MvlSlab,
     Relaxation__Vasp__Quality00,
     Relaxation__Vasp__Quality01,
     Relaxation__Vasp__Quality02,
     Relaxation__Vasp__Quality03,
     Relaxation__Vasp__Quality04,
     Relaxation__Vasp__Staged,
 )
-
-from .dynamics.all import (
-    Dynamics__Vasp__Mit,
-    Dynamics__Vasp__Matproj,
-    Dynamics__Vasp__MvlNpt,
+from .static_energy.all import (
+    StaticEnergy__Vasp__Matproj,
+    StaticEnergy__Vasp__MatprojHse,
+    StaticEnergy__Vasp__MatprojScan,
+    StaticEnergy__Vasp__Mit,
+    StaticEnergy__Vasp__MvlNebEndpoint,
+    StaticEnergy__Vasp__Quality04,
 )
-
-from .customized import Customized__Vasp__UserConfig
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/base.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # -*- coding: utf-8 -*-
 
-from pathlib import Path
-import shutil
 import logging
+import shutil
+from pathlib import Path
 
 import yaml
-
 from pymatgen.analysis.structure_matcher import StructureMatcher
-from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 from pymatgen.io.vasp.outputs import Vasprun
+from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 
+from simmate.calculators.vasp.inputs import Incar, Kpoints, Poscar, Potcar
 from simmate.toolkit import Structure
-from simmate.calculators.vasp.inputs import Incar, Poscar, Kpoints, Potcar
 from simmate.workflow_engine import S3Workflow
 
 
 def get_default_parallel_settings():
     """
     We load the user's default parallel settings from
         ~/simmate/vasp/INCAR_parallel_settings
@@ -262,15 +261,15 @@
         # load the xml file and all of the vasprun data
         try:
             vasprun = Vasprun(
                 filename=directory / "vasprun.xml",
                 exception_on_bad_xml=True,
             )
         except:
-            logging.warn(
+            logging.warning(
                 "XML is malformed. This typically means there's an error with your"
                 " calculation that wasn't caught by your ErrorHandlers. We try"
                 " salvaging data here though."
             )
             vasprun = Vasprun(
                 filename=directory / "vasprun.xml",
                 exception_on_bad_xml=False,
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/customized.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/customized.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,29 +34,30 @@
 structure: POSCAR
 command: mpirun -n 5 vasp_std > vasp.out
 ```
 """
 
 import logging
 
-from simmate.workflow_engine import Workflow, S3Workflow
+from simmate.workflow_engine import S3Workflow, Workflow
 
 
 class Customized__Vasp__UserConfig(Workflow):
     """
     "VASP calculation with updated INCAR/POTCAR settings
     """
 
     @staticmethod
     def run_config(
         workflow_base: Workflow,
         updated_settings: dict,
         input_parameters: dict,
+        **kwargs,
     ):
-        logging.warn(
+        logging.warning(
             "WARNING: customized workflows are meant only for quick testing. "
             "If you are using custom settings regularly, we highly recommend "
             "making a new workflow inside a Simmate project instead. "
             "Read through tutorial 06 for more information."
         )
 
         # ensure this workflow has a S3Task class attribute
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/diffusion/README.md` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/diffusion/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/diffusion/neb_all_paths_mit.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/diffusion/neb_all_paths_mit.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,28 +19,23 @@
         ├── 03
         ...
         └── N  # corresponds to image number
 ```
 """
 
 from pathlib import Path
-from typing import List
 
-from simmate.toolkit import Structure
-from simmate.toolkit.diffusion import DistinctPathFinder
-from simmate.workflow_engine import Workflow
-from simmate.calculators.vasp.workflows.relaxation.mit import (
-    Relaxation__Vasp__Mit,
-)
-from simmate.calculators.vasp.workflows.static_energy.mit import (
-    StaticEnergy__Vasp__Mit,
-)
 from simmate.calculators.vasp.workflows.diffusion.neb_single_path_mit import (
     Diffusion__Vasp__NebSinglePathMit,
 )
+from simmate.calculators.vasp.workflows.relaxation.mit import Relaxation__Vasp__Mit
+from simmate.calculators.vasp.workflows.static_energy.mit import StaticEnergy__Vasp__Mit
+from simmate.toolkit import Structure
+from simmate.toolkit.diffusion import DistinctPathFinder
+from simmate.workflow_engine import Workflow
 
 
 class Diffusion__Vasp__NebAllPathsMit(Workflow):
     """
     Runs a full diffusion analysis on a bulk crystal structure using NEB.
 
     The bulk structure will be geometry optimized and then
@@ -96,14 +91,15 @@
         directory: Path = None,
         is_restart: bool = False,
         # parameters for supercell and image generation
         nimages: int = 5,
         min_atoms: int = 80,
         max_atoms: int = 240,
         min_length: float = 10,
+        **kwargs,
     ):
 
         # Our step is to run a relaxation on the bulk structure and it uses our inputs
         # directly. The remaining one tasks pass on results.
         bulk_relax_result = Relaxation__Vasp__Mit.run(
             structure=structure,
             command=command,  # subcommands["command_bulk"]
@@ -162,15 +158,15 @@
     def _build_diffusion_analysis(
         cls,
         structure: Structure,
         migrating_specie: str,
         vacancy_mode: bool,
         directory: Path = None,
         **kwargs,
-    ) -> List[str]:
+    ) -> list[str]:
         """
         Given a bulk crystal structure, returns all symmetrically unique pathways
         for the migrating specie (up until the path is percolating). This
         also create all relevent database entries for this struture and its
         migration hops.
 
         #### Parameters
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/diffusion/neb_from_endpoints_mit.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/diffusion/neb_from_endpoints_mit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 
 import os
 from pathlib import Path
 
-from simmate.toolkit import Structure
-from simmate.workflow_engine import Workflow
+from simmate.calculators.vasp.workflows.diffusion.neb_from_images_mit import (
+    Diffusion__Vasp__NebFromImagesMit,
+)
 from simmate.calculators.vasp.workflows.diffusion.utilities import (
     get_migration_images_from_endpoints,
 )
 from simmate.calculators.vasp.workflows.relaxation.mvl_neb_endpoint import (
     Relaxation__Vasp__MvlNebEndpoint,
 )
-from simmate.calculators.vasp.workflows.diffusion.neb_from_images_mit import (
-    Diffusion__Vasp__NebFromImagesMit,
-)
+from simmate.toolkit import Structure
+from simmate.workflow_engine import Workflow
 
 
 class Diffusion__Vasp__NebFromEndpointsMit(Workflow):
     """
     Runs a full diffusion analysis from a start and end supercell using NEB.
 
     The input start/end structures will be relaxed using the relaxation/neb-endpoint
@@ -60,14 +60,15 @@
         directory: Path = None,
         source: dict = None,
         command: str = None,
         nimages: int = 5,
         # This helps link results to a higher-level table.
         diffusion_analysis_id: int = None,
         is_restart: bool = False,
+        **kwargs,
     ):
         raise NotImplementedError("TBD -jacksund")
         # command list expects three subcommands:
         #   command_bulk, command_supercell, and command_neb
         subcommands = parse_multi_command(
             command,
             commands_out=["command_supercell", "command_neb"],
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/diffusion/neb_from_images_base.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/diffusion/neb_from_images_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 
+import logging
 import shutil
-import yaml
-import numpy
 from pathlib import Path
-import logging
 
+import numpy
+import yaml
 from pymatgen.analysis.transition_state import NEBAnalysis
 
-from simmate.toolkit.diffusion import MigrationImages
 from simmate.calculators.vasp.inputs import Incar, Poscar, Potcar
 from simmate.calculators.vasp.workflows.base import VaspWorkflow
+from simmate.toolkit.diffusion import MigrationImages
 
 
 class VaspNebFromImagesWorkflow(VaspWorkflow):
     """
     A base class for Nudged Elastic Band (NEB) calculations. This is not meant
     to be used directly but instead should be inherited from.
 
@@ -143,15 +143,15 @@
 
     @classmethod
     def setup_restart(cls, directory: Path, **kwargs):
         """
         From a working directory of a past calculation, sets up for the calculation
         to be restarted.
         """
-        logging.warn("CONTCARs are not yet copied to POSCARs for NEB restarts.")
+        logging.warning("CONTCARs are not yet copied to POSCARs for NEB restarts.")
 
         # establish filenames
         stopcar_filename = directory / "STOPCAR"
 
         # delete the stopcar if it exists
         if stopcar_filename.exists():
             stopcar_filename.unlink()
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/diffusion/neb_from_images_mit.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/diffusion/neb_from_images_mit.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
-from simmate.calculators.vasp.workflows.relaxation.mit import Relaxation__Vasp__Mit
 from simmate.calculators.vasp.workflows.diffusion.neb_from_images_base import (
     VaspNebFromImagesWorkflow,
 )
+from simmate.calculators.vasp.workflows.relaxation.mit import Relaxation__Vasp__Mit
 
 
 class Diffusion__Vasp__NebFromImagesMit(
     VaspNebFromImagesWorkflow, Relaxation__Vasp__Mit
 ):
     """
     This task is a reimplementation of pymatgen's
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/diffusion/neb_from_images_mvl_ci.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/diffusion/neb_from_images_mvl_ci.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/diffusion/neb_single_path_mit.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/diffusion/neb_single_path_mit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.toolkit.diffusion import MigrationHop
-from simmate.workflow_engine import Workflow
+from simmate.calculators.vasp.workflows.diffusion.neb_from_images_mit import (
+    Diffusion__Vasp__NebFromImagesMit,
+)
 from simmate.calculators.vasp.workflows.diffusion.utilities import (
     get_migration_images_from_endpoints,
 )
 from simmate.calculators.vasp.workflows.relaxation.mvl_neb_endpoint import (
     Relaxation__Vasp__MvlNebEndpoint,
 )
-from simmate.calculators.vasp.workflows.diffusion.neb_from_images_mit import (
-    Diffusion__Vasp__NebFromImagesMit,
-)
+from simmate.toolkit.diffusion import MigrationHop
+from simmate.workflow_engine import Workflow
 
 
 class Diffusion__Vasp__NebSinglePathMit(Workflow):
     """
     Runs a full diffusion analysis on a single migration hop using NEB.
 
     Typically, this workflow is not ran directly -- but instead, you would
@@ -59,14 +59,15 @@
         # prefect id once it's a Calculation?
         is_restart: bool = False,
         # parameters for supercell and image generation
         nimages: int = 5,
         min_atoms: int = 80,
         max_atoms: int = 240,
         min_length: float = 10,
+        **kwargs,
     ):
 
         # get the supercell endpoint structures
         supercell_start, supercell_end, _ = migration_hop.get_sc_structures(
             min_atoms=min_atoms,
             max_atoms=max_atoms,
             min_length=min_length,
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/diffusion/utilities.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/diffusion/utilities.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/dynamics/base.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/dynamics/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.toolkit import Structure
+from simmate.calculators.vasp.inputs import Incar, Kpoints, Poscar, Potcar
 from simmate.calculators.vasp.workflows.base import VaspWorkflow
-from simmate.calculators.vasp.inputs import Incar, Poscar, Kpoints, Potcar
+from simmate.toolkit import Structure
 
 
 class DynamicsWorkflow(VaspWorkflow):
     @classmethod
     def setup(
         cls,
         structure: Structure,
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/dynamics/matproj.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/dynamics/matproj.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/dynamics/mit.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/dynamics/mit.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/dynamics/mvl_npt.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/dynamics/mvl_npt.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
-from simmate.toolkit import Structure
 from simmate.calculators.vasp.inputs import Incar
 from simmate.calculators.vasp.workflows.dynamics.mit import Dynamics__Vasp__Mit
+from simmate.toolkit import Structure
 
 
 class Dynamics__Vasp__MvlNpt(Dynamics__Vasp__Mit):
     """
     This task is a reimplementation of pymatgen's
     [MVLNPTMDSet](https://pymatgen.org/pymatgen.io.vasp.sets.html#pymatgen.io.vasp.sets.MVLNPTMDSet).
     """
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/elastic/mvl.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/elastic/mvl.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/base_band_structure.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/base_band_structure.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
+from pymatgen.electronic_structure.plotter import BSPlotter
 from pymatgen.io.vasp.inputs import Kpoints
 from pymatgen.symmetry.bandstructure import HighSymmKpath
-from pymatgen.electronic_structure.plotter import BSPlotter
 
 from simmate.calculators.vasp.inputs import Incar, Poscar, Potcar
 from simmate.calculators.vasp.workflows.static_energy.matproj import (
     StaticEnergy__Vasp__Matproj,
 )
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/base_density_of_states.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/base_density_of_states.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/base_full.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/base_full.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     def run_config(
         cls,
         structure,
         command: str = None,
         source: str = None,
         directory: Path = None,
         copy_previous_directory: str = False,
+        **kwargs,
     ):
 
         static_result = cls.static_energy_workflow.run(
             structure=structure,
             command=command,
             directory=directory / cls.static_energy_workflow.name_full,
             source=source,
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_band_structure.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_band_structure.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_band_structure_hse.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_band_structure_hse.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_density_of_states.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_density_of_states.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_density_of_states_hse.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_density_of_states_hse.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_full.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_full.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 
 from simmate.calculators.vasp.workflows.electronic_structure.base_full import (
     ElectronicStructureWorkflow,
 )
-from simmate.calculators.vasp.workflows.static_energy.matproj import (
-    StaticEnergy__Vasp__Matproj,
+from simmate.calculators.vasp.workflows.electronic_structure.matproj_band_structure import (
+    ElectronicStructure__Vasp__MatprojBandStructure,
 )
 from simmate.calculators.vasp.workflows.electronic_structure.matproj_density_of_states import (
     ElectronicStructure__Vasp__MatprojDensityOfStates,
 )
-from simmate.calculators.vasp.workflows.electronic_structure.matproj_band_structure import (
-    ElectronicStructure__Vasp__MatprojBandStructure,
+from simmate.calculators.vasp.workflows.static_energy.matproj import (
+    StaticEnergy__Vasp__Matproj,
 )
 
 
 class ElectronicStructure__Vasp__MatprojFull(ElectronicStructureWorkflow):
     """
     runs DOS and BS at Materials Project settings
     """
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_hse_full.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/electronic_structure/matproj_hse_full.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 
 from simmate.calculators.vasp.workflows.electronic_structure.base_full import (
     ElectronicStructureWorkflow,
 )
-from simmate.calculators.vasp.workflows.static_energy.matproj_hse import (
-    StaticEnergy__Vasp__MatprojHse,
+from simmate.calculators.vasp.workflows.electronic_structure.matproj_band_structure_hse import (
+    ElectronicStructure__Vasp__MatprojBandStructureHse,
 )
 from simmate.calculators.vasp.workflows.electronic_structure.matproj_density_of_states_hse import (
     ElectronicStructure__Vasp__MatprojDensityOfStatesHse,
 )
-from simmate.calculators.vasp.workflows.electronic_structure.matproj_band_structure_hse import (
-    ElectronicStructure__Vasp__MatprojBandStructureHse,
+from simmate.calculators.vasp.workflows.static_energy.matproj_hse import (
+    StaticEnergy__Vasp__MatprojHse,
 )
 
 
 class ElectronicStructure__Vasp__MatprojHseFull(ElectronicStructureWorkflow):
     """
     runs DOS and BS at Materials Project settings
     """
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/nuclear_magnetic_resonance/matproj_chemical_shifts.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/nuclear_magnetic_resonance/matproj_chemical_shifts.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/nuclear_magnetic_resonance/matproj_field_gradient.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/nuclear_magnetic_resonance/matproj_field_gradient.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from pymatgen.core import Species
 
-from simmate.toolkit import Structure
 from simmate.calculators.vasp.inputs import Incar
 from simmate.calculators.vasp.workflows.static_energy.matproj import (
     StaticEnergy__Vasp__Matproj,
 )
+from simmate.toolkit import Structure
 
 
 class Nmr__Vasp__MatprojFieldGradient(StaticEnergy__Vasp__Matproj):
     """
     This task is a reimplementation of pymatgen's
     [MPNMRSet](https://pymatgen.org/pymatgen.io.vasp.sets.html#pymatgen.io.vasp.sets.MPNMRSet)
     with mode="efg" (Electric Field Gradient).
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/population_analysis/badelf.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/population_analysis/badelf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
 from pymatgen.analysis.structure_matcher import StructureMatcher
 
-from simmate.toolkit import Structure
-from simmate.workflow_engine import Workflow
-from simmate.database.third_parties import MatprojStructure
+from simmate.calculators.bader.workflows import PopulationAnalysis__Bader__Badelf
 from simmate.calculators.vasp.workflows.static_energy.matproj import (
     StaticEnergy__Vasp__Matproj,
 )
-from simmate.calculators.bader.workflows import PopulationAnalysis__Bader__Badelf
+from simmate.database.third_parties import MatprojStructure
+from simmate.toolkit import Structure
+from simmate.workflow_engine import Workflow
 
 
 class PopulationAnalysis__Vasp__BadelfMatproj(Workflow):
     """
     Runs a static energy calculation using an extra-fine FFT grid and then
     carries out Bader analysis on the resulting charge density using the ELFCAR
     as a reference when partitioning.
@@ -25,14 +25,15 @@
     @classmethod
     def run_config(
         cls,
         structure: Structure,
         command: str = None,
         source: dict = None,
         directory: Path = None,
+        **kwargs,
     ):
 
         prebadelf_result = PopulationAnalysis__Vasp__PrebadelfMatproj.run(
             structure=structure,
             command=command,
             source=source,
             directory=directory,
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/population_analysis/bader.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/population_analysis/bader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from simmate.toolkit import Structure
-from simmate.workflow_engine import Workflow
-from simmate.calculators.vasp.workflows.static_energy.matproj import (
-    StaticEnergy__Vasp__Matproj,
-)
 from simmate.calculators.bader.workflows import (
     PopulationAnalysis__Bader__Bader,
     PopulationAnalysis__Bader__CombineChgcars,
 )
+from simmate.calculators.vasp.workflows.static_energy.matproj import (
+    StaticEnergy__Vasp__Matproj,
+)
+from simmate.toolkit import Structure
+from simmate.workflow_engine import Workflow
 
 
 class PopulationAnalysis__Vasp__BaderMatproj(Workflow):
     """
     Runs a static energy calculation using an extra-fine FFT grid and then
     carries out Bader analysis on the resulting charge density.
     """
@@ -22,14 +22,15 @@
     @classmethod
     def run_config(
         cls,
         structure: Structure,
         command: str = None,
         source: dict = None,
         directory: Path = None,
+        **kwargs,
     ):
 
         prebader_result = PopulationAnalysis__Vasp__PrebaderMatproj.run(
             structure=structure,
             command=command,
             source=source,
             directory=directory,
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/population_analysis/elf.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/population_analysis/elf.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/all.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/all.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from .matproj import Relaxation__Vasp__Matproj
 from .matproj_hse import Relaxation__Vasp__MatprojHse
-from .matproj_scan import Relaxation__Vasp__MatprojScan
 from .matproj_metal import Relaxation__Vasp__MatprojMetal
+from .matproj_scan import Relaxation__Vasp__MatprojScan
 from .mit import Relaxation__Vasp__Mit
 from .mvl_grainboundary import Relaxation__Vasp__MvlGrainboundary
-from .mvl_slab import Relaxation__Vasp__MvlSlab
 from .mvl_neb_endpoint import Relaxation__Vasp__MvlNebEndpoint
+from .mvl_slab import Relaxation__Vasp__MvlSlab
 from .quality00 import Relaxation__Vasp__Quality00
 from .quality01 import Relaxation__Vasp__Quality01
 from .quality02 import Relaxation__Vasp__Quality02
 from .quality03 import Relaxation__Vasp__Quality03
 from .quality04 import Relaxation__Vasp__Quality04
 from .staged import Relaxation__Vasp__Staged
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/matproj.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/matproj.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 # -*- coding: utf-8 -*-
 
-from simmate.calculators.vasp.workflows.base import VaspWorkflow
-from simmate.calculators.vasp.inputs.potcar_mappings import (
-    PBE_ELEMENT_MAPPINGS,
-)
 from simmate.calculators.vasp.error_handlers import (
-    TetrahedronMesh,
-    RotationMatrix,
-    Brmix,
-    Zpotrf,
-    SubspaceMatrix,
-    IncorrectShift,
-    RealOptlay,
-    Tetirr,
-    RotationNonIntMatrix,
-    LongVector,
-    TripleProduct,
-    Pricel,
     Brions,
-    Zbrent,
-    InsufficientBands,
-    Pssyevx,
-    Eddrmm,
+    Brmix,
     Edddav,
+    Eddrmm,
     Edwav,
-    Zheev,
     ElfKpar,
-    Rhosyg,
-    Posmap,
-    PointGroup,
-    SymprecNoise,
+    Frozen,
+    IncorrectShift,
     IncorrectSmearing,
+    InsufficientBands,
+    LargeSigma,
+    LongVector,
     MeshSymmetry,
-    Unconverged,
     NonConverging,
-    Potim,
+    PointGroup,
     PositiveEnergy,
-    Frozen,
-    LargeSigma,
+    Posmap,
+    Potim,
+    Pricel,
+    Pssyevx,
+    RealOptlay,
+    Rhosyg,
+    RotationMatrix,
+    RotationNonIntMatrix,
+    SubspaceMatrix,
+    SymprecNoise,
+    Tetirr,
+    TetrahedronMesh,
+    TripleProduct,
+    Unconverged,
     Walltime,
+    Zbrent,
+    Zheev,
+    Zpotrf,
 )
+from simmate.calculators.vasp.inputs.potcar_mappings import PBE_ELEMENT_MAPPINGS
+from simmate.calculators.vasp.workflows.base import VaspWorkflow
 
 
 class Relaxation__Vasp__Matproj(VaspWorkflow):
     """
     This task is a reimplementation of pymatgen's
     [MPRelaxSet](https://pymatgen.org/pymatgen.io.vasp.sets.html#pymatgen.io.vasp.sets.MPRelaxSet).
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/matproj_hse.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/matproj_hse.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 # -*- coding: utf-8 -*-
 
-from simmate.calculators.vasp.workflows.base import VaspWorkflow
-from simmate.calculators.vasp.inputs.potcar_mappings import (
-    PBE_ELEMENT_MAPPINGS,
-)
 from simmate.calculators.vasp.error_handlers import (
-    TetrahedronMesh,
-    RotationMatrix,
-    Brmix,
-    Zpotrf,
-    SubspaceMatrix,
-    IncorrectShift,
-    RealOptlay,
-    Tetirr,
-    RotationNonIntMatrix,
-    LongVector,
-    TripleProduct,
-    Pricel,
     Brions,
-    Zbrent,
-    InsufficientBands,
-    Pssyevx,
-    Eddrmm,
+    Brmix,
     Edddav,
+    Eddrmm,
     Edwav,
-    Zheev,
     ElfKpar,
-    Rhosyg,
-    Posmap,
-    PointGroup,
-    SymprecNoise,
+    Frozen,
+    IncorrectShift,
     IncorrectSmearing,
+    InsufficientBands,
+    LargeSigma,
+    LongVector,
     MeshSymmetry,
-    Unconverged,
     NonConverging,
-    Potim,
+    PointGroup,
     PositiveEnergy,
-    Frozen,
-    LargeSigma,
+    Posmap,
+    Potim,
+    Pricel,
+    Pssyevx,
+    RealOptlay,
+    Rhosyg,
+    RotationMatrix,
+    RotationNonIntMatrix,
+    SubspaceMatrix,
+    SymprecNoise,
+    Tetirr,
+    TetrahedronMesh,
+    TripleProduct,
+    Unconverged,
     Walltime,
+    Zbrent,
+    Zheev,
+    Zpotrf,
 )
+from simmate.calculators.vasp.inputs.potcar_mappings import PBE_ELEMENT_MAPPINGS
+from simmate.calculators.vasp.workflows.base import VaspWorkflow
 
 
 class Relaxation__Vasp__MatprojHse(VaspWorkflow):
     """
     This task is a reimplementation of pymatgen's
     [MPHSERelaxSet](https://pymatgen.org/pymatgen.io.vasp.sets.html#pymatgen.io.vasp.sets.MPHSERelaxSet).
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/matproj_metal.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/matproj_metal.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/matproj_scan.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/matproj_scan.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 # -*- coding: utf-8 -*-
 
-from simmate.calculators.vasp.workflows.base import VaspWorkflow
-from simmate.calculators.vasp.inputs.potcar_mappings import (
-    PBE_ELEMENT_MAPPINGS,
-)
 from simmate.calculators.vasp.error_handlers import (
-    TetrahedronMesh,
-    RotationMatrix,
-    Brmix,
-    Zpotrf,
-    SubspaceMatrix,
-    IncorrectShift,
-    RealOptlay,
-    Tetirr,
-    RotationNonIntMatrix,
-    LongVector,
-    TripleProduct,
-    Pricel,
     Brions,
-    Zbrent,
-    InsufficientBands,
-    Pssyevx,
-    Eddrmm,
+    Brmix,
     Edddav,
+    Eddrmm,
     Edwav,
-    Zheev,
     ElfKpar,
-    Rhosyg,
-    Posmap,
-    PointGroup,
-    SymprecNoise,
+    Frozen,
+    IncorrectShift,
     IncorrectSmearing,
+    InsufficientBands,
+    LargeSigma,
+    LongVector,
     MeshSymmetry,
-    Unconverged,
     NonConverging,
-    Potim,
+    PointGroup,
     PositiveEnergy,
-    Frozen,
-    LargeSigma,
+    Posmap,
+    Potim,
+    Pricel,
+    Pssyevx,
+    RealOptlay,
+    Rhosyg,
+    RotationMatrix,
+    RotationNonIntMatrix,
+    SubspaceMatrix,
+    SymprecNoise,
+    Tetirr,
+    TetrahedronMesh,
+    TripleProduct,
+    Unconverged,
     Walltime,
+    Zbrent,
+    Zheev,
+    Zpotrf,
 )
+from simmate.calculators.vasp.inputs.potcar_mappings import PBE_ELEMENT_MAPPINGS
+from simmate.calculators.vasp.workflows.base import VaspWorkflow
 
 
 class Relaxation__Vasp__MatprojScan(VaspWorkflow):
     """
     This task is a reimplementation of pymatgen's
     [MPScanRelaxSet](https://pymatgen.org/pymatgen.io.vasp.sets.html#pymatgen.io.vasp.sets.MPScanRelaxSet).
     """
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/mit.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/mit.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 # -*- coding: utf-8 -*-
 
-from simmate.calculators.vasp.workflows.base import VaspWorkflow
-from simmate.calculators.vasp.inputs.potcar_mappings import (
-    PBE_ELEMENT_MAPPINGS_LOW_QUALITY,
-)
 from simmate.calculators.vasp.error_handlers import (
-    TetrahedronMesh,
-    RotationMatrix,
-    Brmix,
-    Zpotrf,
-    SubspaceMatrix,
-    IncorrectShift,
-    RealOptlay,
-    Tetirr,
-    RotationNonIntMatrix,
-    LongVector,
-    TripleProduct,
-    Pricel,
     Brions,
-    Zbrent,
-    InsufficientBands,
-    Pssyevx,
-    Eddrmm,
+    Brmix,
     Edddav,
+    Eddrmm,
     Edwav,
-    Zheev,
     ElfKpar,
-    Rhosyg,
-    Posmap,
-    PointGroup,
-    SymprecNoise,
+    Frozen,
+    IncorrectShift,
     IncorrectSmearing,
+    InsufficientBands,
+    LargeSigma,
+    LongVector,
     MeshSymmetry,
-    Unconverged,
     NonConverging,
-    Potim,
+    PointGroup,
     PositiveEnergy,
-    Frozen,
-    LargeSigma,
+    Posmap,
+    Potim,
+    Pricel,
+    Pssyevx,
+    RealOptlay,
+    Rhosyg,
+    RotationMatrix,
+    RotationNonIntMatrix,
+    SubspaceMatrix,
+    SymprecNoise,
+    Tetirr,
+    TetrahedronMesh,
+    TripleProduct,
+    Unconverged,
     Walltime,
+    Zbrent,
+    Zheev,
+    Zpotrf,
 )
+from simmate.calculators.vasp.inputs.potcar_mappings import (
+    PBE_ELEMENT_MAPPINGS_LOW_QUALITY,
+)
+from simmate.calculators.vasp.workflows.base import VaspWorkflow
 
 
 class Relaxation__Vasp__Mit(VaspWorkflow):
     """
     This task is a reimplementation of pymatgen's
     [MITRelaxSet](https://pymatgen.org/pymatgen.io.vasp.sets.html#pymatgen.io.vasp.sets.MITRelaxSet).
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/mvl_grainboundary.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/mvl_grainboundary.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/mvl_neb_endpoint.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/mvl_neb_endpoint.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/mvl_slab.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/mvl_slab.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/quality00.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/quality00.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
-from simmate.calculators.vasp.workflows.base import VaspWorkflow
 from simmate.calculators.vasp.inputs.potcar_mappings import (
     PBE_ELEMENT_MAPPINGS_LOW_QUALITY,
 )
+from simmate.calculators.vasp.workflows.base import VaspWorkflow
 
 
 class Relaxation__Vasp__Quality00(VaspWorkflow):
     """
     Runs a very rough VASP geometry optimization with fixed lattice volume.
     `Quality 00` indicates these are absolute lowest quality settings used in
     our available presets.
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/quality01.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/quality01.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
-from simmate.calculators.vasp.workflows.base import VaspWorkflow
 from simmate.calculators.vasp.inputs.potcar_mappings import (
     PBE_ELEMENT_MAPPINGS_LOW_QUALITY,
 )
+from simmate.calculators.vasp.workflows.base import VaspWorkflow
 
 
 class Relaxation__Vasp__Quality01(VaspWorkflow):
     """
     Runs a VERY rough VASP geometry optimization.
 
     `Quality 01` indicates that on a scale from 00 to 04, these are ranked 01 in
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/quality02.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/quality02.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
-from simmate.calculators.vasp.workflows.base import VaspWorkflow
 from simmate.calculators.vasp.inputs.potcar_mappings import (
     PBE_ELEMENT_MAPPINGS_LOW_QUALITY,
 )
+from simmate.calculators.vasp.workflows.base import VaspWorkflow
 
 
 class Relaxation__Vasp__Quality02(VaspWorkflow):
     """
     Runs a rough VASP geometry optimization.
 
     `Quality 02` indicates that on a scale from 00 to 04, these are ranked 02 in
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/quality03.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/quality03.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
-from simmate.calculators.vasp.workflows.base import VaspWorkflow
 from simmate.calculators.vasp.inputs.potcar_mappings import (
     PBE_ELEMENT_MAPPINGS_LOW_QUALITY,
 )
+from simmate.calculators.vasp.workflows.base import VaspWorkflow
 
 
 class Relaxation__Vasp__Quality03(VaspWorkflow):
     """
     Runs a rough VASP geometry optimization.
 
     `Quality 03` indicates that on a scale from 00 to 04, these are ranked 03 in
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/relaxation/quality04.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/relaxation/quality04.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
-from simmate.calculators.vasp.workflows.base import VaspWorkflow
 from simmate.calculators.vasp.inputs.potcar_mappings import (
     PBE_ELEMENT_MAPPINGS_LOW_QUALITY,
 )
+from simmate.calculators.vasp.workflows.base import VaspWorkflow
 
 
 class Relaxation__Vasp__Quality04(VaspWorkflow):
     """
     Runs a rough VASP geometry optimization.
 
     `Quality 04` indicates that on a scale from 00 to 04, these are ranked 04 in
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/static_energy/matproj.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/static_energy/matproj.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/static_energy/matproj_hse.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/static_energy/matproj_hse.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/static_energy/matproj_scan.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/static_energy/matproj_scan.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/static_energy/mit.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/static_energy/mit.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/static_energy/mvl_neb_endpoint.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/static_energy/mvl_neb_endpoint.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/static_energy/quality04.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/static_energy/quality04.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/test/test_all_paths.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/test/test_all_paths.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
 
 import pytest
 
-from simmate.conftest import copy_test_files
-from simmate.workflow_engine import S3Workflow
 from simmate.calculators.vasp.inputs import Potcar
 from simmate.calculators.vasp.workflows.diffusion.all import (
     Diffusion__Vasp__NebAllPathsMit,
 )
+from simmate.conftest import copy_test_files
+from simmate.workflow_engine import S3Workflow
+
 
 # @pytest.mark.prefect_db
 @pytest.mark.slow
 @pytest.mark.django_db
 def test_neb(sample_structures, tmp_path, mocker):
 
     copy_test_files(
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/test/test_band_structure.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/test/test_band_structure.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
-from simmate.conftest import copy_test_files, make_dummy_files
 from simmate.calculators.vasp.inputs import Potcar
+from simmate.calculators.vasp.inputs.potcar_mappings import PBE_ELEMENT_MAPPINGS
 from simmate.calculators.vasp.workflows.electronic_structure.matproj_band_structure import (
     ElectronicStructure__Vasp__MatprojBandStructure,
 )
-from simmate.calculators.vasp.inputs.potcar_mappings import PBE_ELEMENT_MAPPINGS
+from simmate.conftest import copy_test_files, make_dummy_files
 
 
 def test_band_structure_setup(structure, tmp_path, mocker):
 
     # estabilish filenames that we make and commonly reference
     incar_filename = tmp_path / "INCAR"
     poscar_filename = tmp_path / "POSCAR"
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/test/test_base.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/test/test_base.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import pytest
 
-from simmate.conftest import copy_test_files, make_dummy_files
 from simmate.calculators.vasp.inputs import Potcar
-from simmate.calculators.vasp.workflows.base import VaspWorkflow
 from simmate.calculators.vasp.inputs.potcar_mappings import PBE_ELEMENT_MAPPINGS
+from simmate.calculators.vasp.workflows.base import VaspWorkflow
+from simmate.conftest import copy_test_files, make_dummy_files
 
 
 class Testing__Vasp__Dummy(VaspWorkflow):
     """
     A minimal example VaspWorkflow that is just for testing
     """
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/test/test_density_of_states.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/test/test_density_of_states.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
-from simmate.conftest import copy_test_files
 from simmate.calculators.vasp.workflows.electronic_structure.matproj_density_of_states import (
     ElectronicStructure__Vasp__MatprojDensityOfStates,
 )
+from simmate.conftest import copy_test_files
 
 
 def test_density_of_states_workup(tmp_path):
     copy_test_files(
         tmp_path,
         test_directory=__file__,
         test_folder="density_of_states.zip",
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/test/test_nudged_elastic_band.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/test/test_nudged_elastic_band.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # -*- coding: utf-8 -*-
 
-from simmate.conftest import copy_test_files, make_dummy_files
-
-from simmate.toolkit.diffusion import MigrationImages
-
 from simmate.calculators.vasp.inputs import Potcar
-from simmate.calculators.vasp.workflows.diffusion.neb_from_images_mit import (
-    Diffusion__Vasp__NebFromImagesMit,
-)
 from simmate.calculators.vasp.inputs.potcar_mappings import (
     PBE_ELEMENT_MAPPINGS_LOW_QUALITY,
 )
+from simmate.calculators.vasp.workflows.diffusion.neb_from_images_mit import (
+    Diffusion__Vasp__NebFromImagesMit,
+)
+from simmate.conftest import copy_test_files, make_dummy_files
+from simmate.toolkit.diffusion import MigrationImages
 
 
 def test_neb_setup(sample_structures, tmp_path, mocker):
 
     # To test this task we need to create images, which we do using I diffusion
     # in Y2CI2. We use [0] to grab the shortest path.
     structure = sample_structures["Y2CI2_mp-1206803_primitive"]
```

### Comparing `simmate-0.8.0/src/simmate/calculators/vasp/workflows/test/test_pymatgen_sets.py` & `simmate-0.9.0/src/simmate/calculators/vasp/workflows/test/test_pymatgen_sets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,47 @@
 # -*- coding: utf-8 -*-
 
 import pytest
-
-from simmate.conftest import make_dummy_files
-from simmate.calculators.vasp.inputs import Incar, Potcar
-from simmate.toolkit.diffusion import MigrationImages
-
+from pymatgen.analysis.diffusion.neb.io import MVLCINEBEndPointSet, MVLCINEBSet
+from pymatgen.io.vasp.sets import MITNEBSet  # MVLNPTMDSet,
 from pymatgen.io.vasp.sets import (
-    MPRelaxSet,
-    MITRelaxSet,
-    MPStaticSet,
     MITMDSet,
-    MPMDSet,
-    MPHSERelaxSet,
+    MITRelaxSet,
     MPHSEBSSet,
-    MPNonSCFSet,
+    MPHSERelaxSet,
+    MPMDSet,
     MPMetalRelaxSet,
+    MPNMRSet,
+    MPNonSCFSet,
+    MPRelaxSet,
     MPScanRelaxSet,
     MPScanStaticSet,
-    MPNMRSet,
+    MPStaticSet,
     MVLElasticSet,
     MVLGBSet,
-    MITNEBSet,
-    # MVLNPTMDSet,
 )
-from pymatgen.analysis.diffusion.neb.io import MVLCINEBSet, MVLCINEBEndPointSet
 
-from simmate.calculators.vasp.workflows.all import (
+from simmate.calculators.vasp.inputs import Incar, Potcar
+from simmate.calculators.vasp.workflows.all import (  # Dynamics__Vasp__MvlNpt,
     Diffusion__Vasp__NebFromImagesMit,
     Diffusion__Vasp__NebFromImagesMvlCi,
-    StaticEnergy__Vasp__Matproj,
-    StaticEnergy__Vasp__MatprojScan,
+    Dynamics__Vasp__Matproj,
+    Dynamics__Vasp__Mit,
     Relaxation__Vasp__Matproj,
     Relaxation__Vasp__MatprojHse,
-    Relaxation__Vasp__MatprojScan,
     Relaxation__Vasp__MatprojMetal,
+    Relaxation__Vasp__MatprojScan,
     Relaxation__Vasp__Mit,
     Relaxation__Vasp__MvlGrainboundary,
-    Relaxation__Vasp__MvlSlab,
     Relaxation__Vasp__MvlNebEndpoint,
-    Dynamics__Vasp__Mit,
-    Dynamics__Vasp__Matproj,
-    # Dynamics__Vasp__MvlNpt,
+    Relaxation__Vasp__MvlSlab,
+    StaticEnergy__Vasp__Matproj,
+    StaticEnergy__Vasp__MatprojScan,
 )
+from simmate.calculators.vasp.workflows.elastic.mvl import Elastic__Vasp__Mvl
 
 # extras that are hidden from the all endpoint
 # NOTE: these imports are long/ugly because we hide the imports from users --
 # and instead point them to higher-level workflows that call these.
 from simmate.calculators.vasp.workflows.electronic_structure.matproj_band_structure import (
     ElectronicStructure__Vasp__MatprojBandStructure,
 )
@@ -59,15 +54,16 @@
 from simmate.calculators.vasp.workflows.electronic_structure.matproj_density_of_states_hse import (
     ElectronicStructure__Vasp__MatprojDensityOfStatesHse,
 )
 from simmate.calculators.vasp.workflows.nuclear_magnetic_resonance.all import (
     Nmr__Vasp__MatprojChemicalShifts,
     Nmr__Vasp__MatprojFieldGradient,
 )
-from simmate.calculators.vasp.workflows.elastic.mvl import Elastic__Vasp__Mvl
+from simmate.conftest import make_dummy_files
+from simmate.toolkit.diffusion import MigrationImages
 
 MD_KWARGS = {
     "start_temp": 300,
     "end_temp": 1200,
     "nsteps": 10000,
 }
```

### Comparing `simmate-0.8.0/src/simmate/command_line/README.md` & `simmate-0.9.0/src/simmate/command_line/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/command_line/base_command.py` & `simmate-0.9.0/src/simmate/command_line/base_command.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 """
 This defines the base "simmate" command that all other commands stem from.
 """
 
 import click
 
 from simmate.command_line.database import database
-from simmate.command_line.workflows import workflows
-from simmate.command_line.workflow_engine import workflow_engine
 from simmate.command_line.run_server import run_server
 from simmate.command_line.start_project import start_project
+from simmate.command_line.utilities import utilities
+from simmate.command_line.workflow_engine import workflow_engine
+from simmate.command_line.workflows import workflows
 
 
 @click.group()
 def simmate():
     """
     This is the base command that all others stem from.
 
@@ -33,10 +34,11 @@
 # All commands are organized into other files, so we need to manually register
 # them to our base "simmate" command here.
 simmate.add_command(database)
 simmate.add_command(workflows)
 simmate.add_command(workflow_engine)
 simmate.add_command(run_server)
 simmate.add_command(start_project)
+simmate.add_command(utilities)
 
 # explicitly list functions so that pdoc doesn't skip them
 __all__ = ["simmate"]
```

### Comparing `simmate-0.8.0/src/simmate/command_line/database.py` & `simmate-0.9.0/src/simmate/command_line/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,30 +44,24 @@
 
     using_sqlite = DATABASES["default"]["ENGINE"] == "django.db.backends.sqlite3"
     if using_sqlite and use_prebuilt == None:
         use_prebuilt = click.confirm(
             "It looks like you are using the default database backend (sqlite3). "
             "Would you like to use a prebuilt-database with all third-party data "
             "already loaded? If this is the first time you using the prebuild, "
-            "this will involve a ~3GB download and will unpack to roughly 7GB. A "
-            "backup of the download will be stored as well (so another ~3GB disk "
+            "this will involve a ~1.5GB download and will unpack to roughly 5GB. A "
+            "backup of the download will be stored as well (so another ~1.5GB disk "
             "space will be used). We recommend answering 'yes' for beginners."
         )
 
-    # We can now proceed with reseting the database
-    click.echo("Removing database and rebuilding...")
-
     from simmate.database import connect
     from simmate.database.utilities import reset_database
 
     reset_database(use_prebuilt=use_prebuilt)
 
-    # Let the user know everything succeeded
-    click.echo("Success! Your database has been reset.")
-
 
 @database.command()
 def update():
     """Updates the database with any changes made."""
 
     # check Django if there are any updates to be made
     click.echo("Checking for updates...")
```

### Comparing `simmate-0.8.0/src/simmate/command_line/run_server.py` & `simmate-0.9.0/src/simmate/command_line/run_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     working website at http://127.0.0.1:8000/
 
     This command is exactly the same as running...
 
     django runserver --settings=simmate.configuration.django.settings
     """
 
-    from simmate.database import connect
     from django.core.management import call_command
 
+    from simmate.database import connect
+
     call_command("runserver")
 
 
 # explicitly list functions so that pdoc doesn't skip them
 __all__ = ["run_server"]
```

### Comparing `simmate-0.8.0/src/simmate/command_line/start_project.py` & `simmate-0.9.0/src/simmate/command_line/start_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 def start_project(project_name):
     """
     This creates a new folder and fills it with an example project to
     get you started with custom simmate code.
     """
 
     from pathlib import Path
+
     from django.core.management import call_command
+
     from simmate import configuration  # needed just for the filepath
 
     # This directory is where our template folder is located. We find this
     # by looking at the import path to see where python installed it.
     config_directory = Path(configuration.__file__).absolute().parent
 
     # We add on "project_template" to this file path as that's our full template
```

### Comparing `simmate-0.8.0/src/simmate/command_line/test/test_database_cli.py` & `simmate-0.9.0/src/simmate/command_line/test/test_database_cli.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/command_line/test/test_worker_cli.py` & `simmate-0.9.0/src/simmate/command_line/test/test_worker_cli.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/command_line/test/test_workflows_cli.py` & `simmate-0.9.0/src/simmate/command_line/test/test_workflows_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
 
 import yaml
 
 from simmate.calculators.vasp.inputs import Potcar
-from simmate.workflow_engine import Workflow
-from simmate.workflow_engine.workflow import DummyState
-
 from simmate.command_line.workflows import workflows
 from simmate.conftest import make_dummy_files
+from simmate.workflow_engine import Workflow
+from simmate.workflow_engine.workflow import DummyState
 
 
 def test_workflows_list_all(command_line_runner):
     # list the workflows
     result = command_line_runner.invoke(workflows, ["list-all"])
     assert result.exit_code == 0
```

### Comparing `simmate-0.8.0/src/simmate/command_line/workflow_engine.py` & `simmate-0.9.0/src/simmate/command_line/workflow_engine.py`

 * *Files 7% similar despite different names*

```diff
@@ -93,13 +93,39 @@
     """
 
     from simmate.workflow_engine import Worker
 
     Worker.run_singleflow_worker()
 
 
+@workflow_engine.command()
+@click.argument(
+    "nworkers",
+    type=int,
+)
+@click.option(
+    "--worker_command",
+    "-c",
+    default="simmate workflow-engine start-worker",
+    type=str,
+    help="the command to start each worker with. See start-worker for options",
+)
+def start_cluster(nworkers, worker_command):
+    """
+    This starts many Simmate Workers that each run in a local subprocess.
+    """
+
+    from simmate.workflow_engine.execution.utilities import start_cluster
+
+    start_cluster(
+        nworkers=nworkers,
+        worker_command=worker_command,
+    )
+
+
 # explicitly list functions so that pdoc doesn't skip them
 __all__ = [
     "workflow_engine",
     "start_worker",
     "start_singleflow_worker",
+    "start_cluster",
 ]
```

### Comparing `simmate-0.8.0/src/simmate/command_line/workflow_engine_prefect.py` & `simmate-0.9.0/src/simmate/command_line/workflow_engine_prefect.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,17 +173,15 @@
         if key == "cpus_per_worker":
             agent_kwargs["job_cpu"] = agent_kwargs.pop(key)
         elif key == "memory_per_worker":
             agent_kwargs["job_mem"] = agent_kwargs.pop(key)
         elif key == "walltime_per_job":
             agent_kwargs["walltime"] = agent_kwargs.pop(key)
 
-    from simmate.configuration.prefect.setup_resources import (
-        run_cluster_and_agent,
-    )
+    from simmate.configuration.prefect.setup_resources import run_cluster_and_agent
 
     run_cluster_and_agent(**agent_kwargs)
 
 
 # explicitly list functions so that pdoc doesn't skip them
 __all__ = [
     "workflow_engine",
```

### Comparing `simmate-0.8.0/src/simmate/command_line/workflows.py` & `simmate-0.9.0/src/simmate/command_line/workflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # -*- coding: utf-8 -*-
 
-from typing import List
 import pathlib
 
 import click
 from click import Context
 
 
 @click.group()
 def workflows():
     """A group of commands for running workflows or viewing their settings."""
     pass
 
 
-def list_options(options: List) -> int:
+def list_options(options: list) -> int:
     """
     This is a utility for click (cli) that prints of list of items as a numbered
     list. It prompts users to select an option from the list.
 
     For example, `["item1", "item2", "item3"]` would print...
     ```
         (01) item1
@@ -107,17 +106,17 @@
     """
     Let's you interactively view all available workflows and see the documentation
     on the one you select.
     """
 
     click.echo("\nGathering all available workflows...")
     from simmate.workflows.utilities import (
-        get_workflow_types,
         get_list_of_workflows_by_type,
         get_workflow,
+        get_workflow_types,
     )
 
     click.echo("\n\nWhat type of analysis are you interested in?")
     workflow_types = get_workflow_types()
     type_index = list_options(workflow_types)
     selected_type = workflow_types[type_index]
```

### Comparing `simmate-0.8.0/src/simmate/configuration/dask/client.py` & `simmate-0.9.0/src/simmate/configuration/dask/client.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/configuration/dask/connect_to_database.py` & `simmate-0.9.0/src/simmate/configuration/dask/connect_to_database.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 from simmate.utilities import get_dask_client
 client = get_dask_client()
 """
 
 # --------------------------------------------------------------------------------------
 
 
-# First setup django settings for simmate
-from simmate.database import connect
-
 # The settings (including the database) are all set up now, but django doesn't
 # actually connect to the database until a query is made. So here, we do a
 # very simple query that should work for any django database. We don't actaully
 # need the output. We just want make a call that establishes a connection.
 # Let's just use the ContentType table because it's typically small.
 from django.contrib.contenttypes.models import ContentType
 
+# First setup django settings for simmate
+from simmate.database import connect
+
 # and make a quick query
 ContentType.objects.count()
 
 
 # --------------------------------------------------------------------------------------
```

### Comparing `simmate-0.8.0/src/simmate/configuration/dask/settings.py` & `simmate-0.9.0/src/simmate/configuration/dask/settings.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/configuration/dask/setup_cluster.py` & `simmate-0.9.0/src/simmate/configuration/dask/setup_cluster.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 
-from dask.distributed import LocalCluster
 import dask_jobqueue
+from dask.distributed import LocalCluster
 from distributed.deploy.spec import SpecCluster
 
-
 # These are the different Cluster types that you can import from dask_jobqueue
 # TODO: Is there a way to dynamically determine this?
 ALLOWED_CLUSTER_TYPES = [
     "Local",
     "PBS",
     "SLURM",
     "SGE",
```

### Comparing `simmate-0.8.0/src/simmate/configuration/dask/submit.py` & `simmate-0.9.0/src/simmate/configuration/dask/submit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 
-from typing import List, Callable
-from dask.distributed import wait, TimeoutError
+from dask.distributed import TimeoutError, wait
+
 from simmate.configuration.dask.client import get_dask_client
 
 
 def batch_submit(
-    function: Callable,
-    args_list: List[dict],
+    function: callable,
+    args_list: list[dict],
     batch_size: int,
     batch_timeout: float = None,
 ):
     """
     Given a function and a list of inputs that should be iterated over, this
     submits all inputs to a Dask local cluster in batches.
```

### Comparing `simmate-0.8.0/src/simmate/configuration/django/settings.py` & `simmate-0.9.0/src/simmate/configuration/django/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 database backend being used.
 """
 
 import os
 import sys
 from pathlib import Path
 
+import dj_database_url  # needed for DigitalOcean database connection
 import yaml
 
-# from django.core.management.utils import get_random_secret_key
+from simmate import website  # needed to specify location of built-in apps
+from simmate.utilities import get_conda_env, get_directory
 
-import dj_database_url  # needed for DigitalOcean database connection
+# from django.core.management.utils import get_random_secret_key
 
-from simmate import website  # needed to specify location of built-in apps
-from simmate.utilities import get_directory, get_conda_env
 
 # --------------------------------------------------------------------------------------
 
 # SET MAIN DIRECTORIES
 
 # We check for extra django apps in the user's home directory and in a "hidden"
 # folder named "simmate/extra_applications".
```

### Comparing `simmate-0.8.0/src/simmate/configuration/django/settings_test.py` & `simmate-0.9.0/src/simmate/configuration/django/settings_test.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/configuration/django/setup.py` & `simmate-0.9.0/src/simmate/configuration/django/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 
+import logging
 import os
 
 import django
 from django.conf import settings
 
 
 def setup_django():
@@ -21,21 +22,23 @@
 
     # see if django has already been configured. If so, just exit this function.
     if settings.configured:
         return
     # BUG: originally I used the code below, but it didn't work with Prefect+Dask:
     #   if "DJANGO_SETTINGS_MODULE" in os.environ:
 
+    logging.info("Configuring database and workflows...")
     # The code below is the equiv of running 'python manage.py shell'
     # This sets up all of django for its full use. You can being importing
     # models after this is setup.
     os.environ.setdefault(
         "DJANGO_SETTINGS_MODULE", "simmate.configuration.django.settings"
     )
     django.setup()
+    logging.info("Configuration complete.")
 
 
 # When I import this module, it automatically configures django for us, including
 # connecting to the database(s). Without this file, I would instead need these two
 #  lines in every single file before I import models:
 #   from simmate.configuration.django import setup
 #   setup_django() # ensures setup
```

### Comparing `simmate-0.8.0/src/simmate/configuration/example_configs/dask_cluster.yaml` & `simmate-0.9.0/src/simmate/configuration/example_configs/dask_cluster.yaml`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/configuration/example_configs/database.yaml` & `simmate-0.9.0/src/simmate/configuration/example_configs/database.yaml`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/configuration/example_configs/prefect_agent.yaml` & `simmate-0.9.0/src/simmate/configuration/example_configs/prefect_agent.yaml`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/configuration/example_project/README.md` & `simmate-0.9.0/src/simmate/configuration/example_project/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/configuration/example_project/example_app/models.py` & `simmate-0.9.0/src/simmate/configuration/example_project/example_app/models.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 columns and features -- rather than creating everything from scratch. 
 
 For more information and advanced guides, be sure to read through our
 [base_data_types documentation](https://jacksund.github.io/simmate/simmate/database/base_data_types.html)
 """
 
 from simmate.database.base_data_types import (
+    Calculation,
     DatabaseTable,
-    table_column,
     Structure,
-    Calculation,
+    table_column,
 )
 
 
 # Mix-ins let you build out custom tables with common types of data. These will
 # automatically build out your table with many different columns. Many
 # also have a `from_toolkit` method that makes populating your database super easy
 class MyCustomTable1(Structure, Calculation):
```

### Comparing `simmate-0.8.0/src/simmate/configuration/example_project/example_app/tests.py` & `simmate-0.9.0/src/simmate/configuration/example_project/example_app/tests.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/configuration/example_project/example_app/urls.py` & `simmate-0.9.0/src/simmate/configuration/example_project/example_app/urls.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 COMING SOON: Simmate will automatically build out views for a workflow based
 on what your database table looks like. Let us know if you are waiting on this
 feature, so we can prioritize it!
 """
 
 from django.urls import path
 
-from .views import example_view, ExampleRelaxationViewSet
+from .views import ExampleRelaxationViewSet, example_view
 
 urlpatterns = [
     path(
         route="",
         view=example_view,
         name="example_app",
     ),
```

### Comparing `simmate-0.8.0/src/simmate/configuration/example_project/example_app/views.py` & `simmate-0.9.0/src/simmate/configuration/example_project/example_app/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from django.shortcuts import render
 
 from simmate.website.core_components.base_api_view import SimmateAPIViewSet
 
 from .models import ExampleRelaxationTable
 
+
 # Simple views (like a homepage) are made following django's normal format
 def example_view(request):
     context = {}
     template = "path/to/my/template.html"
     return render(request, template, context)
```

### Comparing `simmate-0.8.0/src/simmate/configuration/example_project/example_app/workflows.py` & `simmate-0.9.0/src/simmate/configuration/example_project/example_app/workflows.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,42 +13,41 @@
 sure you read through the documentation for 
 [the Workflow class](https://jacksund.github.io/simmate/simmate/workflow_engine/workflow.html) as well as relevent subclasses like the
 [S3Workflow](https://jacksund.github.io/simmate/simmate/workflow_engine/s3_workflow.html)
 or 
 [VaspWorkflow](https://jacksund.github.io/simmate/simmate/calculators/vasp/tasks/base.html)
 """
 
-from simmate.workflow_engine import Workflow
+from simmate.calculators.vasp.error_handlers import (  # There are many more available too!
+    Frozen,
+    NonConverging,
+    Unconverged,
+    Walltime,
+)
 from simmate.calculators.vasp.inputs import Incar
-from simmate.calculators.vasp.workflows.base import VaspWorkflow
 from simmate.calculators.vasp.inputs.potcar_mappings import (
     PBE_ELEMENT_MAPPINGS_LOW_QUALITY,
 )
-from simmate.calculators.vasp.error_handlers import (
-    Unconverged,
-    NonConverging,
-    Frozen,
-    Walltime,
-    # There are many more available too!
-)
+from simmate.calculators.vasp.workflows.base import VaspWorkflow
+from simmate.workflow_engine import Workflow
 
 # Import our tables from the other files.
 from .models import MyCustomTable1, MyCustomTable2
 
 # -----------------------------------------------------------------------------
 # Our first example shows off the basics
 # -----------------------------------------------------------------------------
 
 
 class Example__Python__MyExample1(Workflow):
 
     database_table = MyCustomTable1
 
     @staticmethod
-    def run_config(x, y):
+    def run_config(x, y, **kwargs):
         # This is a boring workflow because it just saves the input values
         # to our table. You can get much more creative with workflows though
         new_entry = MyCustomTable2(
             custom_column_01=x,
             custom_column_02=y,
         )
         new_entry.save()
```

### Comparing `simmate-0.8.0/src/simmate/configuration/prefect/connect_to_dask.py` & `simmate-0.9.0/src/simmate/configuration/prefect/connect_to_dask.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/conftest.py` & `simmate-0.9.0/src/simmate/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 import shutil
 from pathlib import Path
 
 import pytest
 from click.testing import CliRunner
 from django.contrib.auth.models import User
 
-from simmate.utilities import get_directory
-from simmate.toolkit import Structure, Composition, base_data_types
 from simmate.database.base_data_types import Spacegroup
+from simmate.toolkit import Composition, Structure, base_data_types
+from simmate.utilities import get_directory
 from simmate.website.test_app.models import TestStructure
 
 COMPOSITIONS_STRS = [
     "Fe1",
     "Si2",
     "C4",
     "Ti2O4",
```

### Comparing `simmate-0.8.0/src/simmate/database/README.md` & `simmate-0.9.0/src/simmate/database/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/README.md` & `simmate-0.9.0/src/simmate/database/base_data_types/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/__init__.py` & `simmate-0.9.0/src/simmate/database/base_data_types/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # -*- coding: utf-8 -*-
 
+# The order that we import these different modules is important to prevent
+# circular imports errors, so we prevent isort from changing this file.
+# isort: skip_file
+
 from simmate.utilities import get_doc_from_readme
 
 __doc__ = get_doc_from_readme(__file__)
 
 from .base import DatabaseTable, table_column
 
 from .symmetry import Spacegroup
```

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/_to_do.md` & `simmate-0.9.0/src/simmate/database/base_data_types/_to_do.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/band_structure.py` & `simmate-0.9.0/src/simmate/database/base_data_types/band_structure.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from pymatgen.io.vasp.outputs import Vasprun
 from pymatgen.electronic_structure.bandstructure import (
     BandStructureSymmLine as ToolkitBandStructure,
 )
 from pymatgen.electronic_structure.plotter import BSPlotter
+from pymatgen.io.vasp.outputs import Vasprun
 
 from simmate.database.base_data_types import (
-    table_column,
-    DatabaseTable,
     Calculation,
+    DatabaseTable,
     Structure,
+    table_column,
 )
 
 
 class BandStructure(DatabaseTable):
     """
     The electronic band structure holds information about the range of energy
     levels that are available within a material.
```

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/base.py` & `simmate-0.9.0/src/simmate/database/base_data_types/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,36 +5,34 @@
 search results.
 
 See the `simmate.database.base_data_types` (which is the parent module of 
 this one) for example usage.
 """
 
 import inspect
+import json
+import logging
 import shutil
 import urllib
 import warnings
-import yaml
-import json
 from pathlib import Path
-from typing import List, Union
-import logging
 
 import pandas
-from django.db import models  # , transaction
-from django_pandas.io import read_frame
-from django.utils.timezone import datetime
-
+import yaml
 
 # This line does NOTHING but rename a module. I have this because I want to use
 # "table_column.CharField(...)" instead of "models.CharField(...)" in my Models.
 # This let's beginners read my higher level classes and instantly understand what
 # each thing represents -- without them needing to understand
 # that Django Model == Database Table. Experts may find this annoying, so I'm
 # sorry :(
+from django.db import models  # , transaction
 from django.db import models as table_column
+from django.utils.timezone import datetime
+from django_pandas.io import read_frame
 
 
 class SearchResults(models.QuerySet):
     """
     This class adds some extra methods to the results returned from a database
     search. For example, if you searched all Structures and wanted to convert
     these to a pandas dataframe or even a list of pymatgen structures, you can
@@ -53,15 +51,15 @@
 
     All other functionality is inherited from
     [Django QuerySets](https://docs.djangoproject.com/en/4.0/ref/models/querysets/).
     """
 
     def to_dataframe(
         self,
-        fieldnames: List[str] = (),
+        fieldnames: list[str] = (),
         verbose: bool = True,
         index: str = None,
         coerce_float: str = False,
         datetime_index: str = False,
     ) -> pandas.DataFrame:
         """
         Returns a Pandas DataFrame of the search results
@@ -116,15 +114,15 @@
                 "This database table does not have a to_toolkit method implemented"
             )
 
         # now we can iterate through the queryset and return the converted
         # pymatgen objects as a list
         return [obj.to_toolkit() for obj in self]
 
-    def to_archive(self, filename: Union[str, Path] = None):
+    def to_archive(self, filename: Path | str = None):
         """
         Writes a compressed zip file using the table's base_info attribute.
         Underneath, the file is written in a csv format.
 
         This is useful for small making archive files and reloading fixtures
         to a separate database.
 
@@ -226,15 +224,15 @@
     [models in Django](https://docs.djangoproject.com/en/4.0/#the-model-layer)
     where this class only adds extra methods for convenience.
     """
 
     class Meta:
         abstract = True
 
-    base_info: List[str] = []
+    base_info: list[str] = []
     """
     The base information for this database table and only these fields are stored
     when the `to_archive` method is used. Using the columns in this list, all 
     other columns for this table can be calculated, so the columns in this list 
     are effectively the "raw data".
     """
     # TODO: setting base_info is becoming boilerplate. Consider making this
@@ -536,15 +534,15 @@
                 "set confirm_sqlite_parallel=True."
             )
 
     # @transaction.atomic  # We can't have an atomic transaction if we use Dask
     @classmethod
     def load_archive(
         cls,
-        filename: Union[str, Path] = None,
+        filename: str | Path = None,
         delete_on_completion: bool = False,
         confirm_override: bool = False,
         parallel: bool = False,
         confirm_sqlite_parallel: bool = False,
     ):
         """
         Reads a compressed zip file made by `objects.to_archive` and loads the data
@@ -591,14 +589,15 @@
         cls._confirm_override(
             confirm_override,
             parallel,
             confirm_sqlite_parallel,
         )
 
         from tqdm import tqdm
+
         from simmate.toolkit import Structure as ToolkitStructure
 
         # generate the file name if one wasn't given
         if not filename:
             # The name will be something like "MyExampleTable-2022-01-25.zip".
             # We go through all files that match "MyExampleTable-*.zip" and then
             # grab the most recent date.
@@ -747,15 +746,15 @@
                     "This table does not have a default link to load the archive "
                     " from. You must provide a remote_archive_link."
                 )
             remote_archive_link = cls.remote_archive_link
 
         # tell the user where the data comes from
         if cls._meta.app_label == "third_parties":
-            logging.warn(
+            logging.warning(
                 "this data is NOT from the Simmate team, so be sure "
                 "to visit the provider's website and to cite their work."
                 f" This data is from {cls.source} and the following paper "
                 f"should be cited: {cls.source_doi}"
             )
 
         # Predetermine the file name, which is just the ending of the URL
@@ -774,15 +773,15 @@
             confirm_override=True,  # we already confirmed this above
             parallel=parallel,
             confirm_sqlite_parallel=True,  # we already confirmed this above
         )
         logging.info("Done.")
 
     @classmethod
-    def get_column_names(cls) -> List[str]:
+    def get_column_names(cls) -> list[str]:
         """
         Returns a list of all the column names for this table and indicates which
         columns are related to other tables. This is primarily used to help
         view what data is available.
         """
         return [column.name for column in cls._meta.get_fields()]
 
@@ -820,23 +819,23 @@
             parent
             for parent in cls.__bases__
             if hasattr(simmate_mixins, parent.__name__)
             and parent.__name__ != "DatabaseTable"
         ]
 
     @classmethod
-    def get_mixin_names(cls) -> List[str]:
+    def get_mixin_names(cls) -> list[str]:
         """
         Grabs the mix-in Tables that were used to make this class and returns
         a list of their names.
         """
         return [mixin.__name__ for mixin in cls.get_mixins()]
 
     @classmethod
-    def get_extra_columns(cls) -> List[str]:
+    def get_extra_columns(cls) -> list[str]:
         """
         Finds all columns that aren't covered by the supported Table mix-ins.
 
         For example, a table made from...
 
         ``` python
         from simmate.database.base_data_types import (
```

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/calculation.py` & `simmate-0.9.0/src/simmate/database/base_data_types/calculation.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/calculation_customized.py` & `simmate-0.9.0/src/simmate/database/base_data_types/calculation_customized.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
 from pymatgen.io.vasp.outputs import Vasprun
-from simmate.database.base_data_types import table_column, Calculation
+
+from simmate.database.base_data_types import Calculation, table_column
 
 
 class CustomizedCalculation(Calculation):
     """
     A customized calculation is when the corresponding workflow has been
     fundamentally changed -- meaning critical settings for the workflow were
     updated. For example, we may want to run a workflow that uses different
```

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/calculation_nested.py` & `simmate-0.9.0/src/simmate/database/base_data_types/calculation_nested.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # -*- coding: utf-8 -*-
 
-from simmate.database.base_data_types import table_column, Calculation
-
-from typing import List
+from simmate.database.base_data_types import Calculation, table_column
 
 
 class NestedCalculation(Calculation):
     """
     A nested calculation is extremely similar to a calculation table, except here
     the linked workflow is a NestedWorkflow -- meaning it is made of multiple
     smaller workflows. For example, we may want to run a workflow that runs a
@@ -32,15 +30,15 @@
     corrections = None
     # For now I delete this column. This line removes the field.
 
     @classmethod
     def create_subclass_from_calcs(
         cls,
         name: str,
-        child_database_tables: List[Calculation],
+        child_database_tables: list[Calculation],
         module: str,
         **extra_columns,
     ):
         """
         Dynamically creates a subclass of NestedCalculation -- and handles linking
         together all child calculation tables.
```

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/density_of_states.py` & `simmate-0.9.0/src/simmate/database/base_data_types/density_of_states.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
-from pymatgen.io.vasp.outputs import Vasprun
 from pymatgen.electronic_structure.dos import CompleteDos
 from pymatgen.electronic_structure.plotter import DosPlotter
+from pymatgen.io.vasp.outputs import Vasprun
 
 from simmate.database.base_data_types import (
-    table_column,
-    DatabaseTable,
     Calculation,
+    DatabaseTable,
     Structure,
+    table_column,
 )
 
 
 class DensityofStates(DatabaseTable):
     """
     The electronic density of states holds information about the range of energy
     levels that are available within a material.
```

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/dynamics.py` & `simmate-0.9.0/src/simmate/database/base_data_types/dynamics.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 
 """
 This module is experimental and subject to change.
 """
 
 from pathlib import Path
 
+from pymatgen.io.vasp.outputs import Vasprun
+
 from simmate.database.base_data_types import (
-    table_column,
-    Structure,
+    Calculation,
     Forces,
+    Structure,
     Thermodynamics,
-    Calculation,
+    table_column,
 )
 
-from typing import List
-from pymatgen.io.vasp.outputs import Vasprun
-
 
 class DynamicsRun(Structure, Calculation):
     """
     Holds results from a dynamics simulations -- often referred to as a molecular
     dynamics run.
 
     In addition to the attributes listed, you can also access all ionic steps
@@ -52,15 +51,15 @@
     steps set. In some cases, there may be fewer steps when the simulation is 
     stopped early.
     """
 
     def update_from_vasp_run(
         self,
         vasprun: Vasprun,
-        corrections: List,
+        corrections: list[tuple[str]],
         directory: Path,
     ):
         """
         Given a Vasprun object from a finished dynamics run, this will update the
         DynamicsRun table entry and the corresponding DynamicsIonicStep entries.
 
         #### Parameters
```

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/forces.py` & `simmate-0.9.0/src/simmate/database/base_data_types/forces.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import numpy
 
-from simmate.toolkit import Structure as ToolkitStructure
 from simmate.database.base_data_types import DatabaseTable, table_column
+from simmate.toolkit import Structure as ToolkitStructure
 
 
 class Forces(DatabaseTable):
     class Meta:
         abstract = True
 
     base_info = [
```

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/nudged_elastic_band.py` & `simmate-0.9.0/src/simmate/database/base_data_types/nudged_elastic_band.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,25 +2,22 @@
 
 """
 WARNING: This module is experimental and subject to change.
 """
 
 from pathlib import Path
 
+from pymatgen.analysis.transition_state import NEBAnalysis
 from pymatgen.core.sites import PeriodicSite
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
-from pymatgen.analysis.transition_state import NEBAnalysis
 
+from simmate.database.base_data_types import DatabaseTable, Structure, table_column
 from simmate.toolkit import Structure as ToolkitStructure
 from simmate.toolkit.diffusion import MigrationHop as ToolkitMigrationHop
-from simmate.database.base_data_types import (
-    table_column,
-    DatabaseTable,
-    Structure,
-)
+
 
 # TODO: consider making a NestedCalculation
 class DiffusionAnalysis(Structure):
     class Meta:
         app_label = "workflows"
 
     migrating_specie = table_column.CharField(max_length=4, blank=True, null=True)
```

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/population_analysis.py` & `simmate-0.9.0/src/simmate/database/base_data_types/population_analysis.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/relaxation.py` & `simmate-0.9.0/src/simmate/database/base_data_types/relaxation.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,28 +61,26 @@
 Note there are two tables involved. One stores all of the ionic steps, and the
 other connects all ionic steps to a specific calculation and result.
 
 """
 
 from pathlib import Path
 
+import plotly.graph_objects as plotly_go
+from plotly.subplots import make_subplots
+from pymatgen.io.vasp.outputs import Vasprun
+
 from simmate.database.base_data_types import (
-    table_column,
-    Structure,
+    Calculation,
     Forces,
+    Structure,
     Thermodynamics,
-    Calculation,
+    table_column,
 )
 
-from plotly.subplots import make_subplots
-import plotly.graph_objects as plotly_go
-
-from typing import List
-from pymatgen.io.vasp.outputs import Vasprun
-
 
 class Relaxation(Structure, Thermodynamics, Calculation):
     """
     This table holds all data from a structure relaxation and also links to
     IonicStep table which holds all of the structure/energy/forces for each
     ionic step.
 
@@ -204,15 +202,15 @@
         # TODO: load corrections/directory from the metadata and corrections files.
 
         return relaxation
 
     def update_from_vasp_run(
         self,
         vasprun: Vasprun,
-        corrections: List,
+        corrections: list,
         directory: Path,
     ):
         """
         Given a Vasprun object from a finished relaxation, this will update the
         Relaxation table entry and the corresponding IonicStep entries.
 
         #### Parameters
```

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/static_energy.py` & `simmate-0.9.0/src/simmate/database/base_data_types/static_energy.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 
+from pymatgen.io.vasp.outputs import Vasprun
+
 from simmate.database.base_data_types import (
-    table_column,
-    Structure,
+    Calculation,
     Forces,
+    Structure,
     Thermodynamics,
-    Calculation,
+    table_column,
 )
 
-from pymatgen.io.vasp.outputs import Vasprun
-
 
 class StaticEnergy(Structure, Thermodynamics, Forces, Calculation):
     class Meta:
         app_label = "workflows"
 
     base_info = (
         [
```

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/structure.py` & `simmate-0.9.0/src/simmate/database/base_data_types/structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from scipy.constants import Avogadro
 
+from simmate.database.base_data_types import DatabaseTable, Spacegroup, table_column
 from simmate.toolkit import Structure as ToolkitStructure
-from simmate.database.base_data_types import (
-    DatabaseTable,
-    table_column,
-    Spacegroup,
-)
 
 
 class Structure(DatabaseTable):
     class Meta:
         abstract = True
 
     base_info = ["structure_string"]
```

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/symmetry.py` & `simmate-0.9.0/src/simmate/database/base_data_types/symmetry.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
-from simmate.database.base_data_types import DatabaseTable, table_column
-
 from pymatgen.symmetry.groups import SpaceGroup as PymatgenSpacegroup
 
+from simmate.database.base_data_types import DatabaseTable, table_column
+
 # NOTE: This class is *not* meant to store data about each spacegroup, but instead
 # is just to help with querying Structures. If you want all spacegroup data
 # (such as the list of symmetry operations), then you should instead look at
 # pymatgen.symmetry.groups.SpaceGroup. There is also spglib where you
 # can get data using spglib.get_spacegroup_type(hall_number), but this is organized
 # into 530 hall spacegroups, rather than the typical 230 international spacegroups.
```

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/test/test_base_db.py` & `simmate-0.9.0/src/simmate/database/base_data_types/test/test_base_db.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/test/test_calculation_db.py` & `simmate-0.9.0/src/simmate/database/base_data_types/test/test_calculation_db.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/test/test_dynamics_db.py` & `simmate-0.9.0/src/simmate/database/base_data_types/test/test_dynamics_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
 
 import pytest
-
 from pandas import DataFrame
 
-# from pymatgen.io.vasp.outputs import Vasprun
-
+from simmate.database.base_data_types import DynamicsIonicStep, DynamicsRun
 from simmate.toolkit import Structure
-from simmate.database.base_data_types import DynamicsRun, DynamicsIonicStep
+
+# from pymatgen.io.vasp.outputs import Vasprun
 
 
 @pytest.mark.django_db
 def test_static_energy_table(structure):
 
     # test writing columns
     DynamicsRun.show_columns()
```

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/test/test_forces_db.py` & `simmate-0.9.0/src/simmate/database/base_data_types/test/test_forces_db.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/test/test_relaxation_db.py` & `simmate-0.9.0/src/simmate/database/base_data_types/test/test_relaxation_db.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
 
 import pytest
-
 from pandas import DataFrame
 
-# from pymatgen.io.vasp.outputs import Vasprun
-
+from simmate.database.base_data_types import IonicStep, Relaxation
 from simmate.toolkit import Structure
-from simmate.database.base_data_types import Relaxation, IonicStep
+
+# from pymatgen.io.vasp.outputs import Vasprun
 
 
 @pytest.mark.django_db
 def test_relaxation_table(structure):
 
     # test writing columns
     Relaxation.show_columns()
```

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/test/test_static_energy_db.py` & `simmate-0.9.0/src/simmate/database/base_data_types/test/test_static_energy_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import pytest
-
 from pandas import DataFrame
 
-from simmate.toolkit import Structure
 from simmate.database.base_data_types import StaticEnergy
+from simmate.toolkit import Structure
 
 
 @pytest.mark.django_db
 def test_static_energy_table(structure, tmp_path):
 
     # test writing columns
     StaticEnergy.show_columns()
```

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/test/test_structure_db.py` & `simmate-0.9.0/src/simmate/database/base_data_types/test/test_structure_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # -*- coding: utf-8 -*-
 
 import pytest
-
 from pandas import DataFrame
 
 from simmate.toolkit import Structure
 from simmate.website.test_app.models import TestStructure
 
 
 @pytest.mark.django_db
```

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/test/test_thermodynamics_db.py` & `simmate-0.9.0/src/simmate/database/base_data_types/test/test_thermodynamics_db.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/database/base_data_types/thermodynamics.py` & `simmate-0.9.0/src/simmate/database/base_data_types/thermodynamics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 
-from tqdm import tqdm
 import logging
 
-from simmate.toolkit import Structure as ToolkitStructure
-from simmate.database.base_data_types import DatabaseTable, table_column
-from simmate.utilities import get_chemical_subsystems
-
 # BUG: This prints a tqdm error so we silence it here.
 import warnings
 
+from tqdm import tqdm
+
+from simmate.database.base_data_types import DatabaseTable, table_column
+from simmate.toolkit import Structure as ToolkitStructure
+from simmate.utilities import get_chemical_subsystems
+
 with warnings.catch_warnings(record=True):
-    from pymatgen.analysis.phase_diagram import PDEntry
-    from pymatgen.analysis.phase_diagram import PhaseDiagram
+    from pymatgen.analysis.phase_diagram import PDEntry, PhaseDiagram
 
 
 class Thermodynamics(DatabaseTable):
     class Meta:
         abstract = True
 
     base_info = ["energy"]
@@ -176,15 +176,15 @@
         # Now  go through each and run the analysis.
         # OPTIMIZE: Some systems will be analyzed multiple times. For example,
         # C would be repeatedly updated through C, C-O, Y-C-F, etc.
         for chemical_system in tqdm(chemical_systems):
             try:
                 cls.update_chemical_system_stabilities(chemical_system)
             except ValueError as exception:
-                logging.warn(f"Failed for {chemical_system} with error: {exception}")
+                logging.warning(f"Failed for {chemical_system} with error: {exception}")
 
         # BUG: can't use parallel=True as an input
         # Because different systems may need to update a single one at the same
         # time, errors will be thrown due to row locking. For example, Y-C and
         # Sc-C system might both try to update a C structure at the same time
         # and one will throw an error.
         #
```

### Comparing `simmate-0.8.0/src/simmate/database/connect.py` & `simmate-0.9.0/src/simmate/database/connect.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/database/third_parties/README.md` & `simmate-0.9.0/src/simmate/database/third_parties/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/database/third_parties/aflow/prototypes.py` & `simmate-0.9.0/src/simmate/database/third_parties/aflow/prototypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-from simmate.database.base_data_types import table_column, Structure
+from simmate.database.base_data_types import Structure, table_column
 
 
 class AflowPrototype(Structure):
     """
     A collection of prototype crystal structures from the AFLOW library.
 
     While this is still a table of structures, this should instead be viewed
```

### Comparing `simmate-0.8.0/src/simmate/database/third_parties/aflow/structures.py` & `simmate-0.9.0/src/simmate/database/third_parties/aflow/structures.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-from simmate.database.base_data_types import table_column, Structure, Thermodynamics
+from simmate.database.base_data_types import Structure, Thermodynamics, table_column
 
 
 class AflowStructure(Structure, Thermodynamics):
     """
     Crystal structures from the [AFLOW](http://aflowlib.org/) database.
 
     Currently, this table only stores strucure and thermodynamic information,
```

### Comparing `simmate-0.8.0/src/simmate/database/third_parties/cod.py` & `simmate-0.9.0/src/simmate/database/third_parties/cod.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-from simmate.database.base_data_types import table_column, Structure
+from simmate.database.base_data_types import Structure, table_column
 
 
 class CodStructure(Structure):
     """
     Crystal structures from the [COD](http://www.crystallography.net/cod/) database.
 
     Currently, this table only stores the strucure, plus comments on whether the
```

### Comparing `simmate-0.8.0/src/simmate/database/third_parties/for_providers/README.md` & `simmate-0.9.0/src/simmate/database/third_parties/for_providers/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/database/third_parties/for_providers/_todo/materials_cloud.py` & `simmate-0.9.0/src/simmate/database/third_parties/for_providers/_todo/materials_cloud.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/database/third_parties/for_providers/_todo/mpds.py` & `simmate-0.9.0/src/simmate/database/third_parties/for_providers/_todo/mpds.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,20 @@
 
 NOTE: I'm currently running into permission issues with MPDS, and will return to
 this provider after talking with their team.
 
 """
 
 from django.db import transaction
-
-from tqdm import tqdm
-from simmate.toolkit import Structure
 from mpds_client import MPDSDataRetrieval, MPDSDataTypes
+from tqdm import tqdm
 
 from simmate.database import connect
-
 from simmate.database.third_parties.mpds import MpdsStructure
+from simmate.toolkit import Structure
 
 
 @transaction.atomic
 def load_all_structures(api_key="9WPgw8xYqYcB91ylff1CogIaXd4MGq6RoEZjwC1L0fh66uMw"):
 
     # !!! Remove key in production
```

### Comparing `simmate-0.8.0/src/simmate/database/third_parties/for_providers/aflow.py` & `simmate-0.9.0/src/simmate/database/third_parties/for_providers/aflow.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 Note that this not from the official AFLOW team, but it is made such that keywords
 are pulled dynamically from the AFLOW servers -- any updates in AFLOW's API should
 be properly handled. Also structures are loaded as ASE Atom objects, which we then
 convert to pymatgen.
 
 """
 
-from tqdm import tqdm
 from pymatgen.io.ase import AseAtomsAdaptor
+from tqdm import tqdm
 
 from simmate.database.third_parties.aflow import AflowStructure
 
 
 def load_all_structures():
     """
     Only use this function if you are part of the Simmate dev team!
```

### Comparing `simmate-0.8.0/src/simmate/database/third_parties/for_providers/aflow_prototypes.py` & `simmate-0.9.0/src/simmate/database/third_parties/for_providers/aflow_prototypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,21 @@
 Note that this not from the official AFLOW team, but it is made such that keywords
 are pulled dynamically from the AFLOW servers -- any updates in AFLOW's API should
 be properly handled. Also structures are loaded as ASE Atom objects, which we then
 convert to pymatgen.
 
 """
 
-from tqdm import tqdm
-
 from django.db import transaction
 
 # This looks like the easiest way to grab all of the data -- as AFLOW doesn't
 # have any good documentation on doing this.
 from pymatgen.analysis.prototypes import AFLOW_PROTOTYPE_LIBRARY
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
+from tqdm import tqdm
 
 from simmate.database.third_parties import AflowPrototype
 
 
 @transaction.atomic
 def load_all_prototypes():
```

### Comparing `simmate-0.8.0/src/simmate/database/third_parties/for_providers/cod.py` & `simmate-0.9.0/src/simmate/database/third_parties/for_providers/cod.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/database/third_parties/for_providers/jarvis.py` & `simmate-0.9.0/src/simmate/database/third_parties/for_providers/jarvis.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,18 @@
 
 Alternatively, we could manually download 
 [their database json files](https://jarvis-materials-design.github.io/dbdocs/thedownloads/). We specifically look at the "3D-materials curated data".
 
 """
 
 from django.db import transaction
-
 from tqdm import tqdm
-from simmate.toolkit import Structure
 
 from simmate.database.third_parties import JarvisStructure
+from simmate.toolkit import Structure
 
 
 @transaction.atomic
 def load_all_structures():
     """
     Only use this function if you are part of the Simmate dev team!
```

### Comparing `simmate-0.8.0/src/simmate/database/third_parties/for_providers/materials_project.py` & `simmate-0.9.0/src/simmate/database/third_parties/for_providers/materials_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 PyMatGen offers an easy way to do this in python -- the MPRester class. All you
 need is [an API key from their site](https://materialsproject.org/open) and pymatgen
 installed. For now, we only pull the mp-id, structure, and final energy.
 
 """
 
 from django.db import transaction
-
-from tqdm import tqdm
 from pymatgen.ext.matproj import MPRester
+from tqdm import tqdm
 
 from simmate.database.third_parties import MatprojStructure
 
 
 @transaction.atomic
 def load_all_structures(
     api_key: str,
```

### Comparing `simmate-0.8.0/src/simmate/database/third_parties/for_providers/oqmd.py` & `simmate-0.9.0/src/simmate/database/third_parties/for_providers/oqmd.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 at https://github.com/mohanliu/qmpy_rester. For now the package is only available
 via a pip install.
 
 For other options such as the REST API, check out http://oqmd.org/static/docs/restful.html
 
 """
 
-from tqdm import tqdm
 import pandas
 from django.db import transaction
+from tqdm import tqdm
 
-from simmate.toolkit import Structure
 from simmate.database.third_parties import OqmdStructure
+from simmate.toolkit import Structure
 
 
 @transaction.atomic
 def load_all_structures_from_api():
     """
     Only use this function if you are part of the Simmate dev team!
```

### Comparing `simmate-0.8.0/src/simmate/database/third_parties/jarvis.py` & `simmate-0.9.0/src/simmate/database/third_parties/jarvis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-from simmate.database.base_data_types import table_column, Structure
+from simmate.database.base_data_types import Structure, table_column
 
 
 class JarvisStructure(Structure):
     """
     Crystal structures from the [JARVIS](https://jarvis.nist.gov/) database.
 
     Currently, this table only stores strucure and reported energy above hull.
```

### Comparing `simmate-0.8.0/src/simmate/database/third_parties/materials_project.py` & `simmate-0.9.0/src/simmate/database/third_parties/materials_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-from simmate.database.base_data_types import table_column, Structure, Thermodynamics
+from simmate.database.base_data_types import Structure, Thermodynamics, table_column
 
 
 class MatprojStructure(Structure, Thermodynamics):
     """
     Crystal structures from the [Materials Project](https://materialsproject.org/)
     database.
```

### Comparing `simmate-0.8.0/src/simmate/database/third_parties/oqmd.py` & `simmate-0.9.0/src/simmate/database/third_parties/oqmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-from simmate.database.base_data_types import table_column, Structure
+from simmate.database.base_data_types import Structure, table_column
 
 
 class OqmdStructure(Structure):
     """
     Crystal structures from the [OQMD](http://oqmd.org/) database.
 
     Currently, this table only stores strucure and thermodynamic information,
```

### Comparing `simmate-0.8.0/src/simmate/database/third_parties/utilities.py` & `simmate-0.9.0/src/simmate/database/third_parties/utilities.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # -*- coding: utf-8 -*-
 
-import urllib
-import shutil
 import logging
+import shutil
+import urllib
 
-from simmate.utilities import get_directory
 from simmate.configuration.django.settings import DATABASES, SIMMATE_DIRECTORY
+from simmate.database.third_parties import AflowPrototype  # AflowStructure,
 from simmate.database.third_parties import (
-    # AflowStructure,
-    AflowPrototype,
     CodStructure,
     JarvisStructure,
     MatprojStructure,
     OqmdStructure,
 )
+from simmate.utilities import get_directory
 
 
 def load_remote_archives(**kwargs):
     """
     Goes through all third-party databases and loads their most recent remote
     archives (if available). This utility helps with initializing a new
     database build.
@@ -53,15 +52,15 @@
 def load_default_sqlite3_build():
     """
     Loads a sqlite3 database archive that has all third-party data already
     populated in it.
     """
     # DEV NOTE: the prebuild filename is updated when new versions call for it.
     # Therefore, this value hardcoded specifically for each simmate version
-    archive_filename = "prebuild-2022-08-11.zip"
+    archive_filename = "prebuild-2022-08-17.zip"
 
     # Make sure the backend is using SQLite3 as this is the only allowed format
     assert DATABASES["default"]["ENGINE"] == "django.db.backends.sqlite3"
 
     # check if the prebuild directory exists, and create it if not
     archive_dir = get_directory(SIMMATE_DIRECTORY / "sqlite-prebuilds")
 
@@ -69,23 +68,25 @@
 
     # check if the archive has been downloaded before. If not, download!
     if not archive_filename_full.exists():
         remote_archive_link = f"https://archives.simmate.org/{archive_filename}"
         # Download the archive zip file from the URL to the current working dir
         logging.info("Downloading database file...")
         urllib.request.urlretrieve(remote_archive_link, archive_filename_full)
-        logging.info("Done.")
+        logging.info("Done downloading.")
     else:
         logging.info(
             f"Found past download at {archive_filename_full}. Using archive as base."
         )
 
+    logging.info("Unpacking prebuilt to active database...")
     # uncompress the zip file to archive directory
     shutil.unpack_archive(
         archive_filename_full,
         extract_dir=archive_dir,
     )
 
     # rename and move the sqlite file to be the new database
     db_filename_orig = archive_filename_full.with_suffix(".sqlite3")  # was .zip
     db_filename_new = DATABASES["default"]["NAME"]
     shutil.move(db_filename_orig, db_filename_new)
+    logging.info("Done unpacking.")
```

### Comparing `simmate-0.8.0/src/simmate/database/utilities.py` & `simmate-0.9.0/src/simmate/database/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
+import logging
 import shutil
 from pathlib import Path
-import logging
 
 from django.apps import apps
 from django.core.management import call_command
 
 from simmate.configuration.django.settings import DATABASES
 
 # Lists off which apps to update/create. By default, I do all apps that are installed
@@ -22,24 +22,27 @@
     call_command("migrate")
 
 
 def reset_database(apps_to_migrate=APPS_TO_MIGRATE, use_prebuilt=False):
 
     # BUG: Why doesn't call_command("flush") do this? How is it different?
 
+    # We can now proceed with reseting the database
+    logging.info("Removing database and rebuilding...")
+
     # BUG: this is only for SQLite3
     # Consider wrapping the django-extensions function for this instead:
     #   https://django-extensions.readthedocs.io/en/latest/reset_db.html
     # An example command to call this (when django-extensions is installed) is...
     #   django-admin reset_db --settings=simmate.configuration.django.settings
     # Note: this does not remove migration files or reapply migrating after
     # Make sure the backend is using SQLite3 as this is the only allowed format
     using_sqlite = DATABASES["default"]["ENGINE"] == "django.db.backends.sqlite3"
     if not using_sqlite:
-        logging.warn(
+        logging.warning(
             "reseting your database does not clear your database tables "
             "for non-sqlite3 backends. Make sure you only use this function when "
             "initially building your database and not after."
         )
 
     # grab the location of the database file. I assume the default database for now.
     db_filename = DATABASES["default"]["NAME"]
@@ -64,24 +67,29 @@
     update_database(apps_to_migrate)
 
     # instead of building the database from scratch, we instead download a
     # prebuilt database file.
     if using_sqlite and use_prebuilt:
         from simmate.database.third_parties import load_default_sqlite3_build
 
+        logging.info("Setting up prebuilt database...")
         load_default_sqlite3_build()
 
     # Otherwise we leave the empty database.
     # Because this is our first time building the database, we also want to
     # load the Spacegroup metadata for us to query Structures by.
     else:
         from simmate.database.base_data_types import Spacegroup
 
+        logging.info("Loading default data...")
         Spacegroup._load_database_from_toolkit()
 
+    # Let the user know everything succeeded
+    logging.info("Success! Your database has been reset.")
+
 
 def dump_database_to_json(filename="database_dump.json", exclude=[]):
 
     # execute the following commands to write the database to a json file
     call_command("dumpdata", output=filename, exclude=exclude)
```

### Comparing `simmate-0.8.0/src/simmate/database/workflow_results/README.md` & `simmate-0.9.0/src/simmate/database/workflow_results/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/database/workflow_results/__init__.py` & `simmate-0.9.0/src/simmate/database/workflow_results/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 
 from simmate.utilities import get_doc_from_readme
 
 __doc__ = get_doc_from_readme(__file__)
 
 from simmate.database.base_data_types import (
-    Relaxation,
-    IonicStep,
-    StaticEnergy,
     BandStructureCalc,
+    CustomizedCalculation,
     DensityofStatesCalc,
-    PopulationAnalysis,
-    DynamicsRun,
-    DynamicsIonicStep,
     DiffusionAnalysis,
+    DynamicsIonicStep,
+    DynamicsRun,
+    IonicStep,
     MigrationHop,
     MigrationImage,
-    CustomizedCalculation,
+    PopulationAnalysis,
+    Relaxation,
+    StaticEnergy,
 )
-
 from simmate.toolkit.structure_prediction.evolution.database import (
     EvolutionarySearch,
     StructureSource,
 )
```

### Comparing `simmate-0.8.0/src/simmate/file_converters/README.md` & `simmate-0.9.0/src/simmate/file_converters/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/file_converters/structure/README.md` & `simmate-0.9.0/src/simmate/file_converters/structure/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/file_converters/structure/ase.py` & `simmate-0.9.0/src/simmate/file_converters/structure/ase.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/file_converters/structure/cif.py` & `simmate-0.9.0/src/simmate/file_converters/structure/cif.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/file_converters/structure/database.py` & `simmate-0.9.0/src/simmate/file_converters/structure/database.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -51,17 +51,17 @@
 # access the original database object
 database_structure = toolkit_structure.database_object
 ```
 """
 
 from django.utils.module_loading import import_string
 
-from simmate.toolkit import Structure as ToolkitStructure
 from simmate.database import connect
 from simmate.database.base_data_types import Structure as DatabaseStructure
+from simmate.toolkit import Structure as ToolkitStructure
 from simmate.website.workflows import models as all_datatables
 
 
 class DatabaseAdapter:
     """
     Adaptor for conversion between the Simmate ToolkitStructure object and
     Simmate DatabaseStructure object.
```

### Comparing `simmate-0.8.0/src/simmate/file_converters/structure/jarvis.py` & `simmate-0.9.0/src/simmate/file_converters/structure/jarvis.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/file_converters/structure/pymatgen.py` & `simmate-0.9.0/src/simmate/file_converters/structure/pymatgen.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 new_pmg_object = PyMatGenAdapter.get_pymatgen(structure)
 
 # convert back to PyMatgen/Simmate
 new_toolkit_object = PyMatGenAdapter.get_toolkit(new_pmg_object)
 ```
 """
 
-from simmate.toolkit import Structure as ToolkitStructure
 from pymatgen.core.structure import Structure as PyMatGenStructure
 
+from simmate.toolkit import Structure as ToolkitStructure
+
 
 class PyMatGenAdapter:
     """
     Adaptor for conversion between the Simmate ToolkitStructure object and
     pymatgen Structure objects.
     """
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/README.md` & `simmate-0.9.0/src/simmate/toolkit/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/base_data_types/_to_do/README.md` & `simmate-0.9.0/src/simmate/toolkit/base_data_types/_to_do/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/base_data_types/_to_do/element_data.py` & `simmate-0.9.0/src/simmate/toolkit/base_data_types/_to_do/element_data.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/base_data_types/_to_do/elements.py` & `simmate-0.9.0/src/simmate/toolkit/base_data_types/_to_do/elements.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/base_data_types/_to_do/lattice.py` & `simmate-0.9.0/src/simmate/toolkit/base_data_types/_to_do/lattice.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/base_data_types/_to_do/species.py` & `simmate-0.9.0/src/simmate/toolkit/base_data_types/_to_do/species.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/base_data_types/composition.py` & `simmate-0.9.0/src/simmate/toolkit/base_data_types/composition.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,18 @@
 
 It is a very basic extension PyMatGen's core Composition class, as it only adds
 a few extra methods and does not change any other usage. Note that this class
 is currently NOT used by Simmate's Structure class. For Simmate, 
 Structure.composition will still return a pymatgen composition object.
 """
 
-import warnings
 import itertools
-from typing import List
+import warnings
 
 import numpy
-
 from pymatgen.core import Composition as PymatgenComposition
 
 
 class Composition(PymatgenComposition):
     # Leave docstring blank and just inherit from pymatgen
 
     def radii_estimate(self, radius_method: str = "ionic"):
@@ -185,15 +183,15 @@
                 row.append(limit)
             matrix.append(row)
         # convert the result matrix of list matrix to a numpy array before returning
         element_distance_matrix = numpy.array(matrix)
         return element_distance_matrix
 
     @property
-    def chemical_subsystems(self) -> List[str]:
+    def chemical_subsystems(self) -> list[str]:
         """
         Returns all chemical systems of this composition's chemical system.
 
         For example, Y2C has the chemical system "Y-C" and would return
         ["Y", "C", "C-Y"]. Note that the returned list has elements of a given
         system in alphabetical order (i.e. it gives "C-Y" and not "Y-C")
 
@@ -219,7 +217,24 @@
             for combo in itertools.combinations(system_cleaned, i + 1):
                 # Combo will be a tuple of elements that we then convert back to a
                 # chemical system. We also sort this alphabetically.
                 #   ex: ("Y", "C", "F") ---> "C-F-Y"
                 subsystem = "-".join(sorted(combo))
                 subsystems.append(subsystem)
         return subsystems
+
+    @classmethod
+    def from_dynamic(cls, composition):
+
+        # if the input is already a pymatgen structure, just return it back
+        if isinstance(composition, PymatgenComposition):
+            return composition
+
+        # if the "@module" key is in the dictionary, then we have a pymatgen
+        # structure dict which we convert to a pymatgen object and return
+        elif isinstance(composition, dict) and "@module" in composition.keys():
+            return cls.from_dict(composition)
+
+        # Otherwise attempt to initialize the input, where we expect it to
+        # be one of types accepted (e.g. a string or dictionary)
+        else:
+            return cls(composition)
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/base_data_types/structure.py` & `simmate-0.9.0/src/simmate/toolkit/base_data_types/structure.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/base_data_types/test/test_composition.py` & `simmate-0.9.0/src/simmate/toolkit/base_data_types/test/test_composition.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/creators/lattice.py` & `simmate-0.9.0/src/simmate/toolkit/creators/lattice.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # -*- coding: utf-8 -*-
 
 ##############################################################################
 
 from numpy.random import choice
-
 from pymatgen.core.lattice import Lattice
 
 from simmate.toolkit.creators.vector import (
-    UniformlyDistributedVectors,
     NormallyDistributedVectors,
+    UniformlyDistributedVectors,
 )
 
 ##############################################################################
 
 # Generates a random lattice without symmetry
 # this is the same as RandomSymLattice when spacegroup is assumed to be 1
 class RandomLattice:
@@ -161,14 +160,15 @@
         return lattice
 
 
 ##############################################################################
 
 from simmate.toolkit.symmetry.wyckoff import loadWyckoffData
 
+
 #!!! EASY SPEED/MEMORY IMPROVEMENTS CAN BE MADE HERE (ON INIT)
 class RSLSmartVolume:
     def __init__(
         self,
         composition,
         volume=None,
         spacegroup_include=range(1, 231),
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/creators/sites/random.py` & `simmate-0.9.0/src/simmate/toolkit/creators/sites/random.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/creators/sites/random_wyckoff.py` & `simmate-0.9.0/src/simmate/toolkit/creators/sites/random_wyckoff.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 # -*- coding: utf-8 -*-
 
-from numpy.random import randint, choice
+import logging
 
+from numpy.random import choice, randint
 from tqdm import tqdm
 
+from simmate.toolkit import Composition
+from simmate.toolkit.creators.vector import UniformlyDistributedVectors
 from simmate.toolkit.symmetry.wyckoff import (
+    findValidWyckoffCombos,
     loadAsymmetricUnitData,
     loadWyckoffData,
-    findValidWyckoffCombos,
 )
-from simmate.toolkit.creators.vector import UniformlyDistributedVectors
 
 
 class RandomWySites:
     def __init__(
         self,
-        composition,  # must be a pymatgen Composition object
-        spacegroup_include=range(1, 231),
-        spacegroup_exclude=[],
+        composition: Composition,
+        spacegroup_include: list[int] = range(1, 231),
+        spacegroup_exclude: list[int] = [],
         coords_generation_method=UniformlyDistributedVectors,
-        coords_gen_options=dict(),  # asymmetric_unit_boundries is include in extra_conditions automatically
+        # note, asymmetric_unit_boundries is included in coords_gen_options
+        # automatically so this input is anything extra.
+        coords_gen_options: dict = dict(),
+        lazily_generate_combinations: bool = True,
     ):
 
         # make a list of spacegroups that we are allowed to choose from
         self.spacegroup_options = [
             sg for sg in spacegroup_include if sg not in spacegroup_exclude
         ]
 
@@ -34,146 +39,247 @@
         # it's easier to save that here for reference too
         # convert the composition to a stoichiometry list
         # for example, Mg4Si4O12 composition will have stoich=[4,4,12]
         stoichiometry = [int(composition[element]) for element in composition]
         self.stoichiometry = stoichiometry
 
         # Find valid wyckoff combinatons for all spacegroups and stoichiometry
-        # I want the combinations and info to be stored as a dictionary of {spacegroup:combos/info} entries
+        # I want the combinations and info to be stored as a dictionary of
+        # {spacegroup:combos/info} entries.
+        # We split this into 2 dictionaries becuase we reference each a lot and
+        # it makes the code below easier.
         self.wy_groupinfo = {}
         self.wy_groupcombos = {}
-        # some spacegroups will be incompatible with the given composition -- keep a list of these
+        # some spacegroups will be incompatible with the given composition, so
+        # we keep a list of these
         self.spacegroups_invalid = []
-        #!!! NOTE: This code takes a long time to run in some cases, so I want to do it up front
-        # because this takes time, I print a warning and then use tqdm to track progress
-        message = "Generating Wyckoff combinations for every spacegroup: "
-        for spacegroup in tqdm(self.spacegroup_options, desc=message):
-            sg_combo_data = findValidWyckoffCombos(stoichiometry, spacegroup)
-            # If the spacegroup + stoich combination has no valid combinations, the generator will not work
-            if not sg_combo_data["ValidCombinations"]:
-                self.spacegroups_invalid.append(spacegroup)
-                # no need to save these results so skip to the next spacegroup
-                continue
-            # splitting up this dictionary becuase we reference each a lot
-            # and append the results to respective dictionaries
-            self.wy_groupinfo.update({spacegroup: sg_combo_data["WyckoffGroups"]})
-            self.wy_groupcombos.update({spacegroup: sg_combo_data["ValidCombinations"]})
-        # we need to take the spacegroups that are invalid and update the spacegroup_options with it.
-        # we still save the self.spacegroups_invalid for the user to see #!!! consider removing self.spacegroups_invalid though
-        self.spacegroup_options = [
-            sg for sg in self.spacegroup_options if sg not in self.spacegroups_invalid
-        ]
 
-        # make all generators for each spacegroup
-        # the generators are different for each spacegroup because each has a different asym unit
-        #!!! NOTE: options set in coords_gen_options will apply to all spacegroups
-        # I want the generators to be stored as a dictionary of {spacegroup:generator} entries
+        # Each spacegroup will have a "generator" that manages possible wyckoff
+        # combinations and the asymmetric unit associated with the spacegroup.
+        # These will be stored as a dictionary of  {spacegroup: generator}
         self.coords_generators = {}
-        for spacegroup in self.spacegroup_options:
-            # grab a copy of the user inputs for reference
-            # we will manipulate final_options for each spacegroup for use in the generator
-            final_options = coords_gen_options.copy()
-            # If the spacegroup was found to have no valid wyckoff combinations, there is no need for a generator
-            if spacegroup in self.spacegroups_invalid:
-                # skip to next spacegroup
-                continue
-            # establish the coords generator with asymmetric_unit_boundries
-            # this process is a little more complicated because we require that the asymmetric_unit_boundries be included in extra_conditions
-            asym_bounds = asymmetric_unit_boundries(spacegroup)
-            # if any extra_conditions were provided by the user, we want to combine them with the asym conditions
-            if "extra_conditions" in coords_gen_options.keys():
-                all_bounds = coords_gen_options["extra_conditions"] + asym_bounds
-                final_options.update({"extra_conditions": all_bounds})
-            # otherwise, the asym_bounds are the only boundry conditions for the coordinates
-            else:
-                final_options.update({"extra_conditions": asym_bounds})
-            # now that we have the coords_gen_options updated, we can make the generator
-            coords_generator = coords_generation_method(**final_options)
-            # add this generator to the results
-            self.coords_generators.update({spacegroup: coords_generator})
+        # Options set in coords_gen_options will apply to all spacegroups, so
+        # we store these up front. This because these generators are
+        # sometimes accessed lazily
+        self.coords_generation_method = coords_generation_method
+        self.coords_gen_options = coords_gen_options
+
+        # Generating all wyckoff combinations can take a long time to run in
+        # some cases (e.g. high atom counts), so we may want to do it up front.
+        # There are also scenarios where we don't want to generate the possible
+        # spacegroup combinations until the spacegroup is actually requested.
+        # This saves us time when we want just one structure and then are
+        # done with this system.
+        self.lazily_generate_combinations = lazily_generate_combinations
+        if not lazily_generate_combinations:
+            logging.info("Generating Wyckoff combinations for every spacegroup")
+            # use tqdm to track progress
+            for spacegroup in tqdm(self.spacegroup_options):
+                self._setup_spacegroup_wyckoff_generator(
+                    spacegroup,
+                    show_logging=False,
+                )
+            logging.info("Done.")
 
         # below, I'll need to repeatedly reference wy_data
-        #!!! I want to find a better way of loading wy_data - maybe load only data for spacegroup_options?
+        #!!! I want to find a better way of loading wy_data - maybe load
+        # only data for spacegroup_options?
         self.wy_data = loadWyckoffData().values
 
     def new_sites(self, spacegroup=None):
 
-        # This section of code is checking the spacegroup input
-        # if a spacegroup is not specified, grab a random one from our options
+        # parse spacegroup or grab a random one (with necessary lazy-setup)
+        spacegroup = self._init_spacegroup(spacegroup)
+        # exit if we have an invalid spacegroup
         if not spacegroup:
-            # randomly select a symmetry system
-            spacegroup = choice(self.spacegroup_options)
-        #!!! do I need to check this? This may slow the algorithm, but ensures a user doesn't break the function
-        # if a spacegroup is specified, we still need to make sure it's valid
-        else:
-            check = spacegroup not in self.spacegroups_invalid
-            # if it is invalid, print a message and quit the function
-            if not check:
-                # print('This spacegroup is invalid for the given composition') #!!! consider adding a warning
-                return False
+            return False
 
-        # we need to grab the generators, wyckoff combinations, wyckoff group information for selected spacegroup
+        # we need to grab the generators, wyckoff combinations, wyckoff group
+        # information for selected spacegroup
         coords_generator = self.coords_generators[spacegroup]
         wy_groupcombos = self.wy_groupcombos[spacegroup]
         wy_groupinfo = self.wy_groupinfo[spacegroup]
 
         # randomly grab a wy_group combination
-        # NOTE: this does not have equal probability of grabbing all wyckoff site combinations because some wy_groups have more wy_site posibilities than others
-        # choice(sg_combos['ValidCombinations']) doesn't work here, so we grab a random index instead
+        # NOTE: this does not have equal probability of grabbing all wyckoff
+        # site combinations because some wy_groups have more wy_site p
+        # osibilities than others.
+        # choice(sg_combos['ValidCombinations']) doesn't work here, so we grab
+        # a random index instead
         random_index = randint(0, len(wy_groupcombos))
         wy_group_combo = wy_groupcombos[random_index]
 
         # make an empty list to store all the fractional coordinates
         coords_list = []  # regular list.append is faster than numpy.append
         # as well as an empty list for the species
         species_list = []
 
-        # now we need to iterate through each element in stoich, see which wy_group(s) it was assigned to
+        # now we need to iterate through each element in stoich, see which
+        # wy_group(s) it was assigned to
         for i, wy_groups in enumerate(wy_group_combo):
             # wy_groups represents the combination of wy_group's for a single element
-            # len(stoich) == len(wy_group_combo) because indexes are matched up (i.e. stoich[1] was assigned wy_group_combo[1])
+            # len(stoich) == len(wy_group_combo) because indexes are matched
+            # up (i.e. stoich[1] was assigned wy_group_combo[1])
             # so we can use the index of wy_groups to grab the element
             element = self.composition.elements[i]
             # wy_groups can be a list of wy_group entries
             for wy_group in wy_groups:
                 # now we need to generate the coordinates for this wy_site
                 # for that, we need three things:
                 # (1) a random wy_site from the assigned wy_group
-                # (2) the base wy_site coords corresponding to that wy_site (i.e. (x,y,z) or (0,y,0))
-                # (3) random coords that exist inside the asymmetric unit, used to eval() the coords with
+                # (2) the base wy_site coords corresponding to that wy_site
+                #     (i.e. (x,y,z) or (0,y,0))
+                # (3) random coords that exist inside the asymmetric unit,
+                #     used to eval() the coords with
                 # (4) ensure that the result coordinates have not been used already
                 # wy_group label is a key to the wy_groupinfo dictionary
-                # the wy_sites output is a list of indexes (as numpy array) that correspond to indicies in the loadWyckoffData() output
+                # the wy_sites output is a list of indexes (as numpy array)
+                # that correspond to indicies in the loadWyckoffData() output
                 wy_sites = wy_groupinfo[wy_group]
                 check = False
                 while not check:
                     # randomly choose one of these wy_site indexes
-                    # I have this inside the while-loop because if a special wy_site (i.e. (0,0,0)) is picked when it's already in coords_used, we will get stuck in the while loop
+                    # I have this inside the while-loop because if a special
+                    # wy_site (i.e. (0,0,0)) is picked when it's already in
+                    # coords_used, we will get stuck in the while loop
                     wy_site_i = choice(wy_sites)
                     # use the choice to grab the wy_site
                     wy_site = self.wy_data[wy_site_i]
-                    # grab the first entry (as all others are symmetrically equivalent) for coord template
+                    # grab the first entry (as all others are symmetrically
+                    # equivalent) for coord template
                     wy_coords = wy_site[5]  # index 5 is 'Coordinates'
-                    # generate random x,y,z values that are inside the asymmetric unit
+                    # generate random x,y,z values that are inside the
+                    # asymmetric unit
                     x, y, z = coords_generator.new_vector()
                     # place these x,y,z values into the coords where necessary
-                    # not sure why I need to use None,dict(x=x,y=y,z=z) inside eval. Eval() can't use the locals for some reason.
+                    # not sure why I need to use None,dict(x=x,y=y,z=z)
+                    # inside eval. Eval() can't use the locals for some reason.
                     final_coords = eval(wy_coords, None, dict(x=x, y=y, z=z))
                     # see if the result is already a coordinate used
                     check = final_coords not in coords_list
                 # append the coords and species to our output lists
                 coords_list.append(final_coords)
                 species_list.append(element)
 
-        # maybe make these into pymatgen Site objects? I don't see any advantage to Site object,
-        # because we will later need PeriodicSite objects and there's no direct conversion method
+        # maybe make these into pymatgen Site objects? I don't see any
+        # advantage to Site object, because we will later need PeriodicSite
+        # objects and there's no direct conversion method
         return species_list, coords_list
 
+    def _init_spacegroup(self, spacegroup):
+        # This checks the spacegroup input from a user or grabs a random one.
+        # We isolate this into a separate class because of the complex logic
+        # required to handle lazy
+
+        # if a spacegroup is not specified, grab a random one from our options
+        if not spacegroup:
+            # If we generated the combinatons up front, we can just grab a spacegroup
+            # from all the valid options.
+            if not self.lazily_generate_combinations:
+                spacegroup = choice(self.spacegroup_options)
+
+            # Otherwise, we need to randomly select a symmetry system until we
+            # find a valid one
+            else:
+                spacegroup = -1  # gives non-existing spacegroup to start the loop
+
+                # check if the spacegroup is valid & analyzed before
+                while not spacegroup in self.coords_generators:
+
+                    # bug-note: this loop should not go on endlessly, because
+                    # spacegroup=1 should **always** be valid and it will be
+                    # selected eventually in extreme cases.
+
+                    # grab a new spacegroup
+                    spacegroup = choice(self.spacegroup_options)
+
+                    # generate the possible combinations.
+                    self._setup_spacegroup_wyckoff_generator(spacegroup)
+
+        # if the user provided a spacegroup, we still need to check if its been
+        # analyzed and is valid.
+        else:
+
+            # make sure wyckoff combos have been analyzed before
+            if (
+                self.lazily_generate_combinations
+                and spacegroup not in self.coords_generators
+                and spacegroup not in self.spacegroups_invalid
+            ):
+                # generate the possible combinations.
+                self._setup_spacegroup_wyckoff_generator(spacegroup)
+
+            # Make sure the spacegroup is valid for the given composition
+            if spacegroup in self.spacegroups_invalid:
+                logging.warning(
+                    f"Spacegroup {spacegroup} is invalid for {self.composition}"
+                )
+                return False
+
+        return spacegroup
+
+    def _setup_spacegroup_wyckoff_generator(
+        self, spacegroup: int, show_logging: bool = True
+    ):
+        if show_logging:
+            logging.info(
+                f"Generating possible wyckoff combinations for spacegroup {spacegroup}"
+            )
+        sg_combo_data = findValidWyckoffCombos(self.stoichiometry, spacegroup)
+        if show_logging:
+            logging.info("Done generating combinations.")
+        # If the spacegroup + stoich combination has no valid combinations,
+        # the generator will not work
+        if not sg_combo_data["ValidCombinations"]:
+            self.spacegroups_invalid.append(spacegroup)
+            # we also need to update all the spacegroup_options now that we have
+            # a new invalid one.
+            self.spacegroup_options = [
+                sg
+                for sg in self.spacegroup_options
+                if sg not in self.spacegroups_invalid
+            ]
+            # exit the function -- false indicates we have an invalid spacegroup
+            return False
+        # Otherwise we have valid combos that we want to store -- so that
+        # we don't need to calculate them again.
+        self.wy_groupinfo.update({spacegroup: sg_combo_data["WyckoffGroups"]})
+        self.wy_groupcombos.update({spacegroup: sg_combo_data["ValidCombinations"]})
+
+        # Next we need to setup the asymmetric unit boundry conditions.
+
+        # grab a copy of the user inputs for reference
+        # we will manipulate final_options for each spacegroup for use
+        # in the generator
+        final_options = self.coords_gen_options.copy()
+
+        # establish the coords generator with asymmetric_unit_boundries
+        # this process is a little more complicated because we require
+        # that the asymmetric_unit_boundries be included in extra_conditions
+        asym_bounds = asymmetric_unit_boundries(spacegroup)
+
+        # if any extra_conditions were provided by the user, we want to
+        # combine them with the asym conditions
+        if "extra_conditions" in self.coords_gen_options.keys():
+            all_bounds = self.coords_gen_options["extra_conditions"] + asym_bounds
+            final_options.update({"extra_conditions": all_bounds})
+        # otherwise, the asym_bounds are the only boundry conditions for
+        # the coordinates
+        else:
+            final_options.update({"extra_conditions": asym_bounds})
+
+        # now that we have the coords_gen_options updated, we can make the generator
+        coords_generator = self.coords_generation_method(**final_options)
+
+        # add store this generator
+        self.coords_generators.update({spacegroup: coords_generator})
+
+        # exit the function -- true indicates we have a valid spacegroup
+        return True
 
-##############################################################################
 
 # Grab the boundry conditions for the asymmetric unit of a spacegroup's unitcell
 def asymmetric_unit_boundries(spacegroup, asym_data=loadAsymmetricUnitData()):
 
     # spacegroup = spacegroup that we are interested in
     # asym_data = result of loadAsmmetricUnitData() - this is in the header for speed reasons
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/creators/structure/_todo/random_symmetry_walk.py` & `simmate-0.9.0/src/simmate/toolkit/creators/structure/_todo/random_symmetry_walk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 
-import pandas as pd
-from numpy.random import choice, shuffle
 import itertools
 
-from simmate.toolkit import Structure, Composition
+import pandas as pd
+from numpy.random import choice, shuffle
 
-from simmate.toolkit.symmetry.wyckoff import loadWyckoffData
-from simmate.toolkit.creators.vector import UniformlyDistributedVectors
-from simmate.toolkit.creators.sites.random_wyckoff import (
-    asymmetric_unit_boundries,
-)  #!!! this will move to simmate.toolkit.symmetry in the future
+from simmate.toolkit import Composition, Structure
 from simmate.toolkit.creators.lattice import RSLSmartVolume
+from simmate.toolkit.creators.sites.random_wyckoff import (  # !!! this will move to simmate.toolkit.symmetry in the future
+    asymmetric_unit_boundries,
+)
+from simmate.toolkit.creators.vector import UniformlyDistributedVectors
+from simmate.toolkit.symmetry.wyckoff import loadWyckoffData
 
 # from pymatdisc.core.estimate import distance_matrix # !!! TODO
 
 ##############################################################################
 
 
 class StructureCreator:
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/creators/structure/base.py` & `simmate-0.9.0/src/simmate/toolkit/transformations/from_ase/soft_mutation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,98 +1,103 @@
 # -*- coding: utf-8 -*-
 
-from abc import ABC, abstractmethod
+from simmate.toolkit.transformations.base import Transformation
 
-from dask.distributed import get_client
 
+class SoftMutation(Transformation):
 
-class StructureCreator(ABC):
-    def __init__(self):
-        """
-        This is where you store all settings for the creation and do the setup.
-        For example, you would store the target composition here and/or
-        specify the fixed volume to use. Many times, there are 'setup' steps
-        that require a lot of overhead which you don't want to redo for each
-        new creation. For example, you don't want to find all combinations
-        of allowed wyckoff sites for a specific composition each time you make
-        a new structure, so you would find all valid combinations here in the
-        __init__ so you don't have to repeatedly find combos below in create()
-        """
-        pass
-
-    @abstractmethod
-    def create_structure(self, spacegroup=None):
-        """
-        For all different structure creators, there should be a method of
-        .new_structure() that makes the new object. The main rule for this
-        function is that it must return a single pymatgen structure object.
-        How that structure object is created is up to each method!
-
-        Below is some example code for how Structures are typically made. How
-        the spacegroup/lattice/species/coords is determined is up to each
-        methodand not shown.
-
-        # import module (do this outside the class functions)
-        from simmate.toolkit import Structure
-
-        # run your method that makes the lattice/species/coords or uses the
-        # inputs from above.
-        ...
-
-        # for new_structure method that doesnt use symmetry or wyckoff sites
-        sg = 1 # this is never used but just for bookkeeping
-        structure = Structure(lattice = lattice,
-                              species = species,
-                              coords = coords)
-
-        # for new_structure methods that depend on symmetry and wyckoff sites
-        # If you give the sites in the asym unit, they will be replicated
-        # elsewhere in the unitcell using spacegroup symmetry operations.
-        structure = Structure.from_spacegroup(sg = spacegroup,
-                                              lattice = lattice,
-                                              species = species,
-                                              coords = coords)
-        """
-        raise NotImplementedError
-
-    def create_many_structures(self, n, spacegroup=None):
-        """
-        This is a convience function to create many structures in parallel.
-        In most cases, you don't want to redefine this function.
-        It is assumed that calling create_structure() repeatedly is the
-        fastest method to make new structures, so that is the function
-        parallelized. In some cases (such as the USPEX creator), there is a
-        lot of overhead with a single call to create_structure(), so it may
-        make more sense to have the main structure creation code in this
-        function. See the USPEXStructure Creator class for an example of this.
-
-        Make sure you have a Dask cluster setup as a global variable!
-        Here's how you should do that...
-            from dask.distributed import Client
-            client = Client(processes=False)
-        """
-        # USING DASK FUTURES TO PARALLELIZE
-
-        # grab the dask cluster
-        #!!! Maybe give the client as an optional input? And if none is
-        #!!! given or detected, start up one automatically...?
-        try:
-            client = get_client()
-        except ValueError:
-            print("Set up a Dask cluster before trying to run this!")
+    # construct a dynamical matrix based on bond hardness and mutate site coords along the softest mode
+    # https://uspex-team.org/static/file/USPEX-LargeComplexSystems-2010.pdf
+
+    # This appears to be a means to order a disordered structure, which I can use other pymatgen methods for
+    # from pymatgen.transformations.standard_transformations import OrderDisorderedStructureTransformation
+    # from pymatgen.transformations.advanced_transformations import EnumerateStructureTransformation
+    # After reading through the docs of these functions, it actually looks like "disordered" refers to structures with mixed occupancy sites (e.g. 50% Li / 50% Na)
+    # so... I don't think these functions will help
+    # the same goes for the reverse of these functions:
+    # from pymatgen.transformations.advanced_transformations import DisorderOrderedTransformation
+
+    # I have found that ASE has a version of this function written already
+    # https://wiki.fysik.dtu.dk/ase/tutorials/ga/ga_bulk.html
+    # https://gitlab.com/ase/ase/-/tree/master/ase/ga
+    # from ase.ga.bulk_mutations import SoftMutation
+
+    io_scale = "one_to_one"
+    ninput = 1
+    use_multiprocessing = False
+
+    def __init__(
+        self,
+        composition,
+        ratio_of_covalent_radii=0.1,
+        bounds=[0.5, 2.0],
+        use_tags=False,
+        used_modes_file=None,
+    ):  #!!! add all SoftMutation options or use **kwargs?
+
+        # we can assume the user has ASE installed because it is a dependency of PyMatgen
+        #!!! it looks like the ase.ga module is actively changing so version may introduce errors
+        from ase.ga.soft_mutation import SoftMutation
+        from ase.ga.utilities import closest_distances_generator
+
+        # the closest_distances_generator is exactly the same as an element-dependent distance matrix
+        # expect ASE puts this in dictionary form
+        # the function requires a list of element integers
+        element_ints = [element.number for element in composition]
+        # the default of the ratio of covalent radii (0.1) is based on the ASE tutorial of this function
+        element_distance_matrix = closest_distances_generator(
+            element_ints, ratio_of_covalent_radii
+        )
+
+        # now make the SoftMutation mutator
+        self.softmut = SoftMutation(
+            blmin=element_distance_matrix,
+            bounds=bounds,
+            use_tags=use_tags,
+            used_modes_file=used_modes_file,
+        )
+
+        # we also need to convert pymatgen Structures to ase Atoms below
+        #!!! is it faster and more memory efficient to import below?
+        from pymatgen.io.ase import AseAtomsAdaptor
+
+        self.adaptor = AseAtomsAdaptor
+
+    def apply_transformation(self, structure):
+
+        ### CHECK FOR BUGS
+
+        # This mutation is not possible for structures that have only one site
+        if structure.num_sites == 1:
+            # print('You cannot perform a soft mutation on structures that only have one site!! You can make this a supercell and try again though.')
             return False
-        # launch create_structure(spacegroup) iteratively and in parallel
-        # The pure=False indicates that we will have different answers, even for the same input
-        futures = client.map(self.create_structure, [spacegroup] * n, pure=False)
-        # wait for all of the calls to finish and grab the results
-        results = client.gather(futures)  #!!! faster for dask
-        # we now have a list of structures of size n and can return them
-        return results
-
-    def update_data(self):
-        """
-        TO-DO
-        This is a function to update settings. For example, I could use this
-        to update the self.lattice_creator method to a more accurate volume.
-        I can run machine learning code here before updating too.
-        """
-        pass
+
+        ### RUN
+
+        # first I need to convert the structure to an ASE atoms object
+        structure_ase = self.adaptor.get_atoms(structure)
+
+        # their code searches for a atoms.info['confid'] to check for previously used modes -- it's unfortunately dependent on the entire ga structure
+        # config stands for configuration, which I'm not actually using. So I set this to some random value which has no effect.
+        structure_ase.info.update(
+            {"confid": 0}
+        )  #!!! I don't understand what this index represents and need to contact the dev
+
+        # reset the used_modes to none
+        #!!! I could also fill this if I want to try different modes until I have a unique structure
+        #!!! the dictionary would be {0:[3,4,5...]} if I want to skip modes
+        self.softmut.used_modes = {}
+
+        #!!! Their code suggests the use of .get_new_individual() but I think .mutate() is what we'd like
+        # new_structure_ase, label = self.softmut.get_new_individual([structure_ase])
+        new_structure_ase = self.softmut.mutate(structure_ase)
+
+        # if the mutation failed, None will be returned
+        if new_structure_ase:
+            # now convert back to a pymatgen object
+            new_structure = self.adaptor.get_structure(new_structure_ase)
+        # this indicates the mutation failed
+        #!!! should I retry?
+        else:
+            new_structure = False
+
+        return new_structure
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/creators/structure/prototypes.py` & `simmate-0.9.0/src/simmate/toolkit/creators/structure/prototypes.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 
 import itertools
 
 from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
 
-from simmate.toolkit import Composition, Structure
 from simmate.database import connect
 from simmate.database.third_parties import AflowPrototype
+from simmate.toolkit import Composition, Structure
 
 
 class FromAflowPrototypes:
     """
     Generates structures of a target composition by using AFLOW prototypes as
     templates.
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/creators/structure/random_symmetry.py` & `simmate-0.9.0/src/simmate/toolkit/creators/structure/random_symmetry.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,55 @@
 # -*- coding: utf-8 -*-
 
-##############################################################################
+import logging
 
 from numpy.random import choice
 
-from simmate.toolkit import Structure
-
-# from pymatgen.analysis.structure_prediction.volume_predictor import DLSVolumePredictor #, RLSVolumePredictor
-
-from simmate.toolkit.creators.structure.base import StructureCreator
-from simmate.toolkit.creators.lattice import RSLSmartVolume  # RandomSymLattice
+from simmate.toolkit import Composition, Structure
+from simmate.toolkit.creators.lattice import RSLSmartVolume
 from simmate.toolkit.creators.sites.random_wyckoff import RandomWySites
+from simmate.toolkit.creators.structure.base import StructureCreator
 from simmate.toolkit.creators.utils import NestedFixes
-
 from simmate.toolkit.validators.structure import SiteDistanceMatrix
 
-##############################################################################
-
-#!!!!!!!!!!!!!!!!!!!!!!!!
-# MAJOR POTENTIAL BUG
-# because I use MultiplicityPrimitive in RandomWySites but make a convential cell below,
-# there may be a issue with the input composition vs. output composition number of sites.
-# For example, when making a Ca2N structure with spacegroup 166, I will be given
-# a structure of Ca6N3. I can then convert this to the primitive cell to get Ca2N, but
-# depending on the sym settings that I use, this might not work.
-# I don't currently have structure.get_primitive_structure() in this creator
-# because it will break the Generator workflow (which assumes unchanging cell between validations).
-#!!!!!!!!!!!!!!!!!!!!!!!!
-
 
 class RandomSymStructure(StructureCreator):
 
-    #!!! I assume that all lattice/site methods have three inputs (see init below), which will cause errors... TO-DO
+    # BUG: because I use MultiplicityPrimitive in RandomWySites but make a
+    # convential cell below, there may be a issue with the input composition
+    # vs. output composition number of sites. For example, when making a Ca2N
+    # structure with spacegroup 166, the conventional cell will give a
+    # structure of Ca6N3. I can then convert this to the primitive cell to get
+    # Ca2N, but depending on the sym settings that I use, this might not work.
+    # I don't currently have structure.get_primitive_structure() in this creator
+    # because it will break the Generator workflow (which assumes unchanging
+    # cell between validations).
 
     def __init__(
         self,
-        composition,  # must be a pymatgen Composition object
-        spacegroup_include=range(1, 231),
-        spacegroup_exclude=[],
+        composition: Composition,
+        spacegroup_include: list[int] = range(1, 231),
+        spacegroup_exclude: list[int] = [],
         lattice_generation_method=RSLSmartVolume,
-        lattice_gen_options={},
+        lattice_gen_options: dict = {},
         site_generation_method=RandomWySites,
-        site_gen_options={},
+        site_gen_options: dict = {},
         validator_method=SiteDistanceMatrix,
-        validator_options={},
+        validator_options: dict = {},
         fixindicator_method=NestedFixes,
-        fixindicator_options={
+        fixindicator_options: dict = {
             "fixes": ["new_lattice", "new_sites"],
             "cutoffs": [15, 100],
         },
-        remove_failed_spacegroups=False,
-        cleanup=True,
+        remove_failed_spacegroups: bool = False,
+        cleanup: bool = True,
     ):
 
-        # sg_include = list of spacegroups that we are interested in. Default is all 230 spacegroups
+        # sg_include = list of spacegroups that we are interested in. Default
+        # is all 230 spacegroups
         # sg_exclude = list of spacegroups that we should explicitly ignore
 
         # method settings
         self.remove_failed_spacegroups = remove_failed_spacegroups
         self.removed_spacegroups = []
         self.cleanup = cleanup
 
@@ -84,189 +76,234 @@
                 composition=composition,
                 spacegroup_include=spacegroup_include,
                 spacegroup_exclude=spacegroup_exclude,
             )
         )
         self.site_generator = site_generation_method(**site_gen_options)
 
+        # BUG: I assume that all lattice/site methods have three inputs
+        # which will cause errors when the new classes that don't accept these
+        # this input types.
+
         # establish the validation method and use the specified options
         # many methods include options for composition
         # we want to override that option with what the user indicated here
         validator_options.update(dict(composition=composition))
         self.validator = validator_method(**validator_options)
 
         # establish the FixIndicator method and use the specified options
         self.fixindicator = fixindicator_method(**fixindicator_options)
 
         # make a list of spacegroups that we are allowed to choose from
         self.spacegroup_options = [
             sg for sg in spacegroup_include if sg not in spacegroup_exclude
         ]
 
-        # While a given sg_inlcude and sg_exclude were given, some spacegroup may not be compatible
-        # with the lattice or site method use. For example, the spacegroup 230 is not possible
-        # with a composition of MgSiO3 (1:1:3). Selection of appropriate wy_sites can't be done.
-        # The user still may have 230 in the spacegroup_include. This function will ensure all spacegroups
-        # are compatible -- if not, self.spacegroup_options will be updated by remove the spacegroup.
-        # see which spacegroups are compatible with the lattice creation method and update
-        # see which spacegroups are compatible with the site creation method and
-        #!!! should I have a self.spacegroups_invalid list to keep track of what's been removed?
-        #!!! ERROR WILL BE THROWN IF I DON'T REQUIRE ALL SITE AND LATTICE CREATORS TO HAVE spacegroup_options LISTED!!!
+        # While a given sg_inlcude and sg_exclude were given, some spacegroup
+        # may not be compatible with the lattice or site method used. For example,
+        # the spacegroup 230 is not possible with a composition of MgSiO3 (1:1:3).
+        # Selection of appropriate wy_sites can't be done. The user still may
+        # have 230 in the spacegroup_include. This function will ensure all
+        # spacegroups are compatible -- if not, self.spacegroup_options will be
+        # updated by remove the spacegroup. Therefore, this step is to see
+        # which spacegroups are compatible with BOTH the lattice creation method
+        # and the site creation method.
         self.spacegroup_options = [
             sg
             for sg in self.spacegroup_options
             if sg in self.lattice_generator.spacegroup_options
             and sg in self.site_generator.spacegroup_options
         ]
+        # !!! should I have a self.spacegroups_invalid list to keep track of
+        # what's been removed?
+        #
+        # BUG: this requires all site and lattice creators to have a
+        # spacegroup_options property.
 
     def create_structure(self, spacegroup=None):
 
         # If a spacegroup is not specified, grab a random one from our options
-        # no check is done to see if the spacegroup specified is compatible with the vector_generator built
+        # no check is done to see if the spacegroup specified is compatible
+        # with the vector_generator built
         if not spacegroup:
             # randomly select a spacegroup
             spacegroup = choice(self.spacegroup_options)
+        logging.info(f"Creating structure with spacegroup {spacegroup}")
 
         # Use the lattice generator to make a starting lattice
         lattice = self.lattice_generator.new_lattice(spacegroup)
 
         # Use the site generator to make a starting series of sites
         sites = self.site_generator.new_sites(spacegroup)
-        # if the generator returns None - then the spacegroup is incompatible with the composition
+        # if the generator returns None - then the spacegroup is incompatible
+        # with the composition
         if not sites:
-            # print('The spacegroup is incompatible with the composition and site-generator-method')
-            # REPORT POTENTIAL ISSUE IF THIS POINT IS REACHED
+            # The spacegroup is incompatible with the composition and
+            # site-generator-method.
+            # We do not raise an error in case this method needs to be called
+            # on a guess/check basis.
             return False
         # otherwise, the generator was successful so we can unpack its output
         species, coords = sites
 
         # Set the valid_struct to false so we can start the loop below.
         is_valid = False
         # Keep track of the number of attempts we make to create a structure
         attempts = 0
 
         # we want to continue this loop until we get a valid structure
         while not is_valid:
 
             # add an attempt to the validator
-            #!!! Should this be at the bottom of the while loop? So the first attempt is 0?
             attempts += 1
 
-            # since we only have sites in the asym unit, we use symmetry operations to get the rest of the unitcell
-            #!!! NOTE that I'm not always limiting sites to the asym unit... if I used RandomSites instead of RandomSymSites or RandomWySites, this may give problems
+            # since we only have sites in the asym unit, we use symmetry
+            # operations to get the rest of the unitcell
             structure = Structure.from_spacegroup(spacegroup, lattice, species, coords)
+            # BUG: Note that I'm not always limiting sites to the asym unit...
+            # if I used RandomSites instead of RandomSymSites or RandomWySites,
+            # this may give problems
 
             # Check that the structure is valid
             is_valid = self.validator.check_structure(structure)
 
             # If the validator passes, we can exit the loop!
             # This will be done automatically when 'while not is_valid' is checked
 
-            # Otherwise, we need to try to fix the structure and check it again
+            # Otherwise, we need to try to fix the structure and check it again.
             if not is_valid:
 
                 # see the assigned 'fix' for the validator
                 fix = self.fixindicator.point_to_fix(attempts)
 
                 if not fix:
-                    # if the 'fix' is False, that means we maxed out the attempts on the validator
+                    # if the 'fix' is False, that means we maxed out the attempts
+                    # on the validator.
                     # this indicates a total failure and the function should end
                     structure = False  # set to false indicating a failure
                     break  # exits the while loop with structure = False
-                    # alternatively, I could return False here
-
-                # The defualt settings have strings returned, not objects.
-                # This could tell the function to try making a new structure from
-                # scratch or maybe changing up the lattice.
-                # if type(fix) == str:
-                if fix == "new_structure":
+                    # We do not return False yet because we want to
+                    # I could return False here because we want to check for
+                    # "remove_failed_spacegroups" below
+
+                # The defualt "point_to_fix" settings have strings returned
+                # and not objects. There are only a limited number of options
+                # for the string returned -- e.g. "new_structure indicates
+                # we making a new structure from scratch, while "new_lattice"
+                # says to try changing up the lattice but keep the sites.
+                elif fix == "new_structure":
                     # Use the lattice generator to make a starting lattice
                     lattice = self.lattice_generator.new_lattice(spacegroup)
 
                     # Use the site generator to make a starting series of sites
                     sites = self.site_generator.new_sites(spacegroup)
-                    # if the generator returns None - then the spacegroup is incompatible with the composition
+                    # if the generator returns None - then the spacegroup is
+                    # incompatible with the composition
                     if not sites:
-                        # print('The spacegroup is incompatible with the composition and site-generator-method')
-                        # REPORT POTENTIAL ISSUE IF THIS POINT IS REACHED
+                        logging.warning(
+                            f"Failed to create a structure using spacegroup {spacegroup}."
+                        )
                         return False
-                    # otherwise, the generator was successful so we can unpack its output
+                    # otherwise, the generator was successful so we can unpack
+                    # its output
                     species, coords = sites
+
                 elif fix == "new_lattice":
                     # Use the lattice generator to make a starting lattice
                     lattice = self.lattice_generator.new_lattice(spacegroup)
+
                 elif fix == "new_sites":
                     # Use the site generator to make a starting series of sites
                     sites = self.site_generator.new_sites(spacegroup)
-                    # if the generator returns None - then the spacegroup is incompatible with the composition
+                    # if the generator returns None - then the spacegroup is
+                    # incompatible with the composition
                     if not sites:
-                        # print('The spacegroup is incompatible with the composition and site-generator-method')
-                        # REPORT POTENTIAL ISSUE IF THIS POINT IS REACHED
+                        logging.warning(
+                            f"Failed to create a structure using spacegroup {spacegroup}."
+                        )
                         return False
-                    # otherwise, the generator was successful so we can unpack its output
+                    # otherwise, the generator was successful so we can unpack
+                    # its output
                     species, coords = sites
 
-                # # we need to know if the fix is a transformation or a creation type
-                # #!!! there should be a better way to do this. Such as a check on is-child-class..?
+                # !!! Rather than using "new_structure", "new_lattice", and "new_sites"
+                # like we do above, it would be more powerful to allow specific
+                # settings of different creators or transformations. An example
+                # of this would be using a `transformations.sites` class to
+                # relax sites to a reasonable position. This code below is
+                # a template for how this feature enhancement would look. I keep
+                # it strictly as notes for now.
+                #
                 # fix_type = str(type(fix))
                 # # if fix points to a generator, we want to use its .new_* method
                 # if 'creators.structure' in fix_type:
                 #     structure = fix.new_structure(spacegroup)
-                #     # we need to update the lattice, species, coords otherwise it will be rewritten above
+                #     # we need to update the lattice, species, coords
+                #     # otherwise it will be rewritten above
                 #     lattice = structure.lattice
                 #     species = structure.species
-                #     coords = structure.frac_coords.tolist() #!!! bug with numpy array vs python list
+                #     coords = structure.frac_coords.tolist()
                 # elif 'creators.lattice' in fix_type:
                 #     lattice = fix.new_lattice(spacegroup)
                 # elif 'creators.sites' in fix_type:
                 #     species, coords = fix.new_sites(spacegroup)
-
                 # # if fix points to a transform, we want to use its apply_to_* method
                 # elif 'transformations.structure' in fix_type:
                 #     structure = fix.apply_to_structure(structure)
-                #     # we need to update the lattice, species, coords otherwise it will be rewritten above
+                #     # we need to update the lattice, species, coords otherwise
+                #     # it will be rewritten above
                 #     lattice = structure.lattice
                 #     species = structure.species
-                #     coords = structure.frac_coords.tolist() #!!! bug with numpy array vs python list
+                #     coords = structure.frac_coords.tolist()
                 # elif 'transformations.lattice' in fix_type:
                 #     lattice = fix.apply_to_lattice(structure.lattice)
                 # elif 'transformations.sites' in fix_type:
-                #     species, coords = fix.apply_to_sites(structure.species, structure.coords)
-
-                # regardless of what the next step was, we are going to restart the while-loop
+                #     species, coords = fix.apply_to_sites(
+                #         structure.species,
+                #         structure.coords,
+                #     )
 
         # If the structure creation failed (structure = False), then see if the
         # failed spacegroup should be removed from future choices.
-        if not structure and self.remove_failed_spacegroups:
-            print(
-                "This generator failed to create a structure using spacegroup {}. This spacegroup will be removed from the list of randomly selected spacegroups moving forward.".format(
-                    spacegroup
-                )
+        if not structure:
+            logging.warning(
+                f"Failed to create a structure using spacegroup {spacegroup}."
             )
-            # add the removed spacegroup to our list for reference
-            self.removed_spacegroups.append(spacegroup)
-            # and remove the spacegroup from our list of options
-            self.creator.spacegroup_options.remove(spacegroup)
+            if self.remove_failed_spacegroups:
+                logging.info(
+                    f"Removed spacegroup {spacegroup} from options. "
+                    "This will not be selected moving forward."
+                )
+                # add the removed spacegroup to our list for reference
+                self.removed_spacegroups.append(spacegroup)
+                # and remove the spacegroup from our list of options
+                self.creator.spacegroup_options.remove(spacegroup)
+        else:
+            logging.info("Creation successful.")
 
         # Cleanup does 'fix-up' steps before returning the final structure.
         # This includes converting from the conventional cell to primitive as
         # well as sort the sites by electronegativity
         # Also make sure that structure != False
         if self.cleanup and structure:
             # convert the conventional unitcell to the primitive
             #!!! should I use a spacegroup analyzer instead?
             #!!! Should I LLL reduce?
             structure = structure.get_primitive_structure()
             # make sure the sites are sorted by electronegativity of their elements
             # this is important for some mutations
             structure.sort()  # this is faster than get_sorted_structure
 
-        #!!! In some cases, the stoichometry of the structure will be different from the input composition.
-        # This happens when the structure happens to have higher symmetry than the spacegroup it was made with.
-        # For example, I could make a structure of Mg4Si4O12, but the primitive cell has Mg2Si2O6 or MgSiO3.
-        # So we got back a structure with fewer atoms than what we requested! This could cause issues down the
-        # line, so we may want to check for this.
+        # BUG: In some cases, the stoichometry of the structure will be
+        # different from the input composition. This happens when the structure
+        # happens to have higher symmetry than the spacegroup it was made with.
+        # For example, I could make a structure of Mg4Si4O12, but the primitive
+        # cell has Mg2Si2O6 or MgSiO3. So we got back a structure with fewer
+        # atoms than what we requested! This could cause issues down the line,
+        # so we may want to check for this.
         # if structure.composition.num_atoms != composition.num_atoms:
         #     print('COMP ERROR')
-        #     structure = new_sample(spacegroup) # restart the whole function # might hit a recursion depth error
+        #     # restart the whole function
+        #     structure = new_sample(spacegroup)
+        #     # BUG: might hit a recursion depth error
 
         return structure
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/creators/structure/third_party/_to_do/airss.py` & `simmate-0.9.0/src/simmate/toolkit/creators/structure/third_party/_to_do/airss.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/creators/structure/third_party/_to_do/ase.py` & `simmate-0.9.0/src/simmate/toolkit/creators/structure/third_party/_to_do/ase.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,20 +10,19 @@
         self,
         composition,  # must be a pymatgen Composition object
         ratio_of_covalent_radii=0.5,
     ):
 
         # we can assume the user has ASE installed because it is a dependency of PyMatgen
         #!!! it looks like the ase.ga module is actively changing so version may introduce errors
-        from ase.ga.startgenerator import StartGenerator
-        from ase.ga.utilities import closest_distances_generator
-
         # the slab variable is there to specify dimensionality. The code really just uses the pbc setting
         #!!! I need to doublecheck this
         from ase import Atoms
+        from ase.ga.startgenerator import StartGenerator
+        from ase.ga.utilities import closest_distances_generator
 
         slab = Atoms(
             pbc=True
         )  #!!! I assume 3D structure for now. I could do things like pbc=[1,1,0] for 2D in the future though
 
         # the blocks input is just a list of building blocks and how many to include of each
         # for example, Ca2N would have [('Ca', 2), ('N', 1)].
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/creators/structure/third_party/_to_do/calypso.py` & `simmate-0.9.0/src/simmate/toolkit/creators/structure/third_party/_to_do/calypso.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/creators/structure/third_party/_to_do/gasp.py` & `simmate-0.9.0/src/simmate/toolkit/creators/structure/third_party/_to_do/gasp.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     def __init__(
         self,
         composition,  # must be a pymatgen Composition object
     ):
 
         #!!! this is inside the init because not all users will have this installed!
         try:
-            from gasp.general import CompositionSpace, IDGenerator
             from gasp.development import Constraints
+            from gasp.general import CompositionSpace, IDGenerator
             from gasp.organism_creators import RandomOrganismCreator
         except ModuleNotFoundError:
             #!!! I should raise an error in the future
             print("You must have GASP installed to use GASPStructure!!")
             return  # exit the function as the script will fail later on otherwise
 
         # generate the inputs required for GASP to make a new structure
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/creators/structure/third_party/_to_do/uspex.py` & `simmate-0.9.0/src/simmate/toolkit/creators/structure/third_party/_to_do/uspex.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/creators/structure/third_party/_to_do/xtalopt.py` & `simmate-0.9.0/src/simmate/toolkit/creators/structure/third_party/_to_do/xtalopt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from numpy.random import choice
 
 from simmate.toolkit import Structure
 
+
 #!!! NOT TESTED
 class XtalOptStructure:
 
     # This wrapper actually uses the submodule randSpg written by XtalOpt devs
     # see source: https://github.com/xtalopt/randSpg
     # see tutorials: https://github.com/zbwang/randSpg/commit/73d2f33fc69da531398bf395dbfff581f4dbacad
 
@@ -22,15 +23,15 @@
         #!!! should I add a check to see if each spacegroup option is compatible with the composition?
         self.spacegroup_options = [
             sg for sg in spacegroup_include if sg not in spacegroup_exclude
         ]
 
         #!!! this is inside the init because not all users will have this installed!
         try:
-            from pyrandspg import RandSpgInput, LatticeStruct, RandSpg
+            from pyrandspg import LatticeStruct, RandSpg, RandSpgInput
 
             # save for reference later
             self.RandSpgInput = RandSpgInput
             self.RandSpg = RandSpg
         except ModuleNotFoundError:
             #!!! I should raise an error in the future
             print(
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/creators/structure/third_party/pyxtal.py` & `simmate-0.9.0/src/simmate/toolkit/creators/structure/third_party/pyxtal.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/creators/utils.py` & `simmate-0.9.0/src/simmate/toolkit/creators/utils.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/creators/vector/normal_distribution.py` & `simmate-0.9.0/src/simmate/toolkit/creators/vector/normal_distribution.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/creators/vector/uniform_distribution.py` & `simmate-0.9.0/src/simmate/toolkit/creators/vector/uniform_distribution.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/diffusion/migration_hop.py` & `simmate-0.9.0/src/simmate/toolkit/diffusion/migration_hop.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,17 +53,18 @@
             {
                 "migration_hop_table": "MITMigrationHop",
                 "migration_hop_id": 1,
             }
         """
 
         # Imports are done locally to keep this class modular.
+        from django.utils.module_loading import import_string
+
         from simmate.database import connect
         from simmate.website.workflows import models as all_datatables
-        from django.utils.module_loading import import_string
 
         datatable_str = migration_hop["migration_hop_table"]
 
         if hasattr(all_datatables, datatable_str):
             datatable = getattr(all_datatables, datatable_str)
         else:
             datatable = import_string(datatable_str)
@@ -86,21 +87,21 @@
         supercell_start, supercell_end, supercell_base = super().get_sc_structures(
             vac_mode, min_atoms, max_atoms, min_length, tol
         )
 
         # The parent method doesn't work as itended... I don't want to fix it,
         # so I just warn users.
         if supercell_start.num_sites < min_atoms or supercell_end.num_sites > max_atoms:
-            logging.warn(
+            logging.warning(
                 f"Failed to meet min_atoms={min_atoms} and max_atoms={max_atoms} "
                 "requirements when making supercell. Resulted in"
                 f" {supercell_start.num_sites} atoms."
             )
         if min(supercell_start.lattice.lengths) < min_length:
-            logging.warn(
+            logging.warning(
                 "Failed to meet min_length={min_length} requirement when"
                 " making supercell. Resulted in lattice vectors lengths of "
                 f"{supercell_start.lattice.lengths}."
             )
 
         # BUG-CHECK: There's some rounding issue in the base code that I don't want
         # to mess with, so I just hack fix here.
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/diffusion/migration_images.py` & `simmate-0.9.0/src/simmate/toolkit/diffusion/migration_images.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 # -*- coding: utf-8 -*-
 
 import numpy
-
-from simmate.toolkit import Structure
-
+from pymatgen.analysis.diffusion.neb.pathfinder import DistinctPathFinder, IDPPSolver
 from pymatgen.analysis.diffusion.neb.pathfinder import (
-    DistinctPathFinder,
     MigrationHop as PymatgenMigrationHop,
-    IDPPSolver,
 )
 
-from typing import List
+from simmate.toolkit import Structure
 
 
 class MigrationImages(list):
     """
     This class is just a list of structures for a diffusion pathway. It has
     utility methods to help create these structures but otherwise behaves
     exactly like a python list.
@@ -26,15 +22,15 @@
     a set of supercell images.
 
     All MigrationHop's can be converted to MigrationImages (using the
     `from_migration_hop` method); but not all MigrationImages can be converted
     to MigrationHops.
     """
 
-    def __init__(self, structures: List[Structure]):
+    def __init__(self, structures: list[Structure]):
         # This init function does nothing except apply typing -- specifically,
         # it says that it expects a list of structures.
         super().__init__(structures)
 
     def get_sum_structure(self, tolerance: float = 1e-3):
         """
         Takes all structures and combines them into one. Atoms that are within
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/structure_prediction/evolution/README.md` & `simmate-0.9.0/src/simmate/toolkit/structure_prediction/evolution/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/structure_prediction/evolution/stop_conditions.py` & `simmate-0.9.0/src/simmate/toolkit/structure_prediction/evolution/stop_conditions.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/structure_prediction/evolution/triggered_actions.py` & `simmate-0.9.0/src/simmate/toolkit/structure_prediction/evolution/triggered_actions.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """
 This module is experimental and not used at the moment.
 """
 
-from inspect import signature
 import logging
+from inspect import signature
 
 
 class TriggeredAction:
     def __init__(
         self,
     ):
         # add any unchanging variables or settings here
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/structure_prediction/known.py` & `simmate-0.9.0/src/simmate/toolkit/structure_prediction/known.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # -*- coding: utf-8 -*-
 
-from typing import List
-
-from simmate.toolkit import Composition, Structure
 from simmate.database import connect
 from simmate.database.third_parties import (
     AflowStructure,
     CodStructure,
     JarvisStructure,
     MatprojStructure,
     OqmdStructure,
 )
+from simmate.toolkit import Composition, Structure
 
 
 def get_known_structures(
     composition: Composition,
     strict_nsites: bool = False,
-) -> List[Structure]:
+) -> list[Structure]:
     """
     Goes through all database tables in the `simmate.database.third_parties`
     module and grabs all structures with a matching composition.
 
     Each database table must be populated -- otherwise this function will
     return an empty list.
     """
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/structure_prediction/substitution.py` & `simmate-0.9.0/src/simmate/toolkit/structure_prediction/substitution.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # -*- coding: utf-8 -*-
 
 import itertools
-from typing import List
 import logging
+import warnings
 
-from pymatgen.core import Species
 from pymatgen.analysis.structure_prediction.substitutor import Substitutor
+from pymatgen.core import Species
 
 from simmate.toolkit import Composition, Structure
+
 from .known import get_known_structures
 
 
 def get_structures_from_substitution_of_known(
     composition: Composition,
     **kwargs,  # passed to get_known_structures
-) -> List[Structure]:
+) -> list[Structure]:
     """
     Predicts the most likely element substitutions for a composition, and then
     based off the predictions, it will go through all database tables in the
     `simmate.database.third_parties` module generate substituted structures.
 
     Each database table must be populated -- otherwise this function will
     return an empty list.
@@ -41,53 +42,63 @@
     # init the substitution engine and grab the list of likely substituitions
     substitutor = Substitutor()
 
     # ----------
     # BUG: This code should be a single line:
     #   expected_substituitions = substitutor.pred_from_comp(oxi_composition)
     # Howevever, pymatgen's function fails when even a single element is not
-    # allowed with their dataset (e.g. any carbides will fail). To get around
+    # allowed with their dataset (e.g. any carbide will fail). To get around
     # this, I use pred_from_list instead of pred_from_comp, and I keep trying
     # until I get one that works. The while loop here is try every combination
     # of elements (starting with all of them and then try smaller combos) and
-    # exits as soon as I find one that works.
+    # exits as soon as I find one that works. Pymatgen also randomly logs
+    # within this function call, so we disable the logger while running this.
+    logger = logging.getLogger()
+    logger.disabled = True
     nelements = len(oxi_composition.elements)
     has_subs = False
     while (not has_subs) and (nelements > 0):
         for elements_to_sub in itertools.combinations(
             oxi_composition.elements, nelements
         ):
             try:
                 expected_substituitions = substitutor.pred_from_list(elements_to_sub)
                 break  # exit immediately once successful
             except:
-                expected_substituitions = None
+                expected_substituitions = []
         if expected_substituitions:
             has_subs = True
         else:
             # try the cycle again but with one less element in the combinations
             nelements -= 1
-
-    if not expected_substituitions:
-        raise Exception("Failed to find viable substituitions for this composition")
+    logger.disabled = False
 
     # Confirm charge balance for most-likely structures
     # This loop is copy/pasted from...
     # https://github.com/materialsproject/pymatgen/blob/e0c1ee845e7131213055c5b4fc6df2cb12fcc667/pymatgen/analysis/structure_prediction/substitutor.py#L238
     output = []
     for p in expected_substituitions:
         subs = p["substitutions"]
         charge = 0
         for i_el in oxi_composition.elements:
+            # BUG: not caught in pymatgen -- ex: Composition("C4")
+            if i_el not in subs.keys():
+                continue
             f_el = subs[i_el]
             charge += f_el.oxi_state * oxi_composition[i_el]
         if charge == 0:
             output.append(p)
     expected_substituitions = output
 
+    if not expected_substituitions:
+        # logging.warning(f"Failed to find viable substituitions for {composition}")
+        return []
+
+    # logging.info(f"{len(expected_substituitions)} subsitutions charge balance")
+
     # ----------
 
     # Keep a list of all structures that we create
     structures_final = []
 
     # now iterate through the expected substitutions, grab the known structures
     # from databases, and then perform the substitution to generate new structures
@@ -102,18 +113,22 @@
         # this is the same as above with keys/values flipped
         substituition_cleaned_2 = {
             str(element_orig): str(element_new)
             for element_new, element_orig in substituition["substitutions"].items()
         }
 
         # Generate the composition that we will use for source structures
-        composition_source = oxi_composition.replace(substituition_cleaned.copy())
+        # Pymatgen prints a warning that we are aware of and okay with
+        with warnings.catch_warnings(record=True):
+            composition_source = oxi_composition.replace(substituition_cleaned.copy())
         # BUG: this method is destructive to the input dictionary so we must
         # pass a copy instead
-        logging.info([oxi_composition, composition_source, substituition_cleaned])
+
+        # log the substituition for debugging
+        logging.debug([oxi_composition, composition_source, substituition_cleaned])
 
         # Now grab all known structures with this composition
         source_structures = get_known_structures(composition_source, **kwargs)
 
         # skip to the next substitution type if no structures were found
         if not source_structures:
             continue
@@ -153,12 +168,16 @@
         #     # note, structure is a TransformedStructure obj to start
         #     structure_final = structure.final_structure
         #     structure_final.remove_oxidation_states()
         #     structures_final.append(structure_final)
 
         for structure in source_structures:
             new_structure = structure.copy()
+
             new_structure.replace_species(substituition_cleaned_2)
+
             # TODO: scale structures to reasonable volume..?
             structures_final.append(new_structure)
 
+    # logging.info(f"{len(structures_final)} final subsitutions using known structures")
+
     return structures_final
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/symmetry/asymdata.csv` & `simmate-0.9.0/src/simmate/toolkit/symmetry/asymdata.csv`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/symmetry/webscraper/aflow.py` & `simmate-0.9.0/src/simmate/toolkit/symmetry/webscraper/aflow.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
-from selenium import webdriver
 import pandas as pd
+from selenium import webdriver
 from tqdm import tqdm
 
 # launch the webbrowser
 driver = webdriver.Chrome(
     executable_path="/snap/bin/chromium.chromedriver"
 )  # /snap/bin/chromium gives errors
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/symmetry/webscraper/bilbao_wyckoff.py` & `simmate-0.9.0/src/simmate/toolkit/symmetry/webscraper/bilbao_wyckoff.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 misleading because we know that Ca2N has the spacegroup 166
 
 """
 
 ##############################################################################
 
 
-from selenium import webdriver
 import pandas as pd
+from selenium import webdriver
 from tqdm import tqdm
 
 # launch the webbrowser
 driver = webdriver.Chrome(
     executable_path="/snap/bin/chromium.chromedriver"
 )  # /snap/bin/chromium gives errors
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/symmetry/webscraper/itc_datascrape.py` & `simmate-0.9.0/src/simmate/toolkit/symmetry/webscraper/itc_datascrape.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 on each page. The headers should line up with the tables. For example in
 spacegroup 166, I can see:
     if "HEXAGONAL AXES" in header.text
 
 """
 
 
-from selenium import webdriver
 import pandas as pd
+from selenium import webdriver
 from tqdm import tqdm
 
 # launch the webbrowser
 driver = webdriver.Chrome(
     executable_path="/snap/bin/chromium.chromedriver"
 )  # /snap/bin/chromium gives errors
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/symmetry/wyckoff.py` & `simmate-0.9.0/src/simmate/toolkit/symmetry/wyckoff.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 
+import itertools
 from pathlib import Path
+
 import pandas as pd
-import itertools
 
 
 def loadWyckoffData():
 
     """
     This function loads the csv file containing all wyckoff site data into
     a pandas dataframe. One column that we need is not directly stored in
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/symmetry/wyckoffdata.csv` & `simmate-0.9.0/src/simmate/toolkit/symmetry/wyckoffdata.csv`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/transformations/atomic_permutation.py` & `simmate-0.9.0/src/simmate/toolkit/transformations/atomic_permutation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # -*- coding: utf-8 -*-
 
-from numpy.random import randint, choice
-
+from numpy.random import choice, randint
 from pymatgen.analysis.structure_matcher import StructureMatcher
 
 from simmate.toolkit.transformations.base import Transformation
 
 
 class AtomicPermutation(Transformation):
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/transformations/coordinate_perturation_ordered.py` & `simmate-0.9.0/src/simmate/toolkit/transformations/coordinate_perturation_ordered.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/transformations/coordinate_perturbation.py` & `simmate-0.9.0/src/simmate/toolkit/transformations/coordinate_perturbation.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/transformations/from_ase/atomic_permutation.py` & `simmate-0.9.0/src/simmate/toolkit/transformations/from_ase/atomic_permutation.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/transformations/from_ase/coordinate_perturbation.py` & `simmate-0.9.0/src/simmate/toolkit/transformations/from_ase/coordinate_perturbation.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/transformations/from_ase/heredity_mutation.py` & `simmate-0.9.0/src/simmate/toolkit/transformations/from_ase/heredity_mutation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import numpy
 
 from simmate.toolkit.transformations.base import Transformation
 
-
 #!!! I need to figure out how to implement more than two structures
 
 
 class Heredity(Transformation):
 
     # known as CutAndSplicePairing in ase.ga
     # https://gitlab.com/ase/ase/-/blob/master/ase/ga/cutandsplicepairing.py
@@ -24,19 +23,18 @@
         self,
         composition,
         ratio_of_covalent_radii=0.1,
     ):
 
         # we can assume the user has ASE installed because it is a dependency of PyMatgen
         #!!! it looks like the ase.ga module is actively changing so version may introduce errors
-        from ase.ga.utilities import closest_distances_generator
-
         # the slab variable is there to specify dimensionality. The code really just uses the pbc setting
         #!!! I need to doublecheck this
         from ase import Atoms
+        from ase.ga.utilities import closest_distances_generator
 
         self.slab = Atoms(
             pbc=True
         )  #!!! I assume 3D structure for now. I could do things like pbc=[1,1,0] for 2D in the future though
 
         # the closest_distances_generator is exactly the same as an element-dependent distance matrix
         # expect ASE puts this in dictionary form
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/transformations/from_ase/lattice_strain.py` & `simmate-0.9.0/src/simmate/toolkit/transformations/from_ase/lattice_strain.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/transformations/from_ase/mirror_mutation.py` & `simmate-0.9.0/src/simmate/toolkit/transformations/from_ase/mirror_mutation.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/transformations/from_ase/rotational_mutation.py` & `simmate-0.9.0/src/simmate/toolkit/transformations/from_ase/rotational_mutation.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/transformations/lattice_strain.py` & `simmate-0.9.0/src/simmate/toolkit/transformations/lattice_strain.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pymatgen.analysis.elasticity.strain import Strain, convert_strain_to_deformation
 
-from simmate.toolkit.transformations.base import Transformation
 from simmate.toolkit.creators.vector import UniformlyDistributedVectors
+from simmate.toolkit.transformations.base import Transformation
 
 
 class LatticeStrain(Transformation):
 
     #!!! should I mutate atomic sites too? USPEX is unclear if they do this in addition to lattice strain
     #!!! if I decide to do this, look at CoordinateMutation class below
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/validators/base.py` & `simmate-0.9.0/src/simmate/toolkit/validators/base.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from abc import ABC, abstractmethod
 
-from dask.diagnostics import ProgressBar
 from dask import bag
+from dask.diagnostics import ProgressBar
 
 
 class Validator(ABC):
     @abstractmethod
     def check_structure(self, structure):
         # User needs to define this function where one structure is input.
         # The output should be a True or False value that indicates whether
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/validators/fingerprint/README.md` & `simmate-0.9.0/src/simmate/toolkit/validators/fingerprint/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/toolkit/validators/fingerprint/_to_do/ase.py` & `simmate-0.9.0/src/simmate/toolkit/validators/fingerprint/_to_do/ase.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
-
 from matminer.featurizers.site import CrystalNNFingerprint as cnnf
 
 #!!! is it faster to import these all at once?
-from matminer.featurizers.structure import SiteStatsFingerprint as ssf
-from matminer.featurizers.structure import RadialDistributionFunction as rdf
 from matminer.featurizers.structure import PartialRadialDistributionFunction as prdf
+from matminer.featurizers.structure import RadialDistributionFunction as rdf
+from matminer.featurizers.structure import SiteStatsFingerprint as ssf
 from matminer.featurizers.structure.sites import PartialsSiteStatsFingerprint
-
 from scipy.spatial.distance import cosine
 
 
 class ASEFingerprint:
 
     # ASE cites this as a rewrite of the USPEX fingerprint
     # https://gitlab.com/ase/ase/-/blob/master/ase/ga/ofp_comparator.py
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/validators/fingerprint/_to_do/crystalnn.py` & `simmate-0.9.0/src/simmate/toolkit/validators/fingerprint/_to_do/crystalnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
-
 from matminer.featurizers.site import CrystalNNFingerprint as cnnf
 
 #!!! is it faster to import these all at once?
-from matminer.featurizers.structure import SiteStatsFingerprint as ssf
-from matminer.featurizers.structure import RadialDistributionFunction as rdf
 from matminer.featurizers.structure import PartialRadialDistributionFunction as prdf
+from matminer.featurizers.structure import RadialDistributionFunction as rdf
+from matminer.featurizers.structure import SiteStatsFingerprint as ssf
 
 
 class CrystalNNFingerprint:
 
     # requires matminer code
     # see https://materialsproject.org/docs/structuresimilarity
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/validators/fingerprint/_to_do/prdf.py` & `simmate-0.9.0/src/simmate/toolkit/validators/fingerprint/_to_do/prdf.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
-
 from matminer.featurizers.site import CrystalNNFingerprint as cnnf
 
 #!!! is it faster to import these all at once?
-from matminer.featurizers.structure import SiteStatsFingerprint as ssf
-from matminer.featurizers.structure import RadialDistributionFunction as rdf
 from matminer.featurizers.structure import PartialRadialDistributionFunction as prdf
+from matminer.featurizers.structure import RadialDistributionFunction as rdf
+from matminer.featurizers.structure import SiteStatsFingerprint as ssf
+
 
 #!!! CHANGE TO COS DISTANCE
 class PartialRDFFingerprint:
 
     # requires matminer code
     # see https://materialsproject.org/docs/structuresimilarity
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/validators/fingerprint/_to_do/rdf.py` & `simmate-0.9.0/src/simmate/toolkit/validators/fingerprint/_to_do/rdf.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
-
 from matminer.featurizers.site import CrystalNNFingerprint as cnnf
 
 #!!! is it faster to import these all at once?
-from matminer.featurizers.structure import SiteStatsFingerprint as ssf
-from matminer.featurizers.structure import RadialDistributionFunction as rdf
 from matminer.featurizers.structure import PartialRadialDistributionFunction as prdf
+from matminer.featurizers.structure import RadialDistributionFunction as rdf
+from matminer.featurizers.structure import SiteStatsFingerprint as ssf
+
 
 #!!! CHANGE TO COS DISTANCE
 class RDFFingerprint:
 
     # requires matminer code
     # see https://materialsproject.org/docs/structuresimilarity
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/validators/fingerprint/pcrystalnn.py` & `simmate-0.9.0/src/simmate/toolkit/validators/fingerprint/pcrystalnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # -*- coding: utf-8 -*-
 
-import numpy
-from tqdm import tqdm
 import logging
 
-from django.utils import timezone
-
 # BUG: This prints a tqdm error so we silence it here.
 import warnings
 
+import numpy
+from django.utils import timezone
+from tqdm import tqdm
+
 with warnings.catch_warnings(record=True):
     from matminer.featurizers.site import CrystalNNFingerprint
 
 # BUG: waiting on this pSS to be added to matminer. See the following PR:
 #   https://github.com/hackingmaterials/matminer/pull/809
-from matminer.featurizers.structure.sites import (
+from matminer.featurizers.structure.sites import (  # PartialsSiteStatsFingerprint
     SiteStatsFingerprint,
-)  # PartialsSiteStatsFingerprint
+)
 
-logging.warn(
+logging.warning(
     "PartialsSiteStatsFingerprint current acts as a SiteStatsFingerprint. "
     "We are waiting on a new MatMiner release to fix this issue."
 )
 
 
 class PartialCrystalNNFingerprint:
     def __init__(
```

### Comparing `simmate-0.8.0/src/simmate/toolkit/validators/structure.py` & `simmate-0.9.0/src/simmate/toolkit/validators/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 
 ##############################################################################
 
-import numpy
 import itertools
 
+import numpy
+
 from simmate.toolkit.validators.base import Validator
 
 ##############################################################################
 
 
 class SiteDistance(Validator):
     def __init__(self, distance_cutoff):
```

### Comparing `simmate-0.8.0/src/simmate/utilities/async_wrapper.py` & `simmate-0.9.0/src/simmate/utilities/async_wrapper.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/utilities/files.py` & `simmate-0.9.0/src/simmate/utilities/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
 
-from pathlib import Path
-from tempfile import mkdtemp
 import shutil
 import time
-from typing import List, Union
+from pathlib import Path
+from tempfile import mkdtemp
 
 
-def get_directory(directory: Union[str, Path] = None) -> Path:
+def get_directory(directory: Path | str = None) -> Path:
     """
     Initializes a directory.
 
     There are many cases where the user can choose their working directory
     for a calculation, and they may want to provide their directory in various
     formats. This includes... None, a string, or a TemporaryDirectory instance.
     Based on the input, this function does the following:
@@ -251,15 +250,15 @@
         ):
             foldernames.append(foldername_full)
 
     # now go through this list and archive the folders that met the criteria
     [make_archive(f) for f in foldernames]
 
 
-def empty_directory(directory: Path, files_to_keep: List[Path] = []):
+def empty_directory(directory: Path, files_to_keep: list[Path] = []):
     """
     Deletes all files and folders within a directory, except for those provided
     to the files_to_keep parameter.
 
     #### Parameters
 
     - `directory`:
```

### Comparing `simmate-0.8.0/src/simmate/utilities/other.py` & `simmate-0.9.0/src/simmate/utilities/other.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 
+import logging
 import os
 import sys
-import requests
 from pathlib import Path
-import logging
+
+import requests
 
 import simmate
 
 
 def get_conda_env() -> str:
     """
     Grab the name of the activate conda environment and returns it as a string.
@@ -81,15 +82,15 @@
     """
     Checks if there's a newer version by looking at the latest release on Github
     and comparing it to the currently installed version
     """
     latest_version = get_latest_version()
 
     if current_version != latest_version:
-        logging.warn(
+        logging.warning(
             "There is a new version of Simmate available. "
             f"You are currently using v{current_version} while v{latest_version} "
             "is the latest."
         )
 
 
 def get_chemical_subsystems(chemical_system: str):
```

### Comparing `simmate-0.8.0/src/simmate/utilities/test/test_files.py` & `simmate-0.9.0/src/simmate/utilities/test/test_files.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 # -*- coding: utf-8 -*-
 
 import shutil
 
 from simmate.conftest import copy_test_files
-from simmate.utilities.files import (
-    get_directory,
-    # make_archive,
-    make_error_archive,
-    archive_old_runs,
-    empty_directory,
-)
+from simmate.utilities.files import archive_old_runs  # make_archive,
+from simmate.utilities.files import empty_directory, get_directory, make_error_archive
 
 
 def test_get_directory(tmp_path):
 
     # create and delete a new directory
     new_directory = get_directory()
     assert "simmate-task-" in new_directory.name
```

### Comparing `simmate-0.8.0/src/simmate/visualization/README.md` & `simmate-0.9.0/src/simmate/visualization/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/visualization/structure/blender/README.md` & `simmate-0.9.0/src/simmate/visualization/structure/blender/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/visualization/structure/blender/base.py` & `simmate-0.9.0/src/simmate/visualization/structure/blender/base.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
-import json
 import itertools
+import json
 import subprocess
 from pathlib import Path
 
 import numpy
 
 from simmate.visualization.structure.blender.configuration import get_blender_command
```

### Comparing `simmate-0.8.0/src/simmate/visualization/structure/blender/configuration.py` & `simmate-0.9.0/src/simmate/visualization/structure/blender/configuration.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/visualization/structure/blender/scripts/make_structure.py` & `simmate-0.9.0/src/simmate/visualization/structure/blender/scripts/make_structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
 
+import argparse
 import json
 import sys
-import argparse
-
-import numpy
 
-import bpy
 import bmesh
+import bpy
+import numpy
 
 # These are the RGB values that JMol uses to color atoms
 JMOL_COLORING = {
     "H": [255, 255, 255],
     "He": [217, 255, 255],
     "Li": [204, 128, 255],
     "Be": [194, 255, 0],
```

### Comparing `simmate-0.8.0/src/simmate/visualization/structure/blender/test/test_blender.py` & `simmate-0.9.0/src/simmate/visualization/structure/blender/test/test_blender.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 
 import platform
 
 import pytest
 
 from simmate.visualization.structure.blender.configuration import (
-    get_blender_command,
     BlenderNotInstalledError,
+    get_blender_command,
 )
 
 # Requires blender install which is not possible in CI yet.
 #
 # from simmate.visualization.structure.blender.base import (
 #     make_blender_structure,
 #     serialize_structure_sites,
```

### Comparing `simmate-0.8.0/src/simmate/website/README.md` & `simmate-0.9.0/src/simmate/website/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/core/test/test_core_views.py` & `simmate-0.9.0/src/simmate/website/core/test/test_core_views.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/core/urls.py` & `simmate-0.9.0/src/simmate/website/core/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from django.contrib import admin
 from django.urls import include, path
 
 from simmate.website.core import views
 
-
 urlpatterns = [
     #
     # This is the path to the homepage (just simmate.org)
     path(route="", view=views.home, name="home"),
     #
     # This is the built-in admin site that django provides
     path(route="admin/", view=admin.site.urls, name="admin"),
```

### Comparing `simmate-0.8.0/src/simmate/website/core/views.py` & `simmate-0.9.0/src/simmate/website/core/views.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 
-from django.shortcuts import render
-from django.db.models import F
 from django.contrib.auth.decorators import login_required
+from django.db.models import F
+from django.shortcuts import render
 
-from simmate.website.third_parties.forms import ChemicalSystemForm
 from simmate.database.third_parties import (
     AflowStructure,
     CodStructure,
     JarvisStructure,
     MatprojStructure,
     OqmdStructure,
 )
+from simmate.website.third_parties.forms import ChemicalSystemForm
 
 
 @login_required
 def profile(request):
     # !!! For future reference, you can grab user-associated data via...
     # data = request.user.relateddata.all()
```

### Comparing `simmate-0.8.0/src/simmate/website/core_components/base_api_view.py` & `simmate-0.9.0/src/simmate/website/core_components/base_api_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # -*- coding: utf-8 -*-
 
 from django.http import HttpRequest
 
-from rest_framework.viewsets import GenericViewSet
-
 # from rest_framework.generics import GenericAPIView
 from rest_framework.response import Response
 from rest_framework.serializers import ModelSerializer
+from rest_framework.viewsets import GenericViewSet
 
-from simmate.website.core_components.filters import DatabaseTableFilter
 from simmate.database.base_data_types import DatabaseTable
+from simmate.website.core_components.filters import DatabaseTableFilter
 
 
 class SimmateAPIViewSet(GenericViewSet):
     """
     Example use:
 
     ``` python
```

### Comparing `simmate-0.8.0/src/simmate/website/core_components/filters/band_structure.py` & `simmate-0.9.0/src/simmate/website/core_components/filters/band_structure.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from django_filters import rest_framework as filters
 
+from simmate.database.base_data_types import BandStructure as BandStructureTable
+from simmate.database.base_data_types import BandStructureCalc as BandStructureCalcTable
 from simmate.website.core_components.filters import Calculation, Structure
-from simmate.database.base_data_types import (
-    BandStructure as BandStructureTable,
-    BandStructureCalc as BandStructureCalcTable,
-)
 
 
 class BandStructure(filters.FilterSet):
     class Meta:
         model = BandStructureTable
         fields = dict(
             nbands=["range"],
```

### Comparing `simmate-0.8.0/src/simmate/website/core_components/filters/base.py` & `simmate-0.9.0/src/simmate/website/core_components/filters/base.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/core_components/filters/density_of_states.py` & `simmate-0.9.0/src/simmate/website/core_components/filters/density_of_states.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from django_filters import rest_framework as filters
 
-from simmate.website.core_components.filters import Calculation, Structure
+from simmate.database.base_data_types import DensityofStates as DensityofStatesTable
 from simmate.database.base_data_types import (
-    DensityofStates as DensityofStatesTable,
     DensityofStatesCalc as DensityofStatesCalcTable,
 )
+from simmate.website.core_components.filters import Calculation, Structure
 
 
 class DensityofStates(filters.FilterSet):
     class Meta:
         model = DensityofStatesTable
         fields = dict(
             band_gap=["range"],
```

### Comparing `simmate-0.8.0/src/simmate/website/core_components/filters/dynamics.py` & `simmate-0.9.0/src/simmate/website/core_components/filters/dynamics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 
+from simmate.database.base_data_types.dynamics import (
+    DynamicsIonicStep as DynamicsIonicStepTable,
+)
+from simmate.database.base_data_types.dynamics import DynamicsRun as DynamicsRunTable
 from simmate.website.core_components.filters import (
-    Structure,
+    Calculation,
     Forces,
+    Structure,
     Thermodynamics,
-    Calculation,
-)
-from simmate.database.base_data_types.dynamics import (
-    DynamicsRun as DynamicsRunTable,
-    DynamicsIonicStep as DynamicsIonicStepTable,
 )
 
 
 class DynamicsRun(Structure, Calculation):
     class Meta:
         model = DynamicsRunTable
         fields = dict(
```

### Comparing `simmate-0.8.0/src/simmate/website/core_components/filters/nudged_elastic_band.py` & `simmate-0.9.0/src/simmate/website/core_components/filters/nudged_elastic_band.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # -*- coding: utf-8 -*-
 
 from django_filters import rest_framework as filters
 
-from simmate.website.core_components.filters import Structure
 from simmate.database.base_data_types.nudged_elastic_band import (
     DiffusionAnalysis as DiffusionAnalysisTable,
+)
+from simmate.database.base_data_types.nudged_elastic_band import (
     MigrationHop as MigrationHopTable,
+)
+from simmate.database.base_data_types.nudged_elastic_band import (
     MigrationImage as MigrationImageTable,
 )
+from simmate.website.core_components.filters import Structure
 
 
 class DiffusionAnalysis(Structure):
     class Meta:
         model = DiffusionAnalysisTable
         fields = dict(
             migrating_specie=["exact"],
```

### Comparing `simmate-0.8.0/src/simmate/website/core_components/filters/relaxation.py` & `simmate-0.9.0/src/simmate/website/core_components/filters/relaxation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # -*- coding: utf-8 -*-
 
+from simmate.database.base_data_types.relaxation import IonicStep as IonicStepTable
+from simmate.database.base_data_types.relaxation import Relaxation as RelaxationTable
 from simmate.website.core_components.filters import (
-    Structure,
+    Calculation,
     Forces,
+    Structure,
     Thermodynamics,
-    Calculation,
-)
-from simmate.database.base_data_types.relaxation import (
-    Relaxation as RelaxationTable,
-    IonicStep as IonicStepTable,
 )
 
 
 class Relaxation(Structure, Calculation):
     class Meta:
         model = RelaxationTable
         fields = dict(
```

### Comparing `simmate-0.8.0/src/simmate/website/core_components/filters/static_energy.py` & `simmate-0.9.0/src/simmate/website/core_components/filters/static_energy.py`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 
+from simmate.database.base_data_types import StaticEnergy as StaticEnergyTable
 from simmate.website.core_components.filters import (
-    Structure,
+    Calculation,
     Forces,
+    Structure,
     Thermodynamics,
-    Calculation,
 )
-from simmate.database.base_data_types import StaticEnergy as StaticEnergyTable
 
 
 class StaticEnergy(
     Structure,
     Forces,
     Thermodynamics,
     Calculation,
```

### Comparing `simmate-0.8.0/src/simmate/website/core_components/filters/structure.py` & `simmate-0.9.0/src/simmate/website/core_components/filters/structure.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from django_filters import rest_framework as filters
 
-from simmate.utilities import get_chemical_subsystems
 from simmate.database.base_data_types import Structure as StructureTable
+from simmate.utilities import get_chemical_subsystems
 
 
 class Structure(filters.FilterSet):
     class Meta:
         model = StructureTable
         fields = dict(
             nsites=["range"],
```

### Comparing `simmate-0.8.0/src/simmate/website/core_components/filters/thermodynamics.py` & `simmate-0.9.0/src/simmate/website/core_components/filters/thermodynamics.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/core_components/templatetags/chemical_formula_filter.py` & `simmate-0.9.0/src/simmate/website/core_components/templatetags/chemical_formula_filter.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/core_components/templatetags/markdown_filter.py` & `simmate-0.9.0/src/simmate/website/core_components/templatetags/markdown_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from textwrap import dedent
 
 from django import template
 from django.utils.safestring import mark_safe
-
 from pdoc.render_helpers import to_html
 
-
 # We need a registration instance in order to configure everything with Django
 register = template.Library()
 
 
 @register.filter(name="markdown")
 def markdown_to_html(markdown_str):
     """
```

### Comparing `simmate-0.8.0/src/simmate/website/core_components/templatetags/matplotlib_filter.py` & `simmate-0.9.0/src/simmate/website/core_components/templatetags/matplotlib_filter.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
-from io import BytesIO
 import base64
+from io import BytesIO
 
 from django import template
 from django.utils.safestring import mark_safe
 
 # We need a registration instance in order to configure everything with Django
 register = template.Library()
```

### Comparing `simmate-0.8.0/src/simmate/website/core_components/templatetags/structure_serialize_filter.py` & `simmate-0.9.0/src/simmate/website/core_components/templatetags/structure_serialize_filter.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/core_components/test/test_cc_views.py` & `simmate-0.9.0/src/simmate/website/core_components/test/test_cc_views.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 
 import pytest
 from pytest_django.asserts import assertTemplateUsed
+
 from simmate.website.core_components.templatetags.structure_serialize_filter import (
     structure_to_url,
 )
 
 
 @pytest.mark.django_db
 def test_spacegroup_views(client):
```

### Comparing `simmate-0.8.0/src/simmate/website/core_components/urls.py` & `simmate-0.9.0/src/simmate/website/core_components/urls.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/core_components/views.py` & `simmate-0.9.0/src/simmate/website/core_components/views.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import tempfile
 import time
 from pathlib import Path
 
 from django.shortcuts import render
 
-from simmate.toolkit import Structure
-from simmate.database.base_data_types import Spacegroup
-from simmate.visualization.structure.blender import make_blender_structure
 from simmate.configuration.django import settings
+from simmate.database.base_data_types import Spacegroup
+from simmate.toolkit import Structure
 from simmate.utilities import get_directory
+from simmate.visualization.structure.blender import make_blender_structure
 from simmate.website.core_components.base_api_view import SimmateAPIViewSet
 
 
 class SymmetryViewSet(SimmateAPIViewSet):
     table = Spacegroup
     template_list = "core_components/symmetry.html"
     template_retrieve = "core_components/spacegroup.html"
```

### Comparing `simmate-0.8.0/src/simmate/website/static_files/images/dask-icon.svg` & `simmate-0.9.0/src/simmate/website/static_files/images/dask-icon.svg`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/static_files/images/dask-logo.svg` & `simmate-0.9.0/src/simmate/website/static_files/images/dask-logo.svg`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/static_files/images/digitalocean-icon.svg` & `simmate-0.9.0/src/simmate/website/static_files/images/digitalocean-icon.svg`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/static_files/images/digitalocean-logo.svg` & `simmate-0.9.0/src/simmate/website/static_files/images/digitalocean-logo.svg`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/static_files/images/django-icon.svg` & `simmate-0.9.0/src/simmate/website/static_files/images/django-icon.svg`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/static_files/images/geometry_templates/cube.svg` & `simmate-0.9.0/src/simmate/website/static_files/images/geometry_templates/cube.svg`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/static_files/images/geometry_templates/octahedron.svg` & `simmate-0.9.0/src/simmate/website/static_files/images/geometry_templates/octahedron.svg`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/static_files/images/geometry_templates/tetrahedron.svg` & `simmate-0.9.0/src/simmate/website/static_files/images/geometry_templates/tetrahedron.svg`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/static_files/images/github-icon.svg` & `simmate-0.9.0/src/simmate/website/static_files/images/github-icon.svg`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/static_files/images/prefect-icon.svg` & `simmate-0.9.0/src/simmate/website/static_files/images/prefect-icon.svg`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/static_files/images/prefect-logo.svg` & `simmate-0.9.0/src/simmate/website/static_files/images/prefect-logo.svg`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/static_files/images/simmate-geometries.svg` & `simmate-0.9.0/src/simmate/website/static_files/images/simmate-geometries.svg`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/static_files/images/simmate-icon.svg` & `simmate-0.9.0/src/simmate/website/static_files/images/simmate-icon.svg`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/static_files/images/simmate-logo-dark.svg` & `simmate-0.9.0/src/simmate/website/static_files/images/simmate-logo-dark.svg`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/static_files/images/simmate-logo-other-ideas.svg` & `simmate-0.9.0/src/simmate/website/static_files/images/simmate-logo-other-ideas.svg`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/static_files/images/simmate-logo.svg` & `simmate-0.9.0/src/simmate/website/static_files/images/simmate-logo.svg`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/404.html` & `simmate-0.9.0/src/simmate/website/templates/404.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/500.html` & `simmate-0.9.0/src/simmate/website/templates/500.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/account/login.html` & `simmate-0.9.0/src/simmate/website/templates/account/login.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/account/loginstatus.html` & `simmate-0.9.0/src/simmate/website/templates/account/loginstatus.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/account/logout.html` & `simmate-0.9.0/src/simmate/website/templates/account/logout.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/account/profile.html` & `simmate-0.9.0/src/simmate/website/templates/account/profile.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/account/signup.html` & `simmate-0.9.0/src/simmate/website/templates/account/signup.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/about.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/about.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/band-structure.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/band-structure.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/calculation.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/calculation.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/density-of-states.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/density-of-states.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/forces.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/forces.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/relaxation.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/relaxation.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/static-energy.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/static-energy.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/structure.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/structure.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/base_data_types/thermodynamics.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/base_data_types/thermodynamics.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/band-structure.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/band-structure.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/calculation.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/calculation.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/density-of-states.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/density-of-states.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/diffusion-analysis.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/diffusion-analysis.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/dynamics-run.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/dynamics-run.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/forces.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/forces.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/relaxation.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/relaxation.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/static-energy.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/static-energy.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/structure.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/structure.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/base_filter_types/thermodynamics.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/base_filter_types/thermodynamics.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/contact.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/contact.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/datatable.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/datatable.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/extras.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/extras.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/footer.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/footer.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/footerbar.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/footerbar.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/navbar.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/navbar.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/periodic_table.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/periodic_table.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/search_form.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/search_form.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/search_results_pagination.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/search_results_pagination.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/sidebar.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/sidebar.html`

 * *Files 10% similar despite different names*

```diff
@@ -95,12 +95,23 @@
             <i class="mdi"></i>
         </a>
         <h5 class="mt-3">Download Simmate </h5>
         <p class="mb-3">You can install Simmate to host your own server and access advanced features</p>
         <a href="https://github.com/jacksund/simmate" class="btn btn-outline-primary btn-sm uil-github-alt"> learn more</a>
     </div>
     <!-- end Help Box -->
+    
+    <!-- This is an alert for user to focus on download, not UI -->
+    <div class="alert alert-danger d-flex align-items-center m-2" role="alert">
+        <i class="dripicons-warning me-2"></i>
+        <small>
+            Due to limited resources, our website only includes a small
+            number of features compared to the many available in the command-line and
+            python. We highly recommend installing Simmate for local use, rather
+            than just relying on the website.
+        </small>
+    </div>
 
     <div class="clearfix"></div>
     <!-- Sidebar -left -->
 
 </div>
```

#### html2text {}

```diff
@@ -4,7 +4,12 @@
     *   Third-Party_Data
     *
     *   Extras
 
 ** Download Simmate **
 You can install Simmate to host your own server and access advanced features
 learn_more
+
+ Due to limited resources, our website only includes a small number of features
+compared to the many available in the command-line and python. We highly
+recommend installing Simmate for local use, rather than just relying on the
+website.
```

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/site_base.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/site_base.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/structure_viewer.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/structure_viewer.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/table_entry.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/table_entry.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/core_components/test.html` & `simmate-0.9.0/src/simmate/website/templates/core_components/test.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/home/search-form.html` & `simmate-0.9.0/src/simmate/website/templates/home/search-form.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/home/search-results.html` & `simmate-0.9.0/src/simmate/website/templates/home/search-results.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/third_parties/entry_detail.html` & `simmate-0.9.0/src/simmate/website/templates/third_parties/entry_detail.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/third_parties/provider.html` & `simmate-0.9.0/src/simmate/website/templates/third_parties/provider.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/third_parties/providers_all.html` & `simmate-0.9.0/src/simmate/website/templates/third_parties/providers_all.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/third_parties/search_results.html` & `simmate-0.9.0/src/simmate/website/templates/third_parties/search_results.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/workflows/all.html` & `simmate-0.9.0/src/simmate/website/templates/workflows/all.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/workflows/by_type.html` & `simmate-0.9.0/src/simmate/website/templates/workflows/by_type.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/workflows/detail.html` & `simmate-0.9.0/src/simmate/website/templates/workflows/detail.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/workflows/detail_run.html` & `simmate-0.9.0/src/simmate/website/templates/workflows/detail_run.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/workflows/search_results.html` & `simmate-0.9.0/src/simmate/website/templates/workflows/search_results.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/templates/workflows/submit.html` & `simmate-0.9.0/src/simmate/website/templates/workflows/submit.html`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/test_app/models.py` & `simmate-0.9.0/src/simmate/website/test_app/models.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from simmate.database.base_data_types import (
-    DatabaseTable,
-    table_column,
-    Structure,
     Calculation,
+    DatabaseTable,
     Forces,
+    Structure,
     Thermodynamics,
+    table_column,
 )
 
 
 class TestDatabaseTable(DatabaseTable):
 
     base_info = ["column1", "column2"]
```

### Comparing `simmate-0.8.0/src/simmate/website/third_parties/forms.py` & `simmate-0.9.0/src/simmate/website/third_parties/forms.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/third_parties/test/test_third_parties_views.py` & `simmate-0.9.0/src/simmate/website/third_parties/test/test_third_parties_views.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 import pytest
-from pytest_django.asserts import assertTemplateUsed
 from django.urls import reverse
+from pytest_django.asserts import assertTemplateUsed
 
 
 def test_providers_view(client):
 
     # grabs f"/third-parties/"
     url = reverse("third_parties:home")
```

### Comparing `simmate-0.8.0/src/simmate/website/third_parties/views.py` & `simmate-0.9.0/src/simmate/website/third_parties/views.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/workflows/forms.py` & `simmate-0.9.0/src/simmate/website/workflows/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,15 @@
     ],
     "string": [
         "directory",
         "directory_old",
         "directory_new",
         "command",
         "migrating_specie",
+        "run_id",
     ],
     "integer": [
         "nsteps",
         "diffusion_analysis_id",
         "migration_hop_id",
     ],
     "float": [
```

### Comparing `simmate-0.8.0/src/simmate/website/workflows/test/test_workflows_views.py` & `simmate-0.9.0/src/simmate/website/workflows/test/test_workflows_views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 
 import pytest
-from pytest_django.asserts import assertTemplateUsed
 from django.urls import reverse
+from pytest_django.asserts import assertTemplateUsed
 
 from simmate.workflow_engine import Workflow
 from simmate.workflows.utilities import (
-    get_workflow_types,
     get_list_of_all_workflows,
     get_workflow,
+    get_workflow_types,
 )
 
 ALL_WORKFLOWS = get_list_of_all_workflows()
 
 
 def test_workflows_view(client):
     response = client.get("/workflows/")
@@ -38,14 +38,16 @@
 @pytest.mark.parametrize("workflow_name", ALL_WORKFLOWS)
 def test_workflow_detail_view(client, workflow_name):
 
     # BUG: I assume .vasp. in the view for now and also some views are broken
     if workflow_name in [
         "restart.simmate.automatic",
         "electronic-structure.vasp.matproj-full",
+        "structure-prediction.python.fixed-composition",
+        "structure-prediction.python.new-individual",
     ]:
         return
 
     workflow = get_workflow(workflow_name)
 
     # list view
     # grabs f"/workflows/{type}/{name}/")
@@ -129,9 +131,11 @@
         compress_output=False,
         wait_for_run=False,
         pre_sanitize_structure=False,
         pre_standardize_structure=False,
         # parameters not deserialized yet so these will still be present
         command="",
         directory="",
+        source=None,
+        run_id="",
         is_restart=False,
     )
```

### Comparing `simmate-0.8.0/src/simmate/website/workflows/urls.py` & `simmate-0.9.0/src/simmate/website/workflows/urls.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/website/workflows/views.py` & `simmate-0.9.0/src/simmate/website/workflows/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # -*- coding: utf-8 -*-
 
-from django.shortcuts import render, redirect
 from django.contrib.auth.decorators import login_required
+from django.shortcuts import redirect, render
 
-from simmate.database.base_data_types import DatabaseTable
 from simmate import workflows as workflow_module
-from simmate.workflows.utilities import (
-    # WORKFLOW_TYPES,
-    get_workflow,
+from simmate.database.base_data_types import DatabaseTable
+from simmate.website.core_components.base_api_view import SimmateAPIViewSet
+from simmate.website.workflows.forms import SubmitWorkflow
+from simmate.workflows.utilities import (  # WORKFLOW_TYPES,
     get_list_of_workflows_by_type,
+    get_workflow,
 )
-from simmate.website.workflows.forms import SubmitWorkflow
-from simmate.website.core_components.base_api_view import SimmateAPIViewSet
 
 
 def workflows_all(request):
 
     # TODO: maybe instead load these descriptions from the simmate.{module}'s docstr
     # This would look something like...
     # all_metadata = {}
```

### Comparing `simmate-0.8.0/src/simmate/workflow_engine/README.md` & `simmate-0.9.0/src/simmate/workflow_engine/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/workflow_engine/__init__.py` & `simmate-0.9.0/src/simmate/workflow_engine/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # -*- coding: utf-8 -*-
 
+# The order that we import these different modules is important to prevent
+# circular imports errors, so we prevent isort from changing this file.
+# isort: skip_file
+
 from simmate.utilities import get_doc_from_readme
 
 __doc__ = get_doc_from_readme(__file__)
 
 # OPTIMIZE: These imports are particularly slow because we are configuring
 # django in the code below this. These two imports don't depend on the database
 # module, so it may be worth isolating them for faster imports.
 from .error_handler import ErrorHandler
 
 # All imports below this point depend on the simmate.database module and therefore
 # need a database connection. This line sets up the database connection so
 # that models can be imported.
 from simmate.database import connect
 
+
 from .workflow import Workflow
 from .s3_workflow import S3Workflow
 from .execution import SimmateWorker as Worker
```

### Comparing `simmate-0.8.0/src/simmate/workflow_engine/error_handler.py` & `simmate-0.9.0/src/simmate/workflow_engine/error_handler.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 """
 Full documentation and guides for custom error-handlers is on our to-do this.
 If this is of particular interest to you, please let our team know so that
 we can prioritize creating these guides for you.
 """
 
-from pathlib import Path
-from abc import ABC, abstractmethod
 import subprocess
+from abc import ABC, abstractmethod
+from pathlib import Path
 
 
 class ErrorHandler(ABC):
     """
     Abstract base class for an ErrorHandler. These handlers should be used in
     combination with S3Tasks.
```

### Comparing `simmate-0.8.0/src/simmate/workflow_engine/execution/README.md` & `simmate-0.9.0/src/simmate/workflow_engine/execution/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/workflow_engine/execution/database.py` & `simmate-0.9.0/src/simmate/workflow_engine/execution/database.py`

 * *Files 20% similar despite different names*

```diff
@@ -53,14 +53,23 @@
     """
 
     result = table_column.BinaryField(blank=True, null=True)
     """
     the output of fxn(*args, **kwargs)
     """
 
+    command_not_found_failures = table_column.IntegerField(default=0)
+    """
+    Keeps track of the special-case "CommandNotFound" error that is hidden by
+    workers. This keeps a tally of how many Workers that this task is triggering
+    to shut down. This is important because it helps prevent total cluster
+    shutdown from a single typo in a command. By default, workers will label
+    a task as problematic if 2 workers give CommandNotFound errors.
+    """
+
     source = None
     """
     Source column is not needed so setting this to None disables the column
     """
 
     # These states are based on the python queue module
     class StatusOptions(table_column.TextChoices):
```

### Comparing `simmate-0.8.0/src/simmate/workflow_engine/execution/executor.py` & `simmate-0.9.0/src/simmate/workflow_engine/execution/executor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
-# import pickle
-import cloudpickle  # needed to serialize Prefect workflow runs and tasks
 import logging
 
+import cloudpickle  # needed to serialize Prefect workflow runs and tasks
+
 from simmate.workflow_engine.execution.database import WorkItem
 from simmate.workflow_engine.execution.future import SimmateFuture
 
 
 class SimmateExecutor:
     """
     Sets up a connection to the queue database. Unlike normal executors,
@@ -30,15 +30,20 @@
 
     # This class is modeled after the following...
     # https://github.com/python/cpython/blob/master/Lib/concurrent/futures/thread.py
     # https://docs.python.org/3/library/concurrent.futures.html
     # from concurrent.futures import Executor # No need to inherit at the moment
 
     @staticmethod
-    def submit(fxn, *args, tags=[], **kwargs):
+    def submit(
+        fxn: callable,
+        *args,
+        tags: list[str] = [],
+        **kwargs,
+    ) -> SimmateFuture:
 
         # The *args and **kwargs input separates args into a tuple and kwargs into
         # a dictionary for me, which makes their storage very easy!
 
         # make the WorkItem where all of the provided inputs are pickled and
         # save the workitem to the database.
         # Pickling is just converting them to a byte string format
@@ -56,15 +61,15 @@
         # create the future object
         future = SimmateFuture(pk=workitem.pk)
 
         # and return the future for use
         return future
 
     @staticmethod
-    def wait(self, futures):
+    def wait(futures: SimmateFuture):
         """
         Waits for all futures to complete before returning a list of their results
         """
         # If a dictionary of {key1: future1, key2: future2, ...} is given,
         # then we return a dictionary of which futures replaced by results.
         # NOTE: this is really for compatibility with Prefect's FlowRunner.
         if isinstance(futures, dict):
@@ -85,40 +90,43 @@
     # I attach these directly to the Executor rather than having a separate
     # DjangoQueue class that inherits from python's Queue module.
     # If there is a good reason to make a separate class in the future,
     # I can start from these methods here and the following link:
     # https://docs.python.org/3/library/queue.html
     # -------------------------------------------------------------------------
 
-    def queue_size(self):
+    @staticmethod
+    def queue_size() -> int:
         """
         Return the approximate size of the queue.
         """
         # Count the number of WorkItem(s) that have a status of PENDING
         # !!! Should I include RUNNING in the count? If so I do that with...
         #   from django.db.models import Q
         #   ...filter(Q(status="P") | Q(status="R"))
         queue_size = WorkItem.objects.filter(status="P").count()
         return queue_size
 
-    def clear_queue(self, are_you_sure=False):
+    @staticmethod
+    def clear_queue(are_you_sure: bool = False):
         """
         Empties the WorkItem database table and delete everything. This will
         not stop the workers if they are in the middle of a job though.
         """
         # Make sure the user ment to do this, otherwise raise an exception
         if not are_you_sure:
             raise Exception(
                 "Are you sure you want to do this? it deletes all of your queue"
                 "data and you can't get it back. If so, set are_you_sure=True."
             )
         else:
             WorkItem.objects.all().delete()
 
-    def clear_finished(self, are_you_sure=False):
+    @staticmethod
+    def clear_finished(self, are_you_sure: bool = False):
         """
         Empties the WorkItem database table and delete everything. This will
         not stop the workers if they are in the middle of a job though.
         """
         # Make sure the user ment to do this, otherwise raise an exception
         if not are_you_sure:
             raise Exception
```

### Comparing `simmate-0.8.0/src/simmate/workflow_engine/execution/future.py` & `simmate-0.9.0/src/simmate/workflow_engine/execution/future.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,21 +13,21 @@
     # https://docs.python.org/3/library/concurrent.futures.html
     # Some methods still need to be added, but I have no need for them yet.
     # from concurrent.futures import Future # No need to inherit at the moment
 
     # locking rows is done by...
     # https://docs.djangoproject.com/en/3.1/ref/models/querysets/#select-for-update
 
-    def __init__(self, pk):
+    def __init__(self, pk: int):
 
         # This is the WorkItem personal key which tells us which row in the table
         # we should loook at.
         self.pk = pk
 
-    def cancel(self):
+    def cancel(self) -> bool:
         """
         Attempt to cancel the call. If the call is currently being executed or
         finished running and cannot be cancelled then the method will return
         False, otherwise the call will be cancelled and the method will return
         True.
         """
         # Query the WorkItem, lock it for editting, and check the status.
@@ -42,54 +42,54 @@
         else:
             # If it is still pending, we can go ahead and cancel it.
             # This does not delete the task from the queue database though
             workitem.status = "C"
             workitem.save()
             return True
 
-    def is_cancelled(self):
+    def is_cancelled(self) -> bool:
         """
         Return True if the call was successfully cancelled.
         """
         # I don't use a lock to check the status here
         workitem = WorkItem.objects.only("status").get(pk=self.pk)
 
         # check the status and indicate whether it is CANCELED or not
         if workitem.status == "C":
             return True
         else:
             return False
 
-    def is_running(self):
+    def is_running(self) -> bool:
         """
         Return True if the call is currently being executed and cannot be cancelled.
         """
         # I don't use a lock to check the status here
         workitem = WorkItem.objects.only("status").get(pk=self.pk)
 
         # check the status and indicate whether it is RUNNING or not
         if workitem.status == "R":
             return True
         else:
             return False
 
-    def is_done(self):
+    def is_done(self) -> bool:
         """
         Return True if the call was successfully cancelled or finished running.
         """
         # I don't use a lock to check the status here
         workitem = WorkItem.objects.only("status").get(pk=self.pk)
 
         # check the status and indicate whether it is FINISHED or CANCELED
         if workitem.status == "F" or workitem.status == "C":
             return True
         else:
             return False
 
-    def result(self, timeout=None, sleep_step=0.1):
+    def result(self, timeout: float = None, sleep_step: float = 0.1) -> any:
         """
         Return the value returned by the call. If the call hasn’t yet completed
         then this method will wait up to timeout seconds. If the call hasn’t
         completed in timeout seconds, then a concurrent.futures.TimeoutError
         will be raised. timeout can be an int or float. If timeout is not
         specified or None, there is no limit to the wait time.
```

### Comparing `simmate-0.8.0/src/simmate/workflow_engine/execution/worker.py` & `simmate-0.9.0/src/simmate/workflow_engine/execution/worker.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 
-import time
-import cloudpickle  # needed to serialize Prefect workflow runs and tasks
 import logging
+import time
+import traceback
 
+import cloudpickle  # needed to serialize Prefect workflow runs and tasks
 from django.db import transaction
 
 from simmate.workflow_engine.execution.database import WorkItem
 
 # This string is just something fancy to display in the console when a worker
 # starts up.
 # This uses "Small Slant" from https://patorjk.com/software/taag/
@@ -17,61 +18,84 @@
  _\ \/ /  ' \/  ' \/ _ `/ __/ -_)  | |/ |/ / _ \/ __/  '_/ -_) __/
 /___/_/_/_/_/_/_/_/\_,_/\__/\__/   |__/|__/\___/_/ /_/\_\\__/_/
 
 """
 
 
 class SimmateWorker:
+    """
+    The default worker that connect to Simmate database for workflows submitted
+    via the `run_cloud` method.
+    """
 
     # Ideally, this worker would involve multiple threads threads going. One
     # thread would update the queue database with a "heartbeat" to let it know
     # that it is still working on tasks. The other thread will run the given
     # workitems in serial. I could even allow for more threads so that this
     # worker can run multiple workitems at once and in parallel.
     # However, if this level of implementation is needed, we should instead
     # switch to using Prefect, which has it built in.
 
+    # Consider making this a database object so that we can track workers in
+    # the UI and know how many are running.
+
     def __init__(
         self,
         # limit of tasks and lifetime of the worker
         nitems_max: int = None,
         timeout: float = None,
         # wait_on_timeout=False, # TODO
         # settings on what to do when the queue is empty
         close_on_empty_queue: bool = False,
         waittime_on_empty_queue: float = 1,
         tags: list[str] = ["simmate"],  # should default be empty...?
     ):
-        # the tags to query tasks for. If no tags were given, the worker will
-        # query for tasks that have NO tags
-        self.tags = tags
+        """
+        Configures a worker that connects to the default executor backend.
+        By default the worker will run endlessly.
 
-        # the maximum number of workitems to run before closing down
-        # if no limit was set, we can go to infinity!
-        self.nitems_max = nitems_max or float("inf")
+        #### Parameters:
 
-        # Don't start a new workitem after this time. The worker will be shut down.
-        # if no timeout was set, use infinity so we wait forever.
+        - `nitems_max`:
+            The maximum number of workitems to run before closing down
+            if no limit was set, we can go to infinity.
+
+        - `timeout`:
+            Don't start a new workitem after this time. The worker will be shut down.
+            if no timeout was set, use infinity so we wait forever.
+
+        - `close_on_empty_queue`:
+            whether to close if the queue is empty
+
+        - `waittime_on_empty_queue`:
+            if the queue is found to be empty, check the queue again after
+            this time sleeping.
+
+        - `tags`:
+            the tags to query tasks for. If no tags were given, the worker will
+            query for tasks that have NO tags
+
+        """
+        self.tags = tags
+        self.nitems_max = nitems_max or float("inf")
         self.timeout = timeout or float("inf")
+        self.close_on_empty_queue = close_on_empty_queue
+        self.waittime_on_empty_queue = waittime_on_empty_queue
 
         # whether to wait on the running workitems to finish before shutting down
         # the timedout worker.
         # self.wait_on_timeout = wait_on_timeout # # TODO
 
-        # whether to close if the queue is empty
-        self.close_on_empty_queue = close_on_empty_queue
-        # if the queue is found to be empty, we will give it one last chance
-        # to fill. Check the queue again after this time sleeping and if it is
-        # still empty, close the worker.
-        self.waittime_on_empty_queue = waittime_on_empty_queue
-
     def start(self):
+        """
+        Starts the worker process to begin working through WorkItems
+        """
 
         # print the header in the console to let the user know the worker started
-        print(HEADER_ART)
+        logging.info("\n" + HEADER_ART)
 
         # loggin helpful info
         logging.info(f"Starting worker with tags {list(self.tags)}")
 
         # establish starting point for the worker
         time_start = time.time()
         ntasks_finished = 0
@@ -145,21 +169,77 @@
 
             # Try running the WorkItem
             try:
                 result = fxn(*args, **kwargs)
             # if it fails, we want to "capture" the error and return it
             # rather than have the Worker fail itself.
             except Exception as exception:
+
+                traceback.print_exc()
+
+                logging.warning(
+                    "Task failed with the error shown above. \n\n"
+                    "If you are unfamilar with error tracebacks and find this error "
+                    "difficult to read, you can learn more about these errors "
+                    "here:\n https://realpython.com/python-traceback/\n\n"
+                    "Please open a new issue on our github page if you believe "
+                    "this is a bug:\n https://github.com/jacksund/simmate/issues/\n\n"
+                )
+
+                # local import to prevent circular import issues
+                from simmate.workflow_engine.s3_workflow import CommandNotFoundError
+
+                # The most common error (by far) is a command-not-found issue.
+                # We want to handle this separately -- whereas other exceptions
+                # we just pass on to the results.
+                if isinstance(exception, CommandNotFoundError):
+                    logging.warning(
+                        "This WorkItem failed with a 'command not found' error. "
+                        "This worker is likely improperly configured or "
+                        "you have a typo in your command."
+                    )
+
+                    with transaction.atomic():
+
+                        nfailures = workitem.command_not_found_failures + 1
+
+                        # Check if this task is problematic. If this error happened
+                        # with another worker, we likely have a problematic task
+                        if nfailures == 2:
+                            logging.warning(
+                                "This is the 2nd occurance with this task causing "
+                                "a 'command not found' problem. In case this a typo "
+                                "in your command, we are marking the task as CANCELLED "
+                                "to prevent it from shutting down other workers."
+                            )
+                            workitem.status = "C"
+                            workitem.save()
+                            # the result will be set below
+
+                        # Otherwise the user likely just forgot to use module load
+                        else:
+                            logging.info(
+                                f"Resetting WorkItem {workitem.id} to 'Pending' so "
+                                "another worker can retry."
+                            )
+
+                            workitem.command_not_found_failures = nfailures
+                            workitem.status = "P"
+                            workitem.save()
+                    logging.info("Shutting down to prevent repeated issues.")
+                    return
+
                 result = exception
 
             # whatever the result, we need to try to pickle it now
             try:
                 result_pickled = cloudpickle.dumps(result)
             # if this fails, we even want to pickle the error and return it
             except Exception as exception:
+                # otherwise package the full error
                 result_pickled = cloudpickle.dumps(exception)
 
             # requery the WorkItem to restart our lock
             workitem = WorkItem.objects.select_for_update().get(pk=workitem.pk)
 
             # our lock exists only within this transation
             with transaction.atomic():
@@ -171,28 +251,36 @@
 
             # mark down that we've completed one WorkItem
             ntasks_finished += 1
 
             # Print out the job ID that was just finished for the user to see.
             logging.info("Completed WorkItem")
 
-    def queue_size(self):
+    def queue_size(self) -> int:
         """
         Return the approximate size of the queue.
         """
         # Count the number of WorkItem(s) that have a status of PENDING
         # !!! Should I include RUNNING in the count? If so I do that with...
         #   from django.db.models import Q
         #   ...filter(Q(status="P") | Q(status="R"))
         queue_size = (
             WorkItem.objects.filter(status="P").filter_by_tags(self.tags).count()
         )
         return queue_size
 
     @classmethod
     def run_singleflow_worker(cls):
+        """
+        A convenience method for running a worker that...
+        1. shuts down immediately if the queue is empty
+        2. shuts down after a single workflow run
+
+        Because this type of worker is frequently used for HPC clusters, we
+        make a convenience method for it.
+        """
         worker = cls(
             nitems_max=1,
             close_on_empty_queue=True,
             tags=["simmate"],
         )
         worker.start()
```

### Comparing `simmate-0.8.0/src/simmate/workflow_engine/execution_prefect/worker.py` & `simmate-0.9.0/src/simmate/workflow_engine/execution_prefect/worker.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 
-import anyio
+import logging
 import time
 import uuid
 from functools import cached_property
-import logging
 
+import anyio
+from prefect.agent import OrionAgent
 from prefect.client import get_client
 from prefect.exceptions import PrefectHTTPStatusError
-from prefect.agent import OrionAgent
-from prefect.settings import PREFECT_AGENT_QUERY_INTERVAL
 from prefect.orion.schemas.filters import FlowRunFilter  # FlowFilter,
+from prefect.settings import PREFECT_AGENT_QUERY_INTERVAL
 
 from simmate.utilities import async_to_sync
 
 # This string is just something fancy to display in the console when a worker
 # starts up.
 # This uses "Small Slant" from https://patorjk.com/software/taag/
 HEADER_ART = r"""
```

### Comparing `simmate-0.8.0/src/simmate/workflow_engine/execution_prefect/workflow.py` & `simmate-0.9.0/src/simmate/workflow_engine/execution_prefect/workflow.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 
 from functools import cache  # cached_property doesnt work with classmethod
 
-from prefect.tasks import task  # present only for convience imports elsewhere
-from prefect.flows import Flow
-from prefect.states import State
-from prefect.context import FlowRunContext
 from prefect.client import get_client
+from prefect.context import FlowRunContext
+from prefect.flows import Flow
 from prefect.orion.schemas.filters import FlowFilter, FlowRunFilter
 from prefect.packaging import OrionPackager
 from prefect.packaging.serializers import PickleSerializer
+from prefect.states import State
+from prefect.tasks import task  # present only for convience imports elsewhere
 
 from simmate.utilities import async_to_sync
 
 
 class PrefectWorkflow:
     @classmethod
     def run(cls, **kwargs) -> State:
```

### Comparing `simmate-0.8.0/src/simmate/workflow_engine/s3_workflow.py` & `simmate-0.9.0/src/simmate/workflow_engine/s3_workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,36 +167,26 @@
 For experts, this class can be viewed as a combination of prefect's ShellTask,
 a custodian Job, and Custodian monitoring. When subclassing this, we can absorb
 functionality of `pymatgen.io.vasp.sets` too. By merging all of these together
 into one class, we make things much easier for users and creating new Tasks.
 
 """
 
+import logging
 import os
 import platform
-import time
 import signal
 import subprocess
-from typing import List, Tuple
+import time
 from pathlib import Path
-import logging
 
 import pandas
 
-from simmate.workflow_engine import Workflow, ErrorHandler
-from simmate.utilities import get_directory, make_archive, make_error_archive
-
-# cleanup_on_fail=False, # TODO I should add a Prefect state_handler that can
-# reset the working directory between task retries -- in some cases we may
-# want to delete the entire directory.
-
-# OPTIMIZE: I think this class would greatly benefit from asyncio so that we
-# know exactly when a shelltask completes, rather than looping and checking every
-# set timestep.
-# https://docs.python.org/3/library/asyncio-subprocess.html#asyncio.create_subprocess_exec
+from simmate.utilities import get_directory, make_error_archive
+from simmate.workflow_engine import ErrorHandler, Workflow
 
 
 class S3Workflow(Workflow):
     """
     The base Supervised-Staged-Shell that many workflows inherit from. This class
     encapulates logic for running external programs (like VASP), fixing common
     errors during a calculation, and working up the results.
@@ -212,15 +202,15 @@
     required_files = []
     """
     Before the command is executed, this list of files should be present
     in the working directory. This check will be made after `setup` is called
     and before `execute` is called. By default, no input files are required.
     """
 
-    error_handlers: List[ErrorHandler] = []
+    error_handlers: list[ErrorHandler] = []
     """
     A list of ErrorHandler objects to use in order of priority (that is, highest
     priority is first). If one handler is triggered, the correction will be 
     applied and none of the following handlers will be checked.
     """
 
     max_corrections: int = 10
@@ -252,21 +242,29 @@
     based on the polling_timestep loops. For example, if we have a
     polling_timestep of 10 seconds and a monitor_freq of 2, then we would run
     the monitor checks every other loop -- or every 2x10 = 20 seconds. The
     default values of polling_timestep=10 and monitor_freq=30 indicate that
     we run monitoring functions every 5 minutes (10x30=300s=5min).
     """
 
+    # cleanup_on_fail=False, # TODO I should add a Prefect state_handler that can
+    # reset the working directory between task retries -- in some cases we may
+    # want to delete the entire directory.
+
+    # OPTIMIZE: I think this class would greatly benefit from asyncio so that we
+    # know exactly when a shelltask completes, rather than looping and checking every
+    # set timestep.
+    # https://docs.python.org/3/library/asyncio-subprocess.html#asyncio.create_subprocess_exec
+
     @classmethod
     def run_config(
         cls,
         directory: Path = None,
         command: str = None,
         is_restart: bool = False,
-        compress_output: bool = False,
         **kwargs,
     ):
         """
          Runs the entire staged task (setup, execution, workup), which includes
          supervising during execution.
 
          #### Example use
@@ -288,19 +286,14 @@
 
         - `is_restart`:
             whether or not this calculation is a continuation of a previous run
             (i.e. a restarted calculation). If so, the `setup_restart` will be
             called instead of the setup method. Extra checks will be made to
             see if the calculation completed already too.
 
-        - `compress_output`:
-            Whether to compress the directory to a zip file at the end of the
-            task run. After compression, it will also delete the directory.
-            The default is False.
-
          - `**kwargs`:
              Any extra keywords that should be passed to the setup() method.
 
         #### Returns
 
          - a dictionary of the result, corrections, and working directory used
          for this task run
@@ -356,19 +349,14 @@
             # OPTIMIZE: this same code is at the start of the execute method.
             # Consider making it into a utility.
 
         # run the workup stage of the task. This is where the data/info is pulled
         # out from the calculation and is thus our "result".
         result = cls.workup(directory=directory)
 
-        # if requested, compresses the directory to a zip file and then removes
-        # the directory.
-        if compress_output:
-            make_archive(directory)
-
         # Return our final information as a dictionary
         result = {
             "result": result,
             "corrections": corrections,
             "directory": directory,
         }
 
@@ -459,15 +447,15 @@
                     "The following files must exist in the directory where "
                     f"this task is ran but some are missing: {cls.required_files}"
                 )
             return False  # indicates something is missing
         return True  # indicates all files are present
 
     @classmethod
-    def execute(cls, directory: Path, command: str) -> List[Tuple[str]]:
+    def execute(cls, directory: Path, command: str) -> list[tuple[str]]:
         """
         This calls the command within the target directory and handles all error
         handling as well as monitoring of the job.
 
         You should never call this method directly unless you are debugging. This
         is becuase `execute` is normally called within the `run` method.
 
@@ -625,20 +613,35 @@
 
             # check if the return code is non-zero and thus failed.
             # The 'not has_error' is because terminate() will give a nonzero
             # when a monitor is triggered. We don't want to raise that
             # exception here but instead let the monitor handle that
             # error in the code below.
             if process.returncode != 0 and not has_error:
+
                 # convert the error from bytes to a string
                 errors = errors.decode("utf-8")
-                # and report the error to the user
-                raise NonZeroExitError(
-                    f"The command ({command}) failed. The error output was...\n {errors}"
-                )
+                # and report the error to the user. Mac/Linux label this as exit
+                # code 127, whereas windows doesn't so the message needs to be
+                # read.
+                if process.returncode == 127 or (
+                    platform.system() == "Windows"
+                    and "is not recognized as an internal or external command"
+                ):
+                    raise CommandNotFoundError(
+                        f"The command ({command}) failed becauase it could not be found. "
+                        "This typically means that either (a) you have not installed "
+                        "the program required for this command or (b) you forgot to "
+                        "call 'module load ...' before trying to start the program. "
+                        f"The full error output was:\n\n {errors}"
+                    )
+                else:
+                    raise NonZeroExitError(
+                        f"The command ({command}) failed. The error output was...\n {errors}"
+                    )
 
             # Check for errors again, because a non-monitor may be higher
             # priority than the monitor triggered above (if there was one).
             # Since the error_handlers are in order of priority, only the first
             # will actually be applied and then we can retry the calc.
             for error_handler in cls.error_handlers:
 
@@ -809,7 +812,11 @@
 
 class MaxCorrectionsError(Exception):
     pass
 
 
 class NonZeroExitError(Exception):
     pass
+
+
+class CommandNotFoundError(NonZeroExitError):
+    pass
```

### Comparing `simmate-0.8.0/src/simmate/workflow_engine/test/test_error_handler.py` & `simmate-0.9.0/src/simmate/workflow_engine/test/test_error_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
+
 import pytest
+
 from simmate.workflow_engine.error_handler import ErrorHandler
 
 
 class CheckREADME(ErrorHandler):
     """
     This checks if simmate is in located in this file (which will always be true).
```

### Comparing `simmate-0.8.0/src/simmate/workflow_engine/test/test_s3_workflow.py` & `simmate-0.9.0/src/simmate/workflow_engine/test/test_s3_workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 
 import shutil
 
 import pytest
 
 from simmate.workflow_engine import ErrorHandler, S3Workflow
 from simmate.workflow_engine.s3_workflow import (
-    NonZeroExitError,
+    CommandNotFoundError,
     MaxCorrectionsError,
+    NonZeroExitError,
 )
 
 # ----------------------------------------------------------------------------
 
 # make some a simple ErrorHandlers for us to test with
 
 
@@ -118,35 +119,15 @@
     # make sure that a "simmate-task-*" directory was created
     assert output["directory"].exists()
 
     # and delete that directory
     output["directory"].rmdir()
 
 
-def test_s3workflow_2():
-    # test file compression
-
-    class Customized__Testing__DummyWorkflow(S3Workflow):
-        command = "echo dummy"
-        use_database = False
-        monitor = False
-
-    output = Customized__Testing__DummyWorkflow.run_config(compress_output=True)
-
-    # make sure that a "simmate-task-*.zip" archive was created
-    assert output["directory"].with_suffix(".zip").exists()
-
-    # make sure that a "simmate-task-*" directory was removed
-    assert not output["directory"].exists()
-
-    # and delete the archive
-    output["directory"].with_suffix(".zip").unlink()
-
-
-def test_s3workflow_3(tmp_path):
+def test_s3workflow_2(tmp_path):
     # Make a task with error handlers, monitoring, and specific directory
 
     class Customized__Testing__DummyWorkflow(S3Workflow):
         command = "echo dummy"
         use_database = False
         polling_timestep = 0
         monitor_freq = 2
@@ -160,32 +141,45 @@
     assert Customized__Testing__DummyWorkflow.run_config(directory=tmp_path) == {
         "result": None,
         "corrections": [],
         "directory": tmp_path,
     }
 
 
-def test_s3workflow_4(tmp_path):
-    # test nonzero returncode
+def test_s3workflow_3(tmp_path):
+    # test nonzero returncodes
 
     class Customized__Testing__DummyWorkflow(S3Workflow):
         use_database = False
         command = "NonexistantCommand 404"
         polling_timestep = 0
         monitor_freq = 2
         error_handlers = [AlwaysPassesHandler()]
 
     pytest.raises(
+        CommandNotFoundError,
+        Customized__Testing__DummyWorkflow.run_config,
+        directory=tmp_path,
+    )
+
+    class Customized__Testing__DummyWorkflow(S3Workflow):
+        use_database = False
+        command = "cd xyz123"  # will fail with "directory does not exist"
+        polling_timestep = 0
+        monitor_freq = 2
+        error_handlers = [AlwaysPassesHandler()]
+
+    pytest.raises(
         NonZeroExitError,
         Customized__Testing__DummyWorkflow.run_config,
         directory=tmp_path,
     )
 
 
-def test_s3workflow_5(tmp_path):
+def test_s3workflow_4(tmp_path):
     # testing handler-triggered failures
 
     class Customized__Testing__DummyWorkflow(S3Workflow):
         use_database = False
         command = "echo dummy"
         polling_timestep = 0
         monitor_freq = 2
@@ -194,15 +188,15 @@
     pytest.raises(
         MaxCorrectionsError,
         Customized__Testing__DummyWorkflow.run_config,
         directory=tmp_path,
     )
 
 
-def test_s3workflow_6(tmp_path):
+def test_s3workflow_5(tmp_path):
     # monitor failure
 
     class Customized__Testing__DummyWorkflow(S3Workflow):
         use_database = False
         command = "echo dummy"
         polling_timestep = 0
         monitor_freq = 2
@@ -211,15 +205,15 @@
     pytest.raises(
         MaxCorrectionsError,
         Customized__Testing__DummyWorkflow.run_config,
         directory=tmp_path,
     )
 
 
-def test_s3workflow_7(tmp_path):
+def test_s3workflow_6(tmp_path):
     # special-monitor failure (non-terminating monitor)
 
     class Customized__Testing__DummyWorkflow(S3Workflow):
         use_database = False
         command = "echo dummy"
         polling_timestep = 0
         monitor_freq = 2
@@ -228,30 +222,30 @@
     pytest.raises(
         MaxCorrectionsError,
         Customized__Testing__DummyWorkflow.run_config,
         directory=tmp_path,
     )
 
 
-def test_s3workflow_8(tmp_path):
+def test_s3workflow_7(tmp_path):
     # check that monitor exits cleanly when retries are not allowed and no
     # workup method raises an error
 
     class Customized__Testing__DummyWorkflow(S3Workflow):
         use_database = False
         command = "echo dummy"
         polling_timestep = 0
         monitor_freq = 2
         error_handlers = [AlwaysFailsSpecialMonitorNoRetry()]
 
     result = Customized__Testing__DummyWorkflow.run_config(directory=tmp_path)
     assert len(result["corrections"]) == 1
 
 
-def test_s3workflow_9(tmp_path):
+def test_s3workflow_8(tmp_path):
     # make sure an error is raised when a file is missing
 
     class Customized__Testing__DummyWorkflow(S3Workflow):
         use_database = False
         command = "echo dummy"
         required_files = ["FILE_THAT_DOESNT_EXIST"]
```

### Comparing `simmate-0.8.0/src/simmate/workflow_engine/test/test_workflow.py` & `simmate-0.9.0/src/simmate/workflow_engine/test/test_workflow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import pytest
 
-from simmate.workflow_engine import Workflow
 from simmate.website.test_app.models import TestCalculation
+from simmate.workflow_engine import Workflow
 
 
 class DummyProject__DummyCaclulator__DummyPreset(Workflow):
     """
     Minimal example of a workflow
     """
 
@@ -41,22 +41,46 @@
     assert DummyFlow.name_type == "dummy-project"
     assert DummyFlow.name_calculator == "dummy-caclulator"
     assert DummyFlow.name_preset == "dummy-preset"
 
     # testing class properties
     assert DummyFlow.description_doc == DummyFlow.__doc__
     assert DummyFlow.description_doc.strip() == "Minimal example of a workflow"
-    assert DummyFlow.parameter_names == ["source", "structure"]
-    assert DummyFlow._parameters_to_register == ["source"]
+    assert DummyFlow.parameter_names == [
+        "compress_output",
+        "directory",
+        "run_id",
+        "source",
+        "structure",
+    ]
+    assert DummyFlow._parameters_to_register == [
+        "directory",
+        "run_id",
+        "source",
+    ]
     DummyFlow.show_parameters()  # a print statment w. nothing else to check
 
     assert isinstance(DummyFlow.get_config(), dict)
 
     DummyFlow.show_config()  # a print statment w. nothing else to check
 
+    # test file compression
+    new_dir = tmp_path / "new_folder"
+    state = DummyFlow.run(directory=new_dir, compress_output=True)
+    result = state.result()
+
+    # make sure that a "simmate-task-*.zip" archive was created
+    assert new_dir.with_suffix(".zip").exists()
+
+    # make sure that a "simmate-task-*" directory was removed
+    assert not new_dir.exists()
+
+    # and delete the archive
+    new_dir.with_suffix(".zip").unlink()
+
 
 def test_serialize_parameters():
     class TestParameter1:
         def to_dict(self):
             return {}
 
     class TestParameter2:
```

### Comparing `simmate-0.8.0/src/simmate/workflow_engine/utilities.py` & `simmate-0.9.0/src/simmate/workflow_engine/utilities.py`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/workflow_engine/workflow.py` & `simmate-0.9.0/src/simmate/workflow_engine/workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,42 +28,47 @@
 
 workflow = get_workflow("static-energy.vasp.matproj")
 ```
 
 
 ## Viewing input parameters
 
-A workflow's nput parameters can be analyzed in the following ways:
+A workflow's input parameters can be analyzed in the following ways:
 
 ``` python
 workflow.show_parameters()  # prints out info
 workflow.parameter_names
 workflow.parameter_names_required
 ```
 
 
 ## Running a workflow (local)
 
 To run a workflow locally (i.e. directly on your current computer), you can
-use the `run` method. This is returns a `State` object, which allows
-you to check if the run completed successfully or not. Then final output of your
-workflow run can be accessed using `state.result()`. You can read more about
-`State` objects [here](https://orion-docs.prefect.io/concepts/states/), but as
-a quick example:
+use the `run` method. As a quick example:
 
 ``` python
 state = workflow.run(
     structure="NaCl.cif", 
     command="mpirun -n 4 vasp_std > vasp.out",
 )
 
 if state.is_completed():  # optional check
     result = state.result()
 ```
 
+Note that `run` returned a `State` object, not our result. States allows you to
+check if the run completed successfully or not. Then final output of your
+workflow run can be accessed using `state.result()`. The `State` is based off
+of Prefect's state object, which you can read more about 
+[here](https://orion-docs.prefect.io/concepts/states/). We use `State`s because 
+the status of a run becomes important when we start scheduling runs to run
+remotely, and more importantly, it allows use to building in compatibility with
+other workflow engines like Prefect.
+
 Outside of python, you can also run workflows from the command line, using YAML 
 files, or the website interface. These approaches are covered in the intro
 tutorials.
 
 
 ## Running a workflow (cloud)
 
@@ -117,21 +122,30 @@
 df = table.obects.to_dataframe()
 
 # or grab a specific run result and convert to a toolkit object
 entry = table.objects.get(run_id="example-123456")
 structure = entry.to_toolkit()
 ```
 
+You'll notice the table gives results for all runs of this type (e.g. all
+static-energies). To limit your results to just this specific workflow, you
+can use the `all_results` property:
+
+``` python
+results = workflow.all_results
+
+# the line above is a shortcut for...
+table = workflow.database_table
+results = workflow.database_table.objects.filter(workflow_name=workflow.name_full)
+```
+
 Filtering of results is covered in the `simmate.database` documentation.
 
 <!--
 TODO:
-    - viewing parameter names
-    - accessing results (database_table)
-    - run_cloud and other cloud methods
     - different documentation levels (parameters, mini docstring, etc.)
     - finding the same workflow in the website UI (place this )
 -->
 
 
 
 
@@ -150,29 +164,29 @@
     3.  A unique name to identify the settings used
 
 Examples for each part would be:
     1. relaxation, static-energy, dynamics, ...
     2. vasp, abinit, qe, deepmd, ...
     3. jacks-test, matproj, quality00, ...
 
-Together, an example workflow names would be:
+Together, example workflow names would be:
     - `relaxation.vasp.jacks-test`
     - `static-energy.abinit.matproj`
     - `dynamics.qe.quality00`
 
 When converting this to our workflow name in python, we need to replace
 periods with 2 underscores each and convert our words to
 [pascal case](https://khalilstemmler.com/blogs/camel-case-snake-case-pascal-case/).
 For example, our workflow names become:
     - `Relaxation__Vasp__JacksTest`
     - `StaticEnergy__Abinit__Matproj`
     - `Dynamics__Qe__Quality00`
 
 NOTE: Capitalization is very important here so make sure you double check
-your workflow names.
+your workflow names. Hyphens are placed based on capital letters.
 
 Now let's test this out in python using a similar workflow name:
 ``` python
 from simmate.workflow_engine import Workflow
 
 class Example__Python__MyFavoriteSettings(Workflow):
     pass  # we will build the rest of workflow later
@@ -189,40 +203,37 @@
 ```
 
 You now have a ready-to-use workflow name!
 
 
 ## Example workflow
 
-To convert this to a Simmate workflow, we just need to change the format
-a little. Instead of a `@flow` decorator, we use the `run_config` method
-of a new subclass:
+To build a Simmate workflow, you can have ANY python code you'd like. The only
+requirement is that you place that code inside a `run_config` method of a 
+new subclass for `Workflow`:
 
 ``` python
-# NOTE: this example does not follow Simmate's naming convention, so
-# some higher level features will be broken. We will fix in a later step.
-
 from simmate.workflow_engine import Workflow
 
 class Example__Python__MyFavoriteSettings(Workflow):
     
     use_database = False  # we don't have a database table yet
 
     @staticmethod
-    def run_config():
+    def run_config(**kwargs):
         print("This workflow doesn't do much")
         return 42
 
 # and then run your workflow
 state = MyFavoriteWorkflow.run()
 result = state.result()
 ```
 
 Behind the scenes, the `run` method is converting our `run_config` to a 
-workflow for us.
+workflow and doing extra setup tasks for us.
 
 Now let's look at a realistic example where we build a Workflow that has
 input parameters and accesses class attributes/methods:
 
 ``` python
 
 class Example__Python__MyFavoriteSettings(Workflow):
@@ -261,14 +272,56 @@
 Once you have your new workflow, you can run it as you would any other worfklow:
 
 ``` python
 state = Example__Python__MyFavoriteSettings.run("Jack")
 result = state.result()
 ```
 
+## Default parameters and using kwargs
+
+You'll notice in the workflow above that we used `**kwargs` in each of our
+`run_config` methods -- and if you remove these, the workflow will fail. This
+is because simmate adds default parameters to the `run_config` that can be used
+by all workflows. These parameters are:
+
+- `run_id`: a unique id to help with tracking a calculation
+- `directory`: a unique foldername that the calculation will take place in
+- `compress_output`: whether to compress the directory to a zip file when we're done
+- `source`: where the input of this calculation came from (EXPERIMENTAL FEATURE)
+
+You can use any of these inputs to help with your workflow. Most commonly, you
+just use the `directory` input and just ignore the others by adding `**kwargs`.
+It is important to note that `directory` is given as a 
+[`pathlib.Path`](https://docs.python.org/3/library/pathlib.html) object.
+
+``` python
+from simmate.workflow_engine import Workflow
+
+class Example__Python__MyFavoriteSettings(Workflow):
+    
+    use_database = False  # we don't have a database table yet
+
+    @staticmethod
+    def run_config(directory, **kwargs):
+        
+        # We use the unique directory to write outputs!
+        # Recall that we have a pathlib.Path object.
+        output_file = directory / "my_output.txt"
+        
+        with output_file.open("w") as file:
+            file.write("Writing my output!")
+        
+        # If you don't like/know pathlib.Path, you can
+        # convert the directory name back to a string
+        output_filename = str(output_file)
+        
+        return "Done!"
+
+```
+
 
 ## Modifying an existing workflow
 
 You can use python inheritance to borrow utilities and settings from workflows.
 However, make sure you are making copies of the original workflow settings!
 If you modify them without making a copy, you'll be in a world of trouble.
 
@@ -382,42 +435,42 @@
 # some higher level features will be broken. We will fix in a later step.
 
 from simmate.workflow_engine import Workflow
 
 class Example__Python__MyFavoriteSettings(Workflow):
 
     @staticmethod
-    def run_config():
+    def run_config(**kwargs):
         print("This workflow doesn't do much")
         return 42
 
 # and then run your workflow
 state = MyFavoriteWorkflow.run()
 result = state.result()
 ```
 
 Behind the scenes, the `run` method is converting our `run_config` to a
 Prefect workflow for us. Methods like `run_cloud` will automatically use
 Prefect now too.
 
 """
 
-import logging
+import inspect
 import json
-import cloudpickle
-import yaml
+import logging
 import re
-import inspect
-from typing import List, Any
 import uuid
 from pathlib import Path
 
+import cloudpickle
+import yaml
+
 import simmate
 from simmate.database.base_data_types import Calculation
-from simmate.utilities import get_directory, copy_directory
+from simmate.utilities import copy_directory, get_directory, make_archive
 from simmate.workflow_engine.execution import SimmateExecutor, WorkItem
 
 
 class DummyState:
     """
     This class is meant to emulate Prefect States. By wrapping a result into
     State, we enable higher-level features that depend on a call to
@@ -439,16 +492,14 @@
 
 
 class Workflow:
     """
     An abstract base class for all Simmate workflows.
     """
 
-    # TODO: set storage attribute to module
-
     version: str = simmate.__version__
     """
     Version number for this flow. Defaults to the Simmate version 
     (e.g. "0.7.0").
     """
 
     description_doc_short: str = None
@@ -467,127 +518,197 @@
     `_register_calculation` will save a database entry before the workflow
     starts. This is useful to keep track of workflows that have been
     submitted/started but haven't finished yet.
     
     `_save_to_database` saves the output of the `workup` method to the database.
     """
 
-    _parameter_methods = ["run_config"]
+    _parameter_methods = ["run_config", "_run_full"]
     """
     List of methods that allow unique input parameters. This helps track where
     `**kwargs` are passed and let's us gather the inputs in one place.
     """
 
     # -------------------------------------------------------------------------
     # Core methods that handle how and what a workflow run does
     # and how it is submitted
     # -------------------------------------------------------------------------
 
     @classmethod
-    def run_config(cls):
+    def run(cls, **kwargs) -> DummyState:
         """
-        The workflow method, which can be overwritten when inheriting from this
-        class. This can be either a staticmethod or classmethod.
+        The highest-level method to run a workflow. This includes calling
+        `run_config` and all of the extra steps involved (such as registering
+        a calculation to the database and creating the working directory).
+
+        For advanced users, we recommend reading through the `_run_full` method
+        to see the full workflow logic.
         """
-        raise NotImplementedError(
-            "When creating a custom workflow, make sure you set a run_config method!"
-        )
+        # Note: this is a separate method and wrapper around run_full because
+        # we want to allow Prefect executor to overwrite this method.
+        result = cls._run_full(**kwargs)
+        state = DummyState(result)
+        return state
 
     @classmethod
-    def _run_full(cls, run_id=None, **kwargs):
-        """
-        This method should not be called directly. Use the `run` method instead.
+    def _run_full(
+        cls,
+        run_id: str = None,
+        directory: Path | str = None,
+        compress_output: bool = False,
+        source: dict = None,
+        **kwargs,
+    ):
+        """
+
+        The full logic for a workflow run. This deserialize input parameters,
+        register the calculation to the database, call the defined
+        `run_config` command, and save results to the database.
+
+        This method should not be called directly. Use the `run` method instead,
+        which will properly convert to a `Prefect` workflow (if necessary) and
+        return a State-like object.
+
+        #### Parameters
+
+        - `run_id`:
+            A unique id that is assigned to the workflow run. If an ID was not
+            provided, a randomly-generated id from
+            [UUID4](https://docs.python.org/3/library/uuid.html#uuid.uuid4)
+            is used. We recommend leaving this at default.
+
+         - `directory`:
+             The directory to run everything in. This is passed to the ulitities
+             function simmate.ulitities.get_directory, which generates a
+             unique foldername if not provided. This will be converted into
+             a `pathlib.Path` object.
+
+        - `compress_output`:
+            Whether to compress the directory to a zip file at the end of the
+            task run. After compression, it will also delete the directory.
+            The default is False.
+
+        - `source`: (EXPERIMENTAL FEATURE)
+            The source is JSON-like information that indicates where the
+            input for this calculation came from, which could be a number
+            of things including (another calculation, a simple comment, etc.).
+            This is useful if you want to label results in your database.
+
         """
-        logging.info(f"Starting {cls.name_full}")
         # This method is isolated only because we want to wrap it as a prefect
         # workflow in some cases.
-        run_id = run_id or cls._get_run_id()
-        kwargs_cleaned = cls._load_input_and_register(run_id=run_id, **kwargs)
+        logging.info(f"Starting {cls.name_full}")
+        kwargs_cleaned = cls._load_input_and_register(
+            run_id=run_id,
+            directory=directory,
+            compress_output=compress_output,
+            source=source,
+            **kwargs,
+        )
         result = cls.run_config(**kwargs_cleaned)
         if cls.use_database:
-            result["calculation_id"] = cls._save_to_database(result, run_id=run_id)
-        logging.info(f"Completed {cls.name_full}")
-        return result
+            result["calculation_id"] = cls._save_to_database(
+                result,
+                run_id=kwargs_cleaned["run_id"],
+            )
 
-    @staticmethod
-    def _get_run_id():
-        """
-        generates a random id to use as a workflow run id
-        """
-        # This is a separate method in order to allow the prefect executor to
-        # overwrite this method.
-        unique_id = str(uuid.uuid4())
-        return unique_id
+        # if requested, compresses the directory to a zip file and then removes
+        # the directory.
+        if compress_output:
+            logging.info("Compressing result to a ZIP file.")
+            make_archive(kwargs_cleaned["directory"])
 
-    @classmethod
-    def run(cls, **kwargs) -> DummyState:
-        """
-        runs the workflow locally
-        """
-        # Note: this is a separate method and wrapper around run_full because
-        # we want to allow Prefect executor to overwrite this method.
-        result = cls._run_full(**kwargs)
-        state = DummyState(result)
-        return state
+        logging.info(f"Completed {cls.name_full}")
+        return result
 
     @classmethod
     def run_cloud(
-        cls, return_state: bool = True, tags: list[str] = None, **kwargs
-    ) -> str:
-        """
-        submits the workflow run to cloud database to be ran by a worker
+        cls,
+        return_state: bool = True,
+        tags: list[str] = None,
+        **kwargs,
+    ):
+        """
+        Submits the workflow run to cloud database to be ran by a worker.
+
+        #### Parameters
+
+        - `return_state`:
+            Whether to return a State-like object or just the run_id. Defaults
+            to true, which returns a State.
+
+        - `tags`:
+            A list of flags/labels/tags that the workflow run should be scheduled
+            with. This helps with limiting which workers are allow to pickup
+            and run the workflow. Defaults to the `tags` property of the
+            workflow.
         """
 
         logging.info(f"Submitting new run of {cls.name_full} to cloud")
 
+        # To help with tracking the flow in cloud, we create the flow_id up front.
+        kwargs["run_id"] = kwargs.get("run_id", None) or cls._get_run_id()
+        run_id = kwargs["run_id"]  # just for easy reference below
+
         # If we are submitting using a filename, we don't want to
         # submit to a cluster and have the job fail because it doesn't have
         # access to the file. We therefore deserialize right before
         # serializing in the next line in order to ensure parameters that
         # accept file names are submitted with all necessary data.
         parameters_deserialized = cls._deserialize_parameters(**kwargs)
         parameters_serialized = cls._serialize_parameters(**parameters_deserialized)
 
         # Because we often want to save some info to our database even before
         # the calculation starts/finishes, we do that by calling _register_calc
         # at this higher level. An example is storing the structure and run id.
         # Thus, we create and register the run_id up front
-        run_id = cls._get_run_id()
         if cls.use_database:
-            cls._register_calculation(run_id=run_id, **kwargs)
+            cls._register_calculation(**kwargs)
 
         state = SimmateExecutor.submit(
             cls._run_full,  # should this be the run method...?
-            run_id=run_id,
             tags=tags or cls.tags,
             **parameters_serialized,
         )
 
         logging.info(f"Successfully submitted (run_id={run_id})")
 
         # If the user wants the future, return that instead of the run_id
         if return_state:
             state.run_id = run_id  # attach the run id as an extra
             return state
 
         return run_id
 
+    @classmethod
+    def run_config(cls, **kwargs) -> any:
+        """
+        The workflow method, which can be overwritten when inheriting from this
+        class. This can be either a `staticmethod` or `classmethod`.
+        """
+        raise NotImplementedError(
+            "When creating a custom workflow, make sure you set a run_config method!"
+        )
+
     # -------------------------------------------------------------------------
     # Methods that interact with the Executor class in order to see what
     # has been submitted to cloud.
     # -------------------------------------------------------------------------
 
     @classmethod
     @property
     def nflows_submitted(cls) -> int:
         """
         Queries the Simmate database to see how many workflows are in a
         running or pending state.
         """
-        return WorkItem.objects.filter(status__in=["P", "R"], tags=cls.tags).count()
+        return WorkItem.objects.filter(
+            status__in=["P", "R"],
+            tags=cls.tags,
+        ).count()
 
     # -------------------------------------------------------------------------
     # Methods that help with accessing the database and saving results
     # -------------------------------------------------------------------------
 
     @classmethod
     @property
@@ -613,17 +734,15 @@
             return StaticEnergy
         elif flow_type == "electronic-structure":
             if "band-structure" in flow_preset:
                 from simmate.database.base_data_types import BandStructureCalc
 
                 return BandStructureCalc
             elif "density-of-states" in flow_preset:
-                from simmate.database.base_data_types import (
-                    DensityofStatesCalc,
-                )
+                from simmate.database.base_data_types import DensityofStatesCalc
 
                 return DensityofStatesCalc
         elif flow_type == "population-analysis":
             from simmate.database.base_data_types import PopulationAnalysis
 
             return PopulationAnalysis
         elif flow_type == "dynamics":
@@ -643,15 +762,19 @@
             from simmate.database.base_data_types import CustomizedCalculation
 
             return CustomizedCalculation
         else:
             raise NotImplementedError("Unable to detect proper database table")
 
     @classmethod
-    def _save_to_database(cls, result, run_id):
+    def all_results(cls):  # -> SearchResults
+        return cls.database_table.objects.filter(workflow_name=cls.name_full)
+
+    @classmethod
+    def _save_to_database(cls, result: any, run_id: str):
 
         # split our results and corrections (which are given as a dict) into
         # separate variables
         vasprun = result["result"]
         corrections = result["corrections"]
         directory = result["directory"]
 
@@ -745,15 +868,15 @@
         is the same as `__doc__`. This attribute is only defined for beginners
         to python and for use in django templates for the website interface.
         """
         return cls.__doc__
 
     @classmethod
     @property
-    def parameter_names(cls) -> List[str]:
+    def parameter_names(cls) -> list[str]:
         """
         Gives a list of all the parameter names for this workflow.
         """
         # Iterate through and grab the parameters for the core methods. We also
         # sort parameters alphabetically for consistent results.
         parameters = []
         for method in cls._parameter_methods:
@@ -762,15 +885,15 @@
                 if parameter not in parameters and parameter != "kwargs":
                     parameters += [parameter]
         parameters.sort()
         return parameters
 
     @classmethod
     @property
-    def parameter_names_required(cls) -> List[str]:
+    def parameter_names_required(cls) -> list[str]:
         """
         Gives a list of all the required parameter names for this workflow.
         """
         parameters = []
         for method in cls._parameter_methods:
             sig = inspect.signature(getattr(cls, method))
             for parameter, val in sig.parameters.items():
@@ -817,15 +940,15 @@
 
     # -------------------------------------------------------------------------
     # Properties/method that configure registration of workflow runs and the
     # parameters each is called with.
     # -------------------------------------------------------------------------
 
     @classmethod
-    def _load_input_and_register(cls, run_id: str, **parameters: Any) -> dict:
+    def _load_input_and_register(cls, **parameters: any) -> dict:
         """
         How the input was submitted as a parameter depends on if we are submitting
         to Prefect Cloud, running the flow locally, or even continuing from a
         previous calculation.  Here, we use a task to convert the input to a toolkit
         object and (if requested) provide the directory as well.
 
         For example, a common input parameter for workflows is "structure", which
@@ -941,15 +1064,15 @@
         # "primary_input and" is added to the start to ensure cleaned input exists
         # and therefore prevent an error/bug.
         if source and primary_input and primary_input_cleaned.is_from_past_calc:
             # note primary_input here is a dictionary
             # assert
             if not source == primary_input:
                 # only warning for now because this is experimental
-                logging.warn(
+                logging.warning(
                     "Your source does not match the source of your "
                     "primary input. Sources are an experimental feature, so "
                     "this will not affect your results. Still, please report "
                     "this to our team to help with development. \n\n"
                     f"SOURCE: {source} \n\n"
                     f"PRIMARY_INPUT: {primary_input} \n\n"
                 )
@@ -971,16 +1094,20 @@
             parameters_cleaned["input_parameters"]["source"] = source_cleaned
 
         # ---------------------------------------------------------------------
 
         # STEP 4: Register the calculation so the user can follow along in the UI
         # and also see which structures/runs have been submitted aready.
 
+        parameters_cleaned["run_id"] = (
+            parameters_cleaned.get("run_id", None) or cls._get_run_id()
+        )
+
         if cls.use_database:
-            cls._register_calculation(run_id=run_id, **parameters_cleaned)
+            cls._register_calculation(**parameters_cleaned)
 
         # ---------------------------------------------------------------------
 
         # STEP 5: Write metadata file for user reference
 
         # convert back to json format. We convert back rather than use the original
         # to ensure the input data is all present. For example, we want to store
@@ -993,16 +1120,14 @@
         )
 
         # We want to write a file summarizing the inputs used for this
         # workflow run. This allows future users to reproduce the results if
         # desired -- and it also allows us to load old results into a database.
         input_summary = dict(
             workflow_name=cls.name_full,
-            # this ID is ingored as an input but needed for loading past data
-            run_id=run_id,
             **parameters_serialized,
         )
 
         # now write the summary to file in the same directory as the calc.
         input_summary_filename = directory_cleaned / "simmate_metadata.yaml"
         with input_summary_filename.open("w") as file:
             content = yaml.dump(input_summary)
@@ -1010,25 +1135,37 @@
 
         # ---------------------------------------------------------------------
 
         # Finally we just want to return the dictionary of cleaned parameters
         # to be used by the workflow
         return parameters_cleaned
 
+    @staticmethod
+    def _get_run_id():
+        """
+        Generates a random id to use as a workflow run id.
+
+        This is called automatically within `_load_input_and_register`
+        """
+        # This is a separate method in order to allow the prefect executor to
+        # overwrite this method.
+        unique_id = str(uuid.uuid4())
+        return unique_id
+
     @classmethod
     @property
-    def _parameters_to_register(cls) -> List[str]:
+    def _parameters_to_register(cls) -> list[str]:
         """
         A list of input parameters that should be used to register the calculation.
         """
 
         # run is always used to register but is never an input parameter
         parameters_to_register = []
-        # run_id and workflow_name are used to register but these are
-        # implemented with the _register_calculation elsewhere
+        # workflow_name is also used to register but this implemented within
+        # the _register_calculation method
 
         table_columns = cls.database_table.get_column_names()
 
         for parameter in cls.parameter_names:
             if parameter in table_columns:
                 parameters_to_register.append(parameter)
 
@@ -1038,15 +1175,15 @@
 
         # put in alphabetical order for consistent results
         parameters_to_register.sort()
 
         return parameters_to_register
 
     @classmethod
-    def _register_calculation(cls, run_id=None, **kwargs) -> Calculation:
+    def _register_calculation(cls, **kwargs) -> Calculation:
         """
         If the workflow is linked to a calculation table in the Simmate database,
         this adds the flow run to the database.
 
         Parameters passed should be deserialized and cleaned.
 
         This method should not be called directly as it is used within the
@@ -1077,45 +1214,55 @@
             workflow = cls  # we have the workflow class already
             database_table = cls.database_table
 
         # Registration is only possible if a table is provided. Some
         # special-case workflows don't store calculation information bc the flow
         # is just a quick python analysis.
         if not database_table:
-            logging.warn("No database table found. Skipping registration.")
+            logging.warning("No database table found. Skipping registration.")
             return
 
         # grab the registration kwargs from the parameters provided and then
         # convert them to a python object format for the database method
         register_kwargs = {
             key: kwargs.get(key, None) for key in workflow._parameters_to_register
         }
         register_kwargs_cleaned = cls._deserialize_parameters(
             add_defaults_from_attr=False, **register_kwargs
         )
 
+        # SPECIAL CASE: The exception to the above is with SOURCE, which needs
+        # to be in a JSON-serialized form for the database
+        if "source" in register_kwargs_cleaned:
+            register_kwargs_cleaned["source"] = cls._serialize_parameters(
+                source=kwargs.get("source", None)
+            )["source"]
+            # !!! This is a hacky bug fix that needs refactored
+
         # SPECIAL CASE: for customized workflows we need to convert the inputs
         # back to json before saving to the database.
         if "workflow_base" in register_kwargs_cleaned:
             parameters_serialized = cls._serialize_parameters(**register_kwargs_cleaned)
             calculation = database_table.from_run_context(
-                run_id=run_id,
                 workflow_name=cls.name_full,
                 **parameters_serialized,
             )
         else:
             # load/create the calculation for this workflow run
             calculation = database_table.from_run_context(
-                run_id=run_id,
                 workflow_name=cls.name_full,
                 **register_kwargs_cleaned,
             )
 
         return calculation
 
+    # -------------------------------------------------------------------------
+    # Methods that hanlde serialization and deserialization of input parameters.
+    # -------------------------------------------------------------------------
+
     @classmethod
     def _serialize_parameters(cls, **parameters) -> dict:
         """
         Converts input parameters to json-sealiziable objects that Prefect can
         use.
 
         This method should not be called directly as it is used within the
@@ -1139,23 +1286,31 @@
 
         parameters_serialized = {}
         for parameter_key, parameter_value in parameters.items():
 
             try:
                 json.dumps(parameter_value)
             except TypeError:
-                if hasattr(parameter_value, "as_dict"):
-                    parameter_value = parameter_value.as_dict()
-                elif hasattr(parameter_value, "to_dict"):
-                    parameter_value = parameter_value.to_dict()
-                elif parameter_key == "directory":
-                    parameter_value = str(parameter_value)  # convert Path to str
+
+                # Special cases
+                if parameter_key == "directory":
+                    # convert Path to str
+                    parameter_value = str(parameter_value)
                 elif parameter_key == "source":
                     # recursive call to this function
                     parameter_value = cls._serialize_parameters(**parameter_value)
+                elif parameter_key == "composition":
+                    # convert Composition to str
+                    parameter_value = str(parameter_value)
+
+                # preferred serializiation
+                elif hasattr(parameter_value, "as_dict"):
+                    parameter_value = parameter_value.as_dict()
+                elif hasattr(parameter_value, "to_dict"):
+                    parameter_value = parameter_value.to_dict()
 
                 # workflow_base and input_parameters are special cases that
                 # may require a refactor (for customized workflows)
                 elif parameter_key == "workflow_base":
                     parameter_value = parameter_value.name_full
                 elif parameter_key == "input_parameters":
                     # recursive call to this function
@@ -1172,15 +1327,15 @@
         add_defaults_from_attr: bool = True,
         **parameters,
     ) -> dict:
         """
         converts all parameters to appropriate python objects
         """
 
-        from simmate.toolkit import Structure
+        from simmate.toolkit import Composition, Structure
         from simmate.toolkit.diffusion import MigrationHop, MigrationImages
 
         parameters_cleaned = parameters.copy()
 
         #######
         # SPECIAL CASE: customized workflows have their parameters stored under
         # "input_parameters" instead of the base dict
@@ -1209,22 +1364,30 @@
         # value is set to "None". If it is, then we change to the value set as
         # the class attribute.
         if add_defaults_from_attr:
             for parameter in cls.parameter_names:
                 if parameters.get(parameter, None) == None and hasattr(cls, parameter):
                     parameters_cleaned[parameter] = getattr(cls, parameter)
 
-        # The remaining checks look to intialize input to toolkit objects
+        # The remaining checks look to intialize input to toolkit objects using
+        # the from_dynamic methods.
+        # OPTIMIZE: if I have proper typing and parameter itrospection, I could
+        # potentially grab the from_dynamic method on the fly -- rather than
+        # doing these repeated steps here.
 
         structure = parameters.get("structure", None)
         if structure:
             parameters_cleaned["structure"] = Structure.from_dynamic(structure)
         else:
             parameters_cleaned.pop("structure", None)
 
+        if "composition" in parameters.keys():
+            migration_hop = Composition.from_dynamic(parameters["composition"])
+            parameters_cleaned["composition"] = migration_hop
+
         if "structures" in parameters.keys():
             structure_filenames = parameters["structures"].split(";")
             parameters_cleaned["structures"] = [
                 Structure.from_dynamic(file) for file in structure_filenames
             ]
 
         if "migration_hop" in parameters.keys():
@@ -1249,12 +1412,13 @@
 
         if parameters.get("directory", None):
             parameters_cleaned["directory"] = Path(parameters_cleaned["directory"])
 
         if parameters.get("source", None):
             # !!! are there other types I should account for? Maybe I should just
             # make this a recursive call to catch everything?
-            parameters_cleaned["source"]["directory"] = Path(
-                parameters_cleaned["directory"]
-            )
+            if parameters_cleaned["source"].get("directory", None):
+                parameters_cleaned["source"]["directory"] = Path(
+                    parameters_cleaned["directory"]
+                )
 
         return parameters_cleaned
```

### Comparing `simmate-0.8.0/src/simmate/workflows/README.md` & `simmate-0.9.0/src/simmate/workflows/README.md`

 * *Files identical despite different names*

### Comparing `simmate-0.8.0/src/simmate/workflows/relaxation.py` & `simmate-0.9.0/src/simmate/workflows/relaxation.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 """
 
 # TODO: when I add more calculators, I can do something like this...
 # if "simmate.calculators.Vasp" in installed_apps:
 from simmate.calculators.vasp.workflows.relaxation.all import (
     Relaxation__Vasp__Matproj,
     Relaxation__Vasp__MatprojHse,
-    Relaxation__Vasp__MatprojScan,
     Relaxation__Vasp__MatprojMetal,
+    Relaxation__Vasp__MatprojScan,
     Relaxation__Vasp__Mit,
     Relaxation__Vasp__MvlGrainboundary,
-    Relaxation__Vasp__MvlSlab,
     Relaxation__Vasp__MvlNebEndpoint,
+    Relaxation__Vasp__MvlSlab,
     Relaxation__Vasp__Quality00,
     Relaxation__Vasp__Quality01,
     Relaxation__Vasp__Quality02,
     Relaxation__Vasp__Quality03,
     Relaxation__Vasp__Quality04,
     Relaxation__Vasp__Staged,
 )
```

### Comparing `simmate-0.8.0/src/simmate/workflows/restart.py` & `simmate-0.9.0/src/simmate/workflows/restart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 
-import yaml
 from pathlib import Path
 
-from simmate.workflow_engine import Workflow
+import yaml
+
 from simmate.utilities import copy_directory
+from simmate.workflow_engine import Workflow
 from simmate.workflows.utilities import get_workflow
 
 
 class Restart__Simmate__Automatic(Workflow):
     """
     Given a directory of a incomplete Simmate workflow run, this will use the
     metadata file to restart the calculation.
@@ -21,15 +22,15 @@
     directory_new: path/to/newcalc (optional)
     ```
 
     No other inputs are allowed bc the simmate_metadata.yaml will be used.
     """
 
     @classmethod
-    def run_config(cls, directory_old: Path, directory_new: Path = None):
+    def run_config(cls, directory_old: Path, directory_new: Path = None, **kwargs):
 
         # First copy over the directory
         directory_new_cleaned = copy_directory(directory_old, directory_new)
 
         # grab the metadata file in the new dir
         metadata_filename = directory_new_cleaned / "simmate_metadata.yaml"
         with metadata_filename.open() as file:
```

### Comparing `simmate-0.8.0/src/simmate/workflows/test/test_all_workflow_runs.py` & `simmate-0.9.0/src/simmate/workflows/test/test_all_workflow_runs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # -*- coding: utf-8 -*-
 
 import pytest
 
-from simmate.workflows.utilities import (
-    get_list_of_all_workflows,
-    get_workflow,
-)
+from simmate.workflows.utilities import get_list_of_all_workflows, get_workflow
 
 
 # @pytest.mark.prefect_db
 @pytest.mark.vasp
 @pytest.mark.django_db
 def test_all_workflow_runs(tmp_path, sample_structures):
 
     # For testing, look at the NaCl rocksalt primitive structure
     structure = sample_structures["NaCl_mp-22862_primitive"]
 
     # -------------
     # https://stackoverflow.com/questions/41742317/
-    import os
     import contextlib
+    import os
     from pathlib import Path
 
     @contextlib.contextmanager
     def working_directory(path):
         """Changes working directory and returns to previous on exit."""
         prev_cwd = Path.cwd()
         os.chdir(path)
```

### Comparing `simmate-0.8.0/src/simmate/workflows/test/test_workflows_utilities.py` & `simmate-0.9.0/src/simmate/workflows/test/test_workflows_utilities.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # -*- coding: utf-8 -*-
 
 import pytest
 
 from simmate.conftest import copy_test_files
 from simmate.workflows.utilities import (
-    get_workflow_types,
     get_list_of_all_workflows,
     get_list_of_workflows_by_type,
+    get_unique_parameters,
     get_workflow,
+    get_workflow_types,
     load_results_from_directories,
-    get_unique_parameters,
 )
 
 
 def test_get_workflow_types():
     assert get_workflow_types() == [
         "customized",
         "diffusion",
         "dynamics",
         "electronic-structure",
         "population-analysis",
         "relaxation",
         "restart",
         "static-energy",
+        "structure-prediction",
     ]
 
 
 def test_list_of_all_workflows():
 
     assert get_list_of_all_workflows() == [
         "customized.vasp.user-config",
@@ -59,14 +60,16 @@
         "restart.simmate.automatic",
         "static-energy.vasp.matproj",
         "static-energy.vasp.matproj-hse",
         "static-energy.vasp.matproj-scan",
         "static-energy.vasp.mit",
         "static-energy.vasp.mvl-neb-endpoint",
         "static-energy.vasp.quality04",
+        "structure-prediction.python.fixed-composition",
+        "structure-prediction.python.new-individual",
     ]
 
 
 def test_list_of_workflows_by_type():
 
     assert get_list_of_workflows_by_type("static-energy") == [
         "static-energy.vasp.matproj",
@@ -79,51 +82,68 @@
 
     with pytest.raises(TypeError):
         get_list_of_workflows_by_type("non-existant-type")
 
 
 def test_get_workflow():
 
-    from simmate.workflows.static_energy import (
-        StaticEnergy__Vasp__Matproj as workflow,
-    )
+    from simmate.workflows.static_energy import StaticEnergy__Vasp__Matproj as workflow
 
     assert get_workflow("static-energy.vasp.matproj") == workflow
 
 
 def test_get_unique_paramters():
     assert get_unique_parameters() == [
         "command",
+        "composition",
         "compress_output",
         "copy_previous_directory",
         "diffusion_analysis_id",
         "directory",
         "directory_new",
         "directory_old",
+        "fitness_field",
         "input_parameters",
         "is_restart",
+        "limit_best_survival",
         "max_atoms",
+        "max_structures",
         "migrating_specie",
         "migration_hop",
         "migration_hop_id",
         "migration_images",
         "min_atoms",
         "min_length",
+        "nfirst_generation",
         "nimages",
+        "nsteadystate",
         "nsteps",
         "pre_sanitize_structure",
         "pre_standardize_structure",
+        "run_id",
+        "search_id",
+        "selector_kwargs",
+        "selector_name",
+        "singleshot_sources",
+        "sleep_step",
         "source",
+        "steadystate_sources",
         "structure",
+        "structure_source_id",
+        "subworkflow_kwargs",
+        "subworkflow_name",
         "supercell_end",
         "supercell_start",
+        "tags",
         "temperature_end",
         "temperature_start",
         "time_step",
         "updated_settings",
+        "validator_kwargs",
+        "validator_name",
         "workflow_base",
     ]
 
 
 @pytest.mark.django_db
 def test_load_results_from_directories(tmp_path):
```

### Comparing `simmate-0.8.0/src/simmate/workflows/utilities.py` & `simmate-0.9.0/src/simmate/workflows/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 """
 This module hosts common utilities for Simmate's workflow library. This includes
 functions for grabbing all available workflows as well as dynamically loading
 a workflow using its name.
 """
 
-import yaml
-import shutil
+import logging
 import pkgutil
-from typing import List, Union
+import shutil
 from importlib import import_module
 from pathlib import Path
-import logging
+
+import yaml
 
 from simmate import workflows
 from simmate.utilities import get_directory, make_archive
 from simmate.workflow_engine import Workflow
 
 
 def get_workflow_types():
@@ -38,15 +38,15 @@
 
     return workflow_types
 
 
 def get_list_of_workflows_by_type(
     flow_type: str,
     full_name: bool = True,
-) -> List[str]:
+) -> list[str]:
     """
     Returns a list of all the workflows located in the given module.
     """
 
     # Make sure the type is supported
     workflow_types = get_workflow_types()
     if flow_type not in workflow_types:
@@ -78,15 +78,15 @@
             workflow_names.append(workflow_name)
     # OPTIMIZE: is there a more efficient way to do this?
 
     workflow_names.sort()
     return workflow_names
 
 
-def get_list_of_all_workflows() -> List[str]:
+def get_list_of_all_workflows() -> list[str]:
     """
     Returns a list of all the workflows of all types.
 
     This utility was make specifically for the CLI where we print out all
     workflow names for the user.
     """
 
@@ -188,15 +188,15 @@
 
     # and import the workflow
     workflow = getattr(workflow_module, workflow_class_name)
 
     return workflow
 
 
-def load_results_from_directories(base_directory: Union[str, Path] = "."):
+def load_results_from_directories(base_directory: Path | str = "."):
     """
     Goes through a given directory and finds all "simmate-task-" folders and zip
     archives present. The simmate_metadata.yaml file is used in each of these
     to load results into the database. All folders will be converted to archives
     once they've been loaded.
 
     #### Parameters
@@ -262,18 +262,18 @@
             # Now save the results and convert the folder to an archive
             results_db.save()
             make_archive(foldername)
 
             logging.info("Successfully loaded into database.")
 
         except:
-            logging.warn("Failed to load into database")
+            logging.warning("Failed to load into database")
 
 
-def get_unique_parameters() -> List[str]:
+def get_unique_parameters() -> list[str]:
     """
     Returns a list of all unique parameter names accross all workflows.
 
     This utility is really just to help developers ensure they are covering
     all cases when implementing new features, so this function isn't actually
     called elsewhere.
     """
```

### Comparing `simmate-0.8.0/src/simmate.egg-info/PKG-INFO` & `simmate-0.9.0/src/simmate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simmate
-Version: 0.8.0
+Version: 0.9.0
 Summary: Simmate is a toolbox for computational materials research.
 Author-email: "Jack D. Sundberg" <jacksund@live.unc.edu>
 License: BSD 3-Clause License
 Project-URL: homepage, https://simmate.org/
 Project-URL: repository, https://github.com/jacksund/simmate
 Project-URL: documentation, https://jacksund.github.io/simmate/simmate.html
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `simmate-0.8.0/src/simmate.egg-info/SOURCES.txt` & `simmate-0.9.0/src/simmate.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,15 @@
 src/simmate/calculators/vasp/workflows/test/test_pymatgen_sets.py
 src/simmate/command_line/README.md
 src/simmate/command_line/__init__.py
 src/simmate/command_line/base_command.py
 src/simmate/command_line/database.py
 src/simmate/command_line/run_server.py
 src/simmate/command_line/start_project.py
+src/simmate/command_line/utilities.py
 src/simmate/command_line/workflow_engine.py
 src/simmate/command_line/workflow_engine_prefect.py
 src/simmate/command_line/workflows.py
 src/simmate/command_line/test/test_base_command.py
 src/simmate/command_line/test/test_database_cli.py
 src/simmate/command_line/test/test_worker_cli.py
 src/simmate/command_line/test/test_workflows_cli.py
@@ -323,19 +324,24 @@
 src/simmate/toolkit/diffusion/migration_images.py
 src/simmate/toolkit/structure_prediction/__init__.py
 src/simmate/toolkit/structure_prediction/known.py
 src/simmate/toolkit/structure_prediction/prototypes.py
 src/simmate/toolkit/structure_prediction/substitution.py
 src/simmate/toolkit/structure_prediction/evolution/README.md
 src/simmate/toolkit/structure_prediction/evolution/__init__.py
-src/simmate/toolkit/structure_prediction/evolution/database.py
-src/simmate/toolkit/structure_prediction/evolution/search_engine.py
 src/simmate/toolkit/structure_prediction/evolution/selectors.py
 src/simmate/toolkit/structure_prediction/evolution/stop_conditions.py
 src/simmate/toolkit/structure_prediction/evolution/triggered_actions.py
+src/simmate/toolkit/structure_prediction/evolution/database/__init__.py
+src/simmate/toolkit/structure_prediction/evolution/database/evolutionary_search.py
+src/simmate/toolkit/structure_prediction/evolution/database/structure_source.py
+src/simmate/toolkit/structure_prediction/evolution/workflows/__init__.py
+src/simmate/toolkit/structure_prediction/evolution/workflows/all.py
+src/simmate/toolkit/structure_prediction/evolution/workflows/fixed_composition.py
+src/simmate/toolkit/structure_prediction/evolution/workflows/new_individual.py
 src/simmate/toolkit/symmetry/__init__.py
 src/simmate/toolkit/symmetry/asymdata.csv
 src/simmate/toolkit/symmetry/wyckoff.py
 src/simmate/toolkit/symmetry/wyckoffdata.csv
 src/simmate/toolkit/symmetry/webscraper/aflow.py
 src/simmate/toolkit/symmetry/webscraper/bilbao_wyckoff.py
 src/simmate/toolkit/symmetry/webscraper/itc_datascrape.py
@@ -362,14 +368,15 @@
 src/simmate/toolkit/validators/fingerprint/pcrystalnn.py
 src/simmate/toolkit/validators/fingerprint/_to_do/ase.py
 src/simmate/toolkit/validators/fingerprint/_to_do/crystalnn.py
 src/simmate/toolkit/validators/fingerprint/_to_do/prdf.py
 src/simmate/toolkit/validators/fingerprint/_to_do/rdf.py
 src/simmate/utilities/README.md
 src/simmate/utilities/__init__.py
+src/simmate/utilities/_dev_logging.py
 src/simmate/utilities/async_wrapper.py
 src/simmate/utilities/files.py
 src/simmate/utilities/other.py
 src/simmate/utilities/test/test_files.py
 src/simmate/visualization/README.md
 src/simmate/visualization/__init__.py
 src/simmate/visualization/structure/__init__.py
@@ -514,14 +521,15 @@
 src/simmate/workflow_engine/utilities.py
 src/simmate/workflow_engine/workflow.py
 src/simmate/workflow_engine/execution/README.md
 src/simmate/workflow_engine/execution/__init__.py
 src/simmate/workflow_engine/execution/database.py
 src/simmate/workflow_engine/execution/executor.py
 src/simmate/workflow_engine/execution/future.py
+src/simmate/workflow_engine/execution/utilities.py
 src/simmate/workflow_engine/execution/worker.py
 src/simmate/workflow_engine/execution_prefect/__init__.py
 src/simmate/workflow_engine/execution_prefect/worker.py
 src/simmate/workflow_engine/execution_prefect/workflow.py
 src/simmate/workflow_engine/test/test_error_handler.py
 src/simmate/workflow_engine/test/test_s3_workflow.py
 src/simmate/workflow_engine/test/test_workflow.py
@@ -531,11 +539,12 @@
 src/simmate/workflows/diffusion.py
 src/simmate/workflows/dynamics.py
 src/simmate/workflows/electronic_structure.py
 src/simmate/workflows/population_analysis.py
 src/simmate/workflows/relaxation.py
 src/simmate/workflows/restart.py
 src/simmate/workflows/static_energy.py
+src/simmate/workflows/structure_prediction.py
 src/simmate/workflows/utilities.py
 src/simmate/workflows/test/test_all_workflow_runs.py
 src/simmate/workflows/test/test_workflows_utilities.py
 src/simmate/workflows/test/simmate-task-ERROR/simmate_metadata.yaml
```

### Comparing `simmate-0.8.0/src/simmate.egg-info/requires.txt` & `simmate-0.9.0/src/simmate.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -18,10 +18,11 @@
 nest_asyncio<=1.5.5,>=1.5.5
 pytest<7.1,>=6.2.5
 pytest-django<=4.5.2,>=4.5.2
 pytest-mock<=3.8.2,>=3.7.0
 pytest-xdist<=2.5.0,>=2.5.0
 black<=22.6.0,>=22.1.0
 coverage<=6.4.3,>=6.2
+isort<=5.10.1,>=5.10.1
 pymatgen<=2022.7.25,>=2022.1.9
 pymatgen-analysis-diffusion<=2022.7.21,>=2021.4.29
 matminer<=0.7.8,>=0.7.6
```

