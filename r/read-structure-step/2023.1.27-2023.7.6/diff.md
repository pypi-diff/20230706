# Comparing `tmp/read_structure_step-2023.1.27.tar.gz` & `tmp/read_structure_step-2023.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "read_structure_step-2023.1.27.tar", last modified: Fri Jan 27 20:09:39 2023, max compression
+gzip compressed data, was "read_structure_step-2023.7.6.tar", last modified: Thu Jul  6 20:21:36 2023, max compression
```

## Comparing `read_structure_step-2023.1.27.tar` & `read_structure_step-2023.7.6.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:09:39.805123 read_structure_step-2023.1.27/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-01-27 20:09:39.805123 read_structure_step-2023.1.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:09:39.789123 read_structure_step-2023.1.27/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:09:39.793123 read_structure_step-2023.1.27/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/_static/SEAMM inverted.png
--rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/_static/SEAMM logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/_static/molssi_main_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/_static/molssi_main_logo_inverted_white.png
--rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/_static/molssi_square.png
--rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/_static/nsf.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:09:39.793123 read_structure_step-2023.1.27/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/api/read_structure_step.formats.cif.rst
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/api/read_structure_step.formats.mol2.rst
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/api/read_structure_step.formats.mop.rst
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/api/read_structure_step.formats.openbabel_io.rst
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/api/read_structure_step.formats.rst
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/api/read_structure_step.formats.sdf.rst
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/api/read_structure_step.formats.smi.rst
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/api/read_structure_step.formats.xyz.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     9623 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:09:39.793123 read_structure_step-2023.1.27/docs/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/developer_guide/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/developer_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/developer_guide/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:09:39.793123 read_structure_step-2023.1.27/docs/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)   434049 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/getting_started/dialog.png
--rw-r--r--   0 runner    (1001) docker     (123)   121911 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/getting_started/flowchart.png
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:09:39.793123 read_structure_step-2023.1.27/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/docs/user_guide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:09:39.805123 read_structure_step-2023.1.27/read_structure_step/
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-01-27 20:09:39.805123 read_structure_step-2023.1.27/read_structure_step/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:09:39.797123 read_structure_step-2023.1.27/read_structure_step/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/data/references.bib
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:09:39.797123 read_structure_step-2023.1.27/read_structure_step/formats/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/formats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:09:39.797123 read_structure_step-2023.1.27/read_structure_step/formats/cif/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/formats/cif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/formats/cif/cif.py
--rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/formats/cif/mmcif.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:09:39.797123 read_structure_step-2023.1.27/read_structure_step/formats/mol2/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/formats/mol2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/formats/mol2/mol2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:09:39.797123 read_structure_step-2023.1.27/read_structure_step/formats/mop/
--rw-r--r--   0 runner    (1001) docker     (123)     4280 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/formats/mop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/formats/mop/find_mopac.py
--rw-r--r--   0 runner    (1001) docker     (123)    22956 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/formats/mop/obabel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:09:39.797123 read_structure_step-2023.1.27/read_structure_step/formats/openbabel_io/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/formats/openbabel_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/formats/openbabel_io/checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/formats/openbabel_io/obabel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/formats/registries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:09:39.797123 read_structure_step-2023.1.27/read_structure_step/formats/sdf/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/formats/sdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/formats/sdf/sdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:09:39.801123 read_structure_step-2023.1.27/read_structure_step/formats/smi/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/formats/smi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/formats/smi/smi.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/formats/which.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:09:39.801123 read_structure_step-2023.1.27/read_structure_step/formats/xyz/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/formats/xyz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/formats/xyz/xyz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/read.py
--rw-r--r--   0 runner    (1001) docker     (123)    12413 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/read_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/read_structure_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/read_structure_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/tk_read_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/tk_write_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/write.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/write_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/write_structure_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/read_structure_step/write_structure_step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:09:39.797123 read_structure_step-2023.1.27/read_structure_step.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-01-27 20:09:39.000000 read_structure_step-2023.1.27/read_structure_step.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-01-27 20:09:39.000000 read_structure_step-2023.1.27/read_structure_step.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:09:39.000000 read_structure_step-2023.1.27/read_structure_step.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-01-27 20:09:39.000000 read_structure_step-2023.1.27/read_structure_step.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-27 20:09:39.000000 read_structure_step-2023.1.27/read_structure_step.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-27 20:09:39.000000 read_structure_step-2023.1.27/read_structure_step.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 20:09:28.000000 read_structure_step-2023.1.27/read_structure_step.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-01-27 20:09:39.805123 read_structure_step-2023.1.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:09:39.801123 read_structure_step-2023.1.27/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/build_filenames.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 20:09:39.805123 read_structure_step-2023.1.27/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/data/3TR_model.json
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/data/3TR_model.mol2
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/data/3TR_model.pdb
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/data/3TR_model.sdf
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/data/3TR_model.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/data/3TR_model_MN.xyz
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/data/Cr_ACETCR.mop
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/data/Cu(II)4Br10(2-) (CIVNAW10).mop
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/data/RM1 63 Europium, CCDC entry LAPJAN.mop
--rwxr-xr-x   0 runner    (1001) docker     (123)      658 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/data/acetonitrile.mop
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/data/lithium fluoride, trimer.mop
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/data/methylidyne.mop
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/data/potassium fluoride, dimer.mop
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/data/spc
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/data/spc.xyz
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/methylidyne.mop
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/mopac_exists.py
--rw-r--r--   0 runner    (1001) docker     (123)     8992 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/test_read_structure_step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-01-27 20:09:26.000000 read_structure_step-2023.1.27/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.616279 read_structure_step-2023.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-06 20:21:36.616279 read_structure_step-2023.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.600279 read_structure_step-2023.7.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.600279 read_structure_step-2023.7.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    20790 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/_static/SEAMM inverted.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17802 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/_static/SEAMM logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79373 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/_static/molssi_main_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    68255 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/_static/molssi_main_logo_inverted_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    63967 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/_static/molssi_square.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32355 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/_static/nsf.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.604279 read_structure_step-2023.7.6/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/api/read_structure_step.formats.cif.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/api/read_structure_step.formats.mol2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/api/read_structure_step.formats.mop.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/api/read_structure_step.formats.openbabel_io.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/api/read_structure_step.formats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/api/read_structure_step.formats.sdf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/api/read_structure_step.formats.smi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/api/read_structure_step.formats.xyz.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9623 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.604279 read_structure_step-2023.7.6/docs/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/developer_guide/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/developer_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/developer_guide/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.604279 read_structure_step-2023.7.6/docs/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)   434049 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/getting_started/dialog.png
+-rw-r--r--   0 runner    (1001) docker     (123)   121911 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/getting_started/flowchart.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.604279 read_structure_step-2023.7.6/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/docs/user_guide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.620279 read_structure_step-2023.7.6/read_structure_step/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-06 20:21:36.620279 read_structure_step-2023.7.6/read_structure_step/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.608279 read_structure_step-2023.7.6/read_structure_step/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/data/references.bib
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.612279 read_structure_step-2023.7.6/read_structure_step/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.612279 read_structure_step-2023.7.6/read_structure_step/formats/cif/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/cif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/cif/cif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/cif/mmcif.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.612279 read_structure_step-2023.7.6/read_structure_step/formats/mol2/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/mol2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/mol2/mol2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.612279 read_structure_step-2023.7.6/read_structure_step/formats/mop/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/mop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/mop/find_mopac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22956 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/mop/obabel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.612279 read_structure_step-2023.7.6/read_structure_step/formats/openbabel_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/openbabel_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/openbabel_io/checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10462 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/openbabel_io/obabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/registries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.612279 read_structure_step-2023.7.6/read_structure_step/formats/sdf/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/sdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15572 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/sdf/sdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.612279 read_structure_step-2023.7.6/read_structure_step/formats/smi/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/smi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/smi/smi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/which.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.612279 read_structure_step-2023.7.6/read_structure_step/formats/xyz/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/xyz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/formats/xyz/xyz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12382 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/read_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/read_structure_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/read_structure_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/tk_read_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/tk_write_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/write_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/write_structure_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/read_structure_step/write_structure_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.608279 read_structure_step-2023.7.6/read_structure_step.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-06 20:21:36.000000 read_structure_step-2023.7.6/read_structure_step.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-06 20:21:36.000000 read_structure_step-2023.7.6/read_structure_step.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:21:36.000000 read_structure_step-2023.7.6/read_structure_step.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-06 20:21:36.000000 read_structure_step-2023.7.6/read_structure_step.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 20:21:36.000000 read_structure_step-2023.7.6/read_structure_step.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-06 20:21:36.000000 read_structure_step-2023.7.6/read_structure_step.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:21:21.000000 read_structure_step-2023.7.6/read_structure_step.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-06 20:21:36.620279 read_structure_step-2023.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.616279 read_structure_step-2023.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/build_filenames.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:21:36.616279 read_structure_step-2023.7.6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/3TR_model.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/3TR_model.mol2
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/3TR_model.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/3TR_model.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/3TR_model.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/3TR_model_MN.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/Cr_ACETCR.mop
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/Cu(II)4Br10(2-) (CIVNAW10).mop
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/RM1 63 Europium, CCDC entry LAPJAN.mop
+-rwxr-xr-x   0 runner    (1001) docker     (123)      658 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/acetonitrile.mop
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/lithium fluoride, trimer.mop
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/methylidyne.mop
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/potassium fluoride, dimer.mop
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/spc
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/data/spc.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/methylidyne.mop
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/mopac_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8990 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/test_read_structure_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-06 20:21:17.000000 read_structure_step-2023.7.6/versioneer.py
```

### Comparing `read_structure_step-2023.1.27/CONTRIBUTING.rst` & `read_structure_step-2023.7.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/HISTORY.rst` & `read_structure_step-2023.7.6/HISTORY.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 =======
 History
 =======
 
