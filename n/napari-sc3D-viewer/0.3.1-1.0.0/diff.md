# Comparing `tmp/napari-sc3D-viewer-0.3.1.tar.gz` & `tmp/napari-sc3D-viewer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sc3D-viewer-0.3.1.tar", last modified: Thu Feb  9 16:58:05 2023, max compression
+gzip compressed data, was "napari-sc3D-viewer-1.0.0.tar", last modified: Thu Jul  6 09:09:38 2023, max compression
```

## Comparing `napari-sc3D-viewer-0.3.1.tar` & `napari-sc3D-viewer-1.0.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-02-09 16:58:05.162685 napari-sc3D-viewer-0.3.1/
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1079 2022-06-02 09:43:22.000000 napari-sc3D-viewer-0.3.1/LICENSE
--rw-r--r--   0 leo.guignard   (501) staff       (20)       96 2022-05-02 08:05:43.000000 napari-sc3D-viewer-0.3.1/MANIFEST.in
--rw-r--r--   0 leo.guignard   (501) staff       (20)    11766 2023-02-09 16:58:05.162773 napari-sc3D-viewer-0.3.1/PKG-INFO
--rw-r--r--   0 leo.guignard   (501) staff       (20)    10487 2023-02-06 15:47:07.000000 napari-sc3D-viewer-0.3.1/README.md
--rw-r--r--   0 leo.guignard   (501) staff       (20)      727 2023-02-09 15:07:40.000000 napari-sc3D-viewer-0.3.1/pyproject.toml
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1834 2023-02-09 16:58:05.163158 napari-sc3D-viewer-0.3.1/setup.cfg
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-02-09 16:58:05.159815 napari-sc3D-viewer-0.3.1/src/
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-02-09 16:58:05.161556 napari-sc3D-viewer-0.3.1/src/napari_sc3D_viewer.egg-info/
--rw-r--r--   0 leo.guignard   (501) staff       (20)    11766 2023-02-09 16:58:05.000000 napari-sc3D-viewer-0.3.1/src/napari_sc3D_viewer.egg-info/PKG-INFO
--rw-r--r--   0 leo.guignard   (501) staff       (20)      688 2023-02-09 16:58:05.000000 napari-sc3D-viewer-0.3.1/src/napari_sc3D_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)        1 2023-02-09 16:58:05.000000 napari-sc3D-viewer-0.3.1/src/napari_sc3D_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)       70 2023-02-09 16:58:05.000000 napari-sc3D-viewer-0.3.1/src/napari_sc3D_viewer.egg-info/entry_points.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)      112 2023-02-09 16:58:05.000000 napari-sc3D-viewer-0.3.1/src/napari_sc3D_viewer.egg-info/requires.txt
--rw-r--r--   0 leo.guignard   (501) staff       (20)       19 2023-02-09 16:58:05.000000 napari-sc3D-viewer-0.3.1/src/napari_sc3D_viewer.egg-info/top_level.txt
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-02-09 16:58:05.162377 napari-sc3D-viewer-0.3.1/src/napari_sc3d_viewer/
--rw-r--r--   0 leo.guignard   (501) staff       (20)      102 2023-02-09 15:07:40.000000 napari-sc3D-viewer-0.3.1/src/napari_sc3d_viewer/__init__.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)    41616 2023-02-08 14:49:05.000000 napari-sc3D-viewer-0.3.1/src/napari_sc3d_viewer/_display_embryo.py
-drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-02-09 16:58:05.162583 napari-sc3D-viewer-0.3.1/src/napari_sc3d_viewer/_tests/
--rw-r--r--   0 leo.guignard   (501) staff       (20)        0 2022-05-02 08:05:43.000000 napari-sc3D-viewer-0.3.1/src/napari_sc3d_viewer/_tests/__init__.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)     5051 2023-02-07 16:41:17.000000 napari-sc3D-viewer-0.3.1/src/napari_sc3d_viewer/_tests/test_widget.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)    15701 2023-02-07 16:41:17.000000 napari-sc3D-viewer-0.3.1/src/napari_sc3d_viewer/_umap_selection.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)     1175 2023-02-07 16:41:17.000000 napari-sc3D-viewer-0.3.1/src/napari_sc3d_viewer/_utils.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)     5939 2023-02-07 16:41:17.000000 napari-sc3D-viewer-0.3.1/src/napari_sc3d_viewer/_widget_load.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)    12359 2023-02-07 16:43:49.000000 napari-sc3D-viewer-0.3.1/src/napari_sc3d_viewer/_widget_register.py
--rw-r--r--   0 leo.guignard   (501) staff       (20)      562 2022-07-11 15:14:34.000000 napari-sc3D-viewer-0.3.1/src/napari_sc3d_viewer/napari.yaml
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-06 09:09:38.538357 napari-sc3D-viewer-1.0.0/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1079 2023-05-17 08:01:30.000000 napari-sc3D-viewer-1.0.0/LICENSE
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       96 2022-05-02 08:05:43.000000 napari-sc3D-viewer-1.0.0/MANIFEST.in
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    11999 2023-07-06 09:09:38.538450 napari-sc3D-viewer-1.0.0/PKG-INFO
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    10720 2023-05-17 08:13:17.000000 napari-sc3D-viewer-1.0.0/README.md
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      727 2023-07-06 09:09:17.000000 napari-sc3D-viewer-1.0.0/pyproject.toml
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1834 2023-07-06 09:09:38.538844 napari-sc3D-viewer-1.0.0/setup.cfg
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-06 09:09:38.535232 napari-sc3D-viewer-1.0.0/src/
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-06 09:09:38.537168 napari-sc3D-viewer-1.0.0/src/napari_sc3D_viewer.egg-info/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    11999 2023-07-06 09:09:38.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3D_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      688 2023-07-06 09:09:38.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3D_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)        1 2023-07-06 09:09:38.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3D_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       70 2023-07-06 09:09:38.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3D_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      112 2023-07-06 09:09:38.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3D_viewer.egg-info/requires.txt
+-rw-r--r--   0 leo.guignard   (501) staff       (20)       19 2023-07-06 09:09:38.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3D_viewer.egg-info/top_level.txt
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-06 09:09:38.538051 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      102 2023-07-06 09:09:17.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/__init__.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    41446 2023-07-06 09:07:36.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_display_embryo.py
+drwxr-xr-x   0 leo.guignard   (501) staff       (20)        0 2023-07-06 09:09:38.538267 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_tests/
+-rw-r--r--   0 leo.guignard   (501) staff       (20)        0 2022-05-02 08:05:43.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_tests/__init__.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     5051 2023-05-17 08:01:31.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_tests/test_widget.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    15701 2023-05-17 08:01:31.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_umap_selection.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     1175 2023-05-17 08:01:31.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_utils.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)     5939 2023-05-17 08:01:31.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_widget_load.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)    12359 2023-05-17 08:01:31.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_widget_register.py
+-rw-r--r--   0 leo.guignard   (501) staff       (20)      562 2023-05-17 08:01:31.000000 napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/napari.yaml
```

### Comparing `napari-sc3D-viewer-0.3.1/LICENSE` & `napari-sc3D-viewer-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sc3D-viewer-0.3.1/PKG-INFO` & `napari-sc3D-viewer-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sc3D-viewer
-Version: 0.3.1
+Version: 1.0.0
 Summary: A plugin to visualize 3D single cell omics
 Home-page: https://github.com/GuignardLab/napari-sc3D-viewer
 Author: Leo Guignard
 Author-email: leo.guignard@univ-amu.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/GuignardLab/napari-sc3D-viewer/issues
 Project-URL: Documentation, https://github.com/GuignardLab/napari-sc3D-viewer#README.md
