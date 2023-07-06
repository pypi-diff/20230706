# Comparing `tmp/lightshow-0.1.2.tar.gz` & `tmp/lightshow-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightshow-0.1.2.tar", last modified: Wed Apr 26 16:58:26 2023, max compression
+gzip compressed data, was "lightshow-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lightshow-0.1.2.tar` & `lightshow-0.1.3.tar`

### file list

```diff
@@ -1,88 +1,89 @@
--rw-r--r--   0        0        0      135 2023-04-26 16:58:19.808681 lightshow-0.1.2/.coveragerc
--rw-r--r--   0        0        0      221 2023-04-26 16:58:19.808681 lightshow-0.1.2/.flake8
--rw-r--r--   0        0        0     6310 2023-04-26 16:58:19.808681 lightshow-0.1.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2106 2023-04-26 16:58:19.808681 lightshow-0.1.2/.gitignore
--rw-r--r--   0        0        0      336 2023-04-26 16:58:19.808681 lightshow-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1099 2023-04-26 16:58:19.808681 lightshow-0.1.2/AUTHORS.rst
--rw-r--r--   0        0        0     1574 2023-04-26 16:58:19.808681 lightshow-0.1.2/LICENSE
--rw-r--r--   0        0        0     5427 2023-04-26 16:58:19.808681 lightshow-0.1.2/README.md
--rw-r--r--   0        0        0      673 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/Makefile
--rw-r--r--   0        0        0    60563 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/_static/images/lightshow.jpg
--rw-r--r--   0        0        0   118686 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/_static/images/lightshow_old.jpg
--rw-r--r--   0        0        0      797 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/make.bat
--rw-r--r--   0        0        0        0 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/_static/.placeholder
--rw-r--r--   0        0        0     6725 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/conf.py
--rw-r--r--   0        0        0     2023 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/index.rst
--rw-r--r--   0        0        0     1181 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/installation.rst
--rw-r--r--   0        0        0     1053 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/lightshow.parameters.rst
--rw-r--r--   0        0        0      559 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/lightshow.rst
--rw-r--r--   0        0        0       86 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/modules.rst
--rw-r--r--   0        0        0      337 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/project.rst
--rw-r--r--   0        0        0       34 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/project/authors.rst
--rw-r--r--   0        0        0     1720 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/project/funding.rst
--rw-r--r--   0        0        0       47 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/project/license.rst
--rw-r--r--   0        0        0    21003 2023-04-26 16:58:19.808681 lightshow-0.1.2/docs/source/quickstart.rst
--rw-r--r--   0        0        0    92531 2023-04-26 16:58:19.808681 lightshow-0.1.2/figures/Lightshow_Workflow_Diagram.jpg
--rw-r--r--   0        0        0    25190 2023-04-26 16:58:19.808681 lightshow-0.1.2/figures/Lightshow_Workflow_Diagram.pdf
--rw-r--r--   0        0        0     1887 2023-04-26 16:58:26.428712 lightshow-0.1.2/lightshow/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 16:58:19.808681 lightshow-0.1.2/lightshow/_tests/__init__.py
--rw-r--r--   0        0        0     1540 2023-04-26 16:58:19.808681 lightshow-0.1.2/lightshow/_tests/conftest.py
--rw-r--r--   0        0        0       40 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/dummy_chpsp_files/Core_O.wfc
--rw-r--r--   0        0        0       42 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/dummy_chpsp_files/Core_Ti.wfc
--rw-r--r--   0        0        0       34 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/dummy_chpsp_files/O.fch.upf
--rw-r--r--   0        0        0       35 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/dummy_chpsp_files/Ti.fch.upf
--rw-r--r--   0        0        0      476 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/dummy_potcar_files/O_GW/POTCAR
--rw-r--r--   0        0        0      480 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/dummy_potcar_files/Ti_sv_GW/POTCAR
--rw-r--r--   0        0        0       24 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/dummy_psp_files/O.mock.upf
--rw-r--r--   0        0        0       25 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/dummy_psp_files/Ti.mock.upf
--rw-r--r--   0        0        0      152 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/dummy_psp_files/mock_cutoff_table.json
--rw-r--r--   0        0        0        0 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/helpers/__init__.py
--rw-r--r--   0        0        0    11401 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/helpers/geometry.py
--rw-r--r--   0        0        0       82 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/sample_files/README.rst
--rw-r--r--   0        0        0    42630 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/sample_files/ene_dep_broad.txt
--rw-r--r--   0        0        0    43441 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/sample_files/gauss_broad.txt
--rw-r--r--   0        0        0    43519 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/sample_files/lorentz_broad.txt
--rw-r--r--   0        0        0    43398 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/sample_files/voigt_broad.txt
--rw-r--r--   0        0        0      376 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/structure_files/mp-10734/POSCAR
--rw-r--r--   0        0        0      198 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/structure_files/mp-1215/POSCAR
--rw-r--r--   0        0        0      814 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/structure_files/mp-1840/POSCAR
--rw-r--r--   0        0        0      284 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/structure_files/mp-2657/POSCAR
--rw-r--r--   0        0        0      167 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/structure_files/mp-2664/POSCAR
--rw-r--r--   0        0        0      287 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/structure_files/mp-390/POSCAR
--rw-r--r--   0        0        0      460 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/structure_files/mp-430/POSCAR
--rw-r--r--   0        0        0      403 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/structure_files/mp-458/POSCAR
--rw-r--r--   0        0        0      461 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/structure_files/mvc-11115/POSCAR
--rw-r--r--   0        0        0     1702 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/test_broaden.py
--rw-r--r--   0        0        0     3372 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/test_database.py
--rw-r--r--   0        0        0    12398 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/test_exciting.py
--rw-r--r--   0        0        0     1166 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/_tests/test_vasp.py
--rw-r--r--   0        0        0        0 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/common/__init__.py
--rw-r--r--   0        0        0     2558 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/common/kpoints.py
--rw-r--r--   0        0        0     3322 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/common/nbands.py
--rw-r--r--   0        0        0    21933 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/database.py
--rw-r--r--   0        0        0      602 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/defaults.py
--rw-r--r--   0        0        0        0 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/parameters/__init__.py
--rw-r--r--   0        0        0      206 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/parameters/_base.py
--rw-r--r--   0        0        0     9115 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/parameters/exciting.py
--rw-r--r--   0        0        0     7407 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/parameters/feff.py
--rw-r--r--   0        0        0    14284 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/parameters/ocean.py
--rw-r--r--   0        0        0    29413 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/parameters/vasp.py
--rw-r--r--   0        0        0    19946 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/parameters/xspectra.py
--rw-r--r--   0        0        0        0 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/postprocess/__init__.py
--rw-r--r--   0        0        0     8977 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/postprocess/broaden.py
--rw-r--r--   0        0        0     2371 2023-04-26 16:58:19.812681 lightshow-0.1.2/lightshow/pymatgen_utils.py
--rw-r--r--   0        0        0    32206 2023-04-26 16:58:19.812681 lightshow-0.1.2/notebooks/00_basic_usage.ipynb
--rw-r--r--   0        0        0    10037 2023-04-26 16:58:19.812681 lightshow-0.1.2/notebooks/01_Ti_K_anatase_broaden.ipynb
--rwxr-xr-x   0        0        0    41029 2023-04-26 16:58:19.812681 lightshow-0.1.2/notebooks/spectra_files/anatase_exciting.txt
--rw-r--r--   0        0        0     3816 2023-04-26 16:58:19.812681 lightshow-0.1.2/notebooks/spectra_files/anatase_exp.txt
--rw-r--r--   0        0        0    54210 2023-04-26 16:58:19.816681 lightshow-0.1.2/notebooks/spectra_files/anatase_ocean.txt
--rw-r--r--   0        0        0     5000 2023-04-26 16:58:19.816681 lightshow-0.1.2/notebooks/spectra_files/anatase_theory_FEFF.txt
--rw-r--r--   0        0        0  2000000 2023-04-26 16:58:19.824681 lightshow-0.1.2/notebooks/spectra_files/anatase_theory_VASP.txt
--rwxr-xr-x   0        0        0    11578 2023-04-26 16:58:19.824681 lightshow-0.1.2/notebooks/spectra_files/anatase_xspectra.txt
--rw-r--r--   0        0        0     2076 2023-04-26 16:58:19.824681 lightshow-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1204 2023-04-26 16:58:19.824681 lightshow-0.1.2/scripts/README.rst
--rw-r--r--   0        0        0      575 2023-04-26 16:58:19.824681 lightshow-0.1.2/scripts/build_docs.sh
--rw-r--r--   0        0        0      118 2023-04-26 16:58:19.824681 lightshow-0.1.2/scripts/build_project.sh
--rw-r--r--   0        0        0      943 2023-04-26 16:58:19.824681 lightshow-0.1.2/scripts/install.sh
--rw-r--r--   0        0        0     1076 2023-04-26 16:58:19.824681 lightshow-0.1.2/scripts/update_version.sh
--rw-r--r--   0        0        0     7154 1970-01-01 00:00:00.000000 lightshow-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      135 2023-07-06 02:32:01.012133 lightshow-0.1.3/.coveragerc
+-rw-r--r--   0        0        0      221 2023-07-06 02:32:01.012133 lightshow-0.1.3/.flake8
+-rw-r--r--   0        0        0     6310 2023-07-06 02:32:01.012133 lightshow-0.1.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2106 2023-07-06 02:32:01.012133 lightshow-0.1.3/.gitignore
+-rw-r--r--   0        0        0      336 2023-07-06 02:32:01.012133 lightshow-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1099 2023-07-06 02:32:01.012133 lightshow-0.1.3/AUTHORS.rst
+-rw-r--r--   0        0        0     1113 2023-07-06 02:32:01.012133 lightshow-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1574 2023-07-06 02:32:01.012133 lightshow-0.1.3/LICENSE
+-rw-r--r--   0        0        0     7012 2023-07-06 02:32:01.012133 lightshow-0.1.3/README.md
+-rw-r--r--   0        0        0      673 2023-07-06 02:32:01.012133 lightshow-0.1.3/docs/Makefile
+-rw-r--r--   0        0        0    60563 2023-07-06 02:32:01.012133 lightshow-0.1.3/docs/_static/images/lightshow.jpg
+-rw-r--r--   0        0        0   118686 2023-07-06 02:32:01.016132 lightshow-0.1.3/docs/_static/images/lightshow_old.jpg
+-rw-r--r--   0        0        0      797 2023-07-06 02:32:01.016132 lightshow-0.1.3/docs/make.bat
+-rw-r--r--   0        0        0        0 2023-07-06 02:32:01.016132 lightshow-0.1.3/docs/source/_static/.placeholder
+-rw-r--r--   0        0        0     6725 2023-07-06 02:32:01.016132 lightshow-0.1.3/docs/source/conf.py
+-rw-r--r--   0        0        0     2023 2023-07-06 02:32:01.016132 lightshow-0.1.3/docs/source/index.rst
+-rw-r--r--   0        0        0     1181 2023-07-06 02:32:01.016132 lightshow-0.1.3/docs/source/installation.rst
+-rw-r--r--   0        0        0     1053 2023-07-06 02:32:01.016132 lightshow-0.1.3/docs/source/lightshow.parameters.rst
+-rw-r--r--   0        0        0      559 2023-07-06 02:32:01.016132 lightshow-0.1.3/docs/source/lightshow.rst
+-rw-r--r--   0        0        0       86 2023-07-06 02:32:01.016132 lightshow-0.1.3/docs/source/modules.rst
+-rw-r--r--   0        0        0      337 2023-07-06 02:32:01.016132 lightshow-0.1.3/docs/source/project.rst
+-rw-r--r--   0        0        0       34 2023-07-06 02:32:01.016132 lightshow-0.1.3/docs/source/project/authors.rst
+-rw-r--r--   0        0        0     1720 2023-07-06 02:32:01.016132 lightshow-0.1.3/docs/source/project/funding.rst
+-rw-r--r--   0        0        0       47 2023-07-06 02:32:01.016132 lightshow-0.1.3/docs/source/project/license.rst
+-rw-r--r--   0        0        0    21003 2023-07-06 02:32:01.016132 lightshow-0.1.3/docs/source/quickstart.rst
+-rw-r--r--   0        0        0    92531 2023-07-06 02:32:01.016132 lightshow-0.1.3/figures/Lightshow_Workflow_Diagram.jpg
+-rw-r--r--   0        0        0    25190 2023-07-06 02:32:01.016132 lightshow-0.1.3/figures/Lightshow_Workflow_Diagram.pdf
+-rw-r--r--   0        0        0     1887 2023-07-06 02:32:08.680277 lightshow-0.1.3/lightshow/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/__init__.py
+-rw-r--r--   0        0        0     1540 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/conftest.py
+-rw-r--r--   0        0        0       40 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/dummy_chpsp_files/Core_O.wfc
+-rw-r--r--   0        0        0       42 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/dummy_chpsp_files/Core_Ti.wfc
+-rw-r--r--   0        0        0       34 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/dummy_chpsp_files/O.fch.upf
+-rw-r--r--   0        0        0       35 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/dummy_chpsp_files/Ti.fch.upf
+-rw-r--r--   0        0        0      476 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/dummy_potcar_files/O_GW/POTCAR
+-rw-r--r--   0        0        0      480 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/dummy_potcar_files/Ti_sv_GW/POTCAR
+-rw-r--r--   0        0        0       24 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/dummy_psp_files/O.mock.upf
+-rw-r--r--   0        0        0       25 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/dummy_psp_files/Ti.mock.upf
+-rw-r--r--   0        0        0      152 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/dummy_psp_files/mock_cutoff_table.json
+-rw-r--r--   0        0        0        0 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/helpers/__init__.py
+-rw-r--r--   0        0        0    11401 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/helpers/geometry.py
+-rw-r--r--   0        0        0       82 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/sample_files/README.rst
+-rw-r--r--   0        0        0    42630 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/sample_files/ene_dep_broad.txt
+-rw-r--r--   0        0        0    43441 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/sample_files/gauss_broad.txt
+-rw-r--r--   0        0        0    43519 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/sample_files/lorentz_broad.txt
+-rw-r--r--   0        0        0    43398 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/sample_files/voigt_broad.txt
+-rw-r--r--   0        0        0      376 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/structure_files/mp-10734/POSCAR
+-rw-r--r--   0        0        0      198 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/structure_files/mp-1215/POSCAR
+-rw-r--r--   0        0        0      814 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/structure_files/mp-1840/POSCAR
+-rw-r--r--   0        0        0      284 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/structure_files/mp-2657/POSCAR
+-rw-r--r--   0        0        0      167 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/structure_files/mp-2664/POSCAR
+-rw-r--r--   0        0        0      287 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/structure_files/mp-390/POSCAR
+-rw-r--r--   0        0        0      460 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/structure_files/mp-430/POSCAR
+-rw-r--r--   0        0        0      403 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/structure_files/mp-458/POSCAR
+-rw-r--r--   0        0        0      461 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/structure_files/mvc-11115/POSCAR
+-rw-r--r--   0        0        0     1702 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/test_broaden.py
+-rw-r--r--   0        0        0     3372 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/test_database.py
+-rw-r--r--   0        0        0    12398 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/test_exciting.py
+-rw-r--r--   0        0        0     1166 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/_tests/test_vasp.py
+-rw-r--r--   0        0        0        0 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/common/__init__.py
+-rw-r--r--   0        0        0     2558 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/common/kpoints.py
+-rw-r--r--   0        0        0     3322 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/common/nbands.py
+-rw-r--r--   0        0        0    21933 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/database.py
+-rw-r--r--   0        0        0      602 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/defaults.py
+-rw-r--r--   0        0        0        0 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/parameters/__init__.py
+-rw-r--r--   0        0        0      206 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/parameters/_base.py
+-rw-r--r--   0        0        0     9115 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/parameters/exciting.py
+-rw-r--r--   0        0        0     7407 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/parameters/feff.py
+-rw-r--r--   0        0        0    14284 2023-07-06 02:32:01.016132 lightshow-0.1.3/lightshow/parameters/ocean.py
+-rw-r--r--   0        0        0    29413 2023-07-06 02:32:01.020133 lightshow-0.1.3/lightshow/parameters/vasp.py
+-rw-r--r--   0        0        0    19946 2023-07-06 02:32:01.020133 lightshow-0.1.3/lightshow/parameters/xspectra.py
+-rw-r--r--   0        0        0        0 2023-07-06 02:32:01.020133 lightshow-0.1.3/lightshow/postprocess/__init__.py
+-rw-r--r--   0        0        0     8977 2023-07-06 02:32:01.020133 lightshow-0.1.3/lightshow/postprocess/broaden.py
+-rw-r--r--   0        0        0     2371 2023-07-06 02:32:01.020133 lightshow-0.1.3/lightshow/pymatgen_utils.py
+-rw-r--r--   0        0        0    32206 2023-07-06 02:32:01.020133 lightshow-0.1.3/notebooks/00_basic_usage.ipynb
+-rw-r--r--   0        0        0    10037 2023-07-06 02:32:01.020133 lightshow-0.1.3/notebooks/01_Ti_K_anatase_broaden.ipynb
+-rwxr-xr-x   0        0        0    41029 2023-07-06 02:32:01.020133 lightshow-0.1.3/notebooks/spectra_files/anatase_exciting.txt
+-rw-r--r--   0        0        0     3816 2023-07-06 02:32:01.020133 lightshow-0.1.3/notebooks/spectra_files/anatase_exp.txt
+-rw-r--r--   0        0        0    54210 2023-07-06 02:32:01.020133 lightshow-0.1.3/notebooks/spectra_files/anatase_ocean.txt
+-rw-r--r--   0        0        0     5000 2023-07-06 02:32:01.020133 lightshow-0.1.3/notebooks/spectra_files/anatase_theory_FEFF.txt
+-rw-r--r--   0        0        0  2000000 2023-07-06 02:32:01.028133 lightshow-0.1.3/notebooks/spectra_files/anatase_theory_VASP.txt
+-rwxr-xr-x   0        0        0    11578 2023-07-06 02:32:01.028133 lightshow-0.1.3/notebooks/spectra_files/anatase_xspectra.txt
+-rw-r--r--   0        0        0     2076 2023-07-06 02:32:01.028133 lightshow-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1204 2023-07-06 02:32:01.028133 lightshow-0.1.3/scripts/README.rst
+-rw-r--r--   0        0        0      575 2023-07-06 02:32:01.028133 lightshow-0.1.3/scripts/build_docs.sh
+-rw-r--r--   0        0        0      118 2023-07-06 02:32:01.028133 lightshow-0.1.3/scripts/build_project.sh
+-rw-r--r--   0        0        0      943 2023-07-06 02:32:01.028133 lightshow-0.1.3/scripts/install.sh
+-rw-r--r--   0        0        0     1076 2023-07-06 02:32:01.028133 lightshow-0.1.3/scripts/update_version.sh
+-rw-r--r--   0        0        0     8739 1970-01-01 00:00:00.000000 lightshow-0.1.3/PKG-INFO
```