+2023.7.6 -- Bugfixes
+  * Fixed output of number of structures written to SDF files, which was off by 1.
+  * Cleaned up the output for the write-structure step
+    
+2023.1.30 -- Fixed issue#43, duplicate systems or configuration created
+
+  * Reading a single structure from e.g. a .sdf file created a second system or
+    configuration, depending on the stucture control options.
+
 2023.1.24 -- Added handler for XYZ files and added properties
 
   * Added a custom handler for XYZ files to cope with some of the variant formats.
 
     * Supports files with no atom count on the first line
 
     * Supports the variant used in the Minnesota Solubility database, which has 3 header
```

### Comparing `read_structure_step-2023.1.27/LICENSE` & `read_structure_step-2023.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/PKG-INFO` & `read_structure_step-2023.7.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: read_structure_step
-Version: 2023.1.27
+Version: 2023.7.6
 Summary: A SEAMM plug-in to read common formats in computational chemistry
 Home-page: https://github.com/molssi-seamm/read_structure_step
 Author: Eliseo Marin-R-Rimoldi
 Author-email: meliseo@vt.edu
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,Open Babel,molecules,atomistic,files
 Platform: Linux
@@ -101,14 +101,23 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
+2023.7.6 -- Bugfixes
+  * Fixed output of number of structures written to SDF files, which was off by 1.
+  * Cleaned up the output for the write-structure step
+    
+2023.1.30 -- Fixed issue#43, duplicate systems or configuration created
+
+  * Reading a single structure from e.g. a .sdf file created a second system or
+    configuration, depending on the stucture control options.
+
 2023.1.24 -- Added handler for XYZ files and added properties
 
   * Added a custom handler for XYZ files to cope with some of the variant formats.
 
     * Supports files with no atom count on the first line
 
     * Supports the variant used in the Minnesota Solubility database, which has 3 header
