# Comparing `tmp/qeplot-1.0.2.tar.gz` & `tmp/qeplot-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qeplot-1.0.2.tar", last modified: Thu Jul  6 12:00:10 2023, max compression
+gzip compressed data, was "qeplot-1.0.3.tar", last modified: Thu Jul  6 12:02:35 2023, max compression
```

## Comparing `qeplot-1.0.2.tar` & `qeplot-1.0.3.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:10.188621 qeplot-1.0.2/
--rw-rw-rw-   0        0        0    35822 2023-01-01 17:34:12.000000 qeplot-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      580 2023-07-06 12:00:10.188621 qeplot-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      870 2023-01-11 23:05:09.000000 qeplot-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:10.048545 qeplot-1.0.2/qeplot/
--rw-rw-rw-   0        0        0      360 2023-01-11 23:07:27.000000 qeplot-1.0.2/qeplot/BibTeX.dat
--rw-rw-rw-   0        0        0    47799 2022-03-23 22:06:30.000000 qeplot-1.0.2/qeplot/DOI.png
--rw-rw-rw-   0        0        0     3592 2023-01-11 23:07:54.000000 qeplot-1.0.2/qeplot/VASProcar.py
--rw-rw-rw-   0        0        0      237 2023-01-01 18:46:27.000000 qeplot-1.0.2/qeplot/__init__.py
--rw-rw-rw-   0        0        0     3592 2023-01-11 23:08:04.000000 qeplot-1.0.2/qeplot/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:10.094392 qeplot-1.0.2/qeplot/src/
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:10.110017 qeplot-1.0.2/qeplot/src/_QE/
--rw-rw-rw-   0        0        0    17032 2023-01-01 18:36:19.000000 qeplot-1.0.2/qeplot/src/_QE/_info.py
--rw-rw-rw-   0        0        0    20395 2023-01-01 18:36:39.000000 qeplot-1.0.2/qeplot/src/_QE/_info_b.py
--rw-rw-rw-   0        0        0    12814 2023-01-01 18:36:44.000000 qeplot-1.0.2/qeplot/src/_QE/_label.py
--rw-rw-rw-   0        0        0    18490 2023-01-01 18:36:50.000000 qeplot-1.0.2/qeplot/src/_QE/_nscf.py
--rw-rw-rw-   0        0        0     3010 2023-01-01 18:36:56.000000 qeplot-1.0.2/qeplot/src/_QE/_var_kpoints.py
--rw-rw-rw-   0        0        0    26243 2023-01-01 18:37:00.000000 qeplot-1.0.2/qeplot/src/_QE/dos_pdos_ldos.py
--rw-rw-rw-   0        0        0    21098 2023-01-01 18:37:06.000000 qeplot-1.0.2/qeplot/src/_QE/kpoints_2D_3D.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:10.125641 qeplot-1.0.2/qeplot/src/_VASP/
--rw-rw-rw-   0        0        0    18327 2023-01-01 18:37:14.000000 qeplot-1.0.2/qeplot/src/_VASP/_info.py
--rw-rw-rw-   0        0        0    14006 2023-01-01 18:37:18.000000 qeplot-1.0.2/qeplot/src/_VASP/_info_b.py
--rw-rw-rw-   0        0        0    15662 2023-01-01 18:37:23.000000 qeplot-1.0.2/qeplot/src/_VASP/_label.py
--rw-rw-rw-   0        0        0    31430 2023-01-01 18:37:28.000000 qeplot-1.0.2/qeplot/src/_VASP/_nscf.py
--rw-rw-rw-   0        0        0    19911 2023-01-01 18:37:33.000000 qeplot-1.0.2/qeplot/src/_VASP/_nscf_b.py
--rw-rw-rw-   0        0        0     9422 2023-01-01 18:37:38.000000 qeplot-1.0.2/qeplot/src/_VASP/_var_kpoints.py
--rw-rw-rw-   0        0        0    32183 2023-01-11 23:00:37.000000 qeplot-1.0.2/qeplot/src/_VASP/contribuicao.py
--rw-rw-rw-   0        0        0    20704 2023-01-11 12:44:41.000000 qeplot-1.0.2/qeplot/src/_VASP/contribuicao_OLD.py
--rw-rw-rw-   0        0        0    14021 2023-01-01 18:37:43.000000 qeplot-1.0.2/qeplot/src/_VASP/dielectric_function.py
--rw-rw-rw-   0        0        0    26243 2023-01-01 18:37:48.000000 qeplot-1.0.2/qeplot/src/_VASP/dos_pdos_ldos.py
--rw-rw-rw-   0        0        0    28272 2023-01-01 18:37:52.000000 qeplot-1.0.2/qeplot/src/_VASP/dos_pdos_ldos_[polarizado].py
--rw-rw-rw-   0        0        0    24293 2023-01-01 18:37:57.000000 qeplot-1.0.2/qeplot/src/_VASP/kpoints_2D_3D.py
--rw-rw-rw-   0        0        0    15069 2023-01-01 18:38:01.000000 qeplot-1.0.2/qeplot/src/_VASP/parchg.py
--rw-rw-rw-   0        0        0    14798 2023-01-01 18:38:06.000000 qeplot-1.0.2/qeplot/src/_VASP/potencial.py
--rw-rw-rw-   0        0        0    15008 2023-01-01 18:38:11.000000 qeplot-1.0.2/qeplot/src/_VASP/wave_function.py
--rw-rw-rw-   0        0        0      626 2023-01-01 18:34:45.000000 qeplot-1.0.2/qeplot/src/_loop.py
--rw-rw-rw-   0        0        0    16246 2023-01-11 19:49:27.000000 qeplot-1.0.2/qeplot/src/_settings.py
--rw-rw-rw-   0        0        0     2934 2023-01-01 18:34:56.000000 qeplot-1.0.2/qeplot/src/_update.py
--rw-rw-rw-   0        0        0    17039 2023-01-01 18:35:01.000000 qeplot-1.0.2/qeplot/src/bandas_2D.py
--rw-rw-rw-   0        0        0    16298 2023-01-01 18:35:11.000000 qeplot-1.0.2/qeplot/src/bandas_3D.py
--rw-rw-rw-   0        0        0    14631 2023-01-01 18:35:16.000000 qeplot-1.0.2/qeplot/src/bandas_4D.py
--rw-rw-rw-   0        0        0     2100 2023-01-01 18:35:27.000000 qeplot-1.0.2/qeplot/src/correction_file.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:10.125641 qeplot-1.0.2/qeplot/src/etc/
--rw-rw-rw-   0        0        0      360 2023-01-11 23:07:27.000000 qeplot-1.0.2/qeplot/src/etc/BibTeX.dat
--rw-rw-rw-   0        0        0    47799 2022-03-23 22:06:30.000000 qeplot-1.0.2/qeplot/src/etc/DOI.png
--rw-rw-rw-   0        0        0   374410 2022-06-01 18:31:32.000000 qeplot-1.0.2/qeplot/src/etc/Greek_alphabet.jpg
--rw-rw-rw-   0        0        0    19627 2023-01-01 18:35:32.000000 qeplot-1.0.2/qeplot/src/fermi_surface.py
--rw-rw-rw-   0        0        0    16979 2023-01-01 18:35:38.000000 qeplot-1.0.2/qeplot/src/level_countour.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:10.172998 qeplot-1.0.2/qeplot/src/plot/
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:10.188621 qeplot-1.0.2/qeplot/src/plot/Grace/
--rw-rw-rw-   0        0        0     5205 2023-01-01 18:39:03.000000 qeplot-1.0.2/qeplot/src/plot/Grace/plot_bandas_2D.py
--rw-rw-rw-   0        0        0     4957 2023-01-01 18:39:09.000000 qeplot-1.0.2/qeplot/src/plot/Grace/plot_dielectric_function.py
--rw-rw-rw-   0        0        0    13217 2023-01-01 18:39:20.000000 qeplot-1.0.2/qeplot/src/plot/Grace/plot_dos_pdos_ldos.py
--rw-rw-rw-   0        0        0    13160 2023-01-01 18:39:24.000000 qeplot-1.0.2/qeplot/src/plot/Grace/plot_dos_pdos_ldos_[polarizado].py
--rw-rw-rw-   0        0        0    11072 2023-01-01 18:39:29.000000 qeplot-1.0.2/qeplot/src/plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py
--rw-rw-rw-   0        0        0     3879 2023-01-01 18:39:33.000000 qeplot-1.0.2/qeplot/src/plot/Grace/plot_parchg.py
--rw-rw-rw-   0        0        0     3795 2023-01-01 18:39:38.000000 qeplot-1.0.2/qeplot/src/plot/Grace/plot_potencial.py
--rw-rw-rw-   0        0        0     6275 2023-01-01 18:39:43.000000 qeplot-1.0.2/qeplot/src/plot/Grace/plot_projecao_localizacao.py
--rw-rw-rw-   0        0        0    11196 2023-01-01 18:39:47.000000 qeplot-1.0.2/qeplot/src/plot/Grace/plot_projecao_orbitais.py
--rw-rw-rw-   0        0        0     6228 2023-01-01 18:39:52.000000 qeplot-1.0.2/qeplot/src/plot/Grace/plot_projecao_psi.py
--rw-rw-rw-   0        0        0    10938 2023-01-01 18:39:56.000000 qeplot-1.0.2/qeplot/src/plot/Grace/plot_projecao_spin.py
--rw-rw-rw-   0        0        0     3986 2023-01-01 18:40:01.000000 qeplot-1.0.2/qeplot/src/plot/Grace/plot_wave_function.py
--rw-rw-rw-   0        0        0     6623 2023-01-01 18:38:43.000000 qeplot-1.0.2/qeplot/src/plot/_plot_settings.py
--rw-rw-rw-   0        0        0     5859 2023-01-01 18:41:14.000000 qeplot-1.0.2/qeplot/src/plot/plot_bandas_2D.py
--rw-rw-rw-   0        0        0     5071 2023-01-01 18:41:25.000000 qeplot-1.0.2/qeplot/src/plot/plot_bandas_3D_matplotlib.py
--rw-rw-rw-   0        0        0     5766 2023-01-01 18:41:39.000000 qeplot-1.0.2/qeplot/src/plot/plot_bandas_3D_plotly.py
--rw-rw-rw-   0        0        0     5247 2023-01-01 18:41:49.000000 qeplot-1.0.2/qeplot/src/plot/plot_bandas_4D_plotly.py
--rw-rw-rw-   0        0        0     4308 2023-01-01 18:42:09.000000 qeplot-1.0.2/qeplot/src/plot/plot_dielectric_function.py
--rw-rw-rw-   0        0        0    13002 2023-01-01 18:42:18.000000 qeplot-1.0.2/qeplot/src/plot/plot_dos_pdos_ldos.py
--rw-rw-rw-   0        0        0    34098 2023-01-01 18:42:27.000000 qeplot-1.0.2/qeplot/src/plot/plot_dos_pdos_ldos_[polarizado].py
--rw-rw-rw-   0        0        0     8322 2023-01-01 18:42:36.000000 qeplot-1.0.2/qeplot/src/plot/plot_fermi_surface.py
--rw-rw-rw-   0        0        0     6501 2023-01-01 18:42:44.000000 qeplot-1.0.2/qeplot/src/plot/plot_level_countour.py
--rw-rw-rw-   0        0        0     4692 2023-01-01 18:42:52.000000 qeplot-1.0.2/qeplot/src/plot/plot_parchg.py
--rw-rw-rw-   0        0        0     4686 2023-01-01 18:43:00.000000 qeplot-1.0.2/qeplot/src/plot/plot_potencial.py
--rw-rw-rw-   0        0        0    14710 2023-01-01 18:43:12.000000 qeplot-1.0.2/qeplot/src/plot/plot_projecao_localizacao.py
--rw-rw-rw-   0        0        0    28396 2023-01-01 18:43:24.000000 qeplot-1.0.2/qeplot/src/plot/plot_projecao_orbitais.py
--rw-rw-rw-   0        0        0    14799 2023-01-01 18:43:34.000000 qeplot-1.0.2/qeplot/src/plot/plot_projecao_psi.py
--rw-rw-rw-   0        0        0     7997 2023-01-01 18:43:44.000000 qeplot-1.0.2/qeplot/src/plot/plot_projecao_spin.py
--rw-rw-rw-   0        0        0    11847 2023-01-01 18:43:56.000000 qeplot-1.0.2/qeplot/src/plot/plot_spin_texture_2D.py
--rw-rw-rw-   0        0        0     9847 2023-01-01 18:44:03.000000 qeplot-1.0.2/qeplot/src/plot/plot_spin_texture_3D.py
--rw-rw-rw-   0        0        0     6322 2023-01-01 18:44:12.000000 qeplot-1.0.2/qeplot/src/plot/plot_spin_texture_4D.py
--rw-rw-rw-   0        0        0     6352 2023-01-01 18:44:20.000000 qeplot-1.0.2/qeplot/src/plot/plot_spin_texture_4D_[iso].py
--rw-rw-rw-   0        0        0    15726 2023-01-01 18:44:28.000000 qeplot-1.0.2/qeplot/src/plot/plot_spin_texture_contour.py
--rw-rw-rw-   0        0        0    17239 2023-01-01 18:44:37.000000 qeplot-1.0.2/qeplot/src/plot/plot_spin_texture_contour_video.py
--rw-rw-rw-   0        0        0     4594 2023-01-01 18:44:45.000000 qeplot-1.0.2/qeplot/src/plot/plot_wave_function.py
--rw-rw-rw-   0        0        0    26618 2023-01-01 18:35:43.000000 qeplot-1.0.2/qeplot/src/projecao_localizacao.py
--rw-rw-rw-   0        0        0    27667 2023-01-01 18:35:47.000000 qeplot-1.0.2/qeplot/src/projecao_orbitais.py
--rw-rw-rw-   0        0        0    33233 2023-01-01 18:35:52.000000 qeplot-1.0.2/qeplot/src/projecao_psi.py
--rw-rw-rw-   0        0        0    24234 2023-01-01 18:35:57.000000 qeplot-1.0.2/qeplot/src/projecao_spin.py
--rw-rw-rw-   0        0        0    22904 2023-01-01 18:36:02.000000 qeplot-1.0.2/qeplot/src/spin_texture.py
--rw-rw-rw-   0        0        0    22428 2023-01-01 18:36:07.000000 qeplot-1.0.2/qeplot/src/spin_texture_contour.py
--rw-rw-rw-   0        0        0    23825 2023-01-01 18:36:11.000000 qeplot-1.0.2/qeplot/src/spin_texture_contour_video.py
-drwxrwxrwx   0        0        0        0 2023-07-06 12:00:10.063134 qeplot-1.0.2/qeplot.egg-info/
--rw-rw-rw-   0        0        0      580 2023-07-06 12:00:09.000000 qeplot-1.0.2/qeplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2984 2023-07-06 12:00:09.000000 qeplot-1.0.2/qeplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 12:00:09.000000 qeplot-1.0.2/qeplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-06 12:00:09.000000 qeplot-1.0.2/qeplot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-06 12:00:09.000000 qeplot-1.0.2/qeplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      114 2023-07-06 12:00:10.188621 qeplot-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      985 2023-07-06 11:59:57.000000 qeplot-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:02:35.138916 qeplot-1.0.3/
+-rw-rw-rw-   0        0        0    35822 2023-01-01 17:34:12.000000 qeplot-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      580 2023-07-06 12:02:35.138916 qeplot-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      870 2023-01-11 23:05:09.000000 qeplot-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 12:02:35.014547 qeplot-1.0.3/qeplot/
+-rw-rw-rw-   0        0        0      360 2023-01-11 23:07:27.000000 qeplot-1.0.3/qeplot/BibTeX.dat
+-rw-rw-rw-   0        0        0    47799 2022-03-23 22:06:30.000000 qeplot-1.0.3/qeplot/DOI.png
+-rw-rw-rw-   0        0        0     3564 2023-07-06 12:02:20.000000 qeplot-1.0.3/qeplot/VASProcar.py
+-rw-rw-rw-   0        0        0      237 2023-01-01 18:46:27.000000 qeplot-1.0.3/qeplot/__init__.py
+-rw-rw-rw-   0        0        0     3564 2023-07-06 12:02:10.000000 qeplot-1.0.3/qeplot/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:02:35.044711 qeplot-1.0.3/qeplot/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 12:02:35.060340 qeplot-1.0.3/qeplot/src/_QE/
+-rw-rw-rw-   0        0        0    17032 2023-01-01 18:36:19.000000 qeplot-1.0.3/qeplot/src/_QE/_info.py
+-rw-rw-rw-   0        0        0    20395 2023-01-01 18:36:39.000000 qeplot-1.0.3/qeplot/src/_QE/_info_b.py
+-rw-rw-rw-   0        0        0    12814 2023-01-01 18:36:44.000000 qeplot-1.0.3/qeplot/src/_QE/_label.py
+-rw-rw-rw-   0        0        0    18490 2023-01-01 18:36:50.000000 qeplot-1.0.3/qeplot/src/_QE/_nscf.py
+-rw-rw-rw-   0        0        0     3010 2023-01-01 18:36:56.000000 qeplot-1.0.3/qeplot/src/_QE/_var_kpoints.py
+-rw-rw-rw-   0        0        0    26243 2023-01-01 18:37:00.000000 qeplot-1.0.3/qeplot/src/_QE/dos_pdos_ldos.py
+-rw-rw-rw-   0        0        0    21098 2023-01-01 18:37:06.000000 qeplot-1.0.3/qeplot/src/_QE/kpoints_2D_3D.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:02:35.075958 qeplot-1.0.3/qeplot/src/_VASP/
+-rw-rw-rw-   0        0        0    18327 2023-01-01 18:37:14.000000 qeplot-1.0.3/qeplot/src/_VASP/_info.py
+-rw-rw-rw-   0        0        0    14006 2023-01-01 18:37:18.000000 qeplot-1.0.3/qeplot/src/_VASP/_info_b.py
+-rw-rw-rw-   0        0        0    15662 2023-01-01 18:37:23.000000 qeplot-1.0.3/qeplot/src/_VASP/_label.py
+-rw-rw-rw-   0        0        0    31430 2023-01-01 18:37:28.000000 qeplot-1.0.3/qeplot/src/_VASP/_nscf.py
+-rw-rw-rw-   0        0        0    19911 2023-01-01 18:37:33.000000 qeplot-1.0.3/qeplot/src/_VASP/_nscf_b.py
+-rw-rw-rw-   0        0        0     9422 2023-01-01 18:37:38.000000 qeplot-1.0.3/qeplot/src/_VASP/_var_kpoints.py
+-rw-rw-rw-   0        0        0    32183 2023-01-11 23:00:37.000000 qeplot-1.0.3/qeplot/src/_VASP/contribuicao.py
+-rw-rw-rw-   0        0        0    20704 2023-01-11 12:44:41.000000 qeplot-1.0.3/qeplot/src/_VASP/contribuicao_OLD.py
+-rw-rw-rw-   0        0        0    14021 2023-01-01 18:37:43.000000 qeplot-1.0.3/qeplot/src/_VASP/dielectric_function.py
+-rw-rw-rw-   0        0        0    26243 2023-01-01 18:37:48.000000 qeplot-1.0.3/qeplot/src/_VASP/dos_pdos_ldos.py
+-rw-rw-rw-   0        0        0    28272 2023-01-01 18:37:52.000000 qeplot-1.0.3/qeplot/src/_VASP/dos_pdos_ldos_[polarizado].py
+-rw-rw-rw-   0        0        0    24293 2023-01-01 18:37:57.000000 qeplot-1.0.3/qeplot/src/_VASP/kpoints_2D_3D.py
+-rw-rw-rw-   0        0        0    15069 2023-01-01 18:38:01.000000 qeplot-1.0.3/qeplot/src/_VASP/parchg.py
+-rw-rw-rw-   0        0        0    14798 2023-01-01 18:38:06.000000 qeplot-1.0.3/qeplot/src/_VASP/potencial.py
+-rw-rw-rw-   0        0        0    15008 2023-01-01 18:38:11.000000 qeplot-1.0.3/qeplot/src/_VASP/wave_function.py
+-rw-rw-rw-   0        0        0      626 2023-01-01 18:34:45.000000 qeplot-1.0.3/qeplot/src/_loop.py
+-rw-rw-rw-   0        0        0    16246 2023-01-11 19:49:27.000000 qeplot-1.0.3/qeplot/src/_settings.py
+-rw-rw-rw-   0        0        0     2934 2023-01-01 18:34:56.000000 qeplot-1.0.3/qeplot/src/_update.py
+-rw-rw-rw-   0        0        0    17039 2023-01-01 18:35:01.000000 qeplot-1.0.3/qeplot/src/bandas_2D.py
+-rw-rw-rw-   0        0        0    16298 2023-01-01 18:35:11.000000 qeplot-1.0.3/qeplot/src/bandas_3D.py
+-rw-rw-rw-   0        0        0    14631 2023-01-01 18:35:16.000000 qeplot-1.0.3/qeplot/src/bandas_4D.py
+-rw-rw-rw-   0        0        0     2100 2023-01-01 18:35:27.000000 qeplot-1.0.3/qeplot/src/correction_file.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:02:35.075958 qeplot-1.0.3/qeplot/src/etc/
+-rw-rw-rw-   0        0        0      360 2023-01-11 23:07:27.000000 qeplot-1.0.3/qeplot/src/etc/BibTeX.dat
+-rw-rw-rw-   0        0        0    47799 2022-03-23 22:06:30.000000 qeplot-1.0.3/qeplot/src/etc/DOI.png
+-rw-rw-rw-   0        0        0   374410 2022-06-01 18:31:32.000000 qeplot-1.0.3/qeplot/src/etc/Greek_alphabet.jpg
+-rw-rw-rw-   0        0        0    19627 2023-01-01 18:35:32.000000 qeplot-1.0.3/qeplot/src/fermi_surface.py
+-rw-rw-rw-   0        0        0    16979 2023-01-01 18:35:38.000000 qeplot-1.0.3/qeplot/src/level_countour.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:02:35.123282 qeplot-1.0.3/qeplot/src/plot/
+drwxrwxrwx   0        0        0        0 2023-07-06 12:02:35.138916 qeplot-1.0.3/qeplot/src/plot/Grace/
+-rw-rw-rw-   0        0        0     5205 2023-01-01 18:39:03.000000 qeplot-1.0.3/qeplot/src/plot/Grace/plot_bandas_2D.py
+-rw-rw-rw-   0        0        0     4957 2023-01-01 18:39:09.000000 qeplot-1.0.3/qeplot/src/plot/Grace/plot_dielectric_function.py
+-rw-rw-rw-   0        0        0    13217 2023-01-01 18:39:20.000000 qeplot-1.0.3/qeplot/src/plot/Grace/plot_dos_pdos_ldos.py
+-rw-rw-rw-   0        0        0    13160 2023-01-01 18:39:24.000000 qeplot-1.0.3/qeplot/src/plot/Grace/plot_dos_pdos_ldos_[polarizado].py
+-rw-rw-rw-   0        0        0    11072 2023-01-01 18:39:29.000000 qeplot-1.0.3/qeplot/src/plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py
+-rw-rw-rw-   0        0        0     3879 2023-01-01 18:39:33.000000 qeplot-1.0.3/qeplot/src/plot/Grace/plot_parchg.py
+-rw-rw-rw-   0        0        0     3795 2023-01-01 18:39:38.000000 qeplot-1.0.3/qeplot/src/plot/Grace/plot_potencial.py
+-rw-rw-rw-   0        0        0     6275 2023-01-01 18:39:43.000000 qeplot-1.0.3/qeplot/src/plot/Grace/plot_projecao_localizacao.py
+-rw-rw-rw-   0        0        0    11196 2023-01-01 18:39:47.000000 qeplot-1.0.3/qeplot/src/plot/Grace/plot_projecao_orbitais.py
+-rw-rw-rw-   0        0        0     6228 2023-01-01 18:39:52.000000 qeplot-1.0.3/qeplot/src/plot/Grace/plot_projecao_psi.py
+-rw-rw-rw-   0        0        0    10938 2023-01-01 18:39:56.000000 qeplot-1.0.3/qeplot/src/plot/Grace/plot_projecao_spin.py
+-rw-rw-rw-   0        0        0     3986 2023-01-01 18:40:01.000000 qeplot-1.0.3/qeplot/src/plot/Grace/plot_wave_function.py
+-rw-rw-rw-   0        0        0     6623 2023-01-01 18:38:43.000000 qeplot-1.0.3/qeplot/src/plot/_plot_settings.py
+-rw-rw-rw-   0        0        0     5859 2023-01-01 18:41:14.000000 qeplot-1.0.3/qeplot/src/plot/plot_bandas_2D.py
+-rw-rw-rw-   0        0        0     5071 2023-01-01 18:41:25.000000 qeplot-1.0.3/qeplot/src/plot/plot_bandas_3D_matplotlib.py
+-rw-rw-rw-   0        0        0     5766 2023-01-01 18:41:39.000000 qeplot-1.0.3/qeplot/src/plot/plot_bandas_3D_plotly.py
+-rw-rw-rw-   0        0        0     5247 2023-01-01 18:41:49.000000 qeplot-1.0.3/qeplot/src/plot/plot_bandas_4D_plotly.py
+-rw-rw-rw-   0        0        0     4308 2023-01-01 18:42:09.000000 qeplot-1.0.3/qeplot/src/plot/plot_dielectric_function.py
+-rw-rw-rw-   0        0        0    13002 2023-01-01 18:42:18.000000 qeplot-1.0.3/qeplot/src/plot/plot_dos_pdos_ldos.py
+-rw-rw-rw-   0        0        0    34098 2023-01-01 18:42:27.000000 qeplot-1.0.3/qeplot/src/plot/plot_dos_pdos_ldos_[polarizado].py
+-rw-rw-rw-   0        0        0     8322 2023-01-01 18:42:36.000000 qeplot-1.0.3/qeplot/src/plot/plot_fermi_surface.py
+-rw-rw-rw-   0        0        0     6501 2023-01-01 18:42:44.000000 qeplot-1.0.3/qeplot/src/plot/plot_level_countour.py
+-rw-rw-rw-   0        0        0     4692 2023-01-01 18:42:52.000000 qeplot-1.0.3/qeplot/src/plot/plot_parchg.py
+-rw-rw-rw-   0        0        0     4686 2023-01-01 18:43:00.000000 qeplot-1.0.3/qeplot/src/plot/plot_potencial.py
+-rw-rw-rw-   0        0        0    14710 2023-01-01 18:43:12.000000 qeplot-1.0.3/qeplot/src/plot/plot_projecao_localizacao.py
+-rw-rw-rw-   0        0        0    28396 2023-01-01 18:43:24.000000 qeplot-1.0.3/qeplot/src/plot/plot_projecao_orbitais.py
+-rw-rw-rw-   0        0        0    14799 2023-01-01 18:43:34.000000 qeplot-1.0.3/qeplot/src/plot/plot_projecao_psi.py
+-rw-rw-rw-   0        0        0     7997 2023-01-01 18:43:44.000000 qeplot-1.0.3/qeplot/src/plot/plot_projecao_spin.py
+-rw-rw-rw-   0        0        0    11847 2023-01-01 18:43:56.000000 qeplot-1.0.3/qeplot/src/plot/plot_spin_texture_2D.py
+-rw-rw-rw-   0        0        0     9847 2023-01-01 18:44:03.000000 qeplot-1.0.3/qeplot/src/plot/plot_spin_texture_3D.py
+-rw-rw-rw-   0        0        0     6322 2023-01-01 18:44:12.000000 qeplot-1.0.3/qeplot/src/plot/plot_spin_texture_4D.py
+-rw-rw-rw-   0        0        0     6352 2023-01-01 18:44:20.000000 qeplot-1.0.3/qeplot/src/plot/plot_spin_texture_4D_[iso].py
+-rw-rw-rw-   0        0        0    15726 2023-01-01 18:44:28.000000 qeplot-1.0.3/qeplot/src/plot/plot_spin_texture_contour.py
+-rw-rw-rw-   0        0        0    17239 2023-01-01 18:44:37.000000 qeplot-1.0.3/qeplot/src/plot/plot_spin_texture_contour_video.py
+-rw-rw-rw-   0        0        0     4594 2023-01-01 18:44:45.000000 qeplot-1.0.3/qeplot/src/plot/plot_wave_function.py
+-rw-rw-rw-   0        0        0    26618 2023-01-01 18:35:43.000000 qeplot-1.0.3/qeplot/src/projecao_localizacao.py
+-rw-rw-rw-   0        0        0    27667 2023-01-01 18:35:47.000000 qeplot-1.0.3/qeplot/src/projecao_orbitais.py
+-rw-rw-rw-   0        0        0    33233 2023-01-01 18:35:52.000000 qeplot-1.0.3/qeplot/src/projecao_psi.py
+-rw-rw-rw-   0        0        0    24234 2023-01-01 18:35:57.000000 qeplot-1.0.3/qeplot/src/projecao_spin.py
+-rw-rw-rw-   0        0        0    22904 2023-01-01 18:36:02.000000 qeplot-1.0.3/qeplot/src/spin_texture.py
+-rw-rw-rw-   0        0        0    22428 2023-01-01 18:36:07.000000 qeplot-1.0.3/qeplot/src/spin_texture_contour.py
+-rw-rw-rw-   0        0        0    23825 2023-01-01 18:36:11.000000 qeplot-1.0.3/qeplot/src/spin_texture_contour_video.py
+drwxrwxrwx   0        0        0        0 2023-07-06 12:02:35.014547 qeplot-1.0.3/qeplot.egg-info/
+-rw-rw-rw-   0        0        0      580 2023-07-06 12:02:34.000000 qeplot-1.0.3/qeplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2984 2023-07-06 12:02:34.000000 qeplot-1.0.3/qeplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 12:02:34.000000 qeplot-1.0.3/qeplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-06 12:02:34.000000 qeplot-1.0.3/qeplot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 12:02:34.000000 qeplot-1.0.3/qeplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      114 2023-07-06 12:02:35.138916 qeplot-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      985 2023-07-06 12:02:27.000000 qeplot-1.0.3/setup.py
```

### Comparing `qeplot-1.0.2/LICENSE.txt` & `qeplot-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/PKG-INFO` & `qeplot-1.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qeplot
-Version: 1.0.2
+Version: 1.0.3
 Summary: VASProcar is an open-source package written in the Python 3 programming language, which aims to provide an intuitive tool for the post-processing of the output files produced by the DFT VASP code, through an interactive user interface.
 Home-page: https://doi.org/10.5281/zenodo.6343960
 Download-URL: https://doi.org/10.5281/zenodo.6343960
 Author: Augusto de Lelis Araujo and Renan da Paixao Maciel
 Author-email: augusto-lelis@outlook.com, renan.maciel@physics.uu.se
 License: GNU GPLv3
 License-File: LICENSE.txt
