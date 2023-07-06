# Comparing `tmp/pyiron-atomistics-0.3.0.tar.gz` & `tmp/pyiron-atomistics-0.3.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron-atomistics-0.3.0.tar", last modified: Thu Jun  8 01:10:49 2023, max compression
+gzip compressed data, was "pyiron-atomistics-0.3.0.dev0.tar", last modified: Thu Jul  6 07:54:58 2023, max compression
```

## Comparing `pyiron-atomistics-0.3.0.tar` & `pyiron-atomistics-0.3.0.dev0.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.546330 pyiron-atomistics-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-08 01:10:49.546330 pyiron-atomistics-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.546330 pyiron-atomistics-0.3.0/pyiron_atomistics/
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-08 01:10:49.546330 pyiron-atomistics-0.3.0/pyiron_atomistics/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.530330 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.530330 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/generic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/generic/object_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.530330 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41928 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/atomistic.py
--rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/interactivewrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/potentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/structurecontainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.530330 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/convergence_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    23340 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/elastic.py
--rw-r--r--   0 runner    (1001) docker     (123)    32931 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/murnaghan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    21280 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/quasi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/sqsmaster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.534330 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16778 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/analyse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/atom.py
--rw-r--r--   0 runner    (1001) docker     (123)   128325 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/atoms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.534330 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/aimsgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/ase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/atomsk.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/compound.py
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/materialsproject.py
--rw-r--r--   0 runner    (1001) docker     (123)    20288 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/has_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16196 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/periodic_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/phonopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/pyironase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/pyscal.py
--rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/sparse_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    20264 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/structurestorage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.534330 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/thermodynamics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/thermodynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.534330 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/volumetric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/volumetric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/volumetric/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.534330 pyiron-atomistics-0.3.0/pyiron_atomistics/calphy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/calphy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34986 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/calphy/job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.538330 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/bader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.538330 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/job/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18570 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/job/generic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.538330 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/master/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/master/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/master/convergence_encut_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/master/convergence_encut_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/master/murnaghan_dft.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.538330 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/waves/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/waves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/waves/bandstructure.py
--rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/waves/dos.py
--rw-r--r--   0 runner    (1001) docker     (123)    29606 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/dft/waves/electronic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.538330 pyiron-atomistics-0.3.0/pyiron_atomistics/gpaw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/gpaw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/gpaw/gpaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/gpaw/pyiron_ase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.538330 pyiron-atomistics-0.3.0/pyiron_atomistics/interactive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/interactive/activation_relaxation_technique.py
--rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/interactive/quasi_newton.py
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/interactive/scipy_minimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/interactive/sxextoptint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.538330 pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44523 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    41465 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    33649 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/lammps.py
--rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/potential.py
--rw-r--r--   0 runner    (1001) docker     (123)    25776 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    26176 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.542330 pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    99408 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/sphinx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/volumetric_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.542330 pyiron-atomistics-0.3.0/pyiron_atomistics/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/table/datamining.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/table/funct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.542330 pyiron-atomistics-0.3.0/pyiron_atomistics/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/testing/executable.py
--rw-r--r--   0 runner    (1001) docker     (123)    19469 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/testing/randomatomistic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.542330 pyiron-atomistics-0.3.0/pyiron_atomistics/thermodynamics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/thermodynamics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/thermodynamics/hessian.py
--rw-r--r--   0 runner    (1001) docker     (123)    51129 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/thermodynamics/interfacemethod.py
--rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/thermodynamics/sxphonons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.546330 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   101289 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14988 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)    13769 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/metadyn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/oszicar.py
--rw-r--r--   0 runner    (1001) docker     (123)    45257 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/outcar.py
--rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/procar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    15487 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/vasp.py
--rw-r--r--   0 runner    (1001) docker     (123)    34363 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/vasprun.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/vaspsol.py
--rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/volumetric_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.530330 pyiron-atomistics-0.3.0/pyiron_atomistics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-08 01:10:49.000000 pyiron-atomistics-0.3.0/pyiron_atomistics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-08 01:10:49.000000 pyiron-atomistics-0.3.0/pyiron_atomistics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 01:10:49.000000 pyiron-atomistics-0.3.0/pyiron_atomistics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-08 01:10:49.000000 pyiron-atomistics-0.3.0/pyiron_atomistics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 01:10:49.000000 pyiron-atomistics-0.3.0/pyiron_atomistics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-08 01:10:49.546330 pyiron-atomistics-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-08 01:10:49.000000 pyiron-atomistics-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:10:49.546330 pyiron-atomistics-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/tests/test_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-08 01:10:46.000000 pyiron-atomistics-0.3.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.608847 pyiron-atomistics-0.3.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 07:54:58.608847 pyiron-atomistics-0.3.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.608847 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-06 07:54:58.608847 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.588846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.588846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/generic/object_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.588846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41928 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/atomistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20826 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/interactivewrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/potentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/structurecontainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.592846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/convergence_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23340 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32965 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/murnaghan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21280 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/quasi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/sqsmaster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.596846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16778 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)   128325 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/atoms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.596846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/aimsgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/ase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7550 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/atomsk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/materialsproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20288 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/has_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16196 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/periodic_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/phonopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/pyironase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/pyscal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18506 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/sparse_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22405 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/structurestorage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.596846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/thermodynamics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/thermodynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12234 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.596846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/volumetric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/volumetric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17033 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/volumetric/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.596846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/calphy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/calphy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34986 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/calphy/job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.596846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/bader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.596846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/job/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18570 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/job/generic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.596846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/master/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/master/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/master/convergence_encut_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/master/convergence_encut_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/master/murnaghan_dft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.600846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/waves/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/waves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/waves/bandstructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/waves/dos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29606 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/waves/electronic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.600846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/gpaw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/gpaw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/gpaw/gpaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/gpaw/pyiron_ase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.600846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/interactive/activation_relaxation_technique.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/interactive/quasi_newton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/interactive/scipy_minimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/interactive/sxextoptint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.600846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44523 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41465 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33649 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/lammps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15230 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25776 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26176 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.604847 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99408 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15905 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/volumetric_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.604847 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/table/datamining.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/table/funct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.604847 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/testing/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19469 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/testing/randomatomistic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.604847 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/thermodynamics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/thermodynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/thermodynamics/hessian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51129 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/thermodynamics/interfacemethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18302 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/thermodynamics/sxphonons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.608847 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101289 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14995 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13769 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/metadyn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/oszicar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45257 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/outcar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/procar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15487 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34363 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/vasprun.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/vaspsol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12372 2023-07-06 07:54:54.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/volumetric_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.588846 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-06 07:54:58.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-06 07:54:58.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:54:58.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-06 07:54:58.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-06 07:54:58.000000 pyiron-atomistics-0.3.0.dev0/pyiron_atomistics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-06 07:54:58.608847 pyiron-atomistics-0.3.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-06 07:54:58.000000 pyiron-atomistics-0.3.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:54:58.608847 pyiron-atomistics-0.3.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-06 07:54:55.000000 pyiron-atomistics-0.3.0.dev0/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-06 07:54:55.000000 pyiron-atomistics-0.3.0.dev0/tests/test_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-06 07:54:55.000000 pyiron-atomistics-0.3.0.dev0/versioneer.py
```

### Comparing `pyiron-atomistics-0.3.0/LICENSE` & `pyiron-atomistics-0.3.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/PKG-INFO` & `pyiron-atomistics-0.3.0.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron-atomistics
-Version: 0.3.0
+Version: 0.3.0.dev0
 Summary: pyiron - an integrated development environment (IDE) for computational materials science.
 Home-page: https://github.com/pyiron/pyiron_atomistics
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyiron-atomistics-0.3.0/README.rst` & `pyiron-atomistics-0.3.0.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/__init__.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/_tests.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,8 +52,8 @@
 
 class TestWithCleanProject(TestWithProject, ABC):
     """
     Tests that start and remove a project for their suite, and remove jobs from the project for each test.
     """
 
     def tearDown(self):