```

### Comparing `read_structure_step-2023.1.27/README.rst` & `read_structure_step-2023.7.6/README.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/docs/Makefile` & `read_structure_step-2023.7.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/docs/_static/SEAMM inverted.png` & `read_structure_step-2023.7.6/docs/_static/SEAMM inverted.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/docs/_static/SEAMM logo.png` & `read_structure_step-2023.7.6/docs/_static/SEAMM logo.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/docs/_static/molssi_main_logo.png` & `read_structure_step-2023.7.6/docs/_static/molssi_main_logo.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/docs/_static/molssi_main_logo_inverted_white.png` & `read_structure_step-2023.7.6/docs/_static/molssi_main_logo_inverted_white.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/docs/_static/molssi_square.png` & `read_structure_step-2023.7.6/docs/_static/molssi_square.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/docs/_static/nsf.png` & `read_structure_step-2023.7.6/docs/_static/nsf.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/docs/api/read_structure_step.formats.cif.rst` & `read_structure_step-2023.7.6/docs/api/read_structure_step.formats.cif.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/docs/api/read_structure_step.formats.mop.rst` & `read_structure_step-2023.7.6/docs/api/read_structure_step.formats.mop.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/docs/api/read_structure_step.formats.openbabel_io.rst` & `read_structure_step-2023.7.6/docs/api/read_structure_step.formats.openbabel_io.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/docs/api/read_structure_step.formats.rst` & `read_structure_step-2023.7.6/docs/api/read_structure_step.formats.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/docs/conf.py` & `read_structure_step-2023.7.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/docs/developer_guide/installation.rst` & `read_structure_step-2023.7.6/docs/developer_guide/installation.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/docs/getting_started/dialog.png` & `read_structure_step-2023.7.6/docs/getting_started/dialog.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/docs/getting_started/flowchart.png` & `read_structure_step-2023.7.6/docs/getting_started/flowchart.png`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/docs/getting_started/index.rst` & `read_structure_step-2023.7.6/docs/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/docs/index.rst` & `read_structure_step-2023.7.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/docs/make.bat` & `read_structure_step-2023.7.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/read_structure_step/__init__.py` & `read_structure_step-2023.7.6/read_structure_step/__init__.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/read_structure_step/data/references.bib` & `read_structure_step-2023.7.6/read_structure_step/data/references.bib`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/read_structure_step/errors.py` & `read_structure_step-2023.7.6/read_structure_step/errors.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/read_structure_step/formats/__init__.py` & `read_structure_step-2023.7.6/read_structure_step/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/read_structure_step/formats/cif/cif.py` & `read_structure_step-2023.7.6/read_structure_step/formats/cif/cif.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/read_structure_step/formats/cif/mmcif.py` & `read_structure_step-2023.7.6/read_structure_step/formats/cif/mmcif.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/read_structure_step/formats/mol2/mol2.py` & `read_structure_step-2023.7.6/read_structure_step/formats/mol2/mol2.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/read_structure_step/formats/mop/__init__.py` & `read_structure_step-2023.7.6/read_structure_step/formats/mop/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,16 +268,14 @@
     "XYZ",
     "Z=n",
 ]
 
 
 @register_format_checker(".mop")
 def check_format(file_name):
