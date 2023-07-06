# Comparing `tmp/sc-3D-0.3.3.tar.gz` & `tmp/sc-3D-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc-3D-0.3.3.tar", last modified: Thu Feb  9 15:59:12 2023, max compression
+gzip compressed data, was "sc-3D-1.0.0.tar", last modified: Thu Jul  6 10:35:50 2023, max compression
```

## Comparing `sc-3D-0.3.3.tar` & `sc-3D-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-02-09 15:59:12.861935 sc-3D-0.3.3/
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1068 2022-03-29 13:52:28.000000 sc-3D-0.3.3/LICENSE
--rw-r--r--   0 leo.guignard   (501) staff       (20)    10983 2023-02-09 15:59:12.861995 sc-3D-0.3.3/PKG-INFO
--rw-r--r--   0 leo.guignard   (501) staff       (20)     9823 2023-02-07 10:57:41.000000 sc-3D-0.3.3/README.md
--rw-r--r--   0 leo.guignard   (501) staff       (20)      634 2022-08-10 13:34:47.000000 sc-3D-0.3.3/pyproject.toml
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1579 2023-02-09 15:59:12.862310 sc-3D-0.3.3/setup.cfg
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-02-09 15:59:12.860153 sc-3D-0.3.3/src/
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-02-09 15:59:12.861061 sc-3D-0.3.3/src/sc3D/
--rw-r--r--   0 leo.guignard   (501) staff       (20)       48 2023-02-09 15:52:48.000000 sc-3D-0.3.3/src/sc3D/__init__.py
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-02-09 15:59:12.861321 sc-3D-0.3.3/src/sc3D/_tests/
--rw-r--r--   0 leo.guignard   (501) staff       (20)        0 2022-08-10 13:38:51.000000 sc-3D-0.3.3/src/sc3D/_tests/__init__.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)      989 2023-02-07 16:44:08.000000 sc-3D-0.3.3/src/sc3D/_tests/test_sc3D.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)    94192 2023-02-09 15:13:59.000000 sc-3D-0.3.3/src/sc3D/sc3D.py
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-02-09 15:59:12.861856 sc-3D-0.3.3/src/sc_3D.egg-info/
--rw-r--r--   0 leo.guignard   (501) staff       (20)    10983 2023-02-09 15:59:12.000000 sc-3D-0.3.3/src/sc_3D.egg-info/PKG-INFO
--rw-r--r--   0 leo.guignard   (501) staff       (20)      301 2023-02-09 15:59:12.000000 sc-3D-0.3.3/src/sc_3D.egg-info/SOURCES.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)        1 2023-02-09 15:59:12.000000 sc-3D-0.3.3/src/sc_3D.egg-info/dependency_links.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)      108 2023-02-09 15:59:12.000000 sc-3D-0.3.3/src/sc_3D.egg-info/requires.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)        5 2023-02-09 15:59:12.000000 sc-3D-0.3.3/src/sc_3D.egg-info/top_level.txt
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-06 10:35:50.547548 sc-3D-1.0.0/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1068 2022-03-29 13:52:28.000000 sc-3D-1.0.0/LICENSE
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     7789 2023-07-06 10:35:50.547608 sc-3D-1.0.0/PKG-INFO
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     6629 2023-06-21 13:19:01.000000 sc-3D-1.0.0/README.md
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      634 2022-08-10 13:34:47.000000 sc-3D-1.0.0/pyproject.toml
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1562 2023-07-06 10:35:50.547921 sc-3D-1.0.0/setup.cfg
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-06 10:35:50.544983 sc-3D-1.0.0/src/
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-06 10:35:50.546246 sc-3D-1.0.0/src/sc3D/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       93 2023-07-06 10:35:39.000000 sc-3D-1.0.0/src/sc3D/__init__.py
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-06 10:35:50.546689 sc-3D-1.0.0/src/sc3D/_tests/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)        0 2022-08-10 13:38:51.000000 sc-3D-1.0.0/src/sc3D/_tests/__init__.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      989 2023-02-07 16:44:08.000000 sc-3D-1.0.0/src/sc3D/_tests/test_sc3D.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    94208 2023-07-06 10:16:44.000000 sc-3D-1.0.0/src/sc3D/sc3D.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    11161 2023-07-06 10:21:28.000000 sc-3D-1.0.0/src/sc3D/transformations.py
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-06 10:35:50.547447 sc-3D-1.0.0/src/sc_3D.egg-info/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     7789 2023-07-06 10:35:50.000000 sc-3D-1.0.0/src/sc_3D.egg-info/PKG-INFO
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      329 2023-07-06 10:35:50.000000 sc-3D-1.0.0/src/sc_3D.egg-info/SOURCES.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)        1 2023-07-06 10:35:50.000000 sc-3D-1.0.0/src/sc_3D.egg-info/dependency_links.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       92 2023-07-06 10:35:50.000000 sc-3D-1.0.0/src/sc_3D.egg-info/requires.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)        5 2023-07-06 10:35:50.000000 sc-3D-1.0.0/src/sc_3D.egg-info/top_level.txt
```

### Comparing `sc-3D-0.3.3/LICENSE` & `sc-3D-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sc-3D-0.3.3/README.md` & `sc-3D-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+
 [![License MIT](https://img.shields.io/pypi/l/sc-3D.svg?color=green)](https://github.com/GuignardLab/sc3D/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/sc-3D.svg?color=green)](https://pypi.org/project/sc-3D)
 [![Python Version](https://img.shields.io/pypi/pyversions/sc-3D.svg?color=green)](https://python.org)
 [![tests](https://github.com/GuignardLab/sc3D/workflows/tests/badge.svg)](https://github.com/GuignardLab/sc3D/actions)
 [![codecov](https://codecov.io/gh/GuignardLab/sc3D/branch/main/graph/badge.svg)](https://codecov.io/gh/GuignardLab/sc3D)
 
 # sc3D
 
 __sc3D__ is a Python library to handle 3D spatial transcriptomic datasets.
 
 __To access the 3D viewer for sc3D datasets, you can go to the following link: [GuignardLab/napari-sc3D-viewer](https://github.com/GuignardLab/napari-sc3D-viewer)__
 
-
 You can find it on the Guignard Lab GitHub page: [GuignardLab/sc3D](https://github.com/GuignardLab/sc3D). In there you will be able to find jupyter notebooks giving examples about how to use the datasets.
 
 This code was developed in the context of the following study:
 
 **Spatial transcriptomic maps of whole mouse embryos.** *Abhishek Sampath Kumar, Luyi Tian, Adriano Bolondi et al.*
 
 The __sc3D__ code is based on the [anndata](https://anndata.readthedocs.io/en/latest/) and [Scanpy](https://scanpy.readthedocs.io/en/stable/) libraries and allows to read, register arrays and compute 3D differential expression.
@@ -45,42 +45,48 @@
 
 ```shell
 conda create -n sc-3D
 conda activate sc-3D
 ```
 
 If necessary, install `pip`:
+
 ```shell
 conda install pip
 ```
 
 Then, to install the latest stable version:
+
 ```shell
 pip install sc-3D
 ```
 
 or to install the latest version from the GitHub repository:
+
 ```shell
 git clone https://github.com/GuignardLab/sc3D.git
 cd sc3D
 pip install .
 ```
 
-### Troubleshooting for latest M1 MacOs chips.
+### Troubleshooting for latest M1 MacOs chips
+
 If working with an M1 chip, it is possible that all the necessary libraries are not yet available from the usual channels.
 
 To overcome this issue we recommand to manually install the latest, GitHub version of __sc3D__ using [miniforge](https://github.com/conda-forge/miniforge) instead of anaconda or miniconda.
 
 Once miniforge is installed and working, you can run the following commands:
+
 ```shell
 conda create -n sc-3D
 conda activate sc-3D
 ```
 
 to create your environment, then:
+
 ```shell
 git clone https://github.com/GuignardLab/sc3D.git
 cd sc3D
 conda install pip scipy numpy matplotlib pandas seaborn anndata napari
 pip install .
 ```
 
@@ -93,20 +99,22 @@
 ```python
 from sc3D import Embryo
 ```
 
 To import some data:
 
 **Note: at the time being, the following conventions are expected:**
+
 - **the x-y coordinates are stored in `data.obsm['X_spatial']`**
 - **the array number should be stored in `data.obs['orig.ident']` in the format `".*_[0-9]*"` where the digits after the underscore (`_`) are the id of the array**
 - **the tissue type has to be stored in `data.obs['predicted.id']`**
 - **the gene names have to be stored as indices or in `data.var['feature_name']`**
 
 Since version `0.1.2`, one can specify the name of the columns where the different necessary informations are stored using the following parameters:
+
 - `tissue_id` to inform the tissue id column
 - `array_id` to inform the array/puck/slice id column
 - `pos_id` to inform the position column (an `x, y` position is expected within this given column)
 - `gene_name_id` to inform the gene name column
 - `pos_reg_id` when to inform the registered position column (an `x, y, z` position is expected within this given column)
 
 ```python
@@ -131,115 +139,30 @@
 ```
 
 The dataset used for the project this code is from can be downloaded [there](https://cellxgene.cziscience.com/collections/d74b6979-efba-47cd-990a-9d80ccf29055/private) (under the name `mouse_embryo_E8.5_merged_data`)
 
 Many other functions are available that can be found used in the two provided jupyter notebooks.
 
 ## Running the notebooks
+
 Two example notebooks are provided.
 To run them one wants to first install the jupyter notebook:
+
 ```shell
 conda install jupyter
 ```
+
 or
+
 ```shell
 pip install jupyter
 ```
 
 The notebooks can the be started from a terminal in the folder containing the `.ipynb` files with the following command:
+
 ```shell
 jupyter notebook
 ```
+
 The notebooks should be self content.
 
 Note that the test dataset is not included in this repository put can be downloaded from [there](https://cellxgene.cziscience.com/collections/d74b6979-efba-47cd-990a-9d80ccf29055/private).
-
-<!-- # Visualiser
-
-"Quick" start (from scratch):
-## Installation
-### 1. Installing miniconda
-In order to help a smooth installation, one can use miniconda (that is what we do).
-
-You can check [there](https://docs.conda.io/en/latest/miniconda.html) to see how to install miniconda.
-
-In a nutshell, from a terminal, the following lines could work for MacOs:
-```shell
-curl https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-x86_64.sh > Miniconda3-latest-MacOSX-x86_64.sh
-bash Miniconda3-latest-MacOSX-x86_64.sh
-```
-
-Similarly, for Linux one could install miniconda by running the following commands:
-```shell
-curl https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh > Miniconda3-latest-Linux-x86_64.sh
-bash Miniconda3-latest-Linux-x86_64.sh
-```
-
-### 2. Installing the visualiser
-Once miniconda is installed one can install the visualiser.
-
-To do so, it is necessary to either download or clone the repository from GitHub (https://github.com/GuignardLab/sc3D to download, there is the green "Code" button).
-To clone the repository one can do it the following way:
-```shell
-git clone https://github.com/GuignardLab/sc3D.git
-```
-
-Once downloaded or cloned, one can access the said folder from a terminal:
-```shell
-cd path/to/sc3D
-```
-
-Once there it is probably better to create a virtual environment thanks to miniconda:
-```shell
-conda create -n sc3D python">=3.9"
-```
-Then activate it:
-```shell
-conda activate sc3D
-```
-
-From then you want to install `pip`:
-```shell
-conda install pip
-```
-
-and finally install the library and the script (still from the folder sc3D):
-```shell
-pip install .
-```
-
-Now, the visualiser is installed, you **should** close your terminal (even if you plan on using the visualiser directly, you will need to open a new terminal anyway).
-
-### 2.1 Troubleshooting for latest M1 MacOs chips.
-If working with an M1 chip, it is possible that all the necessary libraries are not yet available from the usual channels.
-
-To overcome this issue we recommand to manually install the latest, GitHub version of __sc3D__ using [miniforge](https://github.com/conda-forge/miniforge) instead of anaconda or miniconda.
-
-Once miniforge is installed and working, you can run the following commands:
-```shell
-conda create -n sc-3D
-conda activate sc-3D
-```
-
-to create your environment, then:
-```shell
-git clone https://github.com/GuignardLab/sc3D.git
-cd sc3D
-conda install pip scipy numpy matplotlib pandas seaborn anndata napari
-pip install .
-```
-
-If the previous commands are still not working, it is possible that you need to install the `pkg-config` package. You can find some information on how to do it there: [install pkg-config](https://gist.github.com/jl/9e5ebbc9ccf44f3c804e)
-
-
-### 3. Running the visualiser
-
-To run the visualiser, you want to
-- start a new terminal
-- activate your conda environement: `conda activate sc3D`
-- start the visualiser by typing: `sc3D-visualiser` (from anywhere in a terminal)
-
-Then you can load the dataset and play with it.
-The `h5ad` file can be find [there](https://cellxgene.cziscience.com/collections/d74b6979-efba-47cd-990a-9d80ccf29055/private).
-The `Tissue name` file can be find in `data/corresptissues.json`.
-
-**"Have fun"** -->
```

### Comparing `sc-3D-0.3.3/pyproject.toml` & `sc-3D-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sc-3D-0.3.3/setup.cfg` & `sc-3D-1.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sc-3D
-version = 0.3.3
+version = 1.0.0
 author = Leo Guignard
 author_email = leo.guignard@univ-amu.fr
 url = https://github.com/GuignardLab/sc3D
 license = MIT
 description = Array alignment and 3D differential expression for 3D sc omics
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -40,15 +40,14 @@
 	scipy
 	numpy
 	matplotlib
 	pandas
 	seaborn
 	scikit-learn
 	anndata
-	transformations
 
 [options.extras_require]
 testing = 
 	tox
 	pytest  # https://docs.pytest.org/en/latest/contents.html
 	pytest-cov  # https://pytest-cov.readthedocs.io/en/latest/
```

### Comparing `sc-3D-0.3.3/src/sc3D/_tests/test_sc3D.py` & `sc-3D-1.0.0/src/sc3D/_tests/test_sc3D.py`

 * *Files identical despite different names*

### Comparing `sc-3D-0.3.3/src/sc3D/sc3D.py` & `sc-3D-1.0.0/src/sc3D/sc3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 from scipy.interpolate import InterpolatedUnivariateSpline, interp1d
 from scipy.stats import zscore, linregress
 from seaborn import scatterplot
 import json
 from pathlib import Path
 
 import anndata
-import transformations as tr
-
+from sc3D.transformations import transformations as tr
 
 class Embryo:
     """
     Embryo class to handle samples from 3D spatial
     single cell omics. It was initially designed with
     a specific dataset in mind but it should work
     for other kinds of datasets.
@@ -1344,17 +1343,18 @@
         if angle_unit == "degree":
             angle = np.deg2rad(angle)
         if rot_orig is None:
             rot_orig = [0, 0, 1]
         if origin is None:
             origin = [0, 0, 0]
         x_angle, y_angle, z_angle = angle
-        rot_x = tr.rotation_matrix_py(x_angle, [1, 0, 0], origin)
-        rot_y = tr.rotation_matrix_py(y_angle, [0, 1, 0], origin)
-        rot_z = tr.rotation_matrix_py(z_angle, [0, 0, 1], origin)
+        print(tr)
+        rot_x = tr.rotation_matrix(x_angle, [1, 0, 0], origin)
+        rot_y = tr.rotation_matrix(y_angle, [0, 1, 0], origin)
+        rot_z = tr.rotation_matrix(z_angle, [0, 0, 1], origin)
         rot_composed = rot_x @ rot_y @ rot_z
         new_axis = (np.hstack([rot_orig, 1]) @ rot_composed)[:-1]
         equation = (
             lambda pos: np.sum(new_axis * pos, axis=1) - origin @ new_axis
         )
         if gene is not None and not isinstance(gene, str):
             if len(gene) == 1:
@@ -1495,17 +1495,17 @@
         if angle_unit == "degree":
             angle = np.deg2rad(angle)
         if rot_orig is None:
             rot_orig = [0, 0, 1]
         if origin is None:
             origin = [0, 0, 0]
         x_angle, y_angle, z_angle = angle
-        rot_x = tr.rotation_matrix_py(x_angle, [1, 0, 0], origin)
-        rot_y = tr.rotation_matrix_py(y_angle, [0, 1, 0], origin)
-        rot_z = tr.rotation_matrix_py(z_angle, [0, 0, 1], origin)
+        rot_x = tr.rotation_matrix(x_angle, [1, 0, 0], origin)
+        rot_y = tr.rotation_matrix(y_angle, [0, 1, 0], origin)
+        rot_z = tr.rotation_matrix(z_angle, [0, 0, 1], origin)
         rot_composed = rot_x @ rot_y @ rot_z
         new_axis = (np.hstack([rot_orig, 1]) @ rot_composed)[:-1]
         equation = (
             lambda pos: np.sum(new_axis * pos, axis=1) - origin @ new_axis
         )
         points, colors, genes = self.produce_em(
             5, tissues_to_plot=None, gene_list=gene_list
@@ -1564,17 +1564,17 @@
         if angle_unit == "degree":
             angle = np.deg2rad(angle)
         if rot_orig is None:
             rot_orig = [0, 0, 1]
         if origin is None:
             origin = [0, 0, 0]
         x_angle, y_angle, z_angle = angle
-        rot_x = tr.rotation_matrix_py(x_angle, [1, 0, 0], origin)
-        rot_y = tr.rotation_matrix_py(y_angle, [0, 1, 0], origin)
-        rot_z = tr.rotation_matrix_py(z_angle, [0, 0, 1], origin)
+        rot_x = tr.rotation_matrix(x_angle, [1, 0, 0], origin)
+        rot_y = tr.rotation_matrix(y_angle, [0, 1, 0], origin)
+        rot_z = tr.rotation_matrix(z_angle, [0, 0, 1], origin)
         rot_composed = rot_x @ rot_y @ rot_z
         new_axis = (np.hstack([rot_orig, 1]) @ rot_composed)[:-1]
         equation = (
             lambda pos: np.sum(new_axis * pos, axis=1) - origin @ new_axis
         )
         cells = np.array(sorted(self.all_cells))
         pos = np.array([list(self.final[c]) + [self.z_pos[c]] for c in cells])
```