-        self.project.remove_jobs_silently(recursive=True)
+        self.project.remove_jobs(recursive=True, silently=True)
```

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/generic/object_type.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/generic/object_type.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/atomistic.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/atomistic.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/interactive.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/interactivewrapper.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/interactivewrapper.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/potentials.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/potentials.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/sqs.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/sqs.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/job/structurecontainer.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/job/structurecontainer.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/convergence_volume.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/convergence_volume.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/elastic.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/elastic.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/murnaghan.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/murnaghan.py`

 * *Files 0% similar despite different names*

```diff
@@ -861,17 +861,17 @@
 
         Returns:
             ax: The axis plotted onto
 
         Raises:
             ValueError: if job is not finished when calling this method
         """
-        if not self.status.finished:
+        if not (self.status.finished or self.status.not_converged):
             raise ValueError(
-                "Job must be successfully run, before calling this method."
+                "Job must have finished executing before calling this method."
             )
 
         if ax is None:
             ax = plt.subplot(111)
         else:
             plt_show = False
         if not self.fit_dict:
```

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/parallel.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/phonopy.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/phonopy.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/quasi.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/quasi.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/serial.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/serial.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/sqsmaster.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/sqsmaster.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/master/structure.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/master/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/analyse.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/analyse.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/atom.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/atom.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/atoms.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/atoms.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/aimsgb.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/aimsgb.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/ase.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/ase.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/atomsk.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/atomsk.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/compound.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/compound.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factories/materialsproject.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factories/materialsproject.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/factory.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/factory.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/has_structure.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/has_structure.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/neighbors.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/neighbors.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/periodic_table.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/periodic_table.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/phonopy.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/phonopy.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/pyironase.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/pyironase.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/pyscal.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/pyscal.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/sparse_list.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/sparse_list.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/structure/structurestorage.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/structure/structurestorage.py`

 * *Files 7% similar despite different names*

```diff
@@ -278,14 +278,26 @@
     """
 
     @seaborn_alarm
     def __init__(self, store: StructureStorage):
         self._store = store
         self._neigh = None
 
+    def atoms(self):
+        """
+        Plot a histogram of the number of atoms in each structure.
+        """
+        length = self._store["length"]
+        lo = length.min()
+        hi = length.max()
+        # make the bins fall in between whole numbers and include hi
+        plt.hist(length, bins=np.arange(lo, hi + 2) - 0.5)
+        plt.xlabel("#Atoms")
+        plt.ylabel("Count")
+
     def cell(self, angle_in_degrees=True):
         """
         Plot histograms of cell parameters.
 
         Plotted are atomic volume, density, cell vector lengths and cell vector angles in separate subplots all on a
         log-scale.
 