-
     with open(file_name, "r") as f:
-
         data = f.read()
 
         if any(keyword in data for keyword in keywords):
             return True
         else:
             return False
```

### Comparing `read_structure_step-2023.1.27/read_structure_step/formats/mop/find_mopac.py` & `read_structure_step-2023.7.6/read_structure_step/formats/mop/find_mopac.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/read_structure_step/formats/mop/obabel.py` & `read_structure_step-2023.7.6/read_structure_step/formats/mop/obabel.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/read_structure_step/formats/openbabel_io/checkers.py` & `read_structure_step-2023.7.6/read_structure_step/formats/openbabel_io/checkers.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/read_structure_step/formats/openbabel_io/obabel.py` & `read_structure_step-2023.7.6/read_structure_step/formats/openbabel_io/obabel.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/read_structure_step/formats/registries.py` & `read_structure_step-2023.7.6/read_structure_step/formats/registries.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,29 +34,27 @@
     "bonds": False,
     "is_complete": True,
     "add_hydrogens": False,
 }
 
 
 def register_reader(file_format):
-
     tmp = file_format.split()
     extension = tmp[0]
     if extension[0] != ".":
         extension = "." + extension
     if len(tmp) == 1:
         description = ""
     else:
         if tmp[1] == "--":
             description = " ".join(tmp[2:])
         else:
             description = " ".join(tmp[1:])
 
     def decorator_function(fn):
-
         REGISTERED_READERS[extension] = {"function": fn, "description": description}
 
         def wrapper_function(*args, **kwargs):
             return fn(*args, **kwargs)
 
         return wrapper_function
 
@@ -86,15 +84,14 @@
         return wrapper_function
 
     return decorator_function
 
 
 def register_format_checker(file_format):
     def decorator_function(fn):
-
         REGISTERED_FORMAT_CHECKERS[file_format] = fn
 
         def wrapper_function(*args, **kwargs):
             return fn(*args, **kwargs)
 
         return wrapper_function
