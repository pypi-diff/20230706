# Comparing `tmp/autopacmen-Paulocracy-0.6.1.tar.gz` & `tmp/autopacmen-Paulocracy-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autopacmen-Paulocracy-0.6.1.tar", last modified: Mon Feb 22 16:19:34 2021, max compression
+gzip compressed data, was "autopacmen-Paulocracy-0.6.2.tar", last modified: Thu Jul  6 11:52:43 2023, max compression
```

## Comparing `autopacmen-Paulocracy-0.6.1.tar` & `autopacmen-Paulocracy-0.6.2.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-22 16:19:34.870655 autopacmen-Paulocracy-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (116)     6988 2021-02-22 16:19:34.870655 autopacmen-Paulocracy-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5918 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-22 16:19:34.866655 autopacmen-Paulocracy-0.6.1/autopacmen/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2990 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/analysis_fva_comparison.py
--rw-r--r--   0 runner    (1001) docker     (116)     2956 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/analysis_fva_prot_pool.py
--rw-r--r--   0 runner    (1001) docker     (116)     2994 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/data_create_combined_kcat_database.py
--rw-r--r--   0 runner    (1001) docker     (116)     2621 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/data_parse_bigg_metabolites_file.py
--rw-r--r--   0 runner    (1001) docker     (116)     3265 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/data_parse_brenda_json_for_model.py
--rw-r--r--   0 runner    (1001) docker     (116)     3687 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/data_parse_brenda_textfile.py
--rw-r--r--   0 runner    (1001) docker     (116)     3510 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/data_parse_sabio_rk_for_model.py
--rw-r--r--   0 runner    (1001) docker     (116)     4396 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/modeling_create_gecko_model.py
--rw-r--r--   0 runner    (1001) docker     (116)     4854 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/modeling_create_smoment_model.py
--rw-r--r--   0 runner    (1001) docker     (116)     2764 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/modeling_get_initial_spreadsheets.py
--rw-r--r--   0 runner    (1001) docker     (116)     2936 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/modeling_get_protein_mass_mapping.py
--rw-r--r--   0 runner    (1001) docker     (116)     5836 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/modeling_get_reactions_kcat_mapping.py
--rw-r--r--   0 runner    (1001) docker     (116)     4064 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/optimization_apply_manual_changes.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-22 16:19:34.870655 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3296 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/apply_manual_changes.py
--rw-r--r--   0 runner    (1001) docker     (116)     6273 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/create_combined_kcat_database.py
--rw-r--r--   0 runner    (1001) docker     (116)    12912 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/create_gecko_model_reaction_wise.py
--rw-r--r--   0 runner    (1001) docker     (116)    17394 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/create_smoment_model_reaction_wise.py
--rw-r--r--   0 runner    (1001) docker     (116)     3113 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/fva_comparison.py
--rw-r--r--   0 runner    (1001) docker     (116)     2328 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/fva_prot_pool.py
--rw-r--r--   0 runner    (1001) docker     (116)     8290 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/get_differential_reactions.py
--rw-r--r--   0 runner    (1001) docker     (116)    14397 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/get_initial_spreadsheets.py
--rw-r--r--   0 runner    (1001) docker     (116)     7251 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/get_protein_mass_mapping.py
--rw-r--r--   0 runner    (1001) docker     (116)    23390 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/get_reactions_kcat_mapping.py
--rw-r--r--   0 runner    (1001) docker     (116)    23905 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/helper_create_model.py
--rw-r--r--   0 runner    (1001) docker     (116)    14180 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/helper_general.py
--rw-r--r--   0 runner    (1001) docker     (116)     4434 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/kegg.py
--rw-r--r--   0 runner    (1001) docker     (116)     7669 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/ncbi_taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (116)     3002 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/parse_bigg_metabolites_file.py
--rw-r--r--   0 runner    (1001) docker     (116)     6354 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/parse_brenda_json_for_model.py
--rw-r--r--   0 runner    (1001) docker     (116)     8641 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/parse_brenda_textfile.py
--rw-r--r--   0 runner    (1001) docker     (116)    23016 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/parse_sabio_rk.py
--rw-r--r--   0 runner    (1001) docker     (116)     3454 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/parse_sabio_rk_for_model.py
--rw-r--r--   0 runner    (1001) docker     (116)     5574 2021-02-22 16:19:25.000000 autopacmen-Paulocracy-0.6.1/autopacmen/submodules/reaction_flux_control_by_scenario.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-22 16:19:34.870655 autopacmen-Paulocracy-0.6.1/autopacmen_Paulocracy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     6988 2021-02-22 16:19:34.000000 autopacmen-Paulocracy-0.6.1/autopacmen_Paulocracy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1840 2021-02-22 16:19:34.000000 autopacmen-Paulocracy-0.6.1/autopacmen_Paulocracy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-22 16:19:34.000000 autopacmen-Paulocracy-0.6.1/autopacmen_Paulocracy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       58 2021-02-22 16:19:34.000000 autopacmen-Paulocracy-0.6.1/autopacmen_Paulocracy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       11 2021-02-22 16:19:34.000000 autopacmen-Paulocracy-0.6.1/autopacmen_Paulocracy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-02-22 16:19:34.870655 autopacmen-Paulocracy-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      837 2021-02-22 16:19:26.000000 autopacmen-Paulocracy-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:43.887524 autopacmen-Paulocracy-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-07-06 11:52:43.887524 autopacmen-Paulocracy-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:43.883524 autopacmen-Paulocracy-0.6.2/autopacmen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/analysis_fva_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/analysis_fva_prot_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2994 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/data_create_combined_kcat_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/data_parse_bigg_metabolites_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/data_parse_brenda_json_for_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/data_parse_brenda_textfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/data_parse_sabio_rk_for_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/modeling_create_gecko_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/modeling_create_smoment_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/modeling_get_initial_spreadsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/modeling_get_protein_mass_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/modeling_get_reactions_kcat_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/optimization_apply_manual_changes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:43.887524 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/apply_manual_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/create_combined_kcat_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/create_gecko_model_reaction_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17394 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/create_smoment_model_reaction_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/fva_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/fva_prot_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/get_differential_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14577 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/get_initial_spreadsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/get_protein_mass_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23390 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/get_reactions_kcat_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/helper_create_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14180 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/helper_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/kegg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/ncbi_taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/parse_bigg_metabolites_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/parse_brenda_json_for_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/parse_brenda_textfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23016 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/parse_sabio_rk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/parse_sabio_rk_for_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/autopacmen/submodules/reaction_flux_control_by_scenario.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:52:43.887524 autopacmen-Paulocracy-0.6.2/autopacmen_Paulocracy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-07-06 11:52:43.000000 autopacmen-Paulocracy-0.6.2/autopacmen_Paulocracy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-06 11:52:43.000000 autopacmen-Paulocracy-0.6.2/autopacmen_Paulocracy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:52:43.000000 autopacmen-Paulocracy-0.6.2/autopacmen_Paulocracy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 11:52:43.000000 autopacmen-Paulocracy-0.6.2/autopacmen_Paulocracy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-06 11:52:43.000000 autopacmen-Paulocracy-0.6.2/autopacmen_Paulocracy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 11:52:43.887524 autopacmen-Paulocracy-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-06 11:52:32.000000 autopacmen-Paulocracy-0.6.2/setup.py
```

### Comparing `autopacmen-Paulocracy-0.6.1/PKG-INFO` & `autopacmen-Paulocracy-0.6.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,98 @@
 Metadata-Version: 2.1
 Name: autopacmen-Paulocracy