@@ -505,29 +517,46 @@
             label=[f"{i}." for i in range(1, num_shells + 1)],
         )
         plt.xticks(ticks)
         plt.xlabel("Number of Neighbors")
         plt.legend(title="Shell")
         plt.title("Neighbor Coordination in Shells")
 
-    def distances(self, bins=50, num_neighbors=None):
+    def distances(
+        self,
+        bins: int = 50,
+        num_neighbors: int = None,
+        normalize: bool = False,
+    ):
         """
         Plot a histogram of the neighbor distances.
 
+        Setting `normalize` plots the radial distribution function.
+
         Args:
             bins (int): number of bins
             num_neighbors (int): maximum number of neighbors to calculate, when 'shells' or 'distances' are not defined in storage
                                  default is the value from the previous call or 36
+            normalize (bool): normalize the distribution by the surface area of
+                              the radial bin, 4pi r^2
         """
         neigh = self._calc_neighbors(num_neighbors=num_neighbors)
-        distances = neigh["distances"]
+        distances = neigh["distances"].flatten()
 
-        plt.hist(distances.flatten(), bins=bins)
-        plt.xlabel(r"Distance [$\AA$]")
-        plt.ylabel("Neighbor count")
+        if normalize:
+            plt.hist(
+                distances,
+                bins=bins,
+                weights=1 / (4 * np.pi * distances**2),
+            )
+            plt.ylabel("Neighbor density [$\mathrm{\AA}^{-2}$]")
+        else:
+            plt.hist(distances, bins=bins)
+            plt.ylabel("Neighbor count")
+        plt.xlabel(r"Distance [$\mathrm{\AA}$]")
 
     def shell_distances(self, num_shells=4, num_neighbors=None):
         """
         Plot a violin plot of the neighbor distances in shells up to `num_shells`.
 
         Args:
             num_shells (int): maximum shell to plot
@@ -542,7 +571,42 @@
         S = shells.ravel()
         d = pd.DataFrame(
             {"distance": R[S < num_shells + 1], "shells": S[S < num_shells + 1]}
         )
         sns.violinplot(y=d.shells, x=d.distance, scale="width", orient="h")
         plt.xlabel(r"Distance [$\AA$]")
         plt.ylabel("Shell")
+
+    def concentration(self, elements: List[str] = None, **kwargs) -> pd.DataFrame:
+        """
+        Plot histograms of the concentrations in each structure.
+
+        Args:
+            elements (list of str): elements to plot the histograms for; default is for all elements in the container
+            **kwargs: passed through to `seaborn.histplot`
+
+        Returns:
+            `pandas.DataFrame`: table of concentrations in each structure; column headers are the element names
+        """
+        if elements is not None:
+            for elem in elements:
+                if elem not in self._store.get_elements():
+                    raise ValueError(f"Element {elem} not present in storage!")
+        else:
+            elements = self._store.get_elements()
+
+        df = pd.DataFrame(
+            [
+                {elem: sum(elem == sym) / len(sym) for elem in elements}
+                for sym in self._store.get_array_ragged("symbols")
+            ]
+        )
+
+        sns.histplot(
+            data=df.melt(var_name="element", value_name="concentration"),
+            x="concentration",
+            hue="element",
+            multiple="dodge",
+            **kwargs,
+        )
+
+        return df
```

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/thermodynamics/thermo_bulk.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/atomistics/volumetric/generic.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/atomistics/volumetric/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/calphy/job.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/calphy/job.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/dft/bader.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/bader.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/dft/job/generic.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/job/generic.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/dft/master/convergence_encut_parallel.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/master/convergence_encut_parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/dft/master/convergence_encut_serial.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/master/convergence_encut_serial.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/master/convergence_kpoint_parallel.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/dft/master/murnaghan_dft.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/master/murnaghan_dft.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/dft/waves/bandstructure.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/waves/bandstructure.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/dft/waves/dos.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/waves/dos.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/dft/waves/electronic.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/dft/waves/electronic.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/gpaw/gpaw.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/gpaw/gpaw.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/gpaw/pyiron_ase.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/gpaw/pyiron_ase.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 # coding: utf-8
 # Copyright (c) Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 # Distributed under the terms of "New BSD License", see the LICENSE file.
 
-from ase.constraints import dict2constraint
-import copy
-import importlib
 import numpy as np
 from pyiron_atomistics.atomistics.job.interactive import GenericInteractive
 from pyiron_atomistics.atomistics.structure.atoms import Atoms
 
 try:
     from ase.cell import Cell
 except ImportError:
@@ -46,33 +43,39 @@
         pre_run_mode = self.server.run_mode
         self.server.run_mode.interactive = True
         self.run_if_interactive()
         self.interactive_close()
         self.server.run_mode = pre_run_mode
 
     def run_if_interactive(self):
-        if self.structure.calc is None:
-            self.set_calculator()
+        self._ensure_structure_calc_is_set()
         super(AseJob, self).run_if_interactive()
         self.interactive_collect()
 
+    def _ensure_structure_calc_is_set(self):
+        if self.structure.calc is None:
+            self.set_calculator()
+
     def set_calculator(self):
         raise NotImplementedError(
-            "The _set_calculator function is not implemented for this code."
+            "The set_calculator function is not implemented for this code. Either set "
+            "an ase calculator to the structure attribute, or subclass this job and "
+            "define set_calculator."
         )
 
     def interactive_structure_setter(self, structure):
         self.structure.calc.calculate(structure)
 
     def interactive_positions_setter(self, positions):
         self.structure.positions = positions
 
     def interactive_initialize_interface(self):
         self.status.running = True
-        self._structure.calc.set_label(self.working_directory + "/")
+        self._ensure_structure_calc_is_set()
+        self.structure.calc.set_label(self.working_directory + "/")
         self._interactive_library = True
 
     def interactive_close(self):
         if self.interactive_is_activated():
             super(AseJob, self).interactive_close()
             with self.project_hdf5.open("output") as h5:
                 if "interactive" in h5.list_groups():
```

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/interactive/activation_relaxation_technique.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/interactive/activation_relaxation_technique.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/interactive/quasi_newton.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/interactive/quasi_newton.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/interactive/scipy_minimizer.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/interactive/scipy_minimizer.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/interactive/sxextoptint.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/interactive/sxextoptint.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/base.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/base.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/control.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/control.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/interactive.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/lammps.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/lammps.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/output.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/output.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/potential.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/structure.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/lammps/units.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/lammps/units.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/project.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/project.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/base.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/base.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/interactive.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/interactive.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/potential.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/sphinx.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/sphinx.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/structure.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/util.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/util.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/sphinx/volumetric_data.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/sphinx/volumetric_data.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/table/datamining.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/table/datamining.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/table/funct.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/table/funct.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/testing/executable.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/testing/executable.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/testing/randomatomistic.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/testing/randomatomistic.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/thermodynamics/hessian.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/thermodynamics/hessian.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/thermodynamics/interfacemethod.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/thermodynamics/interfacemethod.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/thermodynamics/sxphonons.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/thermodynamics/sxphonons.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/toolkit.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/base.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/base.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/interactive.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/interactive.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,15 @@
 
     def _run_if_new(self, debug=False):
         if (
             self.server.run_mode.interactive
             or self.server.run_mode.interactive_non_modal
         ):
             self.interactive_prepare()
-        super(VaspInteractive, self)._run_if_new(debug=debug)
+        return super(VaspInteractive, self)._run_if_new(debug=debug)
 
     def interactive_prepare(self):
         """
         Modifies/adds tags in the INCAR file that make it possible to run VASP interactively
         """
         self._check_incar_parameter(parameter="INTERACTIVE", value=True)
         self._check_incar_parameter(parameter="IBRION", value=-1)
```

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/metadyn.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/metadyn.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/oszicar.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/oszicar.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/outcar.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/outcar.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/potential.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/potential.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/procar.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/procar.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/report.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/report.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/structure.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/structure.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/vasp.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/vasp.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/vasprun.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/vasprun.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/vaspsol.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/vaspsol.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics/vasp/volumetric_data.py` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics/vasp/volumetric_data.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics.egg-info/PKG-INFO` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron-atomistics
-Version: 0.3.0
+Version: 0.3.0.dev0
 Summary: pyiron - an integrated development environment (IDE) for computational materials science.
 Home-page: https://github.com/pyiron/pyiron_atomistics
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyiron-atomistics-0.3.0/pyiron_atomistics.egg-info/SOURCES.txt` & `pyiron-atomistics-0.3.0.dev0/pyiron_atomistics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/setup.py` & `pyiron-atomistics-0.3.0.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,26 +40,26 @@
         "*test_benchmarks*", 
         "*test_integration*", 
         "*.github*"
     ]),
     install_requires=[
         'ase>=3.22.1',
         'defusedxml>=0.7.1',
-        'h5py>=3.8.0',
+        'h5py>=3.9.0',
         'matplotlib>=3.7.1',
-        'mendeleev>=0.13.1',
+        'mendeleev>=0.14.0',
         'mp-api>=0.33.3',
         'numpy>=1.24.3',
-        'pandas>=2.0.2',
-        'phonopy>=2.19.1',
+        'pandas>=2.0.3',
+        'phonopy>=2.20.0',
         'pint>=0.22',
-        'pyiron_base>=0.6.0',
-        'pymatgen>=2023.5.31',
-        'scipy>=1.10.1',
+        'pyiron_base>=0.6.1',
+        'pymatgen>=2023.6.28',
+        'scipy>=1.11.1',
         'seekpath>=2.1.0',
-        'scikit-learn>=1.2.2',
+        'scikit-learn>=1.3.0',
         'spglib>=2.0.2',
-        'structuretoolkit>=0.0.3'
+        'structuretoolkit>=0.0.5'
     ],
     cmdclass=versioneer.get_cmdclass(),
 
     )
```

### Comparing `pyiron-atomistics-0.3.0/tests/test_project.py` & `pyiron-atomistics-0.3.0.dev0/tests/test_project.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,21 +21,21 @@
     def tearDownClass(cls):
         cls.execution_path = os.path.dirname(os.path.abspath(__file__))
         project = Project(os.path.join(cls.execution_path, "test_project"))
         project.remove_jobs(recursive=True, silently=True)
         project.remove(enable=True)
 
     def test_structure_creation(self):
-        self.assertIsInstance(self.project.create_ase_bulk("Al"), Atoms)
-        surface = self.project.create_surface("Al", "fcc111", size=(4, 4, 4), vacuum=10)
+        self.assertIsInstance(self.project.create.structure.ase.bulk("Al"), Atoms)
+        surface = self.project.create.structure.surface("Al", "fcc111", size=(4, 4, 4), vacuum=10)
         self.assertTrue(all(surface.pbc))
         self.assertIsInstance(surface, Atoms)
-        surface = self.project.create_surface("Al", "fcc111", size=(4, 4, 4), vacuum=10, pbc=[True, True, False])
+        surface = self.project.create.structure.surface("Al", "fcc111", size=(4, 4, 4), vacuum=10, pbc=[True, True, False])
         self.assertFalse(all(surface.pbc))
-        self.assertIsInstance(self.project.create_structure("Al", "fcc", 4.05), Atoms)
+        self.assertIsInstance(self.project.create.structure.ase.bulk("Al", a=4.05), Atoms)
 
     def test_remove_jobs(self):
         sample_job = self.project.create_job("ScriptJob", "Sample")
         sample_job.save()
         with unittest.mock.patch('builtins.input', return_value="n"):
             self.project.remove_jobs(recursive=True)
         self.assertEqual(len(self.project.list_nodes()), 1)
```

### Comparing `pyiron-atomistics-0.3.0/tests/test_toolkit.py` & `pyiron-atomistics-0.3.0.dev0/tests/test_toolkit.py`

 * *Files identical despite different names*

### Comparing `pyiron-atomistics-0.3.0/versioneer.py` & `pyiron-atomistics-0.3.0.dev0/versioneer.py`

 * *Files identical despite different names*