```

### Comparing `read_structure_step-2023.1.27/read_structure_step/formats/sdf/sdf.py` & `read_structure_step-2023.7.6/read_structure_step/formats/sdf/sdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,16 +403,16 @@
                         last_t = t1
                         last_percent = percent
 
     if printer:
         t1 = time.time()
         rate = structure_no / (t1 - t0)
         printer(
-            f"Wrote {structure_no} structures in {t1 - t0:.1f} seconds = {rate:.2f} "
-            "per second"
+            f"    Wrote {structure_no - 1} structures in {t1 - t0:.1f} seconds = "
+            f"{rate:.2f} per second"
         )
 
     if references:
         # Add the citations for Open Babel
         references.cite(
             raw=bibliography["openbabel"],
             alias="openbabel_jcinf",
```

### Comparing `read_structure_step-2023.1.27/read_structure_step/formats/smi/smi.py` & `read_structure_step-2023.7.6/read_structure_step/formats/smi/smi.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/read_structure_step/formats/xyz/__init__.py` & `read_structure_step-2023.7.6/read_structure_step/formats/xyz/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from read_structure_step.formats.registries import register_format_checker
 from . import xyz  # noqa: F401
 
 
 @register_format_checker(".xyz")
 def check_format(file_name):
-
     with open(file_name, "r") as f:
         lines = f.read().splitlines()
 
         if len(lines) < 3:
             return False
 
         # Standard XYZ
```

### Comparing `read_structure_step-2023.1.27/read_structure_step/formats/xyz/xyz.py` & `read_structure_step-2023.7.6/read_structure_step/formats/xyz/xyz.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/read_structure_step/read.py` & `read_structure_step-2023.7.6/read_structure_step/read.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,19 +88,17 @@
             """read_structure_step: The file name for the structure file
             was not specified."""
         )
 
     file_name = os.path.abspath(file_name)
 
     if extension is None:
-
         extension = utils.guess_extension(file_name, use_file_name=True)
 
         if extension is None:
-
             extension = utils.guess_extension(file_name, use_file_name=False)
 
     else:
         extension = utils.sanitize_file_format(extension)
 
     if extension is None:
         raise NameError("Extension could not be identified")
```

### Comparing `read_structure_step-2023.1.27/read_structure_step/read_structure.py` & `read_structure_step-2023.7.6/read_structure_step/read_structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,14 @@
         """The git version of this module."""
         return read_structure_step.__git_revision__
 
     def create_parser(self):
         """Setup the command-line / config file parser"""
         # Need to mimic MOPAC step to find the MOPAC executable
         parser_name = "mopac-step"
-        print(f"Parser {parser_name}, {self.step_type=}")
         parser = getParser()
 
         # Remember if the parser exists ... this type of step may have been
         # found before
         parser_exists = parser.exists(parser_name)
         print(f"{parser_exists=}")
 
@@ -151,15 +150,17 @@
 
         if self.is_expr(filename) or self.is_expr(file_type):
             extension = "all"
         else:
             if file_type != "from extension":
                 extension = file_type.split()[0]
             else:
-                if filename != "":
+                if self.is_expr(filename):
+                    extension = "all"
+                elif filename != "":
                     path = PurePath(filename)
                     extension = path.suffix
                     if extension == ".gz":
                         extension = path.with_suffix("").suffix
 
         # Get the metadata for the format
         metadata = get_format_metadata(extension)
@@ -230,17 +231,16 @@
                 configuration_name=str(P["configuration name"]),
                 printer=printer.important,
                 references=self.references,
                 bibliography=self._bibliography,
             )
 
             # Finish the output
-            system, configuration = self.get_system_configuration(
-                P, structure_handling=False
-            )
+            system, configuration = self.get_system_configuration()
+
             if configurations is None or len(configurations) == 1:
                 if configuration.periodicity == 3:
                     space_group = configuration.symmetry.group
                     if space_group == "":
                         symmetry_info = ""
                     else:
                         symmetry_info = f" The space group is {space_group}."