-Version: 0.6.1
+Version: 0.6.2
 Summary: The AutoPACMEN package
 Home-page: https://github.com/Paulocracy/autopacmen
 Author: Paulocracy
 Author-email: bekiaris@mpi-magdeburg.mpg.de
-License: UNKNOWN
-Description: [![PyPI version](https://badge.fury.io/py/autopacmen-Paulocracy.svg)](https://badge.fury.io/py/autopacmen-Paulocracy)
-        
-        # AutoPACMEN (Automatic integration of Protein Allocation Constraints for stoichiometric MEtabolic Networks)
-        
-        
-        ## General Description
-        
-        AutoPACMEN allows one to apply the sMOMENT method of automatically expanding a stoichiometric metabolic
-        model with protein allocation constraints (as described in further detail in [Bekiaris & Klamt, 2020](#autopacmens-publication)).
-        
-        This repository of AutoPACMEN consists of three source code parts:
-        
-        1) The AutoPACMEN Model Generator, implemented as the Python module "autopacmen-Paulocracy" module, which provides a mostly automated way to generate enzyme-constraint-enhanced stoichiometric metabolic models, including an automatic retrieval of k<sub>cat</sub> values. It is primarily dependent on [cobrapy](https://github.com/opencobra/cobrapy).
-        <br>→This module can be found in the "autopacmen" subfolder.
-        
-        2) An optional mixed Python 3/MATLAB AutoPACMEN Model Calibrator whose MATLAB parts primarily use [CellNetAnalyzer](https://www2.mpi-magdeburg.mpg.de/projects/cna/cna.html) and which allows one to optimize given protein allocation constraints in order to get a better fit with <i>in vivo</i> data.
-        <br>→The Python parts can be found in the "autopacmen" subfolder as described in AutoPACMEN's manual,the MATLAB parts can be found in the subfolder "AutoPACMEN_Model_Calibrator_MATLAB".
-        
-        3) The exemplary usage of autopacmen-Paulocracy and the Model Calibrator resulting in the enzyme-constraint-enhanced model iJO1366*, as described in Supplementary File 1 of AutoPACMEN's publication. The final iJO1366* model is stored in a ready-to-use SBML form as "./iJO1366star/ec_model_2019_06_25_output_optimization/iJO1366star.xml".
-        <br>→The relevant scripts and data can be found in the "iJO1366" subfolder. <b>Note:</b> As it has a huge file size, the obligatory downloaded complete BRENDA text file brenda_downloads.txt (as described in AutoPACMEN's manual) is not included here. Instead, it can be downloaded from BRENDA's web site.
-        
-        ## Documentation
-        
-        The combined manual for autopacmen-Paulocracy and the Model Calibrator can be found as "manual.pdf" or LibreOffice-compatible "manual.odt" in the "docs" subfolder folder.
-        It explains the manual installation process (without pip, see next chapter for the installation with pip) and usage of AutoPACMEN in detail.
-        
-        An additional HTML documentation of the source code of AutoPACMEN's Python modules can be found under the "autopacmen" folder's subfolder "html".
-        This HTML documentation was automatically generated using [pdoc3](https://pdoc3.github.io/pdoc/) (link accessed on Oct 30, 2019).
-        The HTML documentation's starting point is "index.html" in the "./autopacmen/html/autopacmen" subfolder.
-        
-        If you are particularily interested in the generation of k<sub>cat</sub> databases from BRENDA and SABIO-RK, look up
-        the scripts "data_parse_brenda_textfile.py", "data_parse_sabio_rk_for_model.py" as well as the combining
-        script "data_create_combined_kcat_database.py". These scripts create JSON files with the k<sub>cat</sub> data from these
-        databases with EC number, organism and substrate information. An exemplary created database with BRENDA is
-        "kcat_database_brenda" in the main folder's  subfolder "./iJO1366star/ec_model_2019_06_25_output", a database with SABIO-RK is
-        "kcat_database_sabio_rk" in the same subfolder.
-        
-        
-        ## Installation of autopacmen-Paulocracy using pip
-        
-        You can install autopacmen-Paulocracy [from PyPI](https://pypi.org/project/autopacmen-Paulocracy/) using pip as follows:
-        <pre>
-        pip install autopacmen-Paulocracy
-        </pre>
-        
-        autopacmen-Paulocracy requires Python >=3.7 for its Python parts, and MATLAB >=2017a for its optional Model Calibrator
-        MATLAB scripts.
-        
-        
-        ## Structure of AutoPACMEN's source code
-        
-        All relevant scripts of autopacmen-Paulocracy are in the "autopacmen" main folder.
-        
-        In this main folder, the scripts which start with "analysis_", "data_" and "modeling_" are command-line interfaces (CLI)
-        for AutoPACMEN's Python modules. These Python modules can be found the main folder's "submodules" subfolder.
-        
-        The subfolder "AutoPACMEN_Model_Calibrator_MATLAB" contains the Model Calibrator's MATLAB parts.
-        
-        All scripts and folders within "iJO1366star" are part of the generation and analysis of iJO1366* (see AutoPACMEN's publication for more about it). From these scripts, these ones
-        starting with "./iJO1366star/ec_model_2019_06_25_figure" create either a full figure or data for a figure used in AutoPACMEN's publication.
-        
-        The main script for the generation of the uncalibrated iJO1366* model is "./iJO1366star/ec_model_2019_06_25_sMOMENT_iJO_CREATION.py" in the "iJO1366" subfolder. This
-        main script uses AutoPACMEN's functionalities as Python modules. The commented steps in this script correspond to the steps described in supplementary
-        File 1 of (Bekiaris & Klamt, in submission).
-        
-        The "iJO1366star" folder's subfolder "iJOstar_MCS_analysis_scripts" contains the scripts used for the computation and the analysis of the published Minimal Cut Set enumeration
-        with iJO1366 and iJO1366*.
-        
-        AutoPACMEN creates a cache of SABIO-RK, NCBI TAXONOMY and UniProt data in the "_cache" main folder's subfolder.  In the current state, the cache is the one
-        from AutoPACMEN's run for iJO1366* around the 25th of June 2019.
-        
-        
-        ## AutoPACMEN's Publication
-        
-        * Bekiaris, P.S., Klamt, S. Automatic construction of metabolic models with enzyme constraints. <i>BMC Bioinformatics</i> <b>21</b>, 19 (2020). [https://doi.org/10.1186/s12859-019-3329-9](https://doi.org/10.1186/s12859-019-3329-9)
-        
-        ## License
-        
-        This project is free and open-source, using the Apache License Version 2.0.
-        
-        
-        ## External sources
-        
-        External sources which are included in this package are given in the respective SOURCES.txt files.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/autopacmen-Paulocracy.svg)](https://badge.fury.io/py/autopacmen-Paulocracy)
+
+# AutoPACMEN (Automatic integration of Protein Allocation Constraints for stoichiometric MEtabolic Networks)
+
+
+## General Description
+
+AutoPACMEN allows one to apply the sMOMENT method of automatically expanding a stoichiometric metabolic
+model with protein allocation constraints (as described in further detail in [Bekiaris & Klamt, 2020](#autopacmens-publication)).
+
+This repository of AutoPACMEN consists of three source code parts:
+
+1) The AutoPACMEN Model Generator, implemented as the Python module "autopacmen-Paulocracy" module, which provides a mostly automated way to generate enzyme-constraint-enhanced stoichiometric metabolic models, including an automatic retrieval of k<sub>cat</sub> values. It is primarily dependent on [cobrapy](https://github.com/opencobra/cobrapy).
+<br>→This module can be found in the "autopacmen" subfolder.
+
+2) An optional mixed Python 3/MATLAB AutoPACMEN Model Calibrator whose MATLAB parts primarily use [CellNetAnalyzer](https://www2.mpi-magdeburg.mpg.de/projects/cna/cna.html) and which allows one to optimize given protein allocation constraints in order to get a better fit with <i>in vivo</i> data.
+<br>→The Python parts can be found in the "autopacmen" subfolder as described in AutoPACMEN's manual,the MATLAB parts can be found in the subfolder "AutoPACMEN_Model_Calibrator_MATLAB".
+
+3) The exemplary usage of autopacmen-Paulocracy and the Model Calibrator resulting in the enzyme-constraint-enhanced model iJO1366*, as described in Supplementary File 1 of AutoPACMEN's publication. The final iJO1366* model is stored in a ready-to-use SBML form as "./iJO1366star/ec_model_2019_06_25_output_optimization/iJO1366star.xml".
+<br>→The relevant scripts and data can be found in the "iJO1366" subfolder. <b>Note:</b> As it has a huge file size, the obligatory downloaded complete BRENDA text file brenda_downloads.txt (as described in AutoPACMEN's manual) is not included here. Instead, it can be downloaded from BRENDA's web site.
+
+## Documentation
+
+The combined manual for autopacmen-Paulocracy and the Model Calibrator can be found as "manual.pdf" or LibreOffice-compatible "manual.odt" in the "docs" subfolder folder.
+It explains the manual installation process (without pip, see next chapter for the installation with pip) and usage of AutoPACMEN in detail.
+
+An additional HTML documentation of the source code of AutoPACMEN's Python modules can be found under the "autopacmen" folder's subfolder "html".
+This HTML documentation was automatically generated using [pdoc3](https://pdoc3.github.io/pdoc/) (link accessed on Oct 30, 2019).
+The HTML documentation's starting point is "index.html" in the "./autopacmen/html/autopacmen" subfolder.
+
+If you are particularily interested in the generation of k<sub>cat</sub> databases from BRENDA and SABIO-RK, look up
+the scripts "data_parse_brenda_textfile.py", "data_parse_sabio_rk_for_model.py" as well as the combining
+script "data_create_combined_kcat_database.py". These scripts create JSON files with the k<sub>cat</sub> data from these
+databases with EC number, organism and substrate information. An exemplary created database with BRENDA is
+"kcat_database_brenda" in the main folder's  subfolder "./iJO1366star/ec_model_2019_06_25_output", a database with SABIO-RK is
+"kcat_database_sabio_rk" in the same subfolder.
+
+
+## Installation of autopacmen-Paulocracy using pip
+
+You can install autopacmen-Paulocracy [from PyPI](https://pypi.org/project/autopacmen-Paulocracy/) using pip as follows:
+<pre>
+pip install autopacmen-Paulocracy
+</pre>
+
+autopacmen-Paulocracy requires Python >=3.7 for its Python parts, and MATLAB >=2017a for its optional Model Calibrator
+MATLAB scripts.
+
+
+## Structure of AutoPACMEN's source code
+
+All relevant scripts of autopacmen-Paulocracy are in the "autopacmen" main folder.
+
+In this main folder, the scripts which start with "analysis_", "data_" and "modeling_" are command-line interfaces (CLI)
+for AutoPACMEN's Python modules. These Python modules can be found the main folder's "submodules" subfolder.
+
+The subfolder "AutoPACMEN_Model_Calibrator_MATLAB" contains the Model Calibrator's MATLAB parts.
+
+All scripts and folders within "iJO1366star" are part of the generation and analysis of iJO1366* (see AutoPACMEN's publication for more about it). From these scripts, these ones
+starting with "./iJO1366star/ec_model_2019_06_25_figure" create either a full figure or data for a figure used in AutoPACMEN's publication.
+
+The main script for the generation of the uncalibrated iJO1366* model is "./iJO1366star/ec_model_2019_06_25_sMOMENT_iJO_CREATION.py" in the "iJO1366" subfolder. This
+main script uses AutoPACMEN's functionalities as Python modules. The commented steps in this script correspond to the steps described in supplementary
+File 1 of (Bekiaris & Klamt, in submission).
+
+The "iJO1366star" folder's subfolder "iJOstar_MCS_analysis_scripts" contains the scripts used for the computation and the analysis of the published Minimal Cut Set enumeration
+with iJO1366 and iJO1366*.
+
+AutoPACMEN creates a cache of SABIO-RK, NCBI TAXONOMY and UniProt data in the "_cache" main folder's subfolder.  In the current state, the cache is the one
+from AutoPACMEN's run for iJO1366* around the 25th of June 2019.
+
+
+## AutoPACMEN's Publication
+
+* Bekiaris, P.S., Klamt, S. Automatic construction of metabolic models with enzyme constraints. <i>BMC Bioinformatics</i> <b>21</b>, 19 (2020). [https://doi.org/10.1186/s12859-019-3329-9](https://doi.org/10.1186/s12859-019-3329-9)
+
+## License
+
+This project is free and open-source, using the Apache License Version 2.0.
+
+
+## External sources
+
+External sources which are included in this package are given in the respective SOURCES.txt files.
```

### Comparing `autopacmen-Paulocracy-0.6.1/README.md` & `autopacmen-Paulocracy-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/analysis_fva_comparison.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/analysis_fva_comparison.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/analysis_fva_prot_pool.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/analysis_fva_prot_pool.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/data_create_combined_kcat_database.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/data_create_combined_kcat_database.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/data_parse_bigg_metabolites_file.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/data_parse_bigg_metabolites_file.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/data_parse_brenda_json_for_model.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/data_parse_brenda_json_for_model.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/data_parse_brenda_textfile.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/data_parse_brenda_textfile.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/data_parse_sabio_rk_for_model.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/data_parse_sabio_rk_for_model.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/modeling_create_gecko_model.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/modeling_create_gecko_model.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/modeling_create_smoment_model.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/modeling_create_smoment_model.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/modeling_get_initial_spreadsheets.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/modeling_get_initial_spreadsheets.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/modeling_get_protein_mass_mapping.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/modeling_get_protein_mass_mapping.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/modeling_get_reactions_kcat_mapping.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/modeling_get_reactions_kcat_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 @click.option("--kcat_database_path",
               required=True,
               type=click.Path(exists=True, file_okay=True, dir_okay=True),
               prompt="kcat database path",
               help="Full path to the SABIO-RK&BRENDA kcat<->reaction JSON which was creates using data_create_combined_kcat_database.py")
 @click.option("--protein_kcat_database_path",
               required=True,
-              type=click.Path(exists=True, file_okay=True, dir_okay=True),
+              type=str,
               default="",
               prompt="protein kcat database path",
               help="Full path to the custom user-defined kcat<->protein JSON. It must be a dictionary containing the protein names"
                    "(as given in the metabolic network's gene rules) as keys and associated kcats as children. See this script's description for more."
                    "Default is '', which means that no user-defined database is given.")
 @click.option("--type_of_kcat_selection",
               required=True,
```

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/optimization_apply_manual_changes.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/optimization_apply_manual_changes.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/submodules/apply_manual_changes.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/submodules/apply_manual_changes.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/submodules/create_combined_kcat_database.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/submodules/create_combined_kcat_database.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/submodules/create_gecko_model_reaction_wise.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/submodules/create_gecko_model_reaction_wise.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/submodules/create_smoment_model_reaction_wise.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/submodules/create_smoment_model_reaction_wise.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/submodules/fva_comparison.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/submodules/fva_comparison.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/submodules/fva_prot_pool.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/submodules/fva_prot_pool.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/submodules/get_differential_reactions.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/submodules/get_differential_reactions.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/submodules/get_initial_spreadsheets.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/submodules/get_initial_spreadsheets.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,45 +22,48 @@
 workflow, after the wanted SBML model was selected and generated.
 """
 
 # IMPORTS
 # External modules
 import cobra
 import xlsxwriter
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List
 # Internal modules
 from .kegg import kegg_rest_get_batch
 from .helper_general import standardize_folder
 
 
 # INTERNAL FUNCTIONS SECTION
 def _gene_rule_as_list(gene_rule: str) -> List[Any]:
     """Returns a given string gene rule in list form.
 
-    I.e. (b0001 or b0002) and b0003 is returned as
+    I.e. (b0001 and b0002) or b0003 is returned as
     [["b0001", "b0002"], "b0003"]
 
     Arguments:
     *gene_rule: str ~ The gene rule which shall be converted into the list form.
     """
-    # Gene rules: Only ) or (, (in blocks only and); No ) and (
-    gene_rule_blocks = gene_rule.split(" ) or ( ")
-    gene_rule_blocks = [x.replace("(", "").replace(")", "") for x in gene_rule_blocks]
-    gene_rules_array: List[Union[str, List[str]]] = []
-    for block in gene_rule_blocks:
-        if " or " in block:
-            block_list = block.split(" or ")
-            block_list = [x.lstrip().rstrip() for x in block_list]
-            gene_rules_array += block_list
-        elif " and " in block:
-            block_list = block.split(" and ")
-            block_list = [x.lstrip().rstrip() for x in block_list]
-            gene_rules_array.append(block_list)
-        else:  # single enzyme
-            gene_rules_array.append(block)
+    gene_rules_array: List[Any] = []
+    if (" or " in gene_rule) and (" and " in gene_rule):
+        gene_rule_split = gene_rule.split("or")
+        gene_rule_split = [x.replace("(", "").replace(")", "") for x in gene_rule_split]
+        for part in gene_rule_split:
+            and_list = part.split(" and ")
+            and_list = [x.replace(" ", "") for x in and_list]
+            gene_rules_array.append(and_list)
+    elif (" or " in gene_rule):
+        gene_rule_split = gene_rule.split(" or ")
+        gene_rule_split = [x.replace("(", "").replace(")", "").replace(" ", "") for x in gene_rule_split]
+        for part in gene_rule_split:
+            gene_rules_array.append(part)
+    else:  # if ("and" in gene_rule):
+        gene_rule_split = gene_rule.split(" and ")
+        gene_rule_split = [x.replace("(", "").replace(")", "").replace(" ", "") for x in gene_rule_split]
+        gene_rules_array.append(gene_rule_split)
+
     return gene_rules_array
 
 
 # PUBLIC FUNCTIONS SECTION
 def get_initial_spreadsheets(model: cobra.Model, project_folder: str, project_name: str) -> None:
     """Creates a number of initially needed XLSX spreadsheets in the given folder.
 
@@ -235,15 +238,15 @@
         worksheet.write(row, 1, compartment_name)
         worksheet.write(row, 2, "NA")
         worksheet.write(row, 3, "NA")
         row += 1
     workbook.close()
 
     # Protein data XLSX :D
-    print("NOTE: "+project_name+"_protein_data.xlsx has as default value for the enzyme pool P 0.095 mmol/gDW.")
+    print("NOTE: "+project_name+"_protein_data.xlsx has as default value for the enzyme pool P 0.095 g/gDW.")
     print("Please adjust the value accordingly for your model!")
     workbook = xlsxwriter.Workbook(basepath+"_protein_data.xlsx")
     worksheet = workbook.add_worksheet("Total protein data")
     worksheet.write(0, 0, "Total protein content [g/gDW]:")
     worksheet.write(0, 1, .095)
     worksheet.write(1, 0, "Fraction of masses of model-included enzymes in comparison to all enzymes (0.0 to 1.0):")
     worksheet.write(1, 1, 1.0)
```

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/submodules/get_protein_mass_mapping.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/submodules/get_protein_mass_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             batch_start += batch_size
             continue
 
         # Create the UniProt query for the batch
         # With 'OR', all given IDs are searched, and subsequently in this script,
         # the right associated masses are being picked.
         query = " OR ".join(batch)
-        uniprot_query_url = f"https://www.uniprot.org/uniprot/?query={query}&format=tab&columns=id,mass"
+        uniprot_query_url = f"https://rest.uniprot.org/uniprotkb/search?query=accession:{query}&format=tsv&fields=accession,mass"
         print(f"UniProt batch search for: {query}")
 
         # Call UniProt's API :-)
         uniprot_data = requests.get(uniprot_query_url).text.split("\n")
         # Wait in order to cool down their server :-)
         time.sleep(2.0)
```

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/submodules/get_reactions_kcat_mapping.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/submodules/get_reactions_kcat_mapping.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/submodules/helper_create_model.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/submodules/helper_create_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
                 reaction_id_gene_rules_protein_stoichiometry_mapping[new_reaction.id][element] = {
                 }
                 reaction_id_gene_rules_protein_stoichiometry_mapping[new_reaction.id][element][element] = \
                     reaction_id_gene_rules_protein_stoichiometry_mapping[reaction_id][element][element]
                 if len(new_gene_reaction_rule) > 0:
                     new_gene_reaction_rule += " or "
                 new_gene_reaction_rule += element
-        model.gene_reaction_rule = new_gene_reaction_rule
+        new_reaction.gene_reaction_rule = new_gene_reaction_rule
 
         if add_arm_reaction:
             if reaction.lower_bound >= 0:
                 new_reaction.add_metabolites({arm_metabolite: 1})
             else:
                 new_reaction.add_metabolites(
                     {arm_metabolite_fwd: 1, arm_metabolite_rev: 1})
```

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/submodules/helper_general.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/submodules/helper_general.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/submodules/kegg.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/submodules/kegg.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/submodules/ncbi_taxonomy.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/submodules/ncbi_taxonomy.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/submodules/parse_bigg_metabolites_file.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/submodules/parse_bigg_metabolites_file.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/submodules/parse_brenda_json_for_model.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/submodules/parse_brenda_json_for_model.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/submodules/parse_brenda_textfile.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/submodules/parse_brenda_textfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,16 +160,18 @@
 
         reference_number_organism_mapping = {}
         organism_lines = ec_number_organsism_lines_mapping[ec_number]
         for organism_line in organism_lines:
             reference_number = organism_line.split("#")[1]
             organism_line_split_first_part = organism_line.split("# ")[1]
             organism_line_split = organism_line_split_first_part.split(" ")
-            organism_line_split = [
-                x for x in organism_line_split if len(x) > 0]
+            
+            for part in organism_line_split:
+                if len(part) > 0:
+                    part = part.replace("\t", "")
 
             end = 1
             for part in organism_line_split:
                 # Some organism names contain their SwissProt or UniProt ID,
                 # since we don't nned them they are excluded
                 if ("swissprot" in part.lower()) or \
                     (part.lower() == "and") or \
```

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/submodules/parse_sabio_rk.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/submodules/parse_sabio_rk.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/submodules/parse_sabio_rk_for_model.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/submodules/parse_sabio_rk_for_model.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen/submodules/reaction_flux_control_by_scenario.py` & `autopacmen-Paulocracy-0.6.2/autopacmen/submodules/reaction_flux_control_by_scenario.py`

 * *Files identical despite different names*

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen_Paulocracy.egg-info/PKG-INFO` & `autopacmen-Paulocracy-0.6.2/autopacmen_Paulocracy.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,99 +1,98 @@
 Metadata-Version: 2.1
 Name: autopacmen-Paulocracy
-Version: 0.6.1
+Version: 0.6.2
 Summary: The AutoPACMEN package
 Home-page: https://github.com/Paulocracy/autopacmen
 Author: Paulocracy
 Author-email: bekiaris@mpi-magdeburg.mpg.de
-License: UNKNOWN
-Description: [![PyPI version](https://badge.fury.io/py/autopacmen-Paulocracy.svg)](https://badge.fury.io/py/autopacmen-Paulocracy)
-        
-        # AutoPACMEN (Automatic integration of Protein Allocation Constraints for stoichiometric MEtabolic Networks)
-        
-        
-        ## General Description
-        
-        AutoPACMEN allows one to apply the sMOMENT method of automatically expanding a stoichiometric metabolic
-        model with protein allocation constraints (as described in further detail in [Bekiaris & Klamt, 2020](#autopacmens-publication)).
-        
-        This repository of AutoPACMEN consists of three source code parts:
-        
-        1) The AutoPACMEN Model Generator, implemented as the Python module "autopacmen-Paulocracy" module, which provides a mostly automated way to generate enzyme-constraint-enhanced stoichiometric metabolic models, including an automatic retrieval of k<sub>cat</sub> values. It is primarily dependent on [cobrapy](https://github.com/opencobra/cobrapy).
-        <br>→This module can be found in the "autopacmen" subfolder.
-        
-        2) An optional mixed Python 3/MATLAB AutoPACMEN Model Calibrator whose MATLAB parts primarily use [CellNetAnalyzer](https://www2.mpi-magdeburg.mpg.de/projects/cna/cna.html) and which allows one to optimize given protein allocation constraints in order to get a better fit with <i>in vivo</i> data.
-        <br>→The Python parts can be found in the "autopacmen" subfolder as described in AutoPACMEN's manual,the MATLAB parts can be found in the subfolder "AutoPACMEN_Model_Calibrator_MATLAB".
-        
-        3) The exemplary usage of autopacmen-Paulocracy and the Model Calibrator resulting in the enzyme-constraint-enhanced model iJO1366*, as described in Supplementary File 1 of AutoPACMEN's publication. The final iJO1366* model is stored in a ready-to-use SBML form as "./iJO1366star/ec_model_2019_06_25_output_optimization/iJO1366star.xml".
-        <br>→The relevant scripts and data can be found in the "iJO1366" subfolder. <b>Note:</b> As it has a huge file size, the obligatory downloaded complete BRENDA text file brenda_downloads.txt (as described in AutoPACMEN's manual) is not included here. Instead, it can be downloaded from BRENDA's web site.
-        
-        ## Documentation
-        
-        The combined manual for autopacmen-Paulocracy and the Model Calibrator can be found as "manual.pdf" or LibreOffice-compatible "manual.odt" in the "docs" subfolder folder.
-        It explains the manual installation process (without pip, see next chapter for the installation with pip) and usage of AutoPACMEN in detail.
-        
-        An additional HTML documentation of the source code of AutoPACMEN's Python modules can be found under the "autopacmen" folder's subfolder "html".
-        This HTML documentation was automatically generated using [pdoc3](https://pdoc3.github.io/pdoc/) (link accessed on Oct 30, 2019).
-        The HTML documentation's starting point is "index.html" in the "./autopacmen/html/autopacmen" subfolder.
-        
-        If you are particularily interested in the generation of k<sub>cat</sub> databases from BRENDA and SABIO-RK, look up
-        the scripts "data_parse_brenda_textfile.py", "data_parse_sabio_rk_for_model.py" as well as the combining
-        script "data_create_combined_kcat_database.py". These scripts create JSON files with the k<sub>cat</sub> data from these
-        databases with EC number, organism and substrate information. An exemplary created database with BRENDA is
-        "kcat_database_brenda" in the main folder's  subfolder "./iJO1366star/ec_model_2019_06_25_output", a database with SABIO-RK is
-        "kcat_database_sabio_rk" in the same subfolder.
-        
-        
-        ## Installation of autopacmen-Paulocracy using pip
-        
-        You can install autopacmen-Paulocracy [from PyPI](https://pypi.org/project/autopacmen-Paulocracy/) using pip as follows:
-        <pre>
-        pip install autopacmen-Paulocracy
-        </pre>
-        
-        autopacmen-Paulocracy requires Python >=3.7 for its Python parts, and MATLAB >=2017a for its optional Model Calibrator
-        MATLAB scripts.
-        
-        
-        ## Structure of AutoPACMEN's source code
-        
-        All relevant scripts of autopacmen-Paulocracy are in the "autopacmen" main folder.
-        
-        In this main folder, the scripts which start with "analysis_", "data_" and "modeling_" are command-line interfaces (CLI)
-        for AutoPACMEN's Python modules. These Python modules can be found the main folder's "submodules" subfolder.
-        
-        The subfolder "AutoPACMEN_Model_Calibrator_MATLAB" contains the Model Calibrator's MATLAB parts.
-        
-        All scripts and folders within "iJO1366star" are part of the generation and analysis of iJO1366* (see AutoPACMEN's publication for more about it). From these scripts, these ones
-        starting with "./iJO1366star/ec_model_2019_06_25_figure" create either a full figure or data for a figure used in AutoPACMEN's publication.
-        
-        The main script for the generation of the uncalibrated iJO1366* model is "./iJO1366star/ec_model_2019_06_25_sMOMENT_iJO_CREATION.py" in the "iJO1366" subfolder. This
-        main script uses AutoPACMEN's functionalities as Python modules. The commented steps in this script correspond to the steps described in supplementary
-        File 1 of (Bekiaris & Klamt, in submission).
-        
-        The "iJO1366star" folder's subfolder "iJOstar_MCS_analysis_scripts" contains the scripts used for the computation and the analysis of the published Minimal Cut Set enumeration
-        with iJO1366 and iJO1366*.
-        
-        AutoPACMEN creates a cache of SABIO-RK, NCBI TAXONOMY and UniProt data in the "_cache" main folder's subfolder.  In the current state, the cache is the one
-        from AutoPACMEN's run for iJO1366* around the 25th of June 2019.
-        
-        
-        ## AutoPACMEN's Publication
-        
-        * Bekiaris, P.S., Klamt, S. Automatic construction of metabolic models with enzyme constraints. <i>BMC Bioinformatics</i> <b>21</b>, 19 (2020). [https://doi.org/10.1186/s12859-019-3329-9](https://doi.org/10.1186/s12859-019-3329-9)
-        
-        ## License
-        
-        This project is free and open-source, using the Apache License Version 2.0.
-        
-        
-        ## External sources
-        
-        External sources which are included in this package are given in the respective SOURCES.txt files.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![PyPI version](https://badge.fury.io/py/autopacmen-Paulocracy.svg)](https://badge.fury.io/py/autopacmen-Paulocracy)
+
+# AutoPACMEN (Automatic integration of Protein Allocation Constraints for stoichiometric MEtabolic Networks)
+
+
+## General Description
+
+AutoPACMEN allows one to apply the sMOMENT method of automatically expanding a stoichiometric metabolic
+model with protein allocation constraints (as described in further detail in [Bekiaris & Klamt, 2020](#autopacmens-publication)).
+
+This repository of AutoPACMEN consists of three source code parts:
+
+1) The AutoPACMEN Model Generator, implemented as the Python module "autopacmen-Paulocracy" module, which provides a mostly automated way to generate enzyme-constraint-enhanced stoichiometric metabolic models, including an automatic retrieval of k<sub>cat</sub> values. It is primarily dependent on [cobrapy](https://github.com/opencobra/cobrapy).
+<br>→This module can be found in the "autopacmen" subfolder.
+
+2) An optional mixed Python 3/MATLAB AutoPACMEN Model Calibrator whose MATLAB parts primarily use [CellNetAnalyzer](https://www2.mpi-magdeburg.mpg.de/projects/cna/cna.html) and which allows one to optimize given protein allocation constraints in order to get a better fit with <i>in vivo</i> data.
+<br>→The Python parts can be found in the "autopacmen" subfolder as described in AutoPACMEN's manual,the MATLAB parts can be found in the subfolder "AutoPACMEN_Model_Calibrator_MATLAB".
+
+3) The exemplary usage of autopacmen-Paulocracy and the Model Calibrator resulting in the enzyme-constraint-enhanced model iJO1366*, as described in Supplementary File 1 of AutoPACMEN's publication. The final iJO1366* model is stored in a ready-to-use SBML form as "./iJO1366star/ec_model_2019_06_25_output_optimization/iJO1366star.xml".
+<br>→The relevant scripts and data can be found in the "iJO1366" subfolder. <b>Note:</b> As it has a huge file size, the obligatory downloaded complete BRENDA text file brenda_downloads.txt (as described in AutoPACMEN's manual) is not included here. Instead, it can be downloaded from BRENDA's web site.
+
+## Documentation
+
+The combined manual for autopacmen-Paulocracy and the Model Calibrator can be found as "manual.pdf" or LibreOffice-compatible "manual.odt" in the "docs" subfolder folder.
+It explains the manual installation process (without pip, see next chapter for the installation with pip) and usage of AutoPACMEN in detail.
+
+An additional HTML documentation of the source code of AutoPACMEN's Python modules can be found under the "autopacmen" folder's subfolder "html".
+This HTML documentation was automatically generated using [pdoc3](https://pdoc3.github.io/pdoc/) (link accessed on Oct 30, 2019).
+The HTML documentation's starting point is "index.html" in the "./autopacmen/html/autopacmen" subfolder.
+
+If you are particularily interested in the generation of k<sub>cat</sub> databases from BRENDA and SABIO-RK, look up
+the scripts "data_parse_brenda_textfile.py", "data_parse_sabio_rk_for_model.py" as well as the combining
+script "data_create_combined_kcat_database.py". These scripts create JSON files with the k<sub>cat</sub> data from these
+databases with EC number, organism and substrate information. An exemplary created database with BRENDA is
+"kcat_database_brenda" in the main folder's  subfolder "./iJO1366star/ec_model_2019_06_25_output", a database with SABIO-RK is
+"kcat_database_sabio_rk" in the same subfolder.
+
+
+## Installation of autopacmen-Paulocracy using pip
+
+You can install autopacmen-Paulocracy [from PyPI](https://pypi.org/project/autopacmen-Paulocracy/) using pip as follows:
+<pre>
+pip install autopacmen-Paulocracy
+</pre>
+
+autopacmen-Paulocracy requires Python >=3.7 for its Python parts, and MATLAB >=2017a for its optional Model Calibrator
+MATLAB scripts.
+
+
+## Structure of AutoPACMEN's source code
+
+All relevant scripts of autopacmen-Paulocracy are in the "autopacmen" main folder.
+
+In this main folder, the scripts which start with "analysis_", "data_" and "modeling_" are command-line interfaces (CLI)
+for AutoPACMEN's Python modules. These Python modules can be found the main folder's "submodules" subfolder.
+
+The subfolder "AutoPACMEN_Model_Calibrator_MATLAB" contains the Model Calibrator's MATLAB parts.
+
+All scripts and folders within "iJO1366star" are part of the generation and analysis of iJO1366* (see AutoPACMEN's publication for more about it). From these scripts, these ones
+starting with "./iJO1366star/ec_model_2019_06_25_figure" create either a full figure or data for a figure used in AutoPACMEN's publication.
+
+The main script for the generation of the uncalibrated iJO1366* model is "./iJO1366star/ec_model_2019_06_25_sMOMENT_iJO_CREATION.py" in the "iJO1366" subfolder. This
+main script uses AutoPACMEN's functionalities as Python modules. The commented steps in this script correspond to the steps described in supplementary
+File 1 of (Bekiaris & Klamt, in submission).
+
+The "iJO1366star" folder's subfolder "iJOstar_MCS_analysis_scripts" contains the scripts used for the computation and the analysis of the published Minimal Cut Set enumeration
+with iJO1366 and iJO1366*.
+
+AutoPACMEN creates a cache of SABIO-RK, NCBI TAXONOMY and UniProt data in the "_cache" main folder's subfolder.  In the current state, the cache is the one
+from AutoPACMEN's run for iJO1366* around the 25th of June 2019.
+
+
+## AutoPACMEN's Publication
+
+* Bekiaris, P.S., Klamt, S. Automatic construction of metabolic models with enzyme constraints. <i>BMC Bioinformatics</i> <b>21</b>, 19 (2020). [https://doi.org/10.1186/s12859-019-3329-9](https://doi.org/10.1186/s12859-019-3329-9)
+
+## License
+
+This project is free and open-source, using the Apache License Version 2.0.
+
+
+## External sources
+
+External sources which are included in this package are given in the respective SOURCES.txt files.
```

### Comparing `autopacmen-Paulocracy-0.6.1/autopacmen_Paulocracy.egg-info/SOURCES.txt` & `autopacmen-Paulocracy-0.6.2/autopacmen_Paulocracy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 autopacmen/__init__.py
 autopacmen/analysis_fva_comparison.py
 autopacmen/analysis_fva_prot_pool.py
 autopacmen/data_create_combined_kcat_database.py
 autopacmen/data_parse_bigg_metabolites_file.py
```

### Comparing `autopacmen-Paulocracy-0.6.1/setup.py` & `autopacmen-Paulocracy-0.6.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="autopacmen-Paulocracy",
-    version="0.6.1",
+    version="0.6.2",
     author="Paulocracy",
     author_email="bekiaris@mpi-magdeburg.mpg.de",
     description="The AutoPACMEN package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Paulocracy/autopacmen",
     packages=setuptools.find_packages(),
```