### Comparing `lightshow-0.1.2/.github/workflows/ci.yml` & `lightshow-0.1.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/.gitignore` & `lightshow-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/AUTHORS.rst` & `lightshow-0.1.3/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/LICENSE` & `lightshow-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/README.md` & `lightshow-0.1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 
 ![sysfs line plot](https://raw.githubusercontent.com/AI-multimodal/Lightshow/master/docs/_static/images/lightshow.jpg)
 
 [![image](https://github.com/AI-multimodal/Lightshow/actions/workflows/ci.yml/badge.svg)](https://github.com/AI-multimodal/Lightshow/actions/workflows/ci.yml)
 [![image](https://codecov.io/gh/AI-multimodal/Lightshow/branch/master/graph/badge.svg?token=CW7BMFA5O7)](https://codecov.io/gh/AI-multimodal/Lightshow)
 [![image](https://app.codacy.com/project/badge/Grade/d31a4e18672c4d71bbaafa719181c140)](https://www.codacy.com/gh/AI-multimodal/Lightshow/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=AI-multimodal/Lightshow&amp;utm_campaign=Badge_Grade)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![python](https://img.shields.io/badge/-Python_>=3.7-blue?logo=python&logoColor=white)](https://github.com/pre-commit/pre-commit) <br>
+[![python](https://img.shields.io/badge/-Python_>=3.7-blue?logo=python&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![PRs](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/AI-multimodal/Lightshow/pulls) <br>
 [![image](https://joss.theoj.org/papers/a9cabcd7f4b85a926a797997c6622b43/status.svg)](https://joss.theoj.org/papers/a9cabcd7f4b85a926a797997c6622b43)
 [![image](https://zenodo.org/badge/DOI/10.48550/arXiv.2211.04452.svg)](https://doi.org/10.48550/arXiv.2211.04452)
 
+
 </div>
     
 ------------------------------------------------------------------------
 
 **Lightshow** is a Python library for easily generating computational
 spectroscopy input files.
 
@@ -51,16 +53,64 @@
 
 To install Lightshow, simply use `pip`
 
 ``` bash
 pip install lightshow
 ```
 
+Make sure you've set your Pymatgen legacy API key as well!
+
+```bash
+export PMG_API_KEY="your_legacy_materials_project_key"
+```
+
+(or preferably, add `PMG_API_KEY` to your bash profile).
+
 More details can be found at our [documentation](https://ai-multimodal.github.io/Lightshow/installation.html).
 
+## Development installation
+
+For developers: after cloning Lightshow locally, install `pre-commit` via
+
+```bash
+pip install pre-commit
+pre-commit
+pre-commit install
+```
+
+and check that the tests (below) work correctly.
+
+## Running tests
+
+For developers: tests can be run via `pytest`. After cloning, simply use
+
+```bash
+pytest lightshow/_tests
+```
+
+or with coverage
+
+```bash
+pytest -v --cov --cov-report xml lightshow/_tests
+```
+
+
+# Contributing 
+
+We welcome any and all contributions by the community, including pull requests, bug reports, etc.
+Please see our [contributing](https://github.com/AI-multimodal/Lightshow/blob/master/CONTRIBUTING.md) document for more details!
+
+## Adding new spectroscopy codes
+
+Adding new spectroscopy codes requires one to inherit the `_BaseParameters` class from `lightshow.parameters._base`.
+The new `Parameters(_BaseParameters)` object should have a `write()` method, which must take a target directory as an
+argument, as well as any other keyword arguments require to write the input file (most notably, the Pymatgen structure,
+either a unit or super cell). The `name` property must also be defined (corresponding to the name of the calculation,
+e.g. "VASP"). Take a look at the examples in the `lightshow.parameters` module for more details!
+
 
 # Funding acknowledgement
 
 This research is based upon work supported by the U.S. Department of
 Energy, Office of Science, Office Basic Energy Sciences, under Award
 Number FWP PS-030. This research used resources of the Center for
 Functional Nanomaterials (CFN), which is a U.S. Department of Energy
```

### Comparing `lightshow-0.1.2/docs/Makefile` & `lightshow-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/docs/_static/images/lightshow.jpg` & `lightshow-0.1.3/docs/_static/images/lightshow.jpg`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/docs/_static/images/lightshow_old.jpg` & `lightshow-0.1.3/docs/_static/images/lightshow_old.jpg`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/docs/make.bat` & `lightshow-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/docs/source/conf.py` & `lightshow-0.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/docs/source/index.rst` & `lightshow-0.1.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/docs/source/installation.rst` & `lightshow-0.1.3/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/docs/source/lightshow.parameters.rst` & `lightshow-0.1.3/docs/source/lightshow.parameters.rst`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/docs/source/lightshow.rst` & `lightshow-0.1.3/docs/source/lightshow.rst`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/docs/source/project/funding.rst` & `lightshow-0.1.3/docs/source/project/funding.rst`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/docs/source/quickstart.rst` & `lightshow-0.1.3/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/figures/Lightshow_Workflow_Diagram.jpg` & `lightshow-0.1.3/figures/Lightshow_Workflow_Diagram.jpg`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/figures/Lightshow_Workflow_Diagram.pdf` & `lightshow-0.1.3/figures/Lightshow_Workflow_Diagram.pdf`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/__init__.py` & `lightshow-0.1.3/lightshow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from os import environ
 
 
 # DO NOT CHANGE BELOW ---------------------------------------------------------
 # This is replaced at build time automatically during deployment and
 # installation. Replacing anything will mess that up and crash the entire
 # build.
-__version__ = '0.1.2'
+__version__ = '0.1.3'
 # DO NOT CHANGE ABOVE ---------------------------------------------------------
 
 
 def _get_API_key_from_environ():
     """Checks for an environment variable PMG_API_KEY. If does not exist,
     returns None.
```

### Comparing `lightshow-0.1.2/lightshow/_tests/conftest.py` & `lightshow-0.1.3/lightshow/_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/_tests/helpers/geometry.py` & `lightshow-0.1.3/lightshow/_tests/helpers/geometry.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/_tests/sample_files/ene_dep_broad.txt` & `lightshow-0.1.3/lightshow/_tests/sample_files/ene_dep_broad.txt`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/_tests/sample_files/gauss_broad.txt` & `lightshow-0.1.3/lightshow/_tests/sample_files/gauss_broad.txt`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/_tests/sample_files/lorentz_broad.txt` & `lightshow-0.1.3/lightshow/_tests/sample_files/lorentz_broad.txt`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/_tests/sample_files/voigt_broad.txt` & `lightshow-0.1.3/lightshow/_tests/sample_files/voigt_broad.txt`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/_tests/structure_files/mp-1840/POSCAR` & `lightshow-0.1.3/lightshow/_tests/structure_files/mp-1840/POSCAR`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/_tests/test_broaden.py` & `lightshow-0.1.3/lightshow/_tests/test_broaden.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/_tests/test_database.py` & `lightshow-0.1.3/lightshow/_tests/test_database.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/_tests/test_exciting.py` & `lightshow-0.1.3/lightshow/_tests/test_exciting.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/_tests/test_vasp.py` & `lightshow-0.1.3/lightshow/_tests/test_vasp.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/common/kpoints.py` & `lightshow-0.1.3/lightshow/common/kpoints.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/common/nbands.py` & `lightshow-0.1.3/lightshow/common/nbands.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/database.py` & `lightshow-0.1.3/lightshow/database.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/defaults.py` & `lightshow-0.1.3/lightshow/defaults.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/parameters/exciting.py` & `lightshow-0.1.3/lightshow/parameters/exciting.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/parameters/feff.py` & `lightshow-0.1.3/lightshow/parameters/feff.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/parameters/ocean.py` & `lightshow-0.1.3/lightshow/parameters/ocean.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/parameters/vasp.py` & `lightshow-0.1.3/lightshow/parameters/vasp.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/parameters/xspectra.py` & `lightshow-0.1.3/lightshow/parameters/xspectra.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/postprocess/broaden.py` & `lightshow-0.1.3/lightshow/postprocess/broaden.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/lightshow/pymatgen_utils.py` & `lightshow-0.1.3/lightshow/pymatgen_utils.py`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/notebooks/00_basic_usage.ipynb` & `lightshow-0.1.3/notebooks/00_basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/notebooks/01_Ti_K_anatase_broaden.ipynb` & `lightshow-0.1.3/notebooks/01_Ti_K_anatase_broaden.ipynb`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/notebooks/spectra_files/anatase_exciting.txt` & `lightshow-0.1.3/notebooks/spectra_files/anatase_exciting.txt`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/notebooks/spectra_files/anatase_exp.txt` & `lightshow-0.1.3/notebooks/spectra_files/anatase_exp.txt`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/notebooks/spectra_files/anatase_ocean.txt` & `lightshow-0.1.3/notebooks/spectra_files/anatase_ocean.txt`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/notebooks/spectra_files/anatase_theory_FEFF.txt` & `lightshow-0.1.3/notebooks/spectra_files/anatase_theory_FEFF.txt`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/notebooks/spectra_files/anatase_theory_VASP.txt` & `lightshow-0.1.3/notebooks/spectra_files/anatase_theory_VASP.txt`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/notebooks/spectra_files/anatase_xspectra.txt` & `lightshow-0.1.3/notebooks/spectra_files/anatase_xspectra.txt`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/pyproject.toml` & `lightshow-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/scripts/README.rst` & `lightshow-0.1.3/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/scripts/build_docs.sh` & `lightshow-0.1.3/scripts/build_docs.sh`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/scripts/install.sh` & `lightshow-0.1.3/scripts/install.sh`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/scripts/update_version.sh` & `lightshow-0.1.3/scripts/update_version.sh`

 * *Files identical despite different names*

### Comparing `lightshow-0.1.2/PKG-INFO` & `lightshow-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightshow
-Version: 0.1.2
+Version: 0.1.3
 Summary: A one-stop-shop for writing computational spectroscopy input files
 Author: Benedikt Maurer, Fabien Peschel, Eli Stavitski, Xiaohui Qu, John T. Vinson, Christian Vorwerk
 Author-email: "Matthew R. Carbone" <mcarbone@bnl.gov>, Fanchen Meng <fmeng1@bnl.gov>, Deyu Lu <dlu@bnl.gov>
 Maintainer-email: "Matthew R. Carbone" <mcarbone@bnl.gov>, Fanchen Meng <fmeng1@bnl.gov>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -43,18 +43,20 @@
 
 ![sysfs line plot](https://raw.githubusercontent.com/AI-multimodal/Lightshow/master/docs/_static/images/lightshow.jpg)
 
 [![image](https://github.com/AI-multimodal/Lightshow/actions/workflows/ci.yml/badge.svg)](https://github.com/AI-multimodal/Lightshow/actions/workflows/ci.yml)
 [![image](https://codecov.io/gh/AI-multimodal/Lightshow/branch/master/graph/badge.svg?token=CW7BMFA5O7)](https://codecov.io/gh/AI-multimodal/Lightshow)
 [![image](https://app.codacy.com/project/badge/Grade/d31a4e18672c4d71bbaafa719181c140)](https://www.codacy.com/gh/AI-multimodal/Lightshow/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=AI-multimodal/Lightshow&amp;utm_campaign=Badge_Grade)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![python](https://img.shields.io/badge/-Python_>=3.7-blue?logo=python&logoColor=white)](https://github.com/pre-commit/pre-commit) <br>
+[![python](https://img.shields.io/badge/-Python_>=3.7-blue?logo=python&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![PRs](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/AI-multimodal/Lightshow/pulls) <br>
 [![image](https://joss.theoj.org/papers/a9cabcd7f4b85a926a797997c6622b43/status.svg)](https://joss.theoj.org/papers/a9cabcd7f4b85a926a797997c6622b43)
 [![image](https://zenodo.org/badge/DOI/10.48550/arXiv.2211.04452.svg)](https://doi.org/10.48550/arXiv.2211.04452)
 
+
 </div>
     
 ------------------------------------------------------------------------
 
 **Lightshow** is a Python library for easily generating computational
 spectroscopy input files.
 
@@ -92,16 +94,64 @@
 
 To install Lightshow, simply use `pip`
 
 ``` bash
 pip install lightshow
 ```
 
+Make sure you've set your Pymatgen legacy API key as well!
+
+```bash
+export PMG_API_KEY="your_legacy_materials_project_key"
+```
+
+(or preferably, add `PMG_API_KEY` to your bash profile).
+
 More details can be found at our [documentation](https://ai-multimodal.github.io/Lightshow/installation.html).
 
+## Development installation
+
+For developers: after cloning Lightshow locally, install `pre-commit` via
+
+```bash
+pip install pre-commit
+pre-commit
+pre-commit install
+```
+
+and check that the tests (below) work correctly.
+
+## Running tests
+
+For developers: tests can be run via `pytest`. After cloning, simply use
+
+```bash
+pytest lightshow/_tests
+```
+
+or with coverage
+
+```bash
+pytest -v --cov --cov-report xml lightshow/_tests
+```
+
+
+# Contributing 
+
+We welcome any and all contributions by the community, including pull requests, bug reports, etc.
+Please see our [contributing](https://github.com/AI-multimodal/Lightshow/blob/master/CONTRIBUTING.md) document for more details!
+
+## Adding new spectroscopy codes
+
+Adding new spectroscopy codes requires one to inherit the `_BaseParameters` class from `lightshow.parameters._base`.
+The new `Parameters(_BaseParameters)` object should have a `write()` method, which must take a target directory as an
+argument, as well as any other keyword arguments require to write the input file (most notably, the Pymatgen structure,
+either a unit or super cell). The `name` property must also be defined (corresponding to the name of the calculation,
+e.g. "VASP"). Take a look at the examples in the `lightshow.parameters` module for more details!
+
 
 # Funding acknowledgement
 
 This research is based upon work supported by the U.S. Department of
 Energy, Office of Science, Office Basic Energy Sciences, under Award
 Number FWP PS-030. This research used resources of the Center for
 Functional Nanomaterials (CFN), which is a U.S. Department of Energy
```