```

### Comparing `read_structure_step-2023.1.27/read_structure_step/read_structure_parameters.py` & `read_structure_step-2023.7.6/read_structure_step/read_structure_parameters.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/read_structure_step/read_structure_step.py` & `read_structure_step-2023.7.6/read_structure_step/read_structure_step.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/read_structure_step/tk_read_structure.py` & `read_structure_step-2023.7.6/read_structure_step/tk_read_structure.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/read_structure_step/tk_write_structure.py` & `read_structure_step-2023.7.6/read_structure_step/tk_write_structure.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/read_structure_step/utils.py` & `read_structure_step-2023.7.6/read_structure_step/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
             return None
 
         return ext.lower()
 
     available_extensions = formats.registries.REGISTERED_FORMAT_CHECKERS.keys()
 
     for extension in available_extensions:
-
         extension_checker = formats.registries.REGISTERED_FORMAT_CHECKERS[extension]
 
         if extension_checker(file_name) is True:
             return extension
 
 
 def sanitize_file_format(file_format):
```

### Comparing `read_structure_step-2023.1.27/read_structure_step/write.py` & `read_structure_step-2023.7.6/read_structure_step/write.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/read_structure_step/write_structure_parameters.py` & `read_structure_step-2023.7.6/read_structure_step/write_structure_parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,28 +72,27 @@
             "default": "current configuration",
             "kind": "string",
             "default_units": "",
             "enumeration": (
                 "current configuration",
                 "current system",
                 "all systems",
-                "list of configurations",
             ),
             "format_string": "s",
             "description": "Structures to write:",
             "help_text": ("The set of structures to write"),
         },
         "configurations": {
             "default": "all",
             "kind": "string",
             "default_units": "",
             "enumeration": ("all",),
             "format_string": "s",
             "description": "Configuration(s) to write:",
-            "help_text": "The configurations to write: a name, or 'all configurations'",
+            "help_text": "The configurations to write: a name, or 'all'",
         },
         "number per file": {
             "default": "all",
             "kind": "integer",
             "default_units": "",
             "enumeration": ("all",),
             "format_string": "",
```

### Comparing `read_structure_step-2023.1.27/read_structure_step/write_structure_step.py` & `read_structure_step-2023.7.6/read_structure_step/write_structure_step.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/read_structure_step.egg-info/PKG-INFO` & `read_structure_step-2023.7.6/read_structure_step.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: read-structure-step
-Version: 2023.1.27
+Version: 2023.7.6
 Summary: A SEAMM plug-in to read common formats in computational chemistry
 Home-page: https://github.com/molssi-seamm/read_structure_step
 Author: Eliseo Marin-R-Rimoldi
 Author-email: meliseo@vt.edu
 License: BSD-3-Clause
 Keywords: SEAMM,plug-in,flowchart,Open Babel,molecules,atomistic,files
 Platform: Linux
@@ -101,14 +101,23 @@
 .. _`National Science Foundation`: https://www.nsf.gov
 
 
 =======
 History
 =======
 
+2023.7.6 -- Bugfixes
+  * Fixed output of number of structures written to SDF files, which was off by 1.
+  * Cleaned up the output for the write-structure step
+    
+2023.1.30 -- Fixed issue#43, duplicate systems or configuration created
+
+  * Reading a single structure from e.g. a .sdf file created a second system or
+    configuration, depending on the stucture control options.
+
 2023.1.24 -- Added handler for XYZ files and added properties
 
   * Added a custom handler for XYZ files to cope with some of the variant formats.
 
     * Supports files with no atom count on the first line
 
     * Supports the variant used in the Minnesota Solubility database, which has 3 header
```

### Comparing `read_structure_step-2023.1.27/read_structure_step.egg-info/SOURCES.txt` & `read_structure_step-2023.7.6/read_structure_step.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/setup.py` & `read_structure_step-2023.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/tests/build_filenames.py` & `read_structure_step-2023.7.6/tests/build_filenames.py`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/tests/data/3TR_model.json` & `read_structure_step-2023.7.6/tests/data/3TR_model.json`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/tests/data/3TR_model.mol2` & `read_structure_step-2023.7.6/tests/data/3TR_model.mol2`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/tests/data/3TR_model.pdb` & `read_structure_step-2023.7.6/tests/data/3TR_model.pdb`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/tests/data/3TR_model.sdf` & `read_structure_step-2023.7.6/tests/data/3TR_model.sdf`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/tests/data/Cr_ACETCR.mop` & `read_structure_step-2023.7.6/tests/data/Cr_ACETCR.mop`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/tests/data/Cu(II)4Br10(2-) (CIVNAW10).mop` & `read_structure_step-2023.7.6/tests/data/Cu(II)4Br10(2-) (CIVNAW10).mop`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/tests/data/RM1 63 Europium, CCDC entry LAPJAN.mop` & `read_structure_step-2023.7.6/tests/data/RM1 63 Europium, CCDC entry LAPJAN.mop`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/tests/data/acetonitrile.mop` & `read_structure_step-2023.7.6/tests/data/acetonitrile.mop`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/tests/data/lithium fluoride, trimer.mop` & `read_structure_step-2023.7.6/tests/data/lithium fluoride, trimer.mop`

 * *Files identical despite different names*

### Comparing `read_structure_step-2023.1.27/tests/test_formats.py` & `read_structure_step-2023.7.6/tests/test_formats.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,14 @@
         "3TR_model.xyz",
         "3TR_model_MN.xyz",
         "3TR_model.pdb",
         "3TR_model.sdf",
     ],
 )
 def test_format(configuration, structure):