@@ -33,95 +33,136 @@
 [![License](https://img.shields.io/pypi/l/napari-sc3D-viewer.svg?color=green)](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/LICENSE)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-sc3D-viewer.svg?color=green)](https://python.org)
 [![PyPI](https://img.shields.io/pypi/v/napari-sc3D-viewer.svg?color=green)](https://pypi.org/project/napari-sc3D-viewer)
 [![tests](https://github.com/GuignardLab/napari-sc3D-viewer/workflows/tests/badge.svg)](https://github.com/GuignardLab/napari-sc3D-viewer/actions)
 [![codecov](https://codecov.io/gh/GuignardLab/napari-sc3D-viewer/branch/main/graph/badge.svg)](https://codecov.io/gh/GuignardLab/napari-sc3D-viewer)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-sc3D-viewer)](https://napari-hub.org/plugins/napari-sc3D-viewer)
 
-
 A plugin to visualise 3D spatial single cell omics
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 ## Test and atlas datasets
 
 Because the datasets representing the mouse embryo at stages E8.5 and E9.0 are rather large, it is not possible to host them on GitHub. They are instead hosted on figshare at the following links:
+
 - [E8.5 replicate 1](https://figshare.com/s/1c29d867bc8b90d754d2)
 - [E8.5 replicate 2](https://doi.org/10.6084/m9.figshare.21695849.v1)
 - [E9.0 replicate 1](https://doi.org/10.6084/m9.figshare.21695879.v1)
 
-Once downloaded, one can open them in the viewer as explained below (note that the files for the tissue names are stored in the json file there: `napari-sc3D-viewer/test_data/corresptissues.json`).
+Once downloaded, one can open them in the viewer as explained below (note that the files for the tissue names are stored in the json file there: `napari-sc3D-viewer/test_data/corresptissues.json`). It can be downloaded by right-clicking on the following [link](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/test_data/corresptissues.json) and then clicking on "Save link as".
 
 ## Installation
-_____
+
+----------------------------------
+
 __Disclaimer:__
-While we tried to make the installation and usage as easy as possible, please keep in mind that [napari-sc3d-viewer] is still under development, it has been and is developed by a single person. We will be happy to answer any question and help in any way.
-_____
+While we tried to make the installation and usage as easy as possible, please keep in mind that [napari-sc3d-viewer] is still under development, it has been and is being developed by a single person. We will be happy to answer any question and help in any way.
+
+----------------------------------
 
 There are many ways to install our viewer, but the global idea is that it works in two steps:
+
 - first installing [napari]
 - then installing the [napari-sc3d-viewer] plugin.
 
 Installing [napari] and the [napari-sc3d-viewer] plugin can be done either through command line or using an interface.
 
 If you have decided to use command line, as [napari] developers do, we strongly recommend to install the viewer in an environement such as a conda environment `conda` for example:
 
-    conda create -n sc3D python=3.10
-    conda activate sc3D
-
+```shell
+conda create -n sc3D python=3.10
+conda activate sc3D
+```
 
 ### Installing napari
+
 The first step is to [install napari](https://napari.org/stable/tutorials/fundamentals/installation.html) on your computer. The previous link should explain how to do so. There you can find either the installation via terminal or directly by [downloading the binary](https://napari.org/stable/tutorials/fundamentals/installation.html#install-as-a-bundled-app).
 
+#### Quick trouble shooting
+
+Installing [napari] can sometimes be difficult. If you try to install [napari] via the command line and it gets stuck "resolving the environment" you can try to install it the following way:
+
+```shell
+conda create -n sc3D python=3.10
+conda activate sc3D
+conda install pyqt pip
+pip install napari
+```
+
 ### Installing napari-sc3D-viewer
+
 Once [napari] is installed, you can install `napari-sc3D-viewer`.
 As for [napari], [napari-sc3D-viewer] can be installed either through an interface or via the terminal.
 
 #### Installation via graphical interface
+
 To install [napari-sc3D-viewer] with a visual interface, you should use the [napari's plugin manager](https://napari.org/stable/plugins/find_and_install_plugin.html) look for the plugin there and install it as explained in the previous link.
 
 #### Installation via the terminal
+
 Another way is to install `napari-sc3D-viewer` via [pip] or via [conda]:
 
-    conda install napari-sc3d-viewer
+```shell
+conda install napari-sc3d-viewer
+```
+
 or
 
-    pip install napari-sc3d-viewer
+```shell
+pip install napari-sc3d-viewer
+```
 
 Finally, to install latest development version :
 
-    pip install git+https://github.com/GuignardLab/napari-sc3D-viewer.git
+```shell
+pip install git+https://github.com/GuignardLab/napari-sc3D-viewer.git
+```
 
 #### Installation of the surface computation module
+
 To install the surface computation enabled version it is necessary to use Python 3.9 (until [VTK] is ported to Python 3.10) and you can run one of the following commands:
 
-    pip install '.[pyvista]'
+```shell
+pip install '.[pyvista]'
+```
+
 from the correct folder or
 
-    pip install 'napari-sc3D-viewer[pyvista]'
+```shell
+pip install 'napari-sc3D-viewer[pyvista]'
+```
+
 or
 
-    conda install 'napari-sc3D-viewer[pyvista]'
+```shell
+conda install 'napari-sc3D-viewer[pyvista]'
+```
 
 to install directly from pip or
 
-    pip install 'napari-sc3D-viewer[pyvista] @ git+https://github.com/GuignardLab/napari-sc3D-viewer.git'
+```shell
+pip install 'napari-sc3D-viewer[pyvista] @ git+https://github.com/GuignardLab/napari-sc3D-viewer.git'
+```
 
 to install the latest version
 
 ## Usage
 
 `napari-sc3D-viewer` allows users to easily visualise and navigate 3D spatial single-cell transcriptomics using napari.
 
 ### Starting the plugin
+
 First, you need to start [napari], for example, one can start it from a terminal just by typing:
 
-    napari
+```shell
+napari
+```
 
 in the correct environment.
 
 Then, one can follow the following steps to browse the dataset.
 
 To open the plugin you can click on the "Load spatial single cell" from the `Plugins -> napari-sc3d-viewer` menu:
 ![loading image](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/0.openplugin.png)
@@ -129,27 +170,30 @@
 Once opened you should have an interface poping similar to the one showed in the image below (note that it might not be exactly the same depending on the version of the viewer you are using).
 
 ### Loading and opening a dataset
 
 The expected dataset is a [scanpy]/[anndata] h5ad file together with an optional json file that maps cluster id numbers to actual tissue/cluster name.
 
 The json file should look like that:
+
 ```json
 {
     "1": "Endoderm",
     "2": "Heart",
     "10": "Anterior neuroectoderm"
 }
 ```
+
 If no json file or a wrong json file is given, the original cluster id numbers are used.
 
 The h5ad file should be informed in (1) and the json file in (2).
 ![loading image](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/1.loading.png)
 
 Let `data` be your h5ad data structure. To work properly, the viewer is expecting 4 different columns to be present in the h5ad file:
+
 - the cluster id column (by default named 'predicted.id' that can be accessed as `data.obs['predicted.id']`)
 - the 3D position column (by default named 'X_spatial_registered' that can be accessed as `data.obsm['X_spatial_registered']`)
 - the gene names if not already in the column name (by default named 'feature_name' that can be accessed as `data.var['feature_name']`)
 - umap coordinates (by default named 'X_umap' that can be accessed as `data.obsm['X_umap']`)
 
 If the default column names are not consistent with your dataset, they can be changed in the tab `Parameters` (3) next to the tab `Loading files`
 
@@ -173,35 +217,42 @@
 
 The 2 Genes (2.2) tab allows to display gene coexpression.
 
 The umap tab (2.3) allows to display the umap of the selected cells and to manually select subcategories of cells to be displayed.
 
 ![viewer](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/3.description.png)
 
-#### Explanatory "videos".
+#### Explanatory "videos"
+
 The plugin is meant to be easy to use. That means that you should be able to play with it and figure things out by yourself.
 
 That being said, it is not always that easy. You can find below a series of videos showing how to perform some of the main features.
 
 #### Loading data
+
 ![Loading data video](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/loading.gif)
 
 #### Selecting tissues
+
 ![Selecting tissues video](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/tissue-select.gif)
 
 #### Displaying one gene
+
 ![Displaying one gene video](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/gene1.gif)
 
 #### Displaying two genes co-expression
+
 ![Displaying genes video](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/gene2.gif)
 
 #### Playing with the umap
+
 ![Playing with the umap video](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/umap.gif)
 
 #### Computing and processing the surface
+
 ![Computing and processing the surface video](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/surfaces.gif)
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
@@ -214,26 +265,18 @@
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
 [napari]: https://github.com/napari/napari
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
 [MIT]: http://opensource.org/licenses/MIT
-[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
-[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
-[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
-[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
-[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 
 [file an issue]: https://github.com/GuignardLab/napari-sc3D-viewer/issues
 [napari-sc3d-viewer]: https://github.com/GuignardLab/napari-sc3D-viewer
-[napari-sc3D-viewer]: https://github.com/GuignardLab/napari-sc3D-viewer
 
-[napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
-[PyPI]: https://pypi.org/
 [VTK]: https://vtk.org/
 [scanpy]: https://scanpy.readthedocs.io/en/latest/index.html
 [anndata]: https://anndata.readthedocs.io/en/latest/
 [conda]: https://conda.io
```

### Comparing `napari-sc3D-viewer-0.3.1/README.md` & `napari-sc3D-viewer-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,95 +3,136 @@
 [![License](https://img.shields.io/pypi/l/napari-sc3D-viewer.svg?color=green)](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/LICENSE)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-sc3D-viewer.svg?color=green)](https://python.org)
 [![PyPI](https://img.shields.io/pypi/v/napari-sc3D-viewer.svg?color=green)](https://pypi.org/project/napari-sc3D-viewer)
 [![tests](https://github.com/GuignardLab/napari-sc3D-viewer/workflows/tests/badge.svg)](https://github.com/GuignardLab/napari-sc3D-viewer/actions)
 [![codecov](https://codecov.io/gh/GuignardLab/napari-sc3D-viewer/branch/main/graph/badge.svg)](https://codecov.io/gh/GuignardLab/napari-sc3D-viewer)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-sc3D-viewer)](https://napari-hub.org/plugins/napari-sc3D-viewer)
 
-
 A plugin to visualise 3D spatial single cell omics
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 ## Test and atlas datasets
 
 Because the datasets representing the mouse embryo at stages E8.5 and E9.0 are rather large, it is not possible to host them on GitHub. They are instead hosted on figshare at the following links:
+
 - [E8.5 replicate 1](https://figshare.com/s/1c29d867bc8b90d754d2)
 - [E8.5 replicate 2](https://doi.org/10.6084/m9.figshare.21695849.v1)
 - [E9.0 replicate 1](https://doi.org/10.6084/m9.figshare.21695879.v1)
 
-Once downloaded, one can open them in the viewer as explained below (note that the files for the tissue names are stored in the json file there: `napari-sc3D-viewer/test_data/corresptissues.json`).
+Once downloaded, one can open them in the viewer as explained below (note that the files for the tissue names are stored in the json file there: `napari-sc3D-viewer/test_data/corresptissues.json`). It can be downloaded by right-clicking on the following [link](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/test_data/corresptissues.json) and then clicking on "Save link as".
 
 ## Installation
-_____
+
+----------------------------------
+
 __Disclaimer:__
-While we tried to make the installation and usage as easy as possible, please keep in mind that [napari-sc3d-viewer] is still under development, it has been and is developed by a single person. We will be happy to answer any question and help in any way.
-_____
+While we tried to make the installation and usage as easy as possible, please keep in mind that [napari-sc3d-viewer] is still under development, it has been and is being developed by a single person. We will be happy to answer any question and help in any way.
+
+----------------------------------
 
 There are many ways to install our viewer, but the global idea is that it works in two steps:
+
 - first installing [napari]
 - then installing the [napari-sc3d-viewer] plugin.
 
 Installing [napari] and the [napari-sc3d-viewer] plugin can be done either through command line or using an interface.
 
 If you have decided to use command line, as [napari] developers do, we strongly recommend to install the viewer in an environement such as a conda environment `conda` for example:
 
-    conda create -n sc3D python=3.10
-    conda activate sc3D
-
+```shell
+conda create -n sc3D python=3.10
+conda activate sc3D
+```
 
 ### Installing napari
+
 The first step is to [install napari](https://napari.org/stable/tutorials/fundamentals/installation.html) on your computer. The previous link should explain how to do so. There you can find either the installation via terminal or directly by [downloading the binary](https://napari.org/stable/tutorials/fundamentals/installation.html#install-as-a-bundled-app).
 
+#### Quick trouble shooting
+
+Installing [napari] can sometimes be difficult. If you try to install [napari] via the command line and it gets stuck "resolving the environment" you can try to install it the following way:
+
+```shell
+conda create -n sc3D python=3.10
+conda activate sc3D
+conda install pyqt pip
+pip install napari
+```
+
 ### Installing napari-sc3D-viewer
+
 Once [napari] is installed, you can install `napari-sc3D-viewer`.
 As for [napari], [napari-sc3D-viewer] can be installed either through an interface or via the terminal.
 
 #### Installation via graphical interface
+
 To install [napari-sc3D-viewer] with a visual interface, you should use the [napari's plugin manager](https://napari.org/stable/plugins/find_and_install_plugin.html) look for the plugin there and install it as explained in the previous link.
 
 #### Installation via the terminal
+
 Another way is to install `napari-sc3D-viewer` via [pip] or via [conda]:
 
-    conda install napari-sc3d-viewer
+```shell
+conda install napari-sc3d-viewer
+```
+
 or
 
-    pip install napari-sc3d-viewer
+```shell
+pip install napari-sc3d-viewer
+```
 
 Finally, to install latest development version :
 
-    pip install git+https://github.com/GuignardLab/napari-sc3D-viewer.git
+```shell
+pip install git+https://github.com/GuignardLab/napari-sc3D-viewer.git
+```
 
 #### Installation of the surface computation module
+
 To install the surface computation enabled version it is necessary to use Python 3.9 (until [VTK] is ported to Python 3.10) and you can run one of the following commands:
 
-    pip install '.[pyvista]'
+```shell
+pip install '.[pyvista]'
+```
+
 from the correct folder or
 
-    pip install 'napari-sc3D-viewer[pyvista]'
+```shell
+pip install 'napari-sc3D-viewer[pyvista]'
+```
+
 or
 
-    conda install 'napari-sc3D-viewer[pyvista]'
+```shell
+conda install 'napari-sc3D-viewer[pyvista]'
+```
 
 to install directly from pip or
 
-    pip install 'napari-sc3D-viewer[pyvista] @ git+https://github.com/GuignardLab/napari-sc3D-viewer.git'
+```shell
+pip install 'napari-sc3D-viewer[pyvista] @ git+https://github.com/GuignardLab/napari-sc3D-viewer.git'
+```
 
 to install the latest version
 
 ## Usage
 
 `napari-sc3D-viewer` allows users to easily visualise and navigate 3D spatial single-cell transcriptomics using napari.
 
 ### Starting the plugin
+
 First, you need to start [napari], for example, one can start it from a terminal just by typing:
 
-    napari
+```shell
+napari
+```
 
 in the correct environment.
 
 Then, one can follow the following steps to browse the dataset.
 
 To open the plugin you can click on the "Load spatial single cell" from the `Plugins -> napari-sc3d-viewer` menu:
 ![loading image](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/0.openplugin.png)
@@ -99,27 +140,30 @@
 Once opened you should have an interface poping similar to the one showed in the image below (note that it might not be exactly the same depending on the version of the viewer you are using).
 
 ### Loading and opening a dataset
 
 The expected dataset is a [scanpy]/[anndata] h5ad file together with an optional json file that maps cluster id numbers to actual tissue/cluster name.
 
 The json file should look like that:
+
 ```json
 {
     "1": "Endoderm",
     "2": "Heart",
     "10": "Anterior neuroectoderm"
 }
 ```
+
 If no json file or a wrong json file is given, the original cluster id numbers are used.
 
 The h5ad file should be informed in (1) and the json file in (2).
 ![loading image](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/1.loading.png)
 
 Let `data` be your h5ad data structure. To work properly, the viewer is expecting 4 different columns to be present in the h5ad file:
+
 - the cluster id column (by default named 'predicted.id' that can be accessed as `data.obs['predicted.id']`)
 - the 3D position column (by default named 'X_spatial_registered' that can be accessed as `data.obsm['X_spatial_registered']`)
 - the gene names if not already in the column name (by default named 'feature_name' that can be accessed as `data.var['feature_name']`)
 - umap coordinates (by default named 'X_umap' that can be accessed as `data.obsm['X_umap']`)
 
 If the default column names are not consistent with your dataset, they can be changed in the tab `Parameters` (3) next to the tab `Loading files`
 
@@ -143,35 +187,42 @@
 
 The 2 Genes (2.2) tab allows to display gene coexpression.
 
 The umap tab (2.3) allows to display the umap of the selected cells and to manually select subcategories of cells to be displayed.
 
 ![viewer](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/3.description.png)
 
-#### Explanatory "videos".
+#### Explanatory "videos"
+
 The plugin is meant to be easy to use. That means that you should be able to play with it and figure things out by yourself.
 
 That being said, it is not always that easy. You can find below a series of videos showing how to perform some of the main features.
 
 #### Loading data
+
 ![Loading data video](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/loading.gif)
 
 #### Selecting tissues
+
 ![Selecting tissues video](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/tissue-select.gif)
 
 #### Displaying one gene
+
 ![Displaying one gene video](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/gene1.gif)
 
 #### Displaying two genes co-expression
+
 ![Displaying genes video](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/gene2.gif)
 
 #### Playing with the umap
+
 ![Playing with the umap video](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/umap.gif)
 
 #### Computing and processing the surface
+
 ![Computing and processing the surface video](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/surfaces.gif)
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
@@ -184,26 +235,18 @@
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
 [napari]: https://github.com/napari/napari
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
 [MIT]: http://opensource.org/licenses/MIT
-[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
-[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
-[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
-[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
-[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 
 [file an issue]: https://github.com/GuignardLab/napari-sc3D-viewer/issues
 [napari-sc3d-viewer]: https://github.com/GuignardLab/napari-sc3D-viewer
-[napari-sc3D-viewer]: https://github.com/GuignardLab/napari-sc3D-viewer
 
-[napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
-[PyPI]: https://pypi.org/
 [VTK]: https://vtk.org/
 [scanpy]: https://scanpy.readthedocs.io/en/latest/index.html
 [anndata]: https://anndata.readthedocs.io/en/latest/
 [conda]: https://conda.io
```

### Comparing `napari-sc3D-viewer-0.3.1/pyproject.toml` & `napari-sc3D-viewer-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 line-length = 79
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.bumpver]
-current_version = "0.3.1"
+current_version = "1.0.0"
 version_pattern = "MAJOR.MINOR.PATCH[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `napari-sc3D-viewer-0.3.1/setup.cfg` & `napari-sc3D-viewer-1.0.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-sc3D-viewer
-version = 0.3.1
+version = 1.0.0
 author = Leo Guignard
 author_email = leo.guignard@univ-amu.fr
 url = https://github.com/GuignardLab/napari-sc3D-viewer
 license = MIT
 description = A plugin to visualize 3D single cell omics
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `napari-sc3D-viewer-0.3.1/src/napari_sc3D_viewer.egg-info/PKG-INFO` & `napari-sc3D-viewer-1.0.0/src/napari_sc3D_viewer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sc3D-viewer
-Version: 0.3.1
+Version: 1.0.0
 Summary: A plugin to visualize 3D single cell omics
 Home-page: https://github.com/GuignardLab/napari-sc3D-viewer
 Author: Leo Guignard
 Author-email: leo.guignard@univ-amu.fr
 License: MIT
 Project-URL: Bug Tracker, https://github.com/GuignardLab/napari-sc3D-viewer/issues
 Project-URL: Documentation, https://github.com/GuignardLab/napari-sc3D-viewer#README.md
@@ -33,95 +33,136 @@
 [![License](https://img.shields.io/pypi/l/napari-sc3D-viewer.svg?color=green)](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/LICENSE)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-sc3D-viewer.svg?color=green)](https://python.org)
 [![PyPI](https://img.shields.io/pypi/v/napari-sc3D-viewer.svg?color=green)](https://pypi.org/project/napari-sc3D-viewer)
 [![tests](https://github.com/GuignardLab/napari-sc3D-viewer/workflows/tests/badge.svg)](https://github.com/GuignardLab/napari-sc3D-viewer/actions)
 [![codecov](https://codecov.io/gh/GuignardLab/napari-sc3D-viewer/branch/main/graph/badge.svg)](https://codecov.io/gh/GuignardLab/napari-sc3D-viewer)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-sc3D-viewer)](https://napari-hub.org/plugins/napari-sc3D-viewer)
 
-
 A plugin to visualise 3D spatial single cell omics
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 ## Test and atlas datasets
 
 Because the datasets representing the mouse embryo at stages E8.5 and E9.0 are rather large, it is not possible to host them on GitHub. They are instead hosted on figshare at the following links:
+
 - [E8.5 replicate 1](https://figshare.com/s/1c29d867bc8b90d754d2)
 - [E8.5 replicate 2](https://doi.org/10.6084/m9.figshare.21695849.v1)
 - [E9.0 replicate 1](https://doi.org/10.6084/m9.figshare.21695879.v1)
 
-Once downloaded, one can open them in the viewer as explained below (note that the files for the tissue names are stored in the json file there: `napari-sc3D-viewer/test_data/corresptissues.json`).
+Once downloaded, one can open them in the viewer as explained below (note that the files for the tissue names are stored in the json file there: `napari-sc3D-viewer/test_data/corresptissues.json`). It can be downloaded by right-clicking on the following [link](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/test_data/corresptissues.json) and then clicking on "Save link as".
 
 ## Installation
-_____
+
+----------------------------------
+
 __Disclaimer:__
-While we tried to make the installation and usage as easy as possible, please keep in mind that [napari-sc3d-viewer] is still under development, it has been and is developed by a single person. We will be happy to answer any question and help in any way.
-_____
+While we tried to make the installation and usage as easy as possible, please keep in mind that [napari-sc3d-viewer] is still under development, it has been and is being developed by a single person. We will be happy to answer any question and help in any way.
+
+----------------------------------
 
 There are many ways to install our viewer, but the global idea is that it works in two steps:
+
 - first installing [napari]
 - then installing the [napari-sc3d-viewer] plugin.
 
 Installing [napari] and the [napari-sc3d-viewer] plugin can be done either through command line or using an interface.
 
 If you have decided to use command line, as [napari] developers do, we strongly recommend to install the viewer in an environement such as a conda environment `conda` for example:
 
-    conda create -n sc3D python=3.10
-    conda activate sc3D
-
+```shell
+conda create -n sc3D python=3.10
+conda activate sc3D
+```
 
 ### Installing napari
+
 The first step is to [install napari](https://napari.org/stable/tutorials/fundamentals/installation.html) on your computer. The previous link should explain how to do so. There you can find either the installation via terminal or directly by [downloading the binary](https://napari.org/stable/tutorials/fundamentals/installation.html#install-as-a-bundled-app).
 
+#### Quick trouble shooting
+
+Installing [napari] can sometimes be difficult. If you try to install [napari] via the command line and it gets stuck "resolving the environment" you can try to install it the following way:
+
+```shell
+conda create -n sc3D python=3.10
+conda activate sc3D
+conda install pyqt pip
+pip install napari
+```
+
 ### Installing napari-sc3D-viewer
+
 Once [napari] is installed, you can install `napari-sc3D-viewer`.
 As for [napari], [napari-sc3D-viewer] can be installed either through an interface or via the terminal.
 
 #### Installation via graphical interface
+
 To install [napari-sc3D-viewer] with a visual interface, you should use the [napari's plugin manager](https://napari.org/stable/plugins/find_and_install_plugin.html) look for the plugin there and install it as explained in the previous link.
 
 #### Installation via the terminal
+
 Another way is to install `napari-sc3D-viewer` via [pip] or via [conda]:
 
-    conda install napari-sc3d-viewer
+```shell
+conda install napari-sc3d-viewer
+```
+
 or
 
-    pip install napari-sc3d-viewer
+```shell
+pip install napari-sc3d-viewer
+```
 
 Finally, to install latest development version :
 
-    pip install git+https://github.com/GuignardLab/napari-sc3D-viewer.git
+```shell
+pip install git+https://github.com/GuignardLab/napari-sc3D-viewer.git
+```
 
 #### Installation of the surface computation module
+
 To install the surface computation enabled version it is necessary to use Python 3.9 (until [VTK] is ported to Python 3.10) and you can run one of the following commands:
 
-    pip install '.[pyvista]'
+```shell
+pip install '.[pyvista]'
+```
+
 from the correct folder or
 
-    pip install 'napari-sc3D-viewer[pyvista]'
+```shell
+pip install 'napari-sc3D-viewer[pyvista]'
+```
+
 or
 
-    conda install 'napari-sc3D-viewer[pyvista]'
+```shell
+conda install 'napari-sc3D-viewer[pyvista]'
+```
 
 to install directly from pip or
 
-    pip install 'napari-sc3D-viewer[pyvista] @ git+https://github.com/GuignardLab/napari-sc3D-viewer.git'
+```shell
+pip install 'napari-sc3D-viewer[pyvista] @ git+https://github.com/GuignardLab/napari-sc3D-viewer.git'
+```
 
 to install the latest version
 
 ## Usage
 
 `napari-sc3D-viewer` allows users to easily visualise and navigate 3D spatial single-cell transcriptomics using napari.
 
 ### Starting the plugin
+
 First, you need to start [napari], for example, one can start it from a terminal just by typing:
 
-    napari
+```shell
+napari
+```
 
 in the correct environment.
 
 Then, one can follow the following steps to browse the dataset.
 
 To open the plugin you can click on the "Load spatial single cell" from the `Plugins -> napari-sc3d-viewer` menu:
 ![loading image](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/0.openplugin.png)
@@ -129,27 +170,30 @@
 Once opened you should have an interface poping similar to the one showed in the image below (note that it might not be exactly the same depending on the version of the viewer you are using).
 
 ### Loading and opening a dataset
 
 The expected dataset is a [scanpy]/[anndata] h5ad file together with an optional json file that maps cluster id numbers to actual tissue/cluster name.
 
 The json file should look like that:
+
 ```json
 {
     "1": "Endoderm",
     "2": "Heart",
     "10": "Anterior neuroectoderm"
 }
 ```
+
 If no json file or a wrong json file is given, the original cluster id numbers are used.
 
 The h5ad file should be informed in (1) and the json file in (2).
 ![loading image](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/1.loading.png)
 
 Let `data` be your h5ad data structure. To work properly, the viewer is expecting 4 different columns to be present in the h5ad file:
+
 - the cluster id column (by default named 'predicted.id' that can be accessed as `data.obs['predicted.id']`)
 - the 3D position column (by default named 'X_spatial_registered' that can be accessed as `data.obsm['X_spatial_registered']`)
 - the gene names if not already in the column name (by default named 'feature_name' that can be accessed as `data.var['feature_name']`)
 - umap coordinates (by default named 'X_umap' that can be accessed as `data.obsm['X_umap']`)
 
 If the default column names are not consistent with your dataset, they can be changed in the tab `Parameters` (3) next to the tab `Loading files`
 
@@ -173,35 +217,42 @@
 
 The 2 Genes (2.2) tab allows to display gene coexpression.
 
 The umap tab (2.3) allows to display the umap of the selected cells and to manually select subcategories of cells to be displayed.
 
 ![viewer](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/3.description.png)
 
-#### Explanatory "videos".
+#### Explanatory "videos"
+
 The plugin is meant to be easy to use. That means that you should be able to play with it and figure things out by yourself.
 
 That being said, it is not always that easy. You can find below a series of videos showing how to perform some of the main features.
 
 #### Loading data
+
 ![Loading data video](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/loading.gif)
 
 #### Selecting tissues
+
 ![Selecting tissues video](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/tissue-select.gif)
 
 #### Displaying one gene
+
 ![Displaying one gene video](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/gene1.gif)
 
 #### Displaying two genes co-expression
+
 ![Displaying genes video](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/gene2.gif)
 
 #### Playing with the umap
+
 ![Playing with the umap video](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/umap.gif)
 
 #### Computing and processing the surface
+
 ![Computing and processing the surface video](https://raw.githubusercontent.com/GuignardLab/napari-sc3D-viewer/main/images/surfaces.gif)
 
 ## Contributing
 
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
@@ -214,26 +265,18 @@
 
 If you encounter any problems, please [file an issue] along with a detailed description.
 
 [napari]: https://github.com/napari/napari
 [Cookiecutter]: https://github.com/audreyr/cookiecutter
 [@napari]: https://github.com/napari
 [MIT]: http://opensource.org/licenses/MIT
-[BSD-3]: http://opensource.org/licenses/BSD-3-Clause
-[GNU GPL v3.0]: http://www.gnu.org/licenses/gpl-3.0.txt
-[GNU LGPL v3.0]: http://www.gnu.org/licenses/lgpl-3.0.txt
-[Apache Software License 2.0]: http://www.apache.org/licenses/LICENSE-2.0
-[Mozilla Public License 2.0]: https://www.mozilla.org/media/MPL/2.0/index.txt
 [cookiecutter-napari-plugin]: https://github.com/napari/cookiecutter-napari-plugin
 
 [file an issue]: https://github.com/GuignardLab/napari-sc3D-viewer/issues
 [napari-sc3d-viewer]: https://github.com/GuignardLab/napari-sc3D-viewer
-[napari-sc3D-viewer]: https://github.com/GuignardLab/napari-sc3D-viewer
 
-[napari]: https://github.com/napari/napari
 [tox]: https://tox.readthedocs.io/en/latest/
 [pip]: https://pypi.org/project/pip/
-[PyPI]: https://pypi.org/
 [VTK]: https://vtk.org/
 [scanpy]: https://scanpy.readthedocs.io/en/latest/index.html
 [anndata]: https://anndata.readthedocs.io/en/latest/
 [conda]: https://conda.io
```

### Comparing `napari-sc3D-viewer-0.3.1/src/napari_sc3D_viewer.egg-info/SOURCES.txt` & `napari-sc3D-viewer-1.0.0/src/napari_sc3D_viewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-sc3D-viewer-0.3.1/src/napari_sc3d_viewer/_display_embryo.py` & `napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_display_embryo.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,17 +98,16 @@
                 ax.legend()
                 ax.set_axis_off()
             elif points.metadata["2genes"] is None:
                 if points.face_contrast_limits is None:
                     m, M = 0, 1
                 else:
                     m, M = points.face_contrast_limits
-                if (
-                    points.face_colormap.name in plt.colormaps()
-                    or isinstance(points.face_colormap, Colormap)
+                if points.face_colormap.name in plt.colormaps() or isinstance(
+                    points.face_colormap, Colormap
                 ):
                     if points.face_colormap.name in plt.colormaps():
                         cmap = points.face_colormap.name
                     else:
                         cmap = points.mplcmap
                     fig.colorbar(
                         cm.ScalarMappable(
@@ -443,31 +442,22 @@
             points.face_color_mode = "colormap"
         if not self.cmap_check.value:
             points.face_colormap = self.cmap.value
             points.mplcmap = None
         else:
             init_value = self.grey.value
             cmap_mpl = {
-                "red": [
-                    [0., init_value, init_value],
-                    [1., 0., 0.]
-                ],
-                "blue": [
-                    [0., init_value, init_value],
-                    [1., 0., 0.]
-                ],
-                "green": [
-                    [0., init_value, init_value],
-                    [1., 0., 0.]
-                ],
+                "red": [[0.0, init_value, init_value], [1.0, 0.0, 0.0]],
+                "blue": [[0.0, init_value, init_value], [1.0, 0.0, 0.0]],
+                "green": [[0.0, init_value, init_value], [1.0, 0.0, 0.0]],
             }
             cmap_mpl[self.manual_color.value.lower()] = [
-                    [0., init_value, init_value],
-                    [1., 1., 1.]
-                ]
+                [0.0, init_value, init_value],
+                [1.0, 1.0, 1.0],
+            ]
             if self.manual_color.value == "Red":
                 color = 0
             elif self.manual_color.value == "Green":
                 color = 1
             else:
                 color = 2
             cmap_val = [
@@ -1002,24 +992,24 @@
             12: [0.7529411764705882, 0.4588235294117647, 0.6509803921568628],
             13: [0.9647058823529412, 0.13333333333333333, 0.1803921568627451],
             14: [0.7411764705882353, 0.43529411764705883, 0.6705882352941176],
             15: [0.9686274509803922, 0.8823529411764706, 0.6274509803921569],
             16: [1.0, 0.9803921568627451, 0.9803921568627451],
             18: [0.47058823529411764, 0.16470588235294117, 0.7137254901960784],
             20: [0.5019607843137255, 0.5019607843137255, 0.5019607843137255],
-            21: [0.9803921568627451, 0.0, 0.5294117647058824],
+            21: [0.19607843137254902, 0.5137254901960784, 0.996078431372549],
             22: [0.5098039215686274, 0.1803921568627451, 0.10980392156862745],
             23: [0.5215686274509804, 0.4, 0.050980392156862744],
             24: [0.803921568627451, 0.1607843137254902, 0.5647058823529412],
             27: [0.6588235294117647, 0.6588235294117647, 0.6588235294117647],
             29: [0.0, 0.0, 0.5450980392156862],
             30: [0.5450980392156862, 0.2784313725490196, 0.36470588235294116],
             31: [1.0, 0.7568627450980392, 0.1450980392156863],
             32: [0.8705882352941177, 0.6274509803921569, 0.9921568627450981],
-            33: [0.19607843137254902, 0.5137254901960784, 0.996078431372549],
+            33: [0.9803921568627451, 0.0, 0.5294117647058824],
             34: [0.9725490196078431, 0.6313725490196078, 0.6235294117647059],
             35: [0.7098039215686275, 0.9372549019607843, 0.7098039215686275],
             36: [0.1803921568627451, 0.8509803921568627, 1.0],
             39: [0.10980392156862745, 0.5137254901960784, 0.33725490196078434],
             40: [1.0, 0.6470588235294118, 0.30980392156862746],
             41: [0.8470588235294118, 0.7490196078431373, 0.8470588235294118],
         }
@@ -1051,14 +1041,15 @@
         self.viewer.dims.ndisplay = 3
         points = self.viewer.add_points(
             positions,
             face_color=colors_rgb,
             properties=properties,
             metadata={"gene": None, "2genes": None},
             shown=shown,
+            size=15,
         )
 
         self.all_tissues = [
             self.embryo.corres_tissue.get(t, f"{t}")
             for t in self.embryo.all_tissues
         ]
 
@@ -1072,16 +1063,16 @@
         self.tab2 = QTabWidget()
         metric_1g_container = self.build_metric_1g_container()
         metric_2g_container = self.build_metric_2g_container()
         umap_container = self.build_umap_container()
         diff_expr_container = self.build_diff_expr_container()
         self.tab2.addTab(metric_1g_container.native, "Single Metric")
         self.tab2.addTab(metric_2g_container.native, "2 Genes")
-        last_tab = self.tab2.addTab(umap_container.native, "umap")
-        self.tab2.addTab(diff_expr_container.native, "Diff Expr")
+        self.tab2.addTab(umap_container.native, "umap")
+        last_tab = self.tab2.addTab(diff_expr_container.native, "Diff Expr")
         self.tab2.nb_tabs = last_tab
 
         self.viewer.window.add_dock_widget(
             self.tab1, name="Tissue visualization"
         )
         self.viewer.window.add_dock_widget(
             self.tab2, name="Metric visualization"
```

### Comparing `napari-sc3D-viewer-0.3.1/src/napari_sc3d_viewer/_tests/test_widget.py` & `napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-sc3D-viewer-0.3.1/src/napari_sc3d_viewer/_umap_selection.py` & `napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_umap_selection.py`

 * *Files identical despite different names*

### Comparing `napari-sc3D-viewer-0.3.1/src/napari_sc3d_viewer/_utils.py` & `napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-sc3D-viewer-0.3.1/src/napari_sc3d_viewer/_widget_load.py` & `napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_widget_load.py`

 * *Files identical despite different names*

### Comparing `napari-sc3D-viewer-0.3.1/src/napari_sc3d_viewer/_widget_register.py` & `napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/_widget_register.py`

 * *Files identical despite different names*

### Comparing `napari-sc3D-viewer-0.3.1/src/napari_sc3d_viewer/napari.yaml` & `napari-sc3D-viewer-1.0.0/src/napari_sc3d_viewer/napari.yaml`

 * *Files identical despite different names*