```

### Comparing `qeplot-1.0.2/README.md` & `qeplot-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/DOI.png` & `qeplot-1.0.3/qeplot/DOI.png`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/VASProcar.py` & `qeplot-1.0.3/qeplot/VASProcar.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,21 @@
 print("# ====================================================================")
 print("# Renan da Paixao Maciel                                              ")
 print("# Uppsala University (Uppsala/Sweden)                                 ")
 print("# e-mail: renan.maciel@physics.uu.se                                  ")
 print("######################################################################")
 print(" ")
 
-"""
 print("######################################################################")
 print("# Which package was used for the DFT calculations? ===================")
 print("# [1] VASP (Vienna Ab initio Simulation Package)                      ")
 print("# [2] QE   (Quantum ESPRESSO)  !!! In Tests (Not Functional) !!!      ")
 print("######################################################################")   
 pacote_dft = input(" "); pacote_dft = int(pacote_dft)
 print(" ")
-"""
-
-pacote_dft = 1
 
 if (pacote_dft == 1):
    DFT = '_VASP/' 
    print("######################################################################")
    print("## VASP =========================================================== ##")
    print("## ================================================================ ##")
    print("# Basic files to execute the code: CONTCAR, KPOINTS, OUTCAR, PROCAR ##")
```

### Comparing `qeplot-1.0.2/qeplot/__main__.py` & `qeplot-1.0.3/qeplot/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,21 @@
 print("# ====================================================================")
 print("# Renan da Paixao Maciel                                              ")
 print("# Uppsala University (Uppsala/Sweden)                                 ")
 print("# e-mail: renan.maciel@physics.uu.se                                  ")
 print("######################################################################")
 print(" ")
 