-
     file_name = build_filenames.build_data_filename(structure)
     read_structure_step.read(file_name, configuration)
 
     assert configuration.n_atoms == 10
     assert all(
         atom in ["N", "N", "N", "N", "C", "C", "H", "H", "H", "H"]
         for atom in configuration.atoms.symbols
@@ -93,15 +92,14 @@
 
 
 @pytest.mark.skipif(
     read_structure_step.formats.mop.find_mopac.find_mopac() is None,
     reason="MOPAC could not be found",
 )
 def test_mopac(configuration):
-
     file_name = build_filenames.build_data_filename("acetonitrile.mop")
     read_structure_step.read(file_name, configuration)
 
     assert configuration.n_atoms == 6
     assert all(
         atom in ["H", "H", "H", "C", "C", "N"] for atom in configuration.atoms.symbols
     )
```

### Comparing `read_structure_step-2023.1.27/tests/test_read_structure_step.py` & `read_structure_step-2023.7.6/tests/test_read_structure_step.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,24 +24,20 @@
         del db
     except:  # noqa: E722
         print("Caught error deleting the database")
 
 
 @pytest.mark.parametrize("file_name", [1, [], {}, 1.0])
 def test_read_filename_type(configuration, file_name):
-
     with pytest.raises(TypeError):
         read_structure_step.read(file_name, configuration)
 
 
 def test_empty_filename(configuration):
-
     with pytest.raises(NameError):
         read_structure_step.read("", configuration)
 
 
 def test_unregistered_reader(configuration):
-
     with pytest.raises(KeyError):
-
         xyz_file = build_filenames.build_data_filename("spc.xyz")
         read_structure_step.read(xyz_file, configuration, extension=".mp3")
```

### Comparing `read_structure_step-2023.1.27/tests/test_utils.py` & `read_structure_step-2023.7.6/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     except:  # noqa: E722
         print("Caught error deleting the database")
 
 
 @pytest.mark.parametrize("file_name", ["spc.xyz", "spc"])
 @pytest.mark.parametrize("extension", [None, ".xyz", "xyz", "XYZ", "xYz"])
 def test_extensions(configuration, file_name, extension):
-
     xyz_file = build_filenames.build_data_filename(file_name)
     read_structure_step.read(xyz_file, configuration, extension=extension)
 
     assert configuration.n_atoms == 3
     assert all(atom in ["O", "H", "H"] for atom in configuration.atoms.symbols)
 
     coordinates = configuration.atoms.coordinates
@@ -48,10 +47,9 @@
     assert configuration.bonds.n_bonds == 2
     if str(configuration.bonds) != bond_string:
         print(configuration.bonds)
     assert str(configuration.bonds) == bond_string
 
 
 def test_sanitize_file_format_regex_validation(configuration):
-
     with pytest.raises(NameError):
         read_structure_step.read("spc.xyz", configuration, extension=".xy-z")
```

### Comparing `read_structure_step-2023.1.27/versioneer.py` & `read_structure_step-2023.7.6/versioneer.py`

 * *Files identical despite different names*