-"""
 print("######################################################################")
 print("# Which package was used for the DFT calculations? ===================")
 print("# [1] VASP (Vienna Ab initio Simulation Package)                      ")
 print("# [2] QE   (Quantum ESPRESSO)  !!! In Tests (Not Functional) !!!      ")
 print("######################################################################")   
 pacote_dft = input(" "); pacote_dft = int(pacote_dft)
 print(" ")
-"""
-
-pacote_dft = 1
 
 if (pacote_dft == 1):
    DFT = '_VASP/' 
    print("######################################################################")
    print("## VASP =========================================================== ##")
    print("## ================================================================ ##")
    print("# Basic files to execute the code: CONTCAR, KPOINTS, OUTCAR, PROCAR ##")
```

### Comparing `qeplot-1.0.2/qeplot/src/_QE/_info.py` & `qeplot-1.0.3/qeplot/src/_QE/_info.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_QE/_info_b.py` & `qeplot-1.0.3/qeplot/src/_QE/_info_b.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_QE/_label.py` & `qeplot-1.0.3/qeplot/src/_QE/_label.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_QE/_nscf.py` & `qeplot-1.0.3/qeplot/src/_QE/_nscf.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_QE/_var_kpoints.py` & `qeplot-1.0.3/qeplot/src/_QE/_var_kpoints.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_QE/dos_pdos_ldos.py` & `qeplot-1.0.3/qeplot/src/_QE/dos_pdos_ldos.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_QE/kpoints_2D_3D.py` & `qeplot-1.0.3/qeplot/src/_QE/kpoints_2D_3D.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_VASP/_info.py` & `qeplot-1.0.3/qeplot/src/_VASP/_info.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_VASP/_info_b.py` & `qeplot-1.0.3/qeplot/src/_VASP/_info_b.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_VASP/_label.py` & `qeplot-1.0.3/qeplot/src/_VASP/_label.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_VASP/_nscf.py` & `qeplot-1.0.3/qeplot/src/_VASP/_nscf.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_VASP/_nscf_b.py` & `qeplot-1.0.3/qeplot/src/_VASP/_nscf_b.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_VASP/_var_kpoints.py` & `qeplot-1.0.3/qeplot/src/_VASP/_var_kpoints.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_VASP/contribuicao.py` & `qeplot-1.0.3/qeplot/src/_VASP/contribuicao.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_VASP/contribuicao_OLD.py` & `qeplot-1.0.3/qeplot/src/_VASP/contribuicao_OLD.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_VASP/dielectric_function.py` & `qeplot-1.0.3/qeplot/src/_VASP/dielectric_function.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_VASP/dos_pdos_ldos.py` & `qeplot-1.0.3/qeplot/src/_VASP/dos_pdos_ldos.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_VASP/dos_pdos_ldos_[polarizado].py` & `qeplot-1.0.3/qeplot/src/_VASP/dos_pdos_ldos_[polarizado].py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_VASP/kpoints_2D_3D.py` & `qeplot-1.0.3/qeplot/src/_VASP/kpoints_2D_3D.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_VASP/parchg.py` & `qeplot-1.0.3/qeplot/src/_VASP/parchg.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_VASP/potencial.py` & `qeplot-1.0.3/qeplot/src/_VASP/potencial.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_VASP/wave_function.py` & `qeplot-1.0.3/qeplot/src/_VASP/wave_function.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_loop.py` & `qeplot-1.0.3/qeplot/src/_loop.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_settings.py` & `qeplot-1.0.3/qeplot/src/_settings.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/_update.py` & `qeplot-1.0.3/qeplot/src/_update.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/bandas_2D.py` & `qeplot-1.0.3/qeplot/src/bandas_2D.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/bandas_3D.py` & `qeplot-1.0.3/qeplot/src/bandas_3D.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/bandas_4D.py` & `qeplot-1.0.3/qeplot/src/bandas_4D.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/correction_file.py` & `qeplot-1.0.3/qeplot/src/correction_file.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/etc/DOI.png` & `qeplot-1.0.3/qeplot/src/etc/DOI.png`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/etc/Greek_alphabet.jpg` & `qeplot-1.0.3/qeplot/src/etc/Greek_alphabet.jpg`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/fermi_surface.py` & `qeplot-1.0.3/qeplot/src/fermi_surface.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/level_countour.py` & `qeplot-1.0.3/qeplot/src/level_countour.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/Grace/plot_bandas_2D.py` & `qeplot-1.0.3/qeplot/src/plot/Grace/plot_bandas_2D.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/Grace/plot_dielectric_function.py` & `qeplot-1.0.3/qeplot/src/plot/Grace/plot_dielectric_function.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/Grace/plot_dos_pdos_ldos.py` & `qeplot-1.0.3/qeplot/src/plot/Grace/plot_dos_pdos_ldos.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/Grace/plot_dos_pdos_ldos_[polarizado].py` & `qeplot-1.0.3/qeplot/src/plot/Grace/plot_dos_pdos_ldos_[polarizado].py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py` & `qeplot-1.0.3/qeplot/src/plot/Grace/plot_dos_pdos_ldos_[polarizado_delta].py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/Grace/plot_parchg.py` & `qeplot-1.0.3/qeplot/src/plot/Grace/plot_parchg.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/Grace/plot_potencial.py` & `qeplot-1.0.3/qeplot/src/plot/Grace/plot_potencial.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/Grace/plot_projecao_localizacao.py` & `qeplot-1.0.3/qeplot/src/plot/Grace/plot_projecao_localizacao.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/Grace/plot_projecao_orbitais.py` & `qeplot-1.0.3/qeplot/src/plot/Grace/plot_projecao_orbitais.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/Grace/plot_projecao_psi.py` & `qeplot-1.0.3/qeplot/src/plot/Grace/plot_projecao_psi.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/Grace/plot_projecao_spin.py` & `qeplot-1.0.3/qeplot/src/plot/Grace/plot_projecao_spin.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/Grace/plot_wave_function.py` & `qeplot-1.0.3/qeplot/src/plot/Grace/plot_wave_function.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/_plot_settings.py` & `qeplot-1.0.3/qeplot/src/plot/_plot_settings.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_bandas_2D.py` & `qeplot-1.0.3/qeplot/src/plot/plot_bandas_2D.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_bandas_3D_matplotlib.py` & `qeplot-1.0.3/qeplot/src/plot/plot_bandas_3D_matplotlib.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_bandas_3D_plotly.py` & `qeplot-1.0.3/qeplot/src/plot/plot_bandas_3D_plotly.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_bandas_4D_plotly.py` & `qeplot-1.0.3/qeplot/src/plot/plot_bandas_4D_plotly.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_dielectric_function.py` & `qeplot-1.0.3/qeplot/src/plot/plot_dielectric_function.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_dos_pdos_ldos.py` & `qeplot-1.0.3/qeplot/src/plot/plot_dos_pdos_ldos.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_dos_pdos_ldos_[polarizado].py` & `qeplot-1.0.3/qeplot/src/plot/plot_dos_pdos_ldos_[polarizado].py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_fermi_surface.py` & `qeplot-1.0.3/qeplot/src/plot/plot_fermi_surface.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_level_countour.py` & `qeplot-1.0.3/qeplot/src/plot/plot_level_countour.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_parchg.py` & `qeplot-1.0.3/qeplot/src/plot/plot_parchg.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_potencial.py` & `qeplot-1.0.3/qeplot/src/plot/plot_potencial.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_projecao_localizacao.py` & `qeplot-1.0.3/qeplot/src/plot/plot_projecao_localizacao.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_projecao_orbitais.py` & `qeplot-1.0.3/qeplot/src/plot/plot_projecao_orbitais.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_projecao_psi.py` & `qeplot-1.0.3/qeplot/src/plot/plot_projecao_psi.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_projecao_spin.py` & `qeplot-1.0.3/qeplot/src/plot/plot_projecao_spin.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_spin_texture_2D.py` & `qeplot-1.0.3/qeplot/src/plot/plot_spin_texture_2D.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_spin_texture_3D.py` & `qeplot-1.0.3/qeplot/src/plot/plot_spin_texture_3D.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_spin_texture_4D.py` & `qeplot-1.0.3/qeplot/src/plot/plot_spin_texture_4D.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_spin_texture_4D_[iso].py` & `qeplot-1.0.3/qeplot/src/plot/plot_spin_texture_4D_[iso].py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_spin_texture_contour.py` & `qeplot-1.0.3/qeplot/src/plot/plot_spin_texture_contour.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_spin_texture_contour_video.py` & `qeplot-1.0.3/qeplot/src/plot/plot_spin_texture_contour_video.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/plot/plot_wave_function.py` & `qeplot-1.0.3/qeplot/src/plot/plot_wave_function.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/projecao_localizacao.py` & `qeplot-1.0.3/qeplot/src/projecao_localizacao.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/projecao_orbitais.py` & `qeplot-1.0.3/qeplot/src/projecao_orbitais.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/projecao_psi.py` & `qeplot-1.0.3/qeplot/src/projecao_psi.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/projecao_spin.py` & `qeplot-1.0.3/qeplot/src/projecao_spin.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/spin_texture.py` & `qeplot-1.0.3/qeplot/src/spin_texture.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/spin_texture_contour.py` & `qeplot-1.0.3/qeplot/src/spin_texture_contour.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot/src/spin_texture_contour_video.py` & `qeplot-1.0.3/qeplot/src/spin_texture_contour_video.py`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/qeplot.egg-info/PKG-INFO` & `qeplot-1.0.3/qeplot.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qeplot
-Version: 1.0.2
+Version: 1.0.3
 Summary: VASProcar is an open-source package written in the Python 3 programming language, which aims to provide an intuitive tool for the post-processing of the output files produced by the DFT VASP code, through an interactive user interface.
 Home-page: https://doi.org/10.5281/zenodo.6343960
 Download-URL: https://doi.org/10.5281/zenodo.6343960
 Author: Augusto de Lelis Araujo and Renan da Paixao Maciel
 Author-email: augusto-lelis@outlook.com, renan.maciel@physics.uu.se
 License: GNU GPLv3
 License-File: LICENSE.txt
```

### Comparing `qeplot-1.0.2/qeplot.egg-info/SOURCES.txt` & `qeplot-1.0.3/qeplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qeplot-1.0.2/setup.py` & `qeplot-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 import json
 from pathlib import Path
 from typing import Optional
 
 setup(
     name = "qeplot",
-    version = "1.0.2",
+    version = "1.0.3",
     description = "VASProcar is an open-source package written in the Python 3 programming language, which aims to provide an intuitive tool for the post-processing of the output files produced by the DFT VASP code, through an interactive user interface.",
     author = "Augusto de Lelis Araujo and Renan da Paixao Maciel", 
     author_email = "augusto-lelis@outlook.com, renan.maciel@physics.uu.se",
     url = "https://doi.org/10.5281/zenodo.6343960",
     download_url = "https://doi.org/10.5281/zenodo.6343960",
     license = "GNU GPLv3",
     install_requires=['numpy','scipy','matplotlib','plotly','moviepy','kaleido'],
```

