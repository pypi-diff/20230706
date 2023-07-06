# Comparing `tmp/pyteseo-0.0.6.tar.gz` & `tmp/pyteseo-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyteseo-0.0.6.tar", last modified: Tue May 23 15:50:47 2023, max compression
+gzip compressed data, was "pyteseo-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyteseo-0.0.6.tar` & `pyteseo-0.0.7.tar`

### file list

```diff
@@ -1,521 +1,539 @@
--rw-r--r--   0        0        0    53248 2023-05-23 10:32:12.589254 pyteseo-0.0.6/.coverage
--rw-r--r--   0        0        0      169 2023-01-23 16:09:52.078560 pyteseo-0.0.6/.flake8
--rw-r--r--   0        0        0     1545 2023-04-17 10:00:47.217406 pyteseo-0.0.6/.github/workflows/docs.yml
--rw-r--r--   0        0        0     1101 2023-05-12 06:59:34.879572 pyteseo-0.0.6/.github/workflows/tests.yml
--rw-r--r--   0        0        0      179 2023-04-25 08:09:50.561302 pyteseo-0.0.6/.gitignore
--rw-r--r--   0        0        0      504 2023-01-16 10:53:29.863142 pyteseo-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2710 2023-05-23 11:45:21.401972 pyteseo-0.0.6/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2023-05-22 06:33:42.865296 pyteseo-0.0.6/LICENSE.md
--rw-r--r--   0        0        0     4271 2023-05-23 11:38:39.646969 pyteseo-0.0.6/README.md
--rw-r--r--   0        0        0      634 2022-12-28 11:40:36.607121 pyteseo-0.0.6/docs/Makefile
--rw-r--r--   0        0        0    31102 2022-12-28 11:40:36.627121 pyteseo-0.0.6/docs/_static/TESEO_logo.png
--rw-r--r--   0        0        0    84936 2023-01-09 07:22:45.451292 pyteseo-0.0.6/docs/_static/doc_snapshoot.png
--rw-r--r--   0        0        0    28715 2022-12-28 11:40:36.627121 pyteseo-0.0.6/docs/_static/pyTESEO_logo.png
--rw-r--r--   0        0        0       55 2023-01-13 08:20:28.115803 pyteseo-0.0.6/docs/changelog.md
--rw-r--r--   0        0        0     1822 2023-01-20 10:27:58.065661 pyteseo-0.0.6/docs/conf.py
--rw-r--r--   0        0        0     2350 2023-01-13 08:20:28.115803 pyteseo-0.0.6/docs/get-started.md
--rw-r--r--   0        0        0     2211 2023-01-13 08:20:28.115803 pyteseo-0.0.6/docs/index.md
--rw-r--r--   0        0        0      800 2022-12-28 11:40:36.627121 pyteseo-0.0.6/docs/make.bat
--rw-r--r--   0        0        0   263466 2023-05-15 10:11:00.364302 pyteseo-0.0.6/docs/notebooks/01_read_domain.ipynb
--rw-r--r--   0        0        0    42212 2023-05-11 13:51:39.835822 pyteseo-0.0.6/docs/notebooks/02_read_forcings.ipynb
--rw-r--r--   0        0        0   947681 2023-05-11 13:51:51.776549 pyteseo-0.0.6/docs/notebooks/03_export_results.ipynb
--rw-r--r--   0        0        0    17456 2023-05-11 13:52:48.710040 pyteseo-0.0.6/docs/notebooks/04_generate_forcings_from_cmems.ipynb
--rw-r--r--   0        0        0   116574 2023-05-11 13:59:37.901052 pyteseo-0.0.6/docs/notebooks/05_drift_simulation.ipynb
--rw-r--r--   0        0        0      711 2023-01-19 16:35:42.758020 pyteseo-0.0.6/docs/notebooks/06_hns_simulation.ipynb
--rw-r--r--   0        0        0      686 2023-05-11 13:54:12.425183 pyteseo-0.0.6/docs/notebooks/07_stochastic_montecarlo.ipynb
--rw-r--r--   0        0        0      753 2023-01-19 16:35:42.758020 pyteseo-0.0.6/docs/notebooks/08_stochastic_kmeans.ipynb
--rw-r--r--   0        0        0      974 2023-01-11 10:07:46.886424 pyteseo-0.0.6/docs/user-guide.md
--rw-r--r--   0        0        0      407 2023-05-17 07:12:34.718790 pyteseo-0.0.6/environment-dev.yml
--rw-r--r--   0        0        0      235 2023-05-17 07:12:57.360321 pyteseo-0.0.6/environment.yml
--rw-r--r--   0        0        0     1933 2023-05-23 15:33:31.407192 pyteseo-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      361 2023-04-18 11:50:41.715252 pyteseo-0.0.6/pyteseo/__init__.py
--rw-r--r--   0        0        0     7776 2023-05-22 08:13:07.751692 pyteseo-0.0.6/pyteseo/classes.py
--rw-r--r--   0        0        0        0 2023-02-13 12:13:20.197722 pyteseo-0.0.6/pyteseo/connections/__init__.py
--rw-r--r--   0        0        0     2346 2023-05-18 14:24:41.952116 pyteseo-0.0.6/pyteseo/connections/bathymetries.py
--rw-r--r--   0        0        0     5957 2023-05-22 06:19:42.815869 pyteseo-0.0.6/pyteseo/connections/cmems.py
--rw-r--r--   0        0        0     3132 2023-05-23 10:26:56.283747 pyteseo-0.0.6/pyteseo/connections/coastlines.py
--rw-r--r--   0        0        0     2535 2023-05-22 06:18:49.791063 pyteseo-0.0.6/pyteseo/connections/noaa_opendap.py
--rw-r--r--   0        0        0    13416 2023-05-18 06:18:08.958963 pyteseo-0.0.6/pyteseo/data/substances/hns.xlsx
--rw-r--r--   0        0        0     5208 2023-05-18 06:16:20.039757 pyteseo-0.0.6/pyteseo/data/substances/hns_units.xlsx
--rw-r--r--   0        0        0     5849 2023-05-18 06:16:00.696375 pyteseo-0.0.6/pyteseo/data/substances/oil.xlsx
--rw-r--r--   0        0        0     5079 2023-05-18 06:16:00.696375 pyteseo-0.0.6/pyteseo/data/substances/oil_units.xlsx
--rw-r--r--   0        0        0     6521 2023-05-22 08:03:45.257543 pyteseo-0.0.6/pyteseo/defaults.py
--rw-r--r--   0        0        0      194 2023-02-02 09:27:00.724058 pyteseo-0.0.6/pyteseo/export/__init__.py
--rw-r--r--   0        0        0     4827 2023-04-19 07:13:56.452163 pyteseo-0.0.6/pyteseo/export/grids.py
--rw-r--r--   0        0        0     3236 2023-04-14 11:07:51.005172 pyteseo-0.0.6/pyteseo/export/particles.py
--rw-r--r--   0        0        0     1627 2023-02-10 07:53:13.427520 pyteseo-0.0.6/pyteseo/export/properties.py
--rw-r--r--   0        0        0      193 2023-02-02 09:18:50.744064 pyteseo-0.0.6/pyteseo/io/__init__.py
--rw-r--r--   0        0        0    16833 2023-05-17 10:24:34.307917 pyteseo-0.0.6/pyteseo/io/cfg.py
--rw-r--r--   0        0        0     4499 2023-05-18 14:49:34.064244 pyteseo-0.0.6/pyteseo/io/coastline.py
--rw-r--r--   0        0        0     6698 2023-05-22 06:57:42.067158 pyteseo-0.0.6/pyteseo/io/forcings.py
--rw-r--r--   0        0        0     2608 2023-05-18 14:48:33.935729 pyteseo-0.0.6/pyteseo/io/grid.py
--rw-r--r--   0        0        0     3448 2023-04-17 07:20:52.886042 pyteseo-0.0.6/pyteseo/io/hns_calib.py
--rw-r--r--   0        0        0     6628 2023-04-17 09:25:25.739679 pyteseo-0.0.6/pyteseo/io/results.py
--rw-r--r--   0        0        0     4797 2023-04-17 09:22:03.598328 pyteseo-0.0.6/pyteseo/io/run.py
--rw-r--r--   0        0        0     1941 2023-05-22 07:08:05.418464 pyteseo-0.0.6/pyteseo/io/substances.py
--rw-r--r--   0        0        0     1915 2023-05-10 15:18:33.918998 pyteseo-0.0.6/pyteseo/io/utils.py
--rw-r--r--   0        0        0        0 2023-05-15 08:24:20.888146 pyteseo-0.0.6/pyteseo/plot/__init__.py
--rw-r--r--   0        0        0     6833 2023-05-15 10:29:06.337329 pyteseo-0.0.6/pyteseo/plot/animations.py
--rw-r--r--   0        0        0     4883 2023-05-18 15:14:13.389991 pyteseo-0.0.6/pyteseo/plot/basics.py
--rw-r--r--   0        0        0     2231 2023-05-18 15:19:31.369304 pyteseo-0.0.6/pyteseo/plot/figures.py
--rw-r--r--   0        0        0     4277 2023-05-23 08:14:04.746173 pyteseo-0.0.6/pyteseo/services.py
--rw-r--r--   0        0        0      309 2023-05-12 06:12:32.629928 pyteseo-0.0.6/pyteseo/tests/__init__.py
--rw-r--r--   0        0        0     1080 2022-11-28 12:31:04.243939 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000000.txt
--rw-r--r--   0        0        0     1440 2022-11-28 12:31:25.250905 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000005.txt
--rw-r--r--   0        0        0     1320 2022-11-28 12:31:42.101870 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000010.txt
--rw-r--r--   0        0        0     1440 2022-11-28 12:31:56.340847 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000015.txt
--rw-r--r--   0        0        0     1800 2022-11-28 12:32:08.201821 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000020.txt
--rw-r--r--   0        0        0     1920 2022-11-28 12:32:19.311799 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000025.txt
--rw-r--r--   0        0        0     1800 2022-11-28 12:32:30.205778 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000030.txt
--rw-r--r--   0        0        0     1920 2022-11-28 12:32:40.120760 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000035.txt
--rw-r--r--   0        0        0     1920 2022-11-28 12:32:49.096757 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000040.txt
--rw-r--r--   0        0        0     2040 2022-11-28 12:32:56.968763 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000045.txt
--rw-r--r--   0        0        0     2280 2022-11-28 12:33:04.886785 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000050.txt
--rw-r--r--   0        0        0     2640 2022-11-28 12:33:12.049766 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000055.txt
--rw-r--r--   0        0        0     2640 2022-11-28 12:33:19.004754 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000060.txt
--rw-r--r--   0        0        0     3240 2022-11-28 12:33:49.743762 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000065.txt
--rw-r--r--   0        0        0     3840 2022-11-28 12:33:56.320750 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000070.txt
--rw-r--r--   0        0        0     3960 2022-11-28 12:34:03.214770 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000075.txt
--rw-r--r--   0        0        0     4440 2022-11-28 12:34:09.897757 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000080.txt
--rw-r--r--   0        0        0     4920 2022-11-28 12:34:17.619757 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000085.txt
--rw-r--r--   0        0        0     5280 2022-11-28 12:34:25.163765 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000090.txt
--rw-r--r--   0        0        0     1080 2022-11-28 12:31:04.243939 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000000.txt
--rw-r--r--   0        0        0     1440 2022-11-28 12:31:25.250905 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000005.txt
--rw-r--r--   0        0        0     1320 2022-11-28 12:31:42.101870 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000010.txt
--rw-r--r--   0        0        0     1440 2022-11-28 12:31:56.340847 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000015.txt
--rw-r--r--   0        0        0     1800 2022-11-28 12:32:08.201821 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000020.txt
--rw-r--r--   0        0        0     1920 2022-11-28 12:32:19.311799 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000025.txt
--rw-r--r--   0        0        0     1800 2022-11-28 12:32:30.205778 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000030.txt
--rw-r--r--   0        0        0     1920 2022-11-28 12:32:40.120760 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000035.txt
--rw-r--r--   0        0        0     1920 2022-11-28 12:32:49.096757 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000040.txt
--rw-r--r--   0        0        0     2040 2022-11-28 12:32:56.968763 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000045.txt
--rw-r--r--   0        0        0     2280 2022-11-28 12:33:04.886785 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000050.txt
--rw-r--r--   0        0        0     2640 2022-11-28 12:33:12.049766 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000055.txt
--rw-r--r--   0        0        0     2640 2022-11-28 12:33:19.004754 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000060.txt
--rw-r--r--   0        0        0     3240 2022-11-28 12:33:49.743762 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000065.txt
--rw-r--r--   0        0        0     3840 2022-11-28 12:33:56.320750 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000070.txt
--rw-r--r--   0        0        0     3960 2022-11-28 12:34:03.214770 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000075.txt
--rw-r--r--   0        0        0     4440 2022-11-28 12:34:09.897757 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000080.txt
--rw-r--r--   0        0        0     4920 2022-11-28 12:34:17.619757 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000085.txt
--rw-r--r--   0        0        0     5280 2022-11-28 12:34:25.163765 pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000090.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:31:04.219939 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000000.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:31:25.362903 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000005.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:31:42.232868 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000010.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:31:56.503846 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000015.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:32:08.296824 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000020.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:32:19.402804 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000025.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:32:30.379778 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000030.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:32:40.259760 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000035.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:32:49.222751 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000040.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:32:57.430761 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000045.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:33:04.996780 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000050.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:33:12.191766 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000055.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:33:19.144753 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000060.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:33:49.896767 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000065.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:33:56.794749 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000070.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:34:03.348770 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000075.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:34:10.956756 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000080.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:34:18.079761 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000085.txt
--rw-r--r--   0        0        0   500100 2022-11-28 12:34:25.335761 pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000090.txt
--rw-r--r--   0        0        0   121220 2022-11-28 12:59:56.013665 pyteseo-0.0.6/pyteseo/tests/data/cas1_properties_001.txt
--rw-r--r--   0        0        0   121220 2022-11-28 12:59:56.013665 pyteseo-0.0.6/pyteseo/tests/data/cas1_properties_002.txt
--rw-r--r--   0        0        0   574769 2023-01-13 08:20:28.115803 pyteseo-0.0.6/pyteseo/tests/data/coastline.dat
--rw-r--r--   0        0        0   574787 2023-01-13 08:20:28.125803 pyteseo-0.0.6/pyteseo/tests/data/coastline_error_range.dat
--rw-r--r--   0        0        0   574787 2023-01-13 08:20:28.125803 pyteseo-0.0.6/pyteseo/tests/data/coastline_othernanformat.dat
--rw-r--r--   0        0        0   558324 2015-03-24 16:18:44.000000 pyteseo-0.0.6/pyteseo/tests/data/costa_poligono1.dat
--rw-r--r--   0        0        0     3861 2015-03-24 16:18:44.000000 pyteseo-0.0.6/pyteseo/tests/data/costa_poligono2.dat
--rw-r--r--   0        0        0    10412 2023-01-13 08:20:28.125803 pyteseo-0.0.6/pyteseo/tests/data/costa_poligono3.dat
--rw-r--r--   0        0        0     2183 2023-01-13 08:20:28.125803 pyteseo-0.0.6/pyteseo/tests/data/costa_poligono4.dat
--rw-r--r--   0        0        0    33889 2023-05-16 06:59:34.843214 pyteseo-0.0.6/pyteseo/tests/data/currents.nc
--rw-r--r--   0        0        0      732 2022-11-14 07:58:35.871414 pyteseo-0.0.6/pyteseo/tests/data/currents_000h.txt
--rw-r--r--   0        0        0      732 2022-11-14 07:58:35.950414 pyteseo-0.0.6/pyteseo/tests/data/currents_001h.txt
--rw-r--r--   0        0        0      732 2022-11-14 07:58:36.019414 pyteseo-0.0.6/pyteseo/tests/data/currents_002h.txt
--rw-r--r--   0        0        0      732 2022-11-14 07:58:36.125414 pyteseo-0.0.6/pyteseo/tests/data/currents_003h.txt
--rw-r--r--   0        0        0     6679 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1.cfg
--rw-r--r--   0        0        0     1539 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1.run
--rw-r--r--   0        0        0      616 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000060.txt
--rw-r--r--   0        0        0      704 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000120.txt
--rw-r--r--   0        0        0      880 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000180.txt
--rw-r--r--   0        0        0      880 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000240.txt
--rw-r--r--   0        0        0      880 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000300.txt
--rw-r--r--   0        0        0     1232 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000360.txt
--rw-r--r--   0        0        0      968 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000420.txt
--rw-r--r--   0        0        0      616 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000480.txt
--rw-r--r--   0        0        0      176 2023-05-08 11:03:41.464391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000540.txt
--rw-r--r--   0        0        0      880 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_002_000060.txt
--rw-r--r--   0        0        0      176 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_002_000120.txt
--rw-r--r--   0        0        0       99 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000000.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000060.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000120.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000180.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000240.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000300.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000360.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000420.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000480.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000540.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000600.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000660.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000720.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000780.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000840.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000900.txt
--rw-r--r--   0        0        0     1173 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_properties_001.txt
--rw-r--r--   0        0        0     1173 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_properties_002.txt
--rw-r--r--   0        0        0  1129110 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/grid_coordinates.txt
--rw-r--r--   0        0        0    63326 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa.dat
--rw-r--r--   0        0        0    36930 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono1.dat
--rw-r--r--   0        0        0      330 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono10.dat
--rw-r--r--   0        0        0      390 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono11.dat
--rw-r--r--   0        0        0      360 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono12.dat
--rw-r--r--   0        0        0      390 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono13.dat
--rw-r--r--   0        0        0      360 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono14.dat
--rw-r--r--   0        0        0      270 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono15.dat
--rw-r--r--   0        0        0      210 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono16.dat
--rw-r--r--   0        0        0      240 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono17.dat
--rw-r--r--   0        0        0      300 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono18.dat
--rw-r--r--   0        0        0      240 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono19.dat
--rw-r--r--   0        0        0    12810 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono2.dat
--rw-r--r--   0        0        0      270 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono20.dat
--rw-r--r--   0        0        0      270 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono21.dat
--rw-r--r--   0        0        0      180 2023-05-08 11:03:41.484391 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono22.dat
--rw-r--r--   0        0        0      210 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono23.dat
--rw-r--r--   0        0        0      300 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono24.dat
--rw-r--r--   0        0        0      210 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono25.dat
--rw-r--r--   0        0        0      270 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono26.dat
--rw-r--r--   0        0        0      240 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono27.dat
--rw-r--r--   0        0        0      240 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono28.dat
--rw-r--r--   0        0        0      330 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono29.dat
--rw-r--r--   0        0        0     1590 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono3.dat
--rw-r--r--   0        0        0      240 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono30.dat
--rw-r--r--   0        0        0      270 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono31.dat
--rw-r--r--   0        0        0      210 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono32.dat
--rw-r--r--   0        0        0      210 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono33.dat
--rw-r--r--   0        0        0      210 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono34.dat
--rw-r--r--   0        0        0      120 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono35.dat
--rw-r--r--   0        0        0      120 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono36.dat
--rw-r--r--   0        0        0     1170 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono4.dat
--rw-r--r--   0        0        0      510 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono5.dat
--rw-r--r--   0        0        0      900 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono6.dat
--rw-r--r--   0        0        0     1020 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono7.dat
--rw-r--r--   0        0        0      510 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono8.dat
--rw-r--r--   0        0        0      600 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono9.dat
--rw-r--r--   0        0        0     8517 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_000h.txt
--rw-r--r--   0        0        0     8502 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_001h.txt
--rw-r--r--   0        0        0     8482 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_002h.txt
--rw-r--r--   0        0        0     8466 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_003h.txt
--rw-r--r--   0        0        0     8455 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_004h.txt
--rw-r--r--   0        0        0     8446 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_005h.txt
--rw-r--r--   0        0        0     8439 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_006h.txt
--rw-r--r--   0        0        0     8430 2023-05-08 11:03:41.494392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_007h.txt
--rw-r--r--   0        0        0     8444 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_008h.txt
--rw-r--r--   0        0        0     8461 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_009h.txt
--rw-r--r--   0        0        0     8467 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_010h.txt
--rw-r--r--   0        0        0     8475 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_011h.txt
--rw-r--r--   0        0        0     8493 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_012h.txt
--rw-r--r--   0        0        0     8498 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_013h.txt
--rw-r--r--   0        0        0     8507 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_014h.txt
--rw-r--r--   0        0        0     8506 2023-05-08 11:59:05.257117 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_015h.txt
--rw-r--r--   0        0        0  1270777 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/grid.dat
--rw-r--r--   0        0        0      288 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/lstcurr_UVW.pre
--rw-r--r--   0        0        0        6 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/lstwaves.pre
--rw-r--r--   0        0        0      195 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/lstwinds.pre
--rw-r--r--   0        0        0     3967 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_000h.txt
--rw-r--r--   0        0        0     3968 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_001h.txt
--rw-r--r--   0        0        0     3965 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_002h.txt
--rw-r--r--   0        0        0     3959 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_003h.txt
--rw-r--r--   0        0        0     3957 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_004h.txt
--rw-r--r--   0        0        0     3951 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_005h.txt
--rw-r--r--   0        0        0     3947 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_006h.txt
--rw-r--r--   0        0        0     3968 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_007h.txt
--rw-r--r--   0        0        0     3958 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_008h.txt
--rw-r--r--   0        0        0     3946 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_009h.txt
--rw-r--r--   0        0        0     3937 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_010h.txt
--rw-r--r--   0        0        0     3941 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_011h.txt
--rw-r--r--   0        0        0     3943 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_012h.txt
--rw-r--r--   0        0        0    58941 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/grids_001.nc
--rw-r--r--   0        0        0    21981 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/grids_002.nc
--rw-r--r--   0        0        0   527627 2023-05-08 11:03:41.504392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/particles_001.csv
--rw-r--r--   0        0        0   792030 2023-05-10 16:13:08.419088 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/particles_001.geojson
--rw-r--r--   0        0        0   447138 2023-05-08 11:03:41.514392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/particles_002.csv
--rw-r--r--   0        0        0   739116 2023-05-10 16:13:08.439088 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/particles_002.geojson
--rw-r--r--   0        0        0      548 2023-05-08 11:03:41.514392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/properties_001.csv
--rw-r--r--   0        0        0     1487 2023-05-10 16:13:08.429088 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/properties_001.json
--rw-r--r--   0        0        0      554 2023-05-08 11:03:41.514392 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/properties_002.csv
--rw-r--r--   0        0        0     1503 2023-05-10 16:13:08.419088 pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/properties_002.json
--rw-r--r--   0        0        0  3177300 2015-03-24 16:18:44.000000 pyteseo-0.0.6/pyteseo/tests/data/grid.dat
--rw-r--r--   0        0        0  1969957 2022-11-28 12:30:41.129982 pyteseo-0.0.6/pyteseo/tests/data/grid_coordinates.txt
--rw-r--r--   0        0        0  3177492 2023-01-09 16:48:14.190649 pyteseo-0.0.6/pyteseo/tests/data/grid_error_var.dat
--rw-r--r--   0        0        0     6725 2023-05-08 11:25:26.958241 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1.cfg
--rw-r--r--   0        0        0     1539 2023-05-08 11:25:26.958241 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1.run
--rw-r--r--   0        0        0      456 2023-05-08 11:25:27.208257 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_grid_001_000060.txt
--rw-r--r--   0        0        0      760 2023-05-08 11:25:27.768293 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_grid_001_000120.txt
--rw-r--r--   0        0        0      608 2023-05-08 11:25:28.078313 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_grid_001_000180.txt
--rw-r--r--   0        0        0      456 2023-05-08 11:25:28.188320 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_grid_001_000240.txt
--rw-r--r--   0        0        0      304 2023-05-08 11:25:27.208257 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_grid_002_000060.txt
--rw-r--r--   0        0        0      760 2023-05-08 11:25:27.768293 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_grid_002_000120.txt
--rw-r--r--   0        0        0       99 2023-05-08 11:25:27.018245 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000000.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:25:27.218258 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000060.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:25:27.768293 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000120.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.088313 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000180.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.188320 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000240.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.288326 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000300.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.388333 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000360.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.488339 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000420.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.588345 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000480.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.658350 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000540.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.688352 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000600.txt
--rw-r--r--   0        0        0     5808 2023-05-08 11:25:28.688352 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_properties_001.txt
--rw-r--r--   0        0        0     5808 2023-05-08 11:25:28.688352 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_properties_002.txt
--rw-r--r--   0        0        0   748950 2023-05-08 11:25:27.018245 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/grid_coordinates.txt
--rw-r--r--   0        0        0     3011 2023-05-10 16:13:08.419088 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/cas1_HNS.calib
--rw-r--r--   0        0        0    63326 2023-05-08 10:31:26.468993 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa.dat
--rw-r--r--   0        0        0    36930 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono1.dat
--rw-r--r--   0        0        0      330 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono10.dat
--rw-r--r--   0        0        0      390 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono11.dat
--rw-r--r--   0        0        0      360 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono12.dat
--rw-r--r--   0        0        0      390 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono13.dat
--rw-r--r--   0        0        0      360 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono14.dat
--rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono15.dat
--rw-r--r--   0        0        0      210 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono16.dat
--rw-r--r--   0        0        0      240 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono17.dat
--rw-r--r--   0        0        0      300 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono18.dat
--rw-r--r--   0        0        0      240 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono19.dat
--rw-r--r--   0        0        0    12810 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono2.dat
--rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono20.dat
--rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono21.dat
--rw-r--r--   0        0        0      180 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono22.dat
--rw-r--r--   0        0        0      210 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono23.dat
--rw-r--r--   0        0        0      300 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono24.dat
--rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono25.dat
--rw-r--r--   0        0        0      270 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono26.dat
--rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono27.dat
--rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono28.dat
--rw-r--r--   0        0        0      330 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono29.dat
--rw-r--r--   0        0        0     1590 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono3.dat
--rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono30.dat
--rw-r--r--   0        0        0      270 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono31.dat
--rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono32.dat
--rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono33.dat
--rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono34.dat
--rw-r--r--   0        0        0      120 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono35.dat
--rw-r--r--   0        0        0      120 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono36.dat
--rw-r--r--   0        0        0     1170 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono4.dat
--rw-r--r--   0        0        0      510 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono5.dat
--rw-r--r--   0        0        0      900 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono6.dat
--rw-r--r--   0        0        0     1020 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono7.dat
--rw-r--r--   0        0        0      510 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono8.dat
--rw-r--r--   0        0        0      600 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono9.dat
--rw-r--r--   0        0        0     5829 2023-05-08 11:25:13.507384 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_000h.txt
--rw-r--r--   0        0        0     5820 2023-05-08 11:25:13.507384 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_001h.txt
--rw-r--r--   0        0        0     5805 2023-05-08 11:25:13.517384 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_002h.txt
--rw-r--r--   0        0        0     5793 2023-05-08 11:25:13.517384 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_003h.txt
--rw-r--r--   0        0        0     5785 2023-05-08 11:25:13.517384 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_004h.txt
--rw-r--r--   0        0        0     5777 2023-05-08 11:25:13.527385 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_005h.txt
--rw-r--r--   0        0        0     5773 2023-05-08 11:25:13.527385 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_006h.txt
--rw-r--r--   0        0        0     5764 2023-05-08 11:25:13.527385 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_007h.txt
--rw-r--r--   0        0        0     5771 2023-05-08 11:25:13.527385 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_008h.txt
--rw-r--r--   0        0        0     5780 2023-05-08 11:25:13.527385 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_009h.txt
--rw-r--r--   0        0        0     5787 2023-05-08 11:25:13.537386 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_010h.txt
--rw-r--r--   0        0        0   840169 2023-05-08 10:31:25.578990 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/grid.dat
--rw-r--r--   0        0        0      198 2023-05-08 11:25:13.527385 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/lstcurr_UVW.pre
--rw-r--r--   0        0        0        6 2023-05-08 11:25:26.928239 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/lstwaves.pre
--rw-r--r--   0        0        0      165 2023-05-08 11:25:26.878236 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/lstwinds.pre
--rw-r--r--   0        0        0     3967 2023-05-08 11:25:26.848234 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_000h.txt
--rw-r--r--   0        0        0     3968 2023-05-08 11:25:26.858235 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_001h.txt
--rw-r--r--   0        0        0     3965 2023-05-08 11:25:26.858235 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_002h.txt
--rw-r--r--   0        0        0     3959 2023-05-08 11:25:26.858235 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_003h.txt
--rw-r--r--   0        0        0     3957 2023-05-08 11:25:26.868235 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_004h.txt
--rw-r--r--   0        0        0     3951 2023-05-08 11:25:26.868235 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_005h.txt
--rw-r--r--   0        0        0     3947 2023-05-08 11:25:26.868235 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_006h.txt
--rw-r--r--   0        0        0     3968 2023-05-08 11:25:26.868235 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_007h.txt
--rw-r--r--   0        0        0     3958 2023-05-08 11:25:26.878236 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_008h.txt
--rw-r--r--   0        0        0     3946 2023-05-08 11:25:26.878236 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_009h.txt
--rw-r--r--   0        0        0     3937 2023-05-08 11:25:26.878236 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_010h.txt
--rw-r--r--   0        0        0    35005 2023-05-08 11:25:29.558407 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/grids_001.nc
--rw-r--r--   0        0        0    24093 2023-05-08 11:25:29.568408 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/grids_002.nc
--rw-r--r--   0        0        0   348805 2023-05-08 11:25:29.208385 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/particles_001.csv
--rw-r--r--   0        0        0   527846 2023-05-10 16:13:08.429088 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/particles_001.geojson
--rw-r--r--   0        0        0   302691 2023-05-08 11:25:29.218386 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/particles_002.csv
--rw-r--r--   0        0        0   497813 2023-05-10 16:13:08.429088 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/particles_002.geojson
--rw-r--r--   0        0        0     2188 2023-05-08 11:25:29.238387 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/properties_001.csv
--rw-r--r--   0        0        0     7169 2023-05-10 16:13:08.429088 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/properties_001.json
--rw-r--r--   0        0        0     2251 2023-05-08 11:25:29.238387 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/properties_002.csv
--rw-r--r--   0        0        0     7242 2023-05-10 16:13:08.429088 pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/properties_002.json
--rw-r--r--   0        0        0    63326 2023-05-08 10:31:26.468993 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa.dat
--rw-r--r--   0        0        0    36930 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono1.dat
--rw-r--r--   0        0        0      330 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono10.dat
--rw-r--r--   0        0        0      390 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono11.dat
--rw-r--r--   0        0        0      360 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono12.dat
--rw-r--r--   0        0        0      390 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono13.dat
--rw-r--r--   0        0        0      360 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono14.dat
--rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono15.dat
--rw-r--r--   0        0        0      210 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono16.dat
--rw-r--r--   0        0        0      240 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono17.dat
--rw-r--r--   0        0        0      300 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono18.dat
--rw-r--r--   0        0        0      240 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono19.dat
--rw-r--r--   0        0        0    12810 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono2.dat
--rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono20.dat
--rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono21.dat
--rw-r--r--   0        0        0      180 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono22.dat
--rw-r--r--   0        0        0      210 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono23.dat
--rw-r--r--   0        0        0      300 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono24.dat
--rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono25.dat
--rw-r--r--   0        0        0      270 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono26.dat
--rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono27.dat
--rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono28.dat
--rw-r--r--   0        0        0      330 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono29.dat
--rw-r--r--   0        0        0     1590 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono3.dat
--rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono30.dat
--rw-r--r--   0        0        0      270 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono31.dat
--rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono32.dat
--rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono33.dat
--rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono34.dat
--rw-r--r--   0        0        0      120 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono35.dat
--rw-r--r--   0        0        0      120 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono36.dat
--rw-r--r--   0        0        0     1170 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono4.dat
--rw-r--r--   0        0        0      510 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono5.dat
--rw-r--r--   0        0        0      900 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono6.dat
--rw-r--r--   0        0        0     1020 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono7.dat
--rw-r--r--   0        0        0      510 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono8.dat
--rw-r--r--   0        0        0      600 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono9.dat
--rw-r--r--   0        0        0   840169 2023-05-08 10:31:25.578990 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/grid.dat
--rw-r--r--   0        0        0   777758 2023-05-08 10:31:27.838997 pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/ibiza_domain.png
--rw-r--r--   0        0        0       72 2023-01-09 16:55:02.280651 pyteseo-0.0.6/pyteseo/tests/data/lstcurr.pre
--rw-r--r--   0        0        0       36 2023-01-27 13:50:37.678084 pyteseo-0.0.6/pyteseo/tests/data/lstcurr_UVW_cte.pre
--rw-r--r--   0        0        0       45 2023-05-17 11:10:20.837289 pyteseo-0.0.6/pyteseo/tests/data/lstcurr_depthavg.pre
--rw-r--r--   0        0        0       60 2023-01-30 12:26:16.443318 pyteseo-0.0.6/pyteseo/tests/data/lstwaves.pre
--rw-r--r--   0        0        0       32 2023-01-31 09:57:32.253738 pyteseo-0.0.6/pyteseo/tests/data/lstwaves_cte.pre
--rw-r--r--   0        0        0       60 2023-01-13 08:20:28.125803 pyteseo-0.0.6/pyteseo/tests/data/lstwinds.pre
--rw-r--r--   0        0        0       36 2023-01-31 09:57:32.253738 pyteseo-0.0.6/pyteseo/tests/data/lstwinds_cte.pre
--rw-r--r--   0        0        0     6701 2023-05-08 11:24:40.005250 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1.cfg
--rw-r--r--   0        0        0     1539 2023-05-08 11:24:40.005250 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1.run
--rw-r--r--   0        0        0      357 2023-05-08 11:24:40.275267 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_grid_001_000060.txt
--rw-r--r--   0        0        0      595 2023-05-08 11:24:40.825302 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_grid_001_000120.txt
--rw-r--r--   0        0        0      595 2023-05-08 11:24:41.105320 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_grid_001_000180.txt
--rw-r--r--   0        0        0      357 2023-05-08 11:24:41.205326 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_grid_001_000240.txt
--rw-r--r--   0        0        0      357 2023-05-08 11:24:40.275267 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_grid_002_000060.txt
--rw-r--r--   0        0        0      476 2023-05-08 11:24:40.825302 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_grid_002_000120.txt
--rw-r--r--   0        0        0       99 2023-05-08 11:24:40.065253 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000000.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:24:40.275267 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000060.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:24:40.825302 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000120.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.105320 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000180.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.205326 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000240.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.305333 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000300.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.405339 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000360.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.515346 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000420.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.615352 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000480.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.685357 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000540.txt
--rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.715359 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000600.txt
--rw-r--r--   0        0        0     5004 2023-05-08 11:24:41.715359 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_properties_001.txt
--rw-r--r--   0        0        0     5004 2023-05-08 11:24:41.715359 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_properties_002.txt
--rw-r--r--   0        0        0   748950 2023-05-08 11:24:40.065253 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/grid_coordinates.txt
--rw-r--r--   0        0        0    63326 2023-05-08 10:31:26.468993 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa.dat
--rw-r--r--   0        0        0    36930 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono1.dat
--rw-r--r--   0        0        0      330 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono10.dat
--rw-r--r--   0        0        0      390 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono11.dat
--rw-r--r--   0        0        0      360 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono12.dat
--rw-r--r--   0        0        0      390 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono13.dat
--rw-r--r--   0        0        0      360 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono14.dat
--rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono15.dat
--rw-r--r--   0        0        0      210 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono16.dat
--rw-r--r--   0        0        0      240 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono17.dat
--rw-r--r--   0        0        0      300 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono18.dat
--rw-r--r--   0        0        0      240 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono19.dat
--rw-r--r--   0        0        0    12810 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono2.dat
--rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono20.dat
--rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono21.dat
--rw-r--r--   0        0        0      180 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono22.dat
--rw-r--r--   0        0        0      210 2023-05-08 10:31:26.448992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono23.dat
--rw-r--r--   0        0        0      300 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono24.dat
--rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono25.dat
--rw-r--r--   0        0        0      270 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono26.dat
--rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono27.dat
--rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono28.dat
--rw-r--r--   0        0        0      330 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono29.dat
--rw-r--r--   0        0        0     1590 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono3.dat
--rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono30.dat
--rw-r--r--   0        0        0      270 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono31.dat
--rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono32.dat
--rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono33.dat
--rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono34.dat
--rw-r--r--   0        0        0      120 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono35.dat
--rw-r--r--   0        0        0      120 2023-05-08 10:31:26.458992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono36.dat
--rw-r--r--   0        0        0     1170 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono4.dat
--rw-r--r--   0        0        0      510 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono5.dat
--rw-r--r--   0        0        0      900 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono6.dat
--rw-r--r--   0        0        0     1020 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono7.dat
--rw-r--r--   0        0        0      510 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono8.dat
--rw-r--r--   0        0        0      600 2023-05-08 10:31:26.438992 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono9.dat
--rw-r--r--   0        0        0     5829 2023-05-08 11:23:49.021999 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_000h.txt
--rw-r--r--   0        0        0     5820 2023-05-08 11:23:49.031999 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_001h.txt
--rw-r--r--   0        0        0     5805 2023-05-08 11:23:49.031999 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_002h.txt
--rw-r--r--   0        0        0     5793 2023-05-08 11:23:49.042000 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_003h.txt
--rw-r--r--   0        0        0     5785 2023-05-08 11:23:49.042000 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_004h.txt
--rw-r--r--   0        0        0     5777 2023-05-08 11:23:49.042000 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_005h.txt
--rw-r--r--   0        0        0     5773 2023-05-08 11:23:49.042000 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_006h.txt
--rw-r--r--   0        0        0     5764 2023-05-08 11:23:49.042000 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_007h.txt
--rw-r--r--   0        0        0     5771 2023-05-08 11:23:49.052000 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_008h.txt
--rw-r--r--   0        0        0     5780 2023-05-08 11:23:49.052000 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_009h.txt
--rw-r--r--   0        0        0     5787 2023-05-08 11:23:49.052000 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_010h.txt
--rw-r--r--   0        0        0   840169 2023-05-08 10:31:25.578990 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/grid.dat
--rw-r--r--   0        0        0      198 2023-05-08 11:23:49.052000 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/lstcurr_UVW.pre
--rw-r--r--   0        0        0        6 2023-05-08 11:24:39.975248 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/lstwaves.pre
--rw-r--r--   0        0        0      165 2023-05-08 11:24:39.925244 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/lstwinds.pre
--rw-r--r--   0        0        0     3967 2023-05-08 11:24:39.895243 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_000h.txt
--rw-r--r--   0        0        0     3968 2023-05-08 11:24:39.905243 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_001h.txt
--rw-r--r--   0        0        0     3965 2023-05-08 11:24:39.905243 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_002h.txt
--rw-r--r--   0        0        0     3959 2023-05-08 11:24:39.905243 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_003h.txt
--rw-r--r--   0        0        0     3957 2023-05-08 11:24:39.915244 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_004h.txt
--rw-r--r--   0        0        0     3951 2023-05-08 11:24:39.915244 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_005h.txt
--rw-r--r--   0        0        0     3947 2023-05-08 11:24:39.915244 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_006h.txt
--rw-r--r--   0        0        0     3968 2023-05-08 11:24:39.915244 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_007h.txt
--rw-r--r--   0        0        0     3958 2023-05-08 11:24:39.915244 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_008h.txt
--rw-r--r--   0        0        0     3946 2023-05-08 11:24:39.925244 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_009h.txt
--rw-r--r--   0        0        0     3937 2023-05-08 11:24:39.925244 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_010h.txt
--rw-r--r--   0        0        0    31485 2023-05-08 11:24:42.585414 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/grids_001.nc
--rw-r--r--   0        0        0    23229 2023-05-08 11:24:42.595415 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/grids_002.nc
--rw-r--r--   0        0        0   348848 2023-05-08 11:24:42.235392 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/particles_001.csv
--rw-r--r--   0        0        0   527956 2023-05-10 16:13:08.419088 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/particles_001.geojson
--rw-r--r--   0        0        0   302657 2023-05-08 11:24:42.245392 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/particles_002.csv
--rw-r--r--   0        0        0   497752 2023-05-10 16:13:08.439088 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/particles_002.geojson
--rw-r--r--   0        0        0     1853 2023-05-08 11:24:42.265394 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/properties_001.csv
--rw-r--r--   0        0        0     6125 2023-05-10 16:13:08.429088 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/properties_001.json
--rw-r--r--   0        0        0     1858 2023-05-08 11:24:42.265394 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/properties_002.csv
--rw-r--r--   0        0        0     6139 2023-05-10 16:13:08.419088 pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/properties_002.json
--rw-r--r--   0        0        0        6 2023-05-10 16:13:08.419088 pyteseo-0.0.6/pyteseo/tests/data/shapefile_cantabria/Cantabria.cpg
--rw-r--r--   0        0        0      382 2023-05-09 14:10:49.121228 pyteseo-0.0.6/pyteseo/tests/data/shapefile_cantabria/Cantabria.dbf
--rw-r--r--   0        0        0      413 2023-05-10 16:13:08.429088 pyteseo-0.0.6/pyteseo/tests/data/shapefile_cantabria/Cantabria.prj
--rw-r--r--   0        0        0      132 2023-05-09 14:10:49.121228 pyteseo-0.0.6/pyteseo/tests/data/shapefile_cantabria/Cantabria.sbn
--rw-r--r--   0        0        0      116 2023-05-09 14:10:49.131229 pyteseo-0.0.6/pyteseo/tests/data/shapefile_cantabria/Cantabria.sbx
--rw-r--r--   0        0        0   259168 2023-05-09 14:10:49.131229 pyteseo-0.0.6/pyteseo/tests/data/shapefile_cantabria/Cantabria.shp
--rw-r--r--   0        0        0    10465 2023-05-09 14:10:49.151231 pyteseo-0.0.6/pyteseo/tests/data/shapefile_cantabria/Cantabria.shp.xml
--rw-r--r--   0        0        0      108 2023-05-09 14:10:49.151231 pyteseo-0.0.6/pyteseo/tests/data/shapefile_cantabria/Cantabria.shx
--rw-r--r--   0        0        0      456 2023-01-30 12:28:00.313319 pyteseo-0.0.6/pyteseo/tests/data/waves_000h.txt
--rw-r--r--   0        0        0      480 2023-01-30 12:28:28.243319 pyteseo-0.0.6/pyteseo/tests/data/waves_001h.txt
--rw-r--r--   0        0        0      480 2023-01-30 12:28:40.053319 pyteseo-0.0.6/pyteseo/tests/data/waves_002h.txt
--rw-r--r--   0        0        0      516 2023-01-31 09:57:32.263738 pyteseo-0.0.6/pyteseo/tests/data/waves_003h.txt
--rw-r--r--   0        0        0    25121 2023-05-16 06:59:43.223472 pyteseo-0.0.6/pyteseo/tests/data/winds.nc
--rw-r--r--   0        0        0      732 2022-11-14 07:58:35.871414 pyteseo-0.0.6/pyteseo/tests/data/winds_000h.txt
--rw-r--r--   0        0        0      732 2022-11-14 07:58:35.950414 pyteseo-0.0.6/pyteseo/tests/data/winds_001h.txt
--rw-r--r--   0        0        0      732 2022-11-14 07:58:36.019414 pyteseo-0.0.6/pyteseo/tests/data/winds_002h.txt
--rw-r--r--   0        0        0      732 2022-11-14 07:58:36.125414 pyteseo-0.0.6/pyteseo/tests/data/winds_003h.txt
--rw-r--r--   0        0        0        0 2023-02-10 07:53:13.427520 pyteseo-0.0.6/pyteseo/tests/integration/__init__.py
--rw-r--r--   0        0        0     1585 2023-05-22 06:19:42.815869 pyteseo-0.0.6/pyteseo/tests/integration/test_cmems.py
--rw-r--r--   0        0        0     1025 2023-05-23 11:05:59.240771 pyteseo-0.0.6/pyteseo/tests/integration/test_create_domain.py
--rw-r--r--   0        0        0      974 2023-05-22 06:39:28.861207 pyteseo-0.0.6/pyteseo/tests/integration/test_noaa_gfs.py
--rw-r--r--   0        0        0     9785 2023-05-18 10:41:21.720535 pyteseo-0.0.6/pyteseo/tests/integration/test_simulation_cmems.py
--rw-r--r--   0        0        0     9609 2023-05-18 10:41:21.720535 pyteseo-0.0.6/pyteseo/tests/integration/test_simulation_cte_forcing.py
--rw-r--r--   0        0        0        0 2023-02-10 07:53:13.427520 pyteseo-0.0.6/pyteseo/tests/unit/__init__.py
--rw-r--r--   0        0        0     4635 2023-05-18 10:41:21.720535 pyteseo-0.0.6/pyteseo/tests/unit/test_cfg.py
--rw-r--r--   0        0        0     6183 2023-05-22 08:08:53.659923 pyteseo-0.0.6/pyteseo/tests/unit/test_clasess.py
--rw-r--r--   0        0        0     2879 2023-05-10 16:02:05.526185 pyteseo-0.0.6/pyteseo/tests/unit/test_export.py
--rw-r--r--   0        0        0     3286 2023-05-10 13:10:41.515296 pyteseo-0.0.6/pyteseo/tests/unit/test_io_coastline.py
--rw-r--r--   0        0        0     3589 2023-05-17 14:25:17.630330 pyteseo-0.0.6/pyteseo/tests/unit/test_io_forcings.py
--rw-r--r--   0        0        0     2552 2023-05-10 15:10:22.789296 pyteseo-0.0.6/pyteseo/tests/unit/test_io_grid.py
--rw-r--r--   0        0        0     1685 2023-05-10 16:00:06.143520 pyteseo-0.0.6/pyteseo/tests/unit/test_io_results.py
--rw-r--r--   0        0        0     1892 2023-05-23 08:06:52.405460 pyteseo-0.0.6/pyteseo/tests/unit/test_plot.py
--rw-r--r--   0        0        0      898 2023-05-22 13:51:54.858831 pyteseo-0.0.6/pyteseo/tests/unit/test_services.py
--rw-r--r--   0        0        0      946 2023-05-22 06:31:48.943904 pyteseo-0.0.6/pyteseo/tests/unit/test_substances.py
--rw-r--r--   0        0        0    14063 2023-05-22 08:25:22.029789 pyteseo-0.0.6/pyteseo/wrapper.py
--rw-r--r--   0        0        0     6073 1970-01-01 00:00:00.000000 pyteseo-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    53248 2023-07-06 08:17:28.147669 pyteseo-0.0.7/.coverage
+-rw-r--r--   0        0        0      169 2023-01-23 16:09:52.078560 pyteseo-0.0.7/.flake8
+-rw-r--r--   0        0        0     1545 2023-04-17 10:00:47.217406 pyteseo-0.0.7/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     1169 2023-07-05 12:00:27.132559 pyteseo-0.0.7/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      191 2023-06-16 08:24:03.629452 pyteseo-0.0.7/.gitignore
+-rw-r--r--   0        0        0      504 2023-01-16 10:53:29.863142 pyteseo-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3135 2023-07-06 10:10:28.906086 pyteseo-0.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-05-22 06:33:42.865296 pyteseo-0.0.7/LICENSE.md
+-rw-r--r--   0        0        0     4648 2023-07-06 10:06:38.704692 pyteseo-0.0.7/README.md
+-rw-r--r--   0        0        0      634 2022-12-28 11:40:36.607121 pyteseo-0.0.7/docs/Makefile
+-rw-r--r--   0        0        0    31102 2022-12-28 11:40:36.627121 pyteseo-0.0.7/docs/_static/TESEO_logo.png
+-rw-r--r--   0        0        0    84936 2023-01-09 07:22:45.451292 pyteseo-0.0.7/docs/_static/doc_snapshoot.png
+-rw-r--r--   0        0        0   197843 2023-07-05 10:51:08.542704 pyteseo-0.0.7/docs/_static/forcings.gif
+-rw-r--r--   0        0        0    33271 2023-07-05 09:33:02.115889 pyteseo-0.0.7/docs/_static/ibiza_extents.png
+-rw-r--r--   0        0        0   405456 2023-07-05 10:45:17.774652 pyteseo-0.0.7/docs/_static/particles_spill_01.gif
+-rw-r--r--   0        0        0    28715 2022-12-28 11:40:36.627121 pyteseo-0.0.7/docs/_static/pyTESEO_logo.png
+-rw-r--r--   0        0        0       55 2023-01-13 08:20:28.115803 pyteseo-0.0.7/docs/changelog.md
+-rw-r--r--   0        0        0     1822 2023-01-20 10:27:58.065661 pyteseo-0.0.7/docs/conf.py
+-rw-r--r--   0        0        0     2326 2023-07-05 11:33:23.468616 pyteseo-0.0.7/docs/get-started.md
+-rw-r--r--   0        0        0     2212 2023-07-04 09:44:42.457716 pyteseo-0.0.7/docs/index.md
+-rw-r--r--   0        0        0      800 2022-12-28 11:40:36.627121 pyteseo-0.0.7/docs/make.bat
+-rw-r--r--   0        0        0   263466 2023-05-15 10:11:00.364302 pyteseo-0.0.7/docs/notebooks/01_read_domain.ipynb
+-rw-r--r--   0        0        0    42212 2023-05-11 13:51:39.835822 pyteseo-0.0.7/docs/notebooks/02_read_forcings.ipynb
+-rw-r--r--   0        0        0   947681 2023-05-11 13:51:51.776549 pyteseo-0.0.7/docs/notebooks/03_export_results.ipynb
+-rw-r--r--   0        0        0    17456 2023-05-11 13:52:48.710040 pyteseo-0.0.7/docs/notebooks/04_generate_forcings_from_cmems.ipynb
+-rw-r--r--   0        0        0   116565 2023-07-03 06:27:37.389896 pyteseo-0.0.7/docs/notebooks/05_drift_simulation.ipynb
+-rw-r--r--   0        0        0      711 2023-01-19 16:35:42.758020 pyteseo-0.0.7/docs/notebooks/06_hns_simulation.ipynb
+-rw-r--r--   0        0        0      686 2023-05-11 13:54:12.425183 pyteseo-0.0.7/docs/notebooks/07_stochastic_montecarlo.ipynb
+-rw-r--r--   0        0        0      753 2023-01-19 16:35:42.758020 pyteseo-0.0.7/docs/notebooks/08_stochastic_kmeans.ipynb
+-rw-r--r--   0        0        0    12683 2023-07-05 11:09:45.427838 pyteseo-0.0.7/docs/tl;dr-guide.md
+-rw-r--r--   0        0        0      497 2023-07-06 08:02:41.702310 pyteseo-0.0.7/environment-dev.yml
+-rw-r--r--   0        0        0      235 2023-06-07 07:48:44.020571 pyteseo-0.0.7/environment.yml
+-rw-r--r--   0        0        0     2018 2023-07-06 10:15:46.221516 pyteseo-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      476 2023-07-06 10:16:31.233682 pyteseo-0.0.7/pyteseo/__init__.py
+-rw-r--r--   0        0        0     7828 2023-07-04 09:23:36.113285 pyteseo-0.0.7/pyteseo/classes.py
+-rw-r--r--   0        0        0    13416 2023-05-18 06:18:08.958963 pyteseo-0.0.7/pyteseo/data/substances/hns.xlsx
+-rw-r--r--   0        0        0     5208 2023-05-18 06:16:20.039757 pyteseo-0.0.7/pyteseo/data/substances/hns_units.xlsx
+-rw-r--r--   0        0        0     5849 2023-05-18 06:16:00.696375 pyteseo-0.0.7/pyteseo/data/substances/oil.xlsx
+-rw-r--r--   0        0        0     5079 2023-05-18 06:16:00.696375 pyteseo-0.0.7/pyteseo/data/substances/oil_units.xlsx
+-rw-r--r--   0        0        0     7285 2023-07-05 06:29:59.365372 pyteseo-0.0.7/pyteseo/defaults.py
+-rw-r--r--   0        0        0      109 2023-07-04 08:27:51.116212 pyteseo-0.0.7/pyteseo/export/__init__.py
+-rw-r--r--   0        0        0     4918 2023-07-05 08:21:19.363467 pyteseo-0.0.7/pyteseo/export/grids.py
+-rw-r--r--   0        0        0     3236 2023-04-14 11:07:51.005172 pyteseo-0.0.7/pyteseo/export/particles.py
+-rw-r--r--   0        0        0     1627 2023-02-10 07:53:13.427520 pyteseo-0.0.7/pyteseo/export/properties.py
+-rw-r--r--   0        0        0       58 2023-07-04 08:27:46.636119 pyteseo-0.0.7/pyteseo/io/__init__.py
+-rw-r--r--   0        0        0    16924 2023-07-03 10:49:18.724686 pyteseo-0.0.7/pyteseo/io/cfg.py
+-rw-r--r--   0        0        0     4553 2023-06-26 13:55:13.706097 pyteseo-0.0.7/pyteseo/io/coastline.py
+-rw-r--r--   0        0        0     6698 2023-05-22 06:57:42.067158 pyteseo-0.0.7/pyteseo/io/forcings.py
+-rw-r--r--   0        0        0     2608 2023-06-26 10:24:53.504429 pyteseo-0.0.7/pyteseo/io/grid.py
+-rw-r--r--   0        0        0     3448 2023-04-17 07:20:52.886042 pyteseo-0.0.7/pyteseo/io/hns_calib.py
+-rw-r--r--   0        0        0     6603 2023-07-05 08:03:38.535336 pyteseo-0.0.7/pyteseo/io/results.py
+-rw-r--r--   0        0        0     4794 2023-07-03 06:27:38.289913 pyteseo-0.0.7/pyteseo/io/run.py
+-rw-r--r--   0        0        0     2497 2023-07-03 10:31:37.017809 pyteseo-0.0.7/pyteseo/io/substances.py
+-rw-r--r--   0        0        0     1915 2023-05-10 15:18:33.918998 pyteseo-0.0.7/pyteseo/io/utils.py
+-rw-r--r--   0        0        0       76 2023-07-04 08:28:58.237591 pyteseo-0.0.7/pyteseo/plot/__init__.py
+-rw-r--r--   0        0        0     6817 2023-07-05 10:54:07.036798 pyteseo-0.0.7/pyteseo/plot/animations.py
+-rw-r--r--   0        0        0     4883 2023-05-18 15:14:13.389991 pyteseo-0.0.7/pyteseo/plot/basics.py
+-rw-r--r--   0        0        0     2226 2023-07-05 09:32:39.685271 pyteseo-0.0.7/pyteseo/plot/figures.py
+-rw-r--r--   0        0        0       94 2023-07-04 08:27:27.175714 pyteseo-0.0.7/pyteseo/preprocess/__init__.py
+-rw-r--r--   0        0        0     6995 2023-06-21 14:34:58.745037 pyteseo-0.0.7/pyteseo/preprocess/dataset.py
+-rw-r--r--   0        0        0     1867 2023-06-26 11:15:46.365813 pyteseo-0.0.7/pyteseo/preprocess/geodataframe.py
+-rw-r--r--   0        0        0     8101 2023-07-03 06:39:12.407114 pyteseo-0.0.7/pyteseo/preprocess/teseo_domain.py
+-rw-r--r--   0        0        0     7437 2023-06-27 14:48:57.973644 pyteseo-0.0.7/pyteseo/preprocess/teseo_forcing.py
+-rw-r--r--   0        0        0     1989 2023-06-21 12:00:22.668216 pyteseo-0.0.7/pyteseo/preprocess/teseo_standarizations.py
+-rw-r--r--   0        0        0     1703 2023-07-04 08:27:20.615578 pyteseo-0.0.7/pyteseo/providers/__init__.py
+-rw-r--r--   0        0        0     1339 2023-07-03 13:01:37.662945 pyteseo-0.0.7/pyteseo/providers/cmems.py
+-rw-r--r--   0        0        0     2764 2023-06-27 14:57:25.051926 pyteseo-0.0.7/pyteseo/providers/connection.py
+-rw-r--r--   0        0        0      156 2023-06-19 13:40:06.599807 pyteseo-0.0.7/pyteseo/providers/emodnet.py
+-rw-r--r--   0        0        0     1997 2023-06-19 13:40:06.599807 pyteseo-0.0.7/pyteseo/providers/ihcantabria.py
+-rw-r--r--   0        0        0      907 2023-06-19 06:13:31.583106 pyteseo-0.0.7/pyteseo/providers/noaa.py
+-rw-r--r--   0        0        0     6510 2023-06-26 11:26:33.810162 pyteseo-0.0.7/pyteseo/providers/providers_registry.json
+-rw-r--r--   0        0        0      309 2023-05-12 06:12:32.629928 pyteseo-0.0.7/pyteseo/tests/__init__.py
+-rw-r--r--   0        0        0     1080 2022-11-28 12:31:04.243939 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000000.txt
+-rw-r--r--   0        0        0     1440 2022-11-28 12:31:25.250905 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000005.txt
+-rw-r--r--   0        0        0     1320 2022-11-28 12:31:42.101870 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000010.txt
+-rw-r--r--   0        0        0     1440 2022-11-28 12:31:56.340847 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000015.txt
+-rw-r--r--   0        0        0     1800 2022-11-28 12:32:08.201821 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000020.txt
+-rw-r--r--   0        0        0     1920 2022-11-28 12:32:19.311799 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000025.txt
+-rw-r--r--   0        0        0     1800 2022-11-28 12:32:30.205778 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000030.txt
+-rw-r--r--   0        0        0     1920 2022-11-28 12:32:40.120760 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000035.txt
+-rw-r--r--   0        0        0     1920 2022-11-28 12:32:49.096757 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000040.txt
+-rw-r--r--   0        0        0     2040 2022-11-28 12:32:56.968763 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000045.txt
+-rw-r--r--   0        0        0     2280 2022-11-28 12:33:04.886785 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000050.txt
+-rw-r--r--   0        0        0     2640 2022-11-28 12:33:12.049766 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000055.txt
+-rw-r--r--   0        0        0     2640 2022-11-28 12:33:19.004754 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000060.txt
+-rw-r--r--   0        0        0     3240 2022-11-28 12:33:49.743762 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000065.txt
+-rw-r--r--   0        0        0     3840 2022-11-28 12:33:56.320750 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000070.txt
+-rw-r--r--   0        0        0     3960 2022-11-28 12:34:03.214770 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000075.txt
+-rw-r--r--   0        0        0     4440 2022-11-28 12:34:09.897757 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000080.txt
+-rw-r--r--   0        0        0     4920 2022-11-28 12:34:17.619757 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000085.txt
+-rw-r--r--   0        0        0     5280 2022-11-28 12:34:25.163765 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000090.txt
+-rw-r--r--   0        0        0     1080 2022-11-28 12:31:04.243939 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000000.txt
+-rw-r--r--   0        0        0     1440 2022-11-28 12:31:25.250905 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000005.txt
+-rw-r--r--   0        0        0     1320 2022-11-28 12:31:42.101870 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000010.txt
+-rw-r--r--   0        0        0     1440 2022-11-28 12:31:56.340847 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000015.txt
+-rw-r--r--   0        0        0     1800 2022-11-28 12:32:08.201821 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000020.txt
+-rw-r--r--   0        0        0     1920 2022-11-28 12:32:19.311799 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000025.txt
+-rw-r--r--   0        0        0     1800 2022-11-28 12:32:30.205778 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000030.txt
+-rw-r--r--   0        0        0     1920 2022-11-28 12:32:40.120760 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000035.txt
+-rw-r--r--   0        0        0     1920 2022-11-28 12:32:49.096757 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000040.txt
+-rw-r--r--   0        0        0     2040 2022-11-28 12:32:56.968763 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000045.txt
+-rw-r--r--   0        0        0     2280 2022-11-28 12:33:04.886785 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000050.txt
+-rw-r--r--   0        0        0     2640 2022-11-28 12:33:12.049766 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000055.txt
+-rw-r--r--   0        0        0     2640 2022-11-28 12:33:19.004754 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000060.txt
+-rw-r--r--   0        0        0     3240 2022-11-28 12:33:49.743762 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000065.txt
+-rw-r--r--   0        0        0     3840 2022-11-28 12:33:56.320750 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000070.txt
+-rw-r--r--   0        0        0     3960 2022-11-28 12:34:03.214770 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000075.txt
+-rw-r--r--   0        0        0     4440 2022-11-28 12:34:09.897757 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000080.txt
+-rw-r--r--   0        0        0     4920 2022-11-28 12:34:17.619757 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000085.txt
+-rw-r--r--   0        0        0     5280 2022-11-28 12:34:25.163765 pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000090.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:31:04.219939 pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000000.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:31:25.362903 pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000005.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:31:42.232868 pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000010.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:31:56.503846 pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000015.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:32:08.296824 pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000020.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:32:19.402804 pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000025.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:32:30.379778 pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000030.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:32:40.259760 pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000035.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:32:49.222751 pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000040.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:32:57.430761 pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000045.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:33:04.996780 pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000050.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:33:12.191766 pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000055.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:33:19.144753 pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000060.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:33:49.896767 pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000065.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:33:56.794749 pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000070.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:34:03.348770 pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000075.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:34:10.956756 pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000080.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:34:18.079761 pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000085.txt
+-rw-r--r--   0        0        0   500100 2022-11-28 12:34:25.335761 pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000090.txt
+-rw-r--r--   0        0        0   121220 2022-11-28 12:59:56.013665 pyteseo-0.0.7/pyteseo/tests/data/cas1_properties_001.txt
+-rw-r--r--   0        0        0   121220 2022-11-28 12:59:56.013665 pyteseo-0.0.7/pyteseo/tests/data/cas1_properties_002.txt
+-rw-r--r--   0        0        0   574769 2023-01-13 08:20:28.115803 pyteseo-0.0.7/pyteseo/tests/data/coastline.dat
+-rw-r--r--   0        0        0   574787 2023-01-13 08:20:28.125803 pyteseo-0.0.7/pyteseo/tests/data/coastline_error_range.dat
+-rw-r--r--   0        0        0   574787 2023-01-13 08:20:28.125803 pyteseo-0.0.7/pyteseo/tests/data/coastline_othernanformat.dat
+-rw-r--r--   0        0        0   558324 2015-03-24 16:18:44.000000 pyteseo-0.0.7/pyteseo/tests/data/costa_poligono1.dat
+-rw-r--r--   0        0        0     3861 2015-03-24 16:18:44.000000 pyteseo-0.0.7/pyteseo/tests/data/costa_poligono2.dat
+-rw-r--r--   0        0        0    10412 2023-01-13 08:20:28.125803 pyteseo-0.0.7/pyteseo/tests/data/costa_poligono3.dat
+-rw-r--r--   0        0        0     2183 2023-01-13 08:20:28.125803 pyteseo-0.0.7/pyteseo/tests/data/costa_poligono4.dat
+-rw-r--r--   0        0        0    33889 2023-05-16 06:59:34.843214 pyteseo-0.0.7/pyteseo/tests/data/currents.nc
+-rw-r--r--   0        0        0      732 2022-11-14 07:58:35.871414 pyteseo-0.0.7/pyteseo/tests/data/currents_000h.txt
+-rw-r--r--   0        0        0      732 2022-11-14 07:58:35.950414 pyteseo-0.0.7/pyteseo/tests/data/currents_001h.txt
+-rw-r--r--   0        0        0      732 2022-11-14 07:58:36.019414 pyteseo-0.0.7/pyteseo/tests/data/currents_002h.txt
+-rw-r--r--   0        0        0      732 2022-11-14 07:58:36.125414 pyteseo-0.0.7/pyteseo/tests/data/currents_003h.txt
+-rw-r--r--   0        0        0     6679 2023-05-08 11:03:41.464391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1.cfg
+-rw-r--r--   0        0        0     1539 2023-05-08 11:03:41.464391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1.run
+-rw-r--r--   0        0        0      616 2023-05-08 11:03:41.464391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_grid_001_000060.txt
+-rw-r--r--   0        0        0      704 2023-05-08 11:03:41.464391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_grid_001_000120.txt
+-rw-r--r--   0        0        0      880 2023-05-08 11:03:41.464391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_grid_001_000180.txt
+-rw-r--r--   0        0        0      880 2023-05-08 11:03:41.464391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_grid_001_000240.txt
+-rw-r--r--   0        0        0      880 2023-05-08 11:03:41.464391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_grid_001_000300.txt
+-rw-r--r--   0        0        0     1232 2023-05-08 11:03:41.464391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_grid_001_000360.txt
+-rw-r--r--   0        0        0      968 2023-05-08 11:03:41.464391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_grid_001_000420.txt
+-rw-r--r--   0        0        0      616 2023-05-08 11:03:41.464391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_grid_001_000480.txt
+-rw-r--r--   0        0        0      176 2023-05-08 11:03:41.464391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_grid_001_000540.txt
+-rw-r--r--   0        0        0      880 2023-05-08 11:03:41.474391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_grid_002_000060.txt
+-rw-r--r--   0        0        0      176 2023-05-08 11:03:41.474391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_grid_002_000120.txt
+-rw-r--r--   0        0        0       99 2023-05-08 11:03:41.474391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000000.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000060.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000120.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000180.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000240.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000300.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000360.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000420.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000480.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000540.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000600.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000660.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000720.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.474391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000780.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000840.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000900.txt
+-rw-r--r--   0        0        0     1173 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_properties_001.txt
+-rw-r--r--   0        0        0     1173 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_properties_002.txt
+-rw-r--r--   0        0        0  1129110 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/grid_coordinates.txt
+-rw-r--r--   0        0        0    63326 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa.dat
+-rw-r--r--   0        0        0    36930 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono1.dat
+-rw-r--r--   0        0        0      330 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono10.dat
+-rw-r--r--   0        0        0      390 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono11.dat
+-rw-r--r--   0        0        0      360 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono12.dat
+-rw-r--r--   0        0        0      390 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono13.dat
+-rw-r--r--   0        0        0      360 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono14.dat
+-rw-r--r--   0        0        0      270 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono15.dat
+-rw-r--r--   0        0        0      210 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono16.dat
+-rw-r--r--   0        0        0      240 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono17.dat
+-rw-r--r--   0        0        0      300 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono18.dat
+-rw-r--r--   0        0        0      240 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono19.dat
+-rw-r--r--   0        0        0    12810 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono2.dat
+-rw-r--r--   0        0        0      270 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono20.dat
+-rw-r--r--   0        0        0      270 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono21.dat
+-rw-r--r--   0        0        0      180 2023-05-08 11:03:41.484391 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono22.dat
+-rw-r--r--   0        0        0      210 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono23.dat
+-rw-r--r--   0        0        0      300 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono24.dat
+-rw-r--r--   0        0        0      210 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono25.dat
+-rw-r--r--   0        0        0      270 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono26.dat
+-rw-r--r--   0        0        0      240 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono27.dat
+-rw-r--r--   0        0        0      240 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono28.dat
+-rw-r--r--   0        0        0      330 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono29.dat
+-rw-r--r--   0        0        0     1590 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono3.dat
+-rw-r--r--   0        0        0      240 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono30.dat
+-rw-r--r--   0        0        0      270 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono31.dat
+-rw-r--r--   0        0        0      210 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono32.dat
+-rw-r--r--   0        0        0      210 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono33.dat
+-rw-r--r--   0        0        0      210 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono34.dat
+-rw-r--r--   0        0        0      120 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono35.dat
+-rw-r--r--   0        0        0      120 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono36.dat
+-rw-r--r--   0        0        0     1170 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono4.dat
+-rw-r--r--   0        0        0      510 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono5.dat
+-rw-r--r--   0        0        0      900 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono6.dat
+-rw-r--r--   0        0        0     1020 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono7.dat
+-rw-r--r--   0        0        0      510 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono8.dat
+-rw-r--r--   0        0        0      600 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono9.dat
+-rw-r--r--   0        0        0     8517 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_000h.txt
+-rw-r--r--   0        0        0     8502 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_001h.txt
+-rw-r--r--   0        0        0     8482 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_002h.txt
+-rw-r--r--   0        0        0     8466 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_003h.txt
+-rw-r--r--   0        0        0     8455 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_004h.txt
+-rw-r--r--   0        0        0     8446 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_005h.txt
+-rw-r--r--   0        0        0     8439 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_006h.txt
+-rw-r--r--   0        0        0     8430 2023-05-08 11:03:41.494392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_007h.txt
+-rw-r--r--   0        0        0     8444 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_008h.txt
+-rw-r--r--   0        0        0     8461 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_009h.txt
+-rw-r--r--   0        0        0     8467 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_010h.txt
+-rw-r--r--   0        0        0     8475 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_011h.txt
+-rw-r--r--   0        0        0     8493 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_012h.txt
+-rw-r--r--   0        0        0     8498 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_013h.txt
+-rw-r--r--   0        0        0     8507 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_014h.txt
+-rw-r--r--   0        0        0     8506 2023-05-08 11:59:05.257117 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_015h.txt
+-rw-r--r--   0        0        0  1270777 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/grid.dat
+-rw-r--r--   0        0        0      288 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/lstcurr_UVW.pre
+-rw-r--r--   0        0        0        6 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/lstwaves.pre
+-rw-r--r--   0        0        0      195 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/lstwinds.pre
+-rw-r--r--   0        0        0     3967 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_000h.txt
+-rw-r--r--   0        0        0     3968 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_001h.txt
+-rw-r--r--   0        0        0     3965 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_002h.txt
+-rw-r--r--   0        0        0     3959 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_003h.txt
+-rw-r--r--   0        0        0     3957 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_004h.txt
+-rw-r--r--   0        0        0     3951 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_005h.txt
+-rw-r--r--   0        0        0     3947 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_006h.txt
+-rw-r--r--   0        0        0     3968 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_007h.txt
+-rw-r--r--   0        0        0     3958 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_008h.txt
+-rw-r--r--   0        0        0     3946 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_009h.txt
+-rw-r--r--   0        0        0     3937 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_010h.txt
+-rw-r--r--   0        0        0     3941 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_011h.txt
+-rw-r--r--   0        0        0     3943 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_012h.txt
+-rw-r--r--   0        0        0    58941 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/output/grids_001.nc
+-rw-r--r--   0        0        0    21981 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/output/grids_002.nc
+-rw-r--r--   0        0        0   527627 2023-05-08 11:03:41.504392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/output/particles_001.csv
+-rw-r--r--   0        0        0   792030 2023-05-10 16:13:08.419088 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/output/particles_001.geojson
+-rw-r--r--   0        0        0   447138 2023-05-08 11:03:41.514392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/output/particles_002.csv
+-rw-r--r--   0        0        0   739116 2023-05-10 16:13:08.439088 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/output/particles_002.geojson
+-rw-r--r--   0        0        0      548 2023-05-08 11:03:41.514392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/output/properties_001.csv
+-rw-r--r--   0        0        0     1487 2023-05-10 16:13:08.429088 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/output/properties_001.json
+-rw-r--r--   0        0        0      554 2023-05-08 11:03:41.514392 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/output/properties_002.csv
+-rw-r--r--   0        0        0     1503 2023-05-10 16:13:08.419088 pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/output/properties_002.json
+-rw-r--r--   0        0        0  3177300 2015-03-24 16:18:44.000000 pyteseo-0.0.7/pyteseo/tests/data/grid.dat
+-rw-r--r--   0        0        0  1969957 2022-11-28 12:30:41.129982 pyteseo-0.0.7/pyteseo/tests/data/grid_coordinates.txt
+-rw-r--r--   0        0        0  3177492 2023-01-09 16:48:14.190649 pyteseo-0.0.7/pyteseo/tests/data/grid_error_var.dat
+-rw-r--r--   0        0        0     6725 2023-05-08 11:25:26.958241 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1.cfg
+-rw-r--r--   0        0        0     1539 2023-05-08 11:25:26.958241 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1.run
+-rw-r--r--   0        0        0      456 2023-05-08 11:25:27.208257 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_grid_001_000060.txt
+-rw-r--r--   0        0        0      760 2023-05-08 11:25:27.768293 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_grid_001_000120.txt
+-rw-r--r--   0        0        0      608 2023-05-08 11:25:28.078313 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_grid_001_000180.txt
+-rw-r--r--   0        0        0      456 2023-05-08 11:25:28.188320 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_grid_001_000240.txt
+-rw-r--r--   0        0        0      304 2023-05-08 11:25:27.208257 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_grid_002_000060.txt
+-rw-r--r--   0        0        0      760 2023-05-08 11:25:27.768293 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_grid_002_000120.txt
+-rw-r--r--   0        0        0       99 2023-05-08 11:25:27.018245 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000000.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:25:27.218258 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000060.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:25:27.768293 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000120.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.088313 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000180.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.188320 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000240.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.288326 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000300.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.388333 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000360.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.488339 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000420.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.588345 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000480.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.658350 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000540.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:25:28.688352 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000600.txt
+-rw-r--r--   0        0        0     5808 2023-05-08 11:25:28.688352 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_properties_001.txt
+-rw-r--r--   0        0        0     5808 2023-05-08 11:25:28.688352 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_properties_002.txt
+-rw-r--r--   0        0        0   748950 2023-05-08 11:25:27.018245 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/grid_coordinates.txt
+-rw-r--r--   0        0        0     3011 2023-05-10 16:13:08.419088 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/cas1_HNS.calib
+-rw-r--r--   0        0        0    63326 2023-05-08 10:31:26.468993 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa.dat
+-rw-r--r--   0        0        0    36930 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono1.dat
+-rw-r--r--   0        0        0      330 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono10.dat
+-rw-r--r--   0        0        0      390 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono11.dat
+-rw-r--r--   0        0        0      360 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono12.dat
+-rw-r--r--   0        0        0      390 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono13.dat
+-rw-r--r--   0        0        0      360 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono14.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono15.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono16.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono17.dat
+-rw-r--r--   0        0        0      300 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono18.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono19.dat
+-rw-r--r--   0        0        0    12810 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono2.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono20.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono21.dat
+-rw-r--r--   0        0        0      180 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono22.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono23.dat
+-rw-r--r--   0        0        0      300 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono24.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono25.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono26.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono27.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono28.dat
+-rw-r--r--   0        0        0      330 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono29.dat
+-rw-r--r--   0        0        0     1590 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono3.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono30.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono31.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono32.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono33.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono34.dat
+-rw-r--r--   0        0        0      120 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono35.dat
+-rw-r--r--   0        0        0      120 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono36.dat
+-rw-r--r--   0        0        0     1170 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono4.dat
+-rw-r--r--   0        0        0      510 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono5.dat
+-rw-r--r--   0        0        0      900 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono6.dat
+-rw-r--r--   0        0        0     1020 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono7.dat
+-rw-r--r--   0        0        0      510 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono8.dat
+-rw-r--r--   0        0        0      600 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono9.dat
+-rw-r--r--   0        0        0     5829 2023-05-08 11:25:13.507384 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_000h.txt
+-rw-r--r--   0        0        0     5820 2023-05-08 11:25:13.507384 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_001h.txt
+-rw-r--r--   0        0        0     5805 2023-05-08 11:25:13.517384 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_002h.txt
+-rw-r--r--   0        0        0     5793 2023-05-08 11:25:13.517384 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_003h.txt
+-rw-r--r--   0        0        0     5785 2023-05-08 11:25:13.517384 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_004h.txt
+-rw-r--r--   0        0        0     5777 2023-05-08 11:25:13.527385 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_005h.txt
+-rw-r--r--   0        0        0     5773 2023-05-08 11:25:13.527385 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_006h.txt
+-rw-r--r--   0        0        0     5764 2023-05-08 11:25:13.527385 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_007h.txt
+-rw-r--r--   0        0        0     5771 2023-05-08 11:25:13.527385 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_008h.txt
+-rw-r--r--   0        0        0     5780 2023-05-08 11:25:13.527385 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_009h.txt
+-rw-r--r--   0        0        0     5787 2023-05-08 11:25:13.537386 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_010h.txt
+-rw-r--r--   0        0        0   840169 2023-05-08 10:31:25.578990 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/grid.dat
+-rw-r--r--   0        0        0      198 2023-05-08 11:25:13.527385 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/lstcurr_UVW.pre
+-rw-r--r--   0        0        0        6 2023-05-08 11:25:26.928239 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/lstwaves.pre
+-rw-r--r--   0        0        0      165 2023-05-08 11:25:26.878236 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/lstwinds.pre
+-rw-r--r--   0        0        0     3967 2023-05-08 11:25:26.848234 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_000h.txt
+-rw-r--r--   0        0        0     3968 2023-05-08 11:25:26.858235 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_001h.txt
+-rw-r--r--   0        0        0     3965 2023-05-08 11:25:26.858235 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_002h.txt
+-rw-r--r--   0        0        0     3959 2023-05-08 11:25:26.858235 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_003h.txt
+-rw-r--r--   0        0        0     3957 2023-05-08 11:25:26.868235 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_004h.txt
+-rw-r--r--   0        0        0     3951 2023-05-08 11:25:26.868235 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_005h.txt
+-rw-r--r--   0        0        0     3947 2023-05-08 11:25:26.868235 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_006h.txt
+-rw-r--r--   0        0        0     3968 2023-05-08 11:25:26.868235 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_007h.txt
+-rw-r--r--   0        0        0     3958 2023-05-08 11:25:26.878236 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_008h.txt
+-rw-r--r--   0        0        0     3946 2023-05-08 11:25:26.878236 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_009h.txt
+-rw-r--r--   0        0        0     3937 2023-05-08 11:25:26.878236 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_010h.txt
+-rw-r--r--   0        0        0    35005 2023-05-08 11:25:29.558407 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/output/grids_001.nc
+-rw-r--r--   0        0        0    24093 2023-05-08 11:25:29.568408 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/output/grids_002.nc
+-rw-r--r--   0        0        0   348805 2023-05-08 11:25:29.208385 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/output/particles_001.csv
+-rw-r--r--   0        0        0   527846 2023-05-10 16:13:08.429088 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/output/particles_001.geojson
+-rw-r--r--   0        0        0   302691 2023-05-08 11:25:29.218386 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/output/particles_002.csv
+-rw-r--r--   0        0        0   497813 2023-05-10 16:13:08.429088 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/output/particles_002.geojson
+-rw-r--r--   0        0        0     2188 2023-05-08 11:25:29.238387 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/output/properties_001.csv
+-rw-r--r--   0        0        0     7169 2023-05-10 16:13:08.429088 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/output/properties_001.json
+-rw-r--r--   0        0        0     2251 2023-05-08 11:25:29.238387 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/output/properties_002.csv
+-rw-r--r--   0        0        0     7242 2023-05-10 16:13:08.429088 pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/output/properties_002.json
+-rw-r--r--   0        0        0    63326 2023-05-08 10:31:26.468993 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa.dat
+-rw-r--r--   0        0        0    36930 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono1.dat
+-rw-r--r--   0        0        0      330 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono10.dat
+-rw-r--r--   0        0        0      390 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono11.dat
+-rw-r--r--   0        0        0      360 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono12.dat
+-rw-r--r--   0        0        0      390 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono13.dat
+-rw-r--r--   0        0        0      360 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono14.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono15.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono16.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono17.dat
+-rw-r--r--   0        0        0      300 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono18.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono19.dat
+-rw-r--r--   0        0        0    12810 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono2.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono20.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono21.dat
+-rw-r--r--   0        0        0      180 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono22.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono23.dat
+-rw-r--r--   0        0        0      300 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono24.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono25.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono26.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono27.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono28.dat
+-rw-r--r--   0        0        0      330 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono29.dat
+-rw-r--r--   0        0        0     1590 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono3.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono30.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono31.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono32.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono33.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono34.dat
+-rw-r--r--   0        0        0      120 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono35.dat
+-rw-r--r--   0        0        0      120 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono36.dat
+-rw-r--r--   0        0        0     1170 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono4.dat
+-rw-r--r--   0        0        0      510 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono5.dat
+-rw-r--r--   0        0        0      900 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono6.dat
+-rw-r--r--   0        0        0     1020 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono7.dat
+-rw-r--r--   0        0        0      510 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono8.dat
+-rw-r--r--   0        0        0      600 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono9.dat
+-rw-r--r--   0        0        0   840169 2023-05-08 10:31:25.578990 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/grid.dat
+-rw-r--r--   0        0        0  1231776 2023-07-04 10:35:20.609421 pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/ibiza_domain.png
+-rw-r--r--   0        0        0       72 2023-01-09 16:55:02.280651 pyteseo-0.0.7/pyteseo/tests/data/lstcurr.pre
+-rw-r--r--   0        0        0       36 2023-01-27 13:50:37.678084 pyteseo-0.0.7/pyteseo/tests/data/lstcurr_UVW_cte.pre
+-rw-r--r--   0        0        0       45 2023-05-17 11:10:20.837289 pyteseo-0.0.7/pyteseo/tests/data/lstcurr_depthavg.pre
+-rw-r--r--   0        0        0       60 2023-01-30 12:26:16.443318 pyteseo-0.0.7/pyteseo/tests/data/lstwaves.pre
+-rw-r--r--   0        0        0       32 2023-01-31 09:57:32.253738 pyteseo-0.0.7/pyteseo/tests/data/lstwaves_cte.pre
+-rw-r--r--   0        0        0       60 2023-01-13 08:20:28.125803 pyteseo-0.0.7/pyteseo/tests/data/lstwinds.pre
+-rw-r--r--   0        0        0       36 2023-01-31 09:57:32.253738 pyteseo-0.0.7/pyteseo/tests/data/lstwinds_cte.pre
+-rw-r--r--   0        0        0     6701 2023-05-08 11:24:40.005250 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1.cfg
+-rw-r--r--   0        0        0     1539 2023-05-08 11:24:40.005250 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1.run
+-rw-r--r--   0        0        0      357 2023-05-08 11:24:40.275267 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_grid_001_000060.txt
+-rw-r--r--   0        0        0      595 2023-05-08 11:24:40.825302 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_grid_001_000120.txt
+-rw-r--r--   0        0        0      595 2023-05-08 11:24:41.105320 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_grid_001_000180.txt
+-rw-r--r--   0        0        0      357 2023-05-08 11:24:41.205326 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_grid_001_000240.txt
+-rw-r--r--   0        0        0      357 2023-05-08 11:24:40.275267 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_grid_002_000060.txt
+-rw-r--r--   0        0        0      476 2023-05-08 11:24:40.825302 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_grid_002_000120.txt
+-rw-r--r--   0        0        0       99 2023-05-08 11:24:40.065253 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000000.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:24:40.275267 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000060.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:24:40.825302 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000120.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.105320 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000180.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.205326 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000240.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.305333 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000300.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.405339 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000360.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.515346 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000420.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.615352 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000480.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.685357 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000540.txt
+-rw-r--r--   0        0        0   198099 2023-05-08 11:24:41.715359 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000600.txt
+-rw-r--r--   0        0        0     5004 2023-05-08 11:24:41.715359 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_properties_001.txt
+-rw-r--r--   0        0        0     5004 2023-05-08 11:24:41.715359 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_properties_002.txt
+-rw-r--r--   0        0        0   748950 2023-05-08 11:24:40.065253 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/grid_coordinates.txt
+-rw-r--r--   0        0        0    63326 2023-05-08 10:31:26.468993 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa.dat
+-rw-r--r--   0        0        0    36930 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono1.dat
+-rw-r--r--   0        0        0      330 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono10.dat
+-rw-r--r--   0        0        0      390 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono11.dat
+-rw-r--r--   0        0        0      360 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono12.dat
+-rw-r--r--   0        0        0      390 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono13.dat
+-rw-r--r--   0        0        0      360 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono14.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono15.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono16.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono17.dat
+-rw-r--r--   0        0        0      300 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono18.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono19.dat
+-rw-r--r--   0        0        0    12810 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono2.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono20.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono21.dat
+-rw-r--r--   0        0        0      180 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono22.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.448992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono23.dat
+-rw-r--r--   0        0        0      300 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono24.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono25.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono26.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono27.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono28.dat
+-rw-r--r--   0        0        0      330 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono29.dat
+-rw-r--r--   0        0        0     1590 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono3.dat
+-rw-r--r--   0        0        0      240 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono30.dat
+-rw-r--r--   0        0        0      270 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono31.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono32.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono33.dat
+-rw-r--r--   0        0        0      210 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono34.dat
+-rw-r--r--   0        0        0      120 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono35.dat
+-rw-r--r--   0        0        0      120 2023-05-08 10:31:26.458992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono36.dat
+-rw-r--r--   0        0        0     1170 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono4.dat
+-rw-r--r--   0        0        0      510 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono5.dat
+-rw-r--r--   0        0        0      900 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono6.dat
+-rw-r--r--   0        0        0     1020 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono7.dat
+-rw-r--r--   0        0        0      510 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono8.dat
+-rw-r--r--   0        0        0      600 2023-05-08 10:31:26.438992 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono9.dat
+-rw-r--r--   0        0        0     5829 2023-05-08 11:23:49.021999 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_000h.txt
+-rw-r--r--   0        0        0     5820 2023-05-08 11:23:49.031999 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_001h.txt
+-rw-r--r--   0        0        0     5805 2023-05-08 11:23:49.031999 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_002h.txt
+-rw-r--r--   0        0        0     5793 2023-05-08 11:23:49.042000 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_003h.txt
+-rw-r--r--   0        0        0     5785 2023-05-08 11:23:49.042000 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_004h.txt
+-rw-r--r--   0        0        0     5777 2023-05-08 11:23:49.042000 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_005h.txt
+-rw-r--r--   0        0        0     5773 2023-05-08 11:23:49.042000 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_006h.txt
+-rw-r--r--   0        0        0     5764 2023-05-08 11:23:49.042000 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_007h.txt
+-rw-r--r--   0        0        0     5771 2023-05-08 11:23:49.052000 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_008h.txt
+-rw-r--r--   0        0        0     5780 2023-05-08 11:23:49.052000 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_009h.txt
+-rw-r--r--   0        0        0     5787 2023-05-08 11:23:49.052000 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_010h.txt
+-rw-r--r--   0        0        0   840169 2023-05-08 10:31:25.578990 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/grid.dat
+-rw-r--r--   0        0        0      198 2023-05-08 11:23:49.052000 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/lstcurr_UVW.pre
+-rw-r--r--   0        0        0        6 2023-05-08 11:24:39.975248 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/lstwaves.pre
+-rw-r--r--   0        0        0      165 2023-05-08 11:24:39.925244 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/lstwinds.pre
+-rw-r--r--   0        0        0     3967 2023-05-08 11:24:39.895243 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_000h.txt
+-rw-r--r--   0        0        0     3968 2023-05-08 11:24:39.905243 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_001h.txt
+-rw-r--r--   0        0        0     3965 2023-05-08 11:24:39.905243 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_002h.txt
+-rw-r--r--   0        0        0     3959 2023-05-08 11:24:39.905243 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_003h.txt
+-rw-r--r--   0        0        0     3957 2023-05-08 11:24:39.915244 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_004h.txt
+-rw-r--r--   0        0        0     3951 2023-05-08 11:24:39.915244 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_005h.txt
+-rw-r--r--   0        0        0     3947 2023-05-08 11:24:39.915244 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_006h.txt
+-rw-r--r--   0        0        0     3968 2023-05-08 11:24:39.915244 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_007h.txt
+-rw-r--r--   0        0        0     3958 2023-05-08 11:24:39.915244 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_008h.txt
+-rw-r--r--   0        0        0     3946 2023-05-08 11:24:39.925244 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_009h.txt
+-rw-r--r--   0        0        0     3937 2023-05-08 11:24:39.925244 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_010h.txt
+-rw-r--r--   0        0        0    31485 2023-05-08 11:24:42.585414 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/output/grids_001.nc
+-rw-r--r--   0        0        0    23229 2023-05-08 11:24:42.595415 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/output/grids_002.nc
+-rw-r--r--   0        0        0   348848 2023-05-08 11:24:42.235392 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/output/particles_001.csv
+-rw-r--r--   0        0        0   527956 2023-05-10 16:13:08.419088 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/output/particles_001.geojson
+-rw-r--r--   0        0        0   302657 2023-05-08 11:24:42.245392 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/output/particles_002.csv
+-rw-r--r--   0        0        0   497752 2023-05-10 16:13:08.439088 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/output/particles_002.geojson
+-rw-r--r--   0        0        0     1853 2023-05-08 11:24:42.265394 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/output/properties_001.csv
+-rw-r--r--   0        0        0     6125 2023-05-10 16:13:08.429088 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/output/properties_001.json
+-rw-r--r--   0        0        0     1858 2023-05-08 11:24:42.265394 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/output/properties_002.csv
+-rw-r--r--   0        0        0     6139 2023-05-10 16:13:08.419088 pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/output/properties_002.json
+-rw-r--r--   0        0        0        6 2023-05-10 16:13:08.419088 pyteseo-0.0.7/pyteseo/tests/data/shapefile_cantabria/Cantabria.cpg
+-rw-r--r--   0        0        0      382 2023-05-09 14:10:49.121228 pyteseo-0.0.7/pyteseo/tests/data/shapefile_cantabria/Cantabria.dbf
+-rw-r--r--   0        0        0      413 2023-05-10 16:13:08.429088 pyteseo-0.0.7/pyteseo/tests/data/shapefile_cantabria/Cantabria.prj
+-rw-r--r--   0        0        0      132 2023-05-09 14:10:49.121228 pyteseo-0.0.7/pyteseo/tests/data/shapefile_cantabria/Cantabria.sbn
+-rw-r--r--   0        0        0      116 2023-05-09 14:10:49.131229 pyteseo-0.0.7/pyteseo/tests/data/shapefile_cantabria/Cantabria.sbx
+-rw-r--r--   0        0        0   259168 2023-05-09 14:10:49.131229 pyteseo-0.0.7/pyteseo/tests/data/shapefile_cantabria/Cantabria.shp
+-rw-r--r--   0        0        0    10465 2023-05-09 14:10:49.151231 pyteseo-0.0.7/pyteseo/tests/data/shapefile_cantabria/Cantabria.shp.xml
+-rw-r--r--   0        0        0      108 2023-05-09 14:10:49.151231 pyteseo-0.0.7/pyteseo/tests/data/shapefile_cantabria/Cantabria.shx
+-rw-r--r--   0        0        0      456 2023-01-30 12:28:00.313319 pyteseo-0.0.7/pyteseo/tests/data/waves_000h.txt
+-rw-r--r--   0        0        0      480 2023-01-30 12:28:28.243319 pyteseo-0.0.7/pyteseo/tests/data/waves_001h.txt
+-rw-r--r--   0        0        0      480 2023-01-30 12:28:40.053319 pyteseo-0.0.7/pyteseo/tests/data/waves_002h.txt
+-rw-r--r--   0        0        0      516 2023-01-31 09:57:32.263738 pyteseo-0.0.7/pyteseo/tests/data/waves_003h.txt
+-rw-r--r--   0        0        0    25121 2023-05-16 06:59:43.223472 pyteseo-0.0.7/pyteseo/tests/data/winds.nc
+-rw-r--r--   0        0        0      732 2022-11-14 07:58:35.871414 pyteseo-0.0.7/pyteseo/tests/data/winds_000h.txt
+-rw-r--r--   0        0        0      732 2022-11-14 07:58:35.950414 pyteseo-0.0.7/pyteseo/tests/data/winds_001h.txt
+-rw-r--r--   0        0        0      732 2022-11-14 07:58:36.019414 pyteseo-0.0.7/pyteseo/tests/data/winds_002h.txt
+-rw-r--r--   0        0        0      732 2022-11-14 07:58:36.125414 pyteseo-0.0.7/pyteseo/tests/data/winds_003h.txt
+-rw-r--r--   0        0        0        0 2023-06-27 13:25:50.521107 pyteseo-0.0.7/pyteseo/tests/e2e/__init__.py
+-rw-r--r--   0        0        0     2771 2023-06-29 15:03:46.715414 pyteseo-0.0.7/pyteseo/tests/e2e/test_create_domain.py
+-rw-r--r--   0        0        0     5497 2023-07-04 11:39:12.073878 pyteseo-0.0.7/pyteseo/tests/e2e/test_create_forcings.py
+-rw-r--r--   0        0        0     3350 2023-07-04 13:05:21.515102 pyteseo-0.0.7/pyteseo/tests/e2e/test_global_simulation.py
+-rw-r--r--   0        0        0     5711 2023-07-05 10:43:36.532299 pyteseo-0.0.7/pyteseo/tests/e2e/test_perform_simulation.py
+-rw-r--r--   0        0        0        0 2023-02-10 07:53:13.427520 pyteseo-0.0.7/pyteseo/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1017 2023-06-20 06:50:11.125799 pyteseo-0.0.7/pyteseo/tests/integration/test_cmems.py
+-rw-r--r--   0        0        0      592 2023-06-19 13:22:19.220765 pyteseo-0.0.7/pyteseo/tests/integration/test_ihcantabria.py
+-rw-r--r--   0        0        0     1941 2023-06-19 09:19:46.311206 pyteseo-0.0.7/pyteseo/tests/integration/test_opendap.py
+-rw-r--r--   0        0        0     3213 2023-06-27 14:48:58.103657 pyteseo-0.0.7/pyteseo/tests/integration/test_providers_datasets.py
+-rw-r--r--   0        0        0      423 2023-06-21 16:02:05.371718 pyteseo-0.0.7/pyteseo/tests/integration/test_providers_init.py
+-rw-r--r--   0        0        0     1167 2023-06-26 11:31:01.395456 pyteseo-0.0.7/pyteseo/tests/integration/test_providers_preprocess.py
+-rw-r--r--   0        0        0     9593 2023-07-03 06:27:38.509917 pyteseo-0.0.7/pyteseo/tests/integration/test_simulation_cte_forcing.py
+-rw-r--r--   0        0        0        0 2023-02-10 07:53:13.427520 pyteseo-0.0.7/pyteseo/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4623 2023-07-03 06:27:38.319913 pyteseo-0.0.7/pyteseo/tests/unit/test_cfg.py
+-rw-r--r--   0        0        0     6183 2023-05-22 08:08:53.659923 pyteseo-0.0.7/pyteseo/tests/unit/test_clasess.py
+-rw-r--r--   0        0        0     2865 2023-07-05 08:22:10.525245 pyteseo-0.0.7/pyteseo/tests/unit/test_export.py
+-rw-r--r--   0        0        0     3286 2023-05-10 13:10:41.515296 pyteseo-0.0.7/pyteseo/tests/unit/test_io_coastline.py
+-rw-r--r--   0        0        0     3589 2023-05-17 14:25:17.630330 pyteseo-0.0.7/pyteseo/tests/unit/test_io_forcings.py
+-rw-r--r--   0        0        0     2552 2023-05-10 15:10:22.789296 pyteseo-0.0.7/pyteseo/tests/unit/test_io_grid.py
+-rw-r--r--   0        0        0     1612 2023-07-05 08:03:38.475334 pyteseo-0.0.7/pyteseo/tests/unit/test_io_results.py
+-rw-r--r--   0        0        0     1650 2023-06-21 16:36:36.468288 pyteseo-0.0.7/pyteseo/tests/unit/test_open_mfdatasets.py
+-rw-r--r--   0        0        0     1892 2023-07-05 10:50:16.631527 pyteseo-0.0.7/pyteseo/tests/unit/test_plot.py
+-rw-r--r--   0        0        0     2045 2023-06-20 07:21:08.582930 pyteseo-0.0.7/pyteseo/tests/unit/test_preprocess_forcings.py
+-rw-r--r--   0        0        0     2358 2023-07-03 10:49:18.674684 pyteseo-0.0.7/pyteseo/tests/unit/test_substances.py
+-rw-r--r--   0        0        0    15980 2023-07-05 08:03:38.545336 pyteseo-0.0.7/pyteseo/wrapper.py
+-rw-r--r--   0        0        0     6506 1970-01-01 00:00:00.000000 pyteseo-0.0.7/PKG-INFO
```

### Comparing `pyteseo-0.0.6/.coverage` & `pyteseo-0.0.7/.coverage`

 * *Files 20% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -12,50 +12,56 @@
     unique (key)
     -- Possible keys:
     --  'has_arcs' boolean      -- Is this data recording branches?
     --  'sys_argv' text         -- The coverage command line that recorded the data.
     --  'version' text          -- The version of coverage.py that made the file.
     --  'when' text             -- Datetime when the file was created.
 );
-INSERT INTO meta VALUES('version','7.2.3');
+INSERT INTO meta VALUES('version','7.2.7');
 INSERT INTO meta VALUES('has_arcs','0');
 CREATE TABLE file (
     -- A row per file measured.
     id integer primary key,
     path text,
     unique (path)
 );
 INSERT INTO file VALUES(1,'/home/aragong/repositories/pyteseo/pyteseo/__init__.py');
-INSERT INTO file VALUES(2,'/home/aragong/repositories/pyteseo/pyteseo/connections/__init__.py');
-INSERT INTO file VALUES(3,'/home/aragong/repositories/pyteseo/pyteseo/connections/cmems.py');
-INSERT INTO file VALUES(4,'/home/aragong/repositories/pyteseo/pyteseo/defaults.py');
-INSERT INTO file VALUES(5,'/home/aragong/repositories/pyteseo/pyteseo/services.py');
-INSERT INTO file VALUES(6,'/home/aragong/repositories/pyteseo/pyteseo/connections/bathymetries.py');
-INSERT INTO file VALUES(7,'/home/aragong/repositories/pyteseo/pyteseo/connections/coastlines.py');
-INSERT INTO file VALUES(8,'/home/aragong/repositories/pyteseo/pyteseo/io/__init__.py');
-INSERT INTO file VALUES(9,'/home/aragong/repositories/pyteseo/pyteseo/io/coastline.py');
-INSERT INTO file VALUES(10,'/home/aragong/repositories/pyteseo/pyteseo/io/grid.py');
-INSERT INTO file VALUES(11,'/home/aragong/repositories/pyteseo/pyteseo/io/utils.py');
-INSERT INTO file VALUES(12,'/home/aragong/repositories/pyteseo/pyteseo/plot/__init__.py');
-INSERT INTO file VALUES(13,'/home/aragong/repositories/pyteseo/pyteseo/plot/figures.py');
-INSERT INTO file VALUES(14,'/home/aragong/repositories/pyteseo/pyteseo/io/forcings.py');
-INSERT INTO file VALUES(15,'/home/aragong/repositories/pyteseo/pyteseo/plot/basics.py');
-INSERT INTO file VALUES(16,'/home/aragong/repositories/pyteseo/pyteseo/connections/noaa_opendap.py');
-INSERT INTO file VALUES(17,'/home/aragong/repositories/pyteseo/pyteseo/wrapper.py');
-INSERT INTO file VALUES(18,'/home/aragong/repositories/pyteseo/pyteseo/classes.py');
-INSERT INTO file VALUES(19,'/home/aragong/repositories/pyteseo/pyteseo/export/__init__.py');
-INSERT INTO file VALUES(20,'/home/aragong/repositories/pyteseo/pyteseo/export/grids.py');
-INSERT INTO file VALUES(21,'/home/aragong/repositories/pyteseo/pyteseo/export/particles.py');
-INSERT INTO file VALUES(22,'/home/aragong/repositories/pyteseo/pyteseo/export/properties.py');
-INSERT INTO file VALUES(23,'/home/aragong/repositories/pyteseo/pyteseo/io/cfg.py');
-INSERT INTO file VALUES(24,'/home/aragong/repositories/pyteseo/pyteseo/io/substances.py');
-INSERT INTO file VALUES(25,'/home/aragong/repositories/pyteseo/pyteseo/io/hns_calib.py');
-INSERT INTO file VALUES(26,'/home/aragong/repositories/pyteseo/pyteseo/io/results.py');
-INSERT INTO file VALUES(27,'/home/aragong/repositories/pyteseo/pyteseo/io/run.py');
-INSERT INTO file VALUES(28,'/home/aragong/repositories/pyteseo/pyteseo/plot/animations.py');
+INSERT INTO file VALUES(2,'/home/aragong/repositories/pyteseo/pyteseo/defaults.py');
+INSERT INTO file VALUES(3,'/home/aragong/repositories/pyteseo/pyteseo/preprocess/__init__.py');
+INSERT INTO file VALUES(4,'/home/aragong/repositories/pyteseo/pyteseo/preprocess/teseo_domain.py');
+INSERT INTO file VALUES(5,'/home/aragong/repositories/pyteseo/pyteseo/io/__init__.py');
+INSERT INTO file VALUES(6,'/home/aragong/repositories/pyteseo/pyteseo/io/coastline.py');
+INSERT INTO file VALUES(7,'/home/aragong/repositories/pyteseo/pyteseo/io/grid.py');
+INSERT INTO file VALUES(8,'/home/aragong/repositories/pyteseo/pyteseo/io/utils.py');
+INSERT INTO file VALUES(9,'/home/aragong/repositories/pyteseo/pyteseo/classes.py');
+INSERT INTO file VALUES(10,'/home/aragong/repositories/pyteseo/pyteseo/io/forcings.py');
+INSERT INTO file VALUES(11,'/home/aragong/repositories/pyteseo/pyteseo/plot/__init__.py');
+INSERT INTO file VALUES(12,'/home/aragong/repositories/pyteseo/pyteseo/plot/figures.py');
+INSERT INTO file VALUES(13,'/home/aragong/repositories/pyteseo/pyteseo/plot/basics.py');
+INSERT INTO file VALUES(14,'/home/aragong/repositories/pyteseo/pyteseo/preprocess/geodataframe.py');
+INSERT INTO file VALUES(15,'/home/aragong/repositories/pyteseo/pyteseo/providers/__init__.py');
+INSERT INTO file VALUES(16,'/home/aragong/repositories/pyteseo/pyteseo/providers/connection.py');
+INSERT INTO file VALUES(17,'/home/aragong/repositories/pyteseo/pyteseo/providers/cmems.py');
+INSERT INTO file VALUES(18,'/home/aragong/repositories/pyteseo/pyteseo/providers/emodnet.py');
+INSERT INTO file VALUES(19,'/home/aragong/repositories/pyteseo/pyteseo/providers/ihcantabria.py');
+INSERT INTO file VALUES(20,'/home/aragong/repositories/pyteseo/pyteseo/preprocess/dataset.py');
+INSERT INTO file VALUES(21,'/home/aragong/repositories/pyteseo/pyteseo/preprocess/teseo_standarizations.py');
+INSERT INTO file VALUES(22,'/home/aragong/repositories/pyteseo/pyteseo/preprocess/teseo_forcing.py');
+INSERT INTO file VALUES(23,'/home/aragong/repositories/pyteseo/pyteseo/wrapper.py');
+INSERT INTO file VALUES(24,'/home/aragong/repositories/pyteseo/pyteseo/export/__init__.py');
+INSERT INTO file VALUES(25,'/home/aragong/repositories/pyteseo/pyteseo/export/grids.py');
+INSERT INTO file VALUES(26,'/home/aragong/repositories/pyteseo/pyteseo/export/particles.py');
+INSERT INTO file VALUES(27,'/home/aragong/repositories/pyteseo/pyteseo/export/properties.py');
+INSERT INTO file VALUES(28,'/home/aragong/repositories/pyteseo/pyteseo/io/cfg.py');
+INSERT INTO file VALUES(29,'/home/aragong/repositories/pyteseo/pyteseo/io/substances.py');
+INSERT INTO file VALUES(30,'/home/aragong/repositories/pyteseo/pyteseo/io/hns_calib.py');
+INSERT INTO file VALUES(31,'/home/aragong/repositories/pyteseo/pyteseo/io/results.py');
+INSERT INTO file VALUES(32,'/home/aragong/repositories/pyteseo/pyteseo/io/run.py');
+INSERT INTO file VALUES(33,'/home/aragong/repositories/pyteseo/pyteseo/plot/animations.py');
+INSERT INTO file VALUES(34,'/home/aragong/repositories/pyteseo/pyteseo/providers/noaa.py');
 CREATE TABLE context (
     -- A row per context measured.
     id integer primary key,
     context text,
     unique (context)
 );
 INSERT INTO context VALUES(1,'');
@@ -65,42 +71,47 @@
     file_id integer,            -- foreign key to `file`.
     context_id integer,         -- foreign key to `context`.
     numbits blob,               -- see the numbits functions in coverage.numbits
     foreign key (file_id) references file (id),
     foreign key (context_id) references context (id),
     unique (file_id, context_id)
 );
-INSERT INTO line_bits VALUES(1,1,X'5a06');
-INSERT INTO line_bits VALUES(2,1,X'01');
-INSERT INTO line_bits VALUES(3,1,X'da130160fe0520ea4b004b004ff800004206c03dc00058');
-INSERT INTO line_bits VALUES(4,1,X'4afff9fffcd1fffffffff33fff7ffedffffd1fffff9f40400000001004');
-INSERT INTO line_bits VALUES(5,1,X'ba9fe00f000010081ae6b2fd69f7f902');
-INSERT INTO line_bits VALUES(6,1,X'9adf87ffb3bccbf702');
-INSERT INTO line_bits VALUES(7,1,X'360e000edfc30fe0d3e916');
-INSERT INTO line_bits VALUES(8,1,X'02');
-INSERT INTO line_bits VALUES(9,1,X'aa4b80bd5b6f12e0a537bf7ffe23005b7e421f01');
-INSERT INTO line_bits VALUES(10,1,X'9e009700762e01b939bcf90f');
-INSERT INTO line_bits VALUES(11,1,X'96e300a60746700c3e');
-INSERT INTO line_bits VALUES(12,1,X'01');
-INSERT INTO line_bits VALUES(13,1,X'da03f07fdff7931fd8ef4b');
-INSERT INTO line_bits VALUES(14,1,X'aa0608402f4b00b604f80480fbdb9c01e0acfd630078a0eefe23f02c');
-INSERT INTO line_bits VALUES(15,1,X'3e814620ff083409cc8fc0fd783f068000880502bb0b');
-INSERT INTO line_bits VALUES(16,1,X'6a320098db59b0b72b');
-INSERT INTO line_bits VALUES(17,1,X'7a06fe900cbc74bff76ebdbb0bd0775d1de0f3eeee0abe7d7f74f7f5d616fc12e008ff06d8c39f0133f3fbffb43f79');
-INSERT INTO line_bits VALUES(18,1,X'fa7a3e0c7e0931f8123170fbf879dfd3420cdc3f7d0b3170fffa1602');
-INSERT INTO line_bits VALUES(19,1,X'02');
-INSERT INTO line_bits VALUES(20,1,X'ba2001609ff3ffbc4980fff37f7e7e7e3e01ff13');
-INSERT INTO line_bits VALUES(21,1,X'7a410600fb9cff370900ee9f06');
-INSERT INTO line_bits VALUES(22,1,X'5a9000b05f7f13');
-INSERT INTO line_bits VALUES(23,1,X'3a60000002986612005f066009009e3fa142154255a5841002aa52544555849c0000f07e2dd97bfc792e813ff386037f');
-INSERT INTO line_bits VALUES(24,1,X'3a0900763702e00d');
-INSERT INTO line_bits VALUES(25,1,X'0a0000000868');
-INSERT INTO line_bits VALUES(26,1,X'aaa200747f9902d0f5afa601e0f5affdfc0cc00900ef12c07e03');
-INSERT INTO line_bits VALUES(27,1,X'ce1ce02b54a55205650e1c38b08103');
-INSERT INTO line_bits VALUES(28,1,X'da07d8cf99ff7b1ebffa7fffc62cfefbf6fffff7f7fffbbb6df76701');
+INSERT INTO line_bits VALUES(1,1,X'9a1e');
+INSERT INTO line_bits VALUES(2,1,X'2afde7ffe38ffeeff8ffffff7ffee7ffcffffbbfffe3ffff13080800000082');
+INSERT INTO line_bits VALUES(3,1,X'02');
+INSERT INTO line_bits VALUES(4,1,X'eefe3009eef67e7900fb7ebff77e7bc1f5db2b9f0370f7f24f080080d047');
+INSERT INTO line_bits VALUES(5,1,X'02');
+INSERT INTO line_bits VALUES(6,1,X'aa4b80bd5b6f12e0a537bffffc8f006cf9097d04');
+INSERT INTO line_bits VALUES(7,1,X'9e008000762e01b939bcf90f');
+INSERT INTO line_bits VALUES(8,1,X'96e300a60746700c3e');
+INSERT INTO line_bits VALUES(9,1,X'eaebf930f825c4e04bc4c0ede3e77d4f0b3170fff42dc4c0fdeb5b08');
+INSERT INTO line_bits VALUES(10,1,X'aa0608402f4b00b604f80480fbdb9c01e0acfd630078a0eefe23f02c');
+INSERT INTO line_bits VALUES(11,1,X'02');
+INSERT INTO line_bits VALUES(12,1,X'da03f07fdff7931fd8ee97');
+INSERT INTO line_bits VALUES(13,1,X'3e814620ff083409cc8fc0fd783f068000880502bb0b');
+INSERT INTO line_bits VALUES(14,1,X'461f00787dfaf9');
+INSERT INTO line_bits VALUES(15,1,X'fa7cc04702f067');
+INSERT INTO line_bits VALUES(16,1,X'ea3807005b66f4bff71f18');
+INSERT INTO line_bits VALUES(17,1,X'dae69c3a');
+INSERT INTO line_bits VALUES(18,1,X'12');
+INSERT INTO line_bits VALUES(19,1,X'700970793900d303');
+INSERT INTO line_bits VALUES(20,1,X'7efa0f000078937f6dbbc7fbe2fb495efe000400e00d00007e00ec6f03');
+INSERT INTO line_bits VALUES(21,1,X'e60300e1b9de498005');
+INSERT INTO line_bits VALUES(22,1,X'b60fe46da77f6f931708e27b043ba77f1bff2d000018c0017ef6cd0f');
+INSERT INTO line_bits VALUES(23,1,X'ea35f08732f0d2fddebb75ee2e40df757580cfbbbb6be0db6f01b8fb7a77ef3db405bf0438c2bf01f6f067c0ccfcfe3fed4f1e');
+INSERT INTO line_bits VALUES(24,1,X'02');
+INSERT INTO line_bits VALUES(25,1,X'ba2001609fe7ff799300ffe7fffcfc047c02fe27');
+INSERT INTO line_bits VALUES(26,1,X'7a410600fb9cff370900ee9f06');
+INSERT INTO line_bits VALUES(27,1,X'5a9000b05f7f13');
+INSERT INTO line_bits VALUES(28,1,X'3a60000002986612005f066009013cff840a55085595124208a84a5115551172020180f76bc9dee3cf7309fc99371cf803');
+INSERT INTO line_bits VALUES(29,1,X'3a0900763702e04d00b7');
+INSERT INTO line_bits VALUES(30,1,X'0a0000000868');
+INSERT INTO line_bits VALUES(31,1,X'aaa200747f9902d0f5afa601f0fad77e7e06e00480770960bf01');
+INSERT INTO line_bits VALUES(32,1,X'ce1ce02b54a55205650e1c38b08103');
+INSERT INTO line_bits VALUES(33,1,X'da07d8cf99ff7b1ebffa7fffc62cfefbf6fffff7f7fffbbb6df76701');
 CREATE TABLE arc (
     -- If recording branches, a row per context per from/to line transition executed.
     file_id integer,            -- foreign key to `file`.
     context_id integer,         -- foreign key to `context`.
     fromno integer,             -- line number jumped from.
     tono integer,               -- line number jumped to.
     foreign key (file_id) references file (id),
```

### Comparing `pyteseo-0.0.6/.github/workflows/docs.yml` & `pyteseo-0.0.7/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/.github/workflows/tests.yml` & `pyteseo-0.0.7/.github/workflows/tests.yml`

 * *Files 26% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macOS-latest, windows-latest]
-        python-version: ["3.8", "3.9", "3.10"] # w/ python 3.11 library installation crash becouse the downgrade of netcdf4<=1.5.8
+        python-version: ["3.8","3.9", "3.10", "3.11"] # w/ python 3.11 library installation crash becouse the downgrade of netcdf4<=1.5.8
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
@@ -34,9 +34,10 @@
       - name: Install python library
         run: pip install "."
 
       - name: Test
         env:
           CMEMS_username: ${{ secrets.CMEMS_username }}
           CMEMS_password: ${{ secrets.CMEMS_password }}
+          DATAHUB_API_URL: "https://datahub.ihcantabria.com"
         run: pytest -m "not slow" -p "no:warnings"
             # pyteseo-tests
```

### Comparing `pyteseo-0.0.6/CHANGELOG.md` & `pyteseo-0.0.7/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,46 @@
 # Changelog
 
-## v0.0.6 - ??/??/2023
+## v0.0.8 - ??/??/2023
+### Added:
+1)
+2)
+3)
+4)
+5)
+### Changed:
+1)
+2)
+3)
+### Fixed:
+1)
+2)
+3)
+<br/><br/>
+
+
+## v0.0.7 - 05/07/2023
+### Added:
+1) preprocessing from any netcdf to teseo netcdf
+2) create_forcings
+3) create_domain
+4) create_simulation
+5) TL;DR guide added to docs
+### Changed:
+1) up for python>=3.8
+2) update documentation
+3) update testing
+### Fixed:
+1) login CMEMS was trigger at each operation
+2)
+3)
+<br/><br/>
+
+
+## v0.0.6 - 23/05/2023
 ### Added:
 1) Classes for forcings
 2) Create null forcings
 3) Create TeseoWrapper class
 4) Create cfg and run files
 5) Create *_hns.calib file
 6) First integration tests runing teseo v1.2.8 (drifter, oil and hns) with cte forcings with and without coastline
```

### Comparing `pyteseo-0.0.6/LICENSE.md` & `pyteseo-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/README.md` & `pyteseo-0.0.7/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -19,76 +19,82 @@
 
 
 **pyTESEO** is a python package developed by [IHCantabria](https://ihcantabria.com/en/) to simplify and facilitate the setup and processing of [TESEO](https://ihcantabria.com/en/specialized-software/teseo/) simulations *(TESEO is a lagrangian numerical model also developed by IHCantabria.)*
 
 
 ---
 
-## :computer: Installation
+## 💻 Installation
 
-1 - Install the python library using pip:
+1. Install pyTESEO library:
 
-```bash
-# From pypi repository
-pip install pyteseo
-
-# Or directly from github repository
-pip install git+https://github.com/IHCantabria/pyteseo
-```
-
-2 - Install TESEO model binary (**Not available yet!**):
-- Get access to the binary: https://github.com/IHCantabria/TESEO/blob/main/bin
-- Set up environment variable "TESEO_PATH" with the path to the model executable. You can use the command following CLI command after activate the python environement (python-dotenv library)
+    [Pip package manager](https://pip.pypa.io/en/stable/) is needed to install the library and
+    it is recommended to be installed from [IHCantabria/pyteseo](https://github.com/IHCantabria/    pyteseo) repository:
+    ```bash
+    pip install git+https://github.com/IHCantabria/pyteseo
+    ```
 
+    *Alternatively, you can install it from pypi but you will need also install some direct dependencies     that are not publish in pipy repositories:*
     ```bash
-        dotenv set TESEO_PATH /path/to/teseo_executable
+    pip install pyteseo
+
+    # direct dependencies:
+    pip install "datahub @ https://github.com/IHCantabria/datahub.client/archive/refs/tags/v0.9.4.zip"
     ```
-3 - Opendap connection to some [CMEMS products](https://data.marine.copernicus.eu/products) is available at the library `pyteseo/connections/cmems.py` but needs authetication through the following environement variables:
-```bash
-dotenv set CMEMS_username your_username_at_CMEMS
-```
-```bash
-dotenv set CMEMS_password your_password_at_CMEMS
-```
+
+2. Install TESEO model binary (**Not available yet!**):
+
+    - Get access to the binary @ (https://github.com/IHCantabria/TESEO/blob/main/bin)
+    - Set up environment variable "TESEO_PATH" with the path to the model executable. You can use the   command following CLI command after activate the python environement (python-dotenv library)
+
+        ```bash
+            dotenv set TESEO_PATH /path/to/teseo_executable
+        ```
+
+3. Online data providers require to stablish opendap connections, and in some cases aditional configurations:
+
+    * [CMEMS products](https://data.marine.copernicus.eu/products) requires authentication. You should set up the environment variables `CMEMS_username` and `CMEMS_password`.
+        ```bash
+        dotenv set CMEMS_username your_username_at_CMEMS
+        ```
+        ```bash
+        dotenv set CMEMS_password your_password_at_CMEMS
+        ```
+
+    * [IHCantabria products](https://discoverymap.ihcantabria.com/) requires connection to IHCantabria datahub API. You should set up the environment variable `DATAHUB_API_URL`.
+        ```bash
+        DATAHUB_API_URL = "https://datahub.ihcantabria.com"
+        ```
 
 ---
 
-## :heavy_check_mark: Tests
+## ✔️ Tests
 Tests are located in `pyteseo/tests/` and data required for tests are located in `pyteseo/tests/data/`.
 Tests have been developed using [pytest](https://docs.pytest.org/).
 
 Run tests to verify your package installation:
 ```bash
 pyteseo-test        # Run tests and prompt pytest-report
 ```
 
-If you have cloned the repository, you also can run `coverage.py` functionalities based on current `pytproyect.toml` configuration from your terminal command line interface:
-```bash
-# Commands should be executed from the root directory of the repo
-
-coverage run        # For run tests and generate ".coverage" file
-coverage report     # For prompt results from ".coverage" file
-coverage html       # For generate html report on "htmlcov" folder
-```
-
 ---
 
-## :recycle: Continuous integration (CI)
+## ♻️ Continuous integration (CI)
 
 * Build and deploy documentation on Github Pages in [.github/workflows/docs.yml](.github/workflows/docs.yml)
 * Install and test package in diferent environments in [.github/workflows/tests.yml](.github/workflows/tests.yml)
 * Precommit hooks for formats and linting in [.pre-commit-config.yaml](.pre-commit-config.yaml)
 
 *For Linux, Windows, MacOS and compatible python versions defined in installation section*
 
 ---
 
-## :books: Documentation
+## 📚 Documentation
 
 Documentation is available at https://ihcantabria.github.io/pyteseo
 
 ---
 
-## :copyright: Credits
-Developed and maintained by :man_technologist: [German Aragon](https://github.com/aragong) @ :office: [IHCantabria](https://github.com/IHCantabria).
+## ©️ Credits
+Developed and maintained by 👨‍💻 [German Aragon](https://github.com/aragong) @ 🏢 [IHCantabria](https://github.com/IHCantabria).
 
 ---
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyteseo-0.0.6/docs/Makefile` & `pyteseo-0.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/docs/_static/TESEO_logo.png` & `pyteseo-0.0.7/docs/_static/TESEO_logo.png`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/docs/_static/doc_snapshoot.png` & `pyteseo-0.0.7/docs/_static/doc_snapshoot.png`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/docs/_static/pyTESEO_logo.png` & `pyteseo-0.0.7/docs/_static/pyTESEO_logo.png`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/docs/conf.py` & `pyteseo-0.0.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/docs/index.md` & `pyteseo-0.0.7/docs/index.md`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 ---
 
 ```{toctree}
 :caption: CONTENTS
 :maxdepth: 3
 
 get-started.md
-user-guide.md
+tl;dr-guide.md
 changelog.md
 autoapi/index.rst
 ```
 
 ```{toctree}
 :caption: USE CASES
 :titlesonly:
```

### Comparing `pyteseo-0.0.6/docs/make.bat` & `pyteseo-0.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/docs/notebooks/01_read_domain.ipynb` & `pyteseo-0.0.7/docs/notebooks/01_read_domain.ipynb`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/docs/notebooks/02_read_forcings.ipynb` & `pyteseo-0.0.7/docs/notebooks/02_read_forcings.ipynb`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/docs/notebooks/03_export_results.ipynb` & `pyteseo-0.0.7/docs/notebooks/03_export_results.ipynb`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/docs/notebooks/04_generate_forcings_from_cmems.ipynb` & `pyteseo-0.0.7/docs/notebooks/04_generate_forcings_from_cmems.ipynb`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/docs/notebooks/05_drift_simulation.ipynb` & `pyteseo-0.0.7/docs/notebooks/05_drift_simulation.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998062015503877%*

 * *Differences: {"'cells'": '{6: {\'source\': {insert: [(22, \'    "forcings_init_time": datetime.utcnow() - '*

 * *            'timedelta(days=4),\\n\'), (32, \'    user_parameters["forcings_init_time"],\\n\'), '*

 * *            '(33, \'    user_parameters["forcings_init_time"] + '*

 * *            'user_parameters["duration"],\\n\')], delete: [33, 32, 22]}}}'}*

```diff
@@ -159,26 +159,26 @@
                 "    },\n",
                 "]\n",
                 "\n",
                 "user_parameters = {\n",
                 "    \"mode\": \"2d\",\n",
                 "    \"motion\": \"forward\",\n",
                 "    \"substance_type\": \"drifter\",\n",
-                "    \"forcing_init_datetime\": datetime.utcnow() - timedelta(days=4),\n",
+                "    \"forcings_init_time\": datetime.utcnow() - timedelta(days=4),\n",
                 "    \"duration\": timedelta(hours=3),\n",
                 "    \"timestep\": timedelta(minutes=1),\n",
                 "    \"use_coastline\": True,\n",
                 "    \"spill_points\": drifter_spill_points,\n",
                 "}\n",
                 "\n",
                 "# 3 - Generate forcings\n",
                 "bbox = (job.grid.x_min, job.grid.y_min, job.grid.x_max, job.grid.y_max)\n",
                 "timebox = (\n",
-                "    user_parameters[\"forcing_init_datetime\"],\n",
-                "    user_parameters[\"forcing_init_datetime\"] + user_parameters[\"duration\"],\n",
+                "    user_parameters[\"forcings_init_time\"],\n",
+                "    user_parameters[\"forcings_init_time\"] + user_parameters[\"duration\"],\n",
                 ")\n",
                 "currents = access_global_currents(username, password, bbox, timebox)\n",
                 "write_2d_forcing(currents, job.input_dir, \"currents\")\n",
                 "\n",
                 "winds = access_global_winds(username, password, bbox, timebox)\n",
                 "write_2d_forcing(winds, job.input_dir, \"winds\")"
             ]
```

### Comparing `pyteseo-0.0.6/docs/notebooks/06_hns_simulation.ipynb` & `pyteseo-0.0.7/docs/notebooks/06_hns_simulation.ipynb`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/docs/notebooks/07_stochastic_montecarlo.ipynb` & `pyteseo-0.0.7/docs/notebooks/07_stochastic_montecarlo.ipynb`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/docs/notebooks/08_stochastic_kmeans.ipynb` & `pyteseo-0.0.7/docs/notebooks/08_stochastic_kmeans.ipynb`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyproject.toml` & `pyteseo-0.0.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -16,34 +16,35 @@
     "Programming Language :: Python",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    # "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version", "description"]
 
 dependencies = [
     "geopandas",
     "owslib",
     "xarray",
     "dask",
-    "netcdf4<=1.5.8",
+    "netcdf4",
     "bottleneck",
     "ipykernel",
     "matplotlib",
     "geojson",
     "pytest >=7",
     "lxml",
     "scipy",
     "python-dotenv",
     "pydap",
-    "openpyxl"
+    "openpyxl",
+    # "datahub @ https://github.com/IHCantabria/datahub.client/archive/refs/tags/v0.9.4.zip"
 ]
 
 
 [project.optional-dependencies]
 dev = ["flit", "black", "sphinx", "coverage[toml]", "myst-nb", "sphinx-autoapi", "sphinx_rtd_theme"]
```

### Comparing `pyteseo-0.0.6/pyteseo/classes.py` & `pyteseo-0.0.7/pyteseo/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Submodule where axuliary clasess are defined"""
+
 from __future__ import annotations
 
 from pathlib import Path
 import numpy as np
 import pandas as pd
 import xarray as xr
 import geopandas as gpd
```

### Comparing `pyteseo-0.0.6/pyteseo/data/substances/hns.xlsx` & `pyteseo-0.0.7/pyteseo/data/substances/hns.xlsx`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/data/substances/hns_units.xlsx` & `pyteseo-0.0.7/pyteseo/data/substances/hns_units.xlsx`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/data/substances/oil.xlsx` & `pyteseo-0.0.7/pyteseo/data/substances/oil.xlsx`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/data/substances/oil_units.xlsx` & `pyteseo-0.0.7/pyteseo/data/substances/oil_units.xlsx`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/defaults.py` & `pyteseo-0.0.7/pyteseo/defaults.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Definition of default values, keys, parameters and varaible maps"""
+
 from datetime import timedelta
 
 import numpy as np
 
 
 DIRECTORY_NAMES = {"input": "input", "output": "output"}
 
@@ -27,26 +29,45 @@
     "teseo_properties": "*_properties_*.txt",
     "teseo_grids": "*_grid_*.txt",
     "export_particles": "particles_*.*",
     "export_properties": "properties_*.*",
     "export_grids": "grids_*.*",
 }
 
+# FIXME - DELETE VARIABLE_NAMES. USE FORCINGS VARAIBLES INSTEAD!
 VARIABLE_NAMES = {
     "currents": {"coords": ["time", "lon", "lat"], "vars": ["u", "v"]},
     "winds": {"coords": ["time", "lon", "lat"], "vars": ["u", "v"]},
     "waves": {"coords": ["time", "lon", "lat"], "vars": ["hs", "dir", "tp"]},
     "currents_depthavg": {
         "coords": ["time", "lon", "lat"],
         "vars": ["u", "v"],
     },
 }
-
+# NOTE - MAYBE I CAN DELETE COORDINATE_NAMES ALSO
 COORDINATE_NAMES = {"t": "time", "x": "lon", "y": "lat", "z": "depth"}
 
+DATASETS_VARNAMES = {
+    "currents": {"t": "time", "x": "lon", "y": "lat", "u": "u", "v": "v"},
+    "winds": {"t": "time", "x": "lon", "y": "lat", "u": "u", "v": "v"},
+    "currents_depthavg": {"t": "time", "x": "lon", "y": "lat", "u": "u", "v": "v"},
+    "waves": {
+        "t": "time",
+        "x": "lon",
+        "y": "lat",
+        "hs": "hs",
+        "dir": "dir",
+        "tp": "tp",
+    },
+    "topobathymetry": {"x": "lon", "y": "lat", "elevation": "elevation"},
+    "bathymetry": {"x": "lon", "y": "lat", "depth": "depth"},
+    "coastline": {"x": "lon", "y": "lat"},
+}
+
+
 RESULTS_MAP = {
     "time (h)": "time",
     "longitude (º)": "lon",
     "latitude (º)": "lat",
     "depth (m)": "depth",
     "status_index (-)": "status_index",
     "spill_id (-)": "spill_id",
@@ -170,15 +191,15 @@
     "save_particles": 1,
     "save_properties": 1,
     "save_grids": 1,
 }
 
 CFG_MAIN_MANDATORY_KEYS = [
     "substance_type",
-    "forcing_init_datetime",
+    "forcings_init_time",
     "duration",
     "spill_points",
 ]
 
 CFG_SPILL_POINT_MANDATORY_KEYS = [
     "lon",
     "lat",
```

### Comparing `pyteseo-0.0.6/pyteseo/export/grids.py` & `pyteseo-0.0.7/pyteseo/export/grids.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,43 +15,44 @@
     file_format: list,
     output_dir: str = ".",
 ) -> list:
     """Export TESEO's grids (by spill_id) to CSV, JSON, or NETCDF
 
     Args:
         df (pd.DataFrame): Grids data obtained with pyteseo.io.read_grids_results
-        file_format (list): csv, json, or nc
+        file_format (list): csv, json, or netcdf
         output_dir (str, optional): directory to export the files. Defaults to "."
 
     Returns:
         list: paths to exported files
     """
 
-    allowed_formats = ["csv", "json", "nc"]
+    allowed_formats = ["csv", "json", "netcdf", "nc"]
     exported_files = []
 
     output_dir = Path(output_dir)
     file_format = file_format.lower()
     if file_format not in allowed_formats:
         raise ValueError(
             f"Invalid format: {file_format}. Allowed formats {allowed_formats}"
         )
     else:
+        file_ext = file_format if file_format != "netcdf" else "nc"
         output_path_pattern = Path(
             output_dir,
-            FILE_PATTERNS["export_grids"].replace(".*", f".{file_format}"),
+            FILE_PATTERNS["export_grids"].replace(".*", f".{file_ext}"),
         )
 
     for spill_id, df in df.groupby("spill_id"):
         output_path = Path(str(output_path_pattern).replace("*", f"{spill_id:03d}"))
         if file_format == "csv":
             df.to_csv(output_path, index=False)
         elif file_format == "json":
             df.to_json(output_path, orient="index")
-        elif file_format == "nc":
+        elif file_format in ["nc", "netcdf"]:
             df = df.set_index(
                 [
                     COORDINATE_NAMES["t"],
                     COORDINATE_NAMES["x"],
                     COORDINATE_NAMES["y"],
                 ]
             )
```

### Comparing `pyteseo-0.0.6/pyteseo/export/particles.py` & `pyteseo-0.0.7/pyteseo/export/particles.py`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/export/properties.py` & `pyteseo-0.0.7/pyteseo/export/properties.py`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/io/cfg.py` & `pyteseo-0.0.7/pyteseo/io/cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,35 +47,35 @@
     cfg_parameters = _add_default_parameters(user_parameters, CFG_MAIN_PARAMETERS)
 
     cfg_parameters["spill_points"] = add_spill_point_default_parameters(
         cfg_parameters["spill_points"]
     )
 
     cfg_parameters["spill_points"] = add_hours_to_release_to_spill_points(
-        cfg_parameters["spill_points"], cfg_parameters["forcing_init_datetime"]
+        cfg_parameters["spill_points"], cfg_parameters["forcings_init_time"]
     )
 
     return cfg_parameters
 
 
 def add_hours_to_release_to_spill_points(
-    spill_points: list[dict], forcing_init_datetime: datetime
+    spill_points: list[dict], forcings_init_time: datetime
 ) -> list[dict]:
     """add parameter 'hours_to_release' as the difference between the 'forcing init time' and the 'release time' of each spill point
 
     Args:
         spill_points (list[dict]): list of spill point definitions
-        forcing_init_datetime (datetime): initial time of the forcings (real initial reference time of TESEO's simulations)
+        forcings_init_time (datetime): initial time of the forcings (real initial reference time of TESEO's simulations)
 
     Returns:
         list[dict]: spill_points updated with 'hours_to_release'
     """
     for i, d in enumerate(spill_points):
         d["hours_to_release"] = (
-            d["release_time"] - forcing_init_datetime
+            d["release_time"] - forcings_init_time
         ).total_seconds() / 3600
         spill_points[i] = d
 
     return spill_points
 
 
 def add_spill_point_default_parameters(
@@ -97,14 +97,15 @@
 
 
 def write_cfg(
     output_path: str,
     filename_parameters: dict[str, str],
     forcing_parameters: dict[str, any],
     simulation_parameters: dict[str, any],
+    df_substances: pd.DataFrame = None,
 ) -> None:
     """write TESEO's cfg-file at the requested path
 
     Args:
         output_path (str): path to write the file
         filename_parameters (dict[str, str]): filenames required
         forcing_parameters (dict[str, any]): forcings parameters required
@@ -119,14 +120,15 @@
     table1, table2, table3 = _create_spill_points_tables(
         simulation_parameters["spill_points"],
         simulation_parameters["substance_type"],
         simulation_parameters["seawater_temperature"],
         simulation_parameters["seawater_density"],
         simulation_parameters["air_temperature"],
         simulation_parameters["suspended_solid_concentration"],
+        df_substances,
     )
 
     cfg_txt = f"""* FICHERO DE CONFIGURACIÓN PARA Modelo TESEO (FUEL-FLOTANTES-HNS, 2D-3D)
 *--------------------------------------------------
 * MALLA:
 *--------------------------------------------------
 * Nombre_malla
@@ -255,14 +257,15 @@
 def _create_spill_points_tables(
     spill_points: list[dict],
     substance_type: str,
     seawater_temperature: float,
     seawater_density: float,
     air_temperature: float,
     suspended_solid_concentration: float,
+    df_substances: pd.DataFrame = None,
 ) -> tuple[str, str, str]:
     """create tables to define spill point related data in cfg-file
 
     Args:
         spill_points (list[dict]): spill point definitions
         substance_type (str): type of the susbtances
         seawater_temperature (float): value for seawater temperature (º)
```

### Comparing `pyteseo-0.0.6/pyteseo/io/coastline.py` & `pyteseo-0.0.7/pyteseo/io/coastline.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,25 +88,27 @@
             polygon_path,
             sep="\t",
             columns=["lon", "lat"],
             header=False,
             index=False,
             float_format="%.8e",
             na_rep="NaN",
+            chunksize=10000,
         )
 
     path = Path(path)
     path.parent.mkdir(parents=True, exist_ok=True)
     teseo_df.to_csv(
         path,
         sep="\t",
         header=False,
         index=False,
         float_format="%.8e",
         na_rep="NaN",
+        chunksize=10000,
     )
 
 
 def coastline_df_to_gdf(df: pd.DataFrame, epsg: str = "4326") -> gpd.GeoDataFrame:
     """convert coastline dataframe[lon,lat,polygon] to geodataframe
 
     Args:
```

### Comparing `pyteseo-0.0.6/pyteseo/io/forcings.py` & `pyteseo-0.0.7/pyteseo/io/forcings.py`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/io/grid.py` & `pyteseo-0.0.7/pyteseo/io/grid.py`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/io/hns_calib.py` & `pyteseo-0.0.7/pyteseo/io/hns_calib.py`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/io/results.py` & `pyteseo-0.0.7/pyteseo/io/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import pandas as pd
 
 from pyteseo.defaults import FILE_NAMES, FILE_PATTERNS, RESULTS_MAP
 
 
 # # 4. RESULTS
-def read_particles_results(
+def read_particles(
     dir_path: str,
     file_pattern: str = FILE_PATTERNS["teseo_particles"],
 ) -> pd.DataFrame:
     """Load TESEO's particles results files "*_properties_*.txt" to DataFrame
 
     Args:
         dir_path (str): path to the results directory
@@ -40,15 +40,15 @@
             for file in files
         ]
 
         df = pd.concat(dfs).reset_index(drop=True)
         return _rename_results_names(df)
 
 
-def read_properties_results(
+def read_properties(
     dir_path: str,
     file_pattern: str = FILE_PATTERNS["teseo_properties"],
 ) -> pd.DataFrame:
     """Load TESEO's propierties results files "*_properties_*.txt" to DataFrame
 
     Args:
         dir_path (str): path to the results directory
@@ -78,20 +78,19 @@
 
             dfs.append(df_)
 
         df = pd.concat(dfs).reset_index(drop=True)
         return _rename_results_names(df)
 
 
-def read_grids_results(
+def read_grids(
     dir_path: str,
     file_pattern: str = FILE_PATTERNS["teseo_grids"],
     fullgrid_filename: str = FILE_NAMES["teseo_grid_coordinates"],
 ) -> pd.DataFrame:
-
     """Load TESEO's grids results files "*_grid_*.txt" to DataFrame
 
     Args:
         dir_path (PosixPath | str):  path to the results directory
         file_pattern (str, optional): file pattern of particles restuls. Defaults to DEF_PATTERNS["teseo_grids"].
         fullgrid_filename (str, optional): filename of results coordinates domain-grid. Defaults to  DEF_FILES["teseo_grid_coordinates"].
```

### Comparing `pyteseo-0.0.6/pyteseo/io/run.py` & `pyteseo-0.0.7/pyteseo/io/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 * ESQUEMA_EULER(1)_RUNGE-KUTTA(2)
 {execution_scheme}
 *
 *--------------------------------------------------
 * RESULTADOS | DERIVADOS[[1]] BORRAR_FICHEROS_FORZAMIENTO[[0]]
 *--------------------------------------------------
 * TIEMPO_PRIMERA_ESCRIT(h) DT_PARTS(s) DT_MALLA(s) DT_PROPRIEDADES(s)
-{round((first_time_saved - run_parameters["forcing_init_datetime"]).total_seconds()/3600, 4)}  {run_parameters["particles_save_dt"].total_seconds()}   {run_parameters["grids_save_dt"].total_seconds()} {run_parameters["properties_save_dt"].total_seconds()}
+{round((first_time_saved - run_parameters["forcings_init_time"]).total_seconds()/3600, 4)}  {run_parameters["particles_save_dt"].total_seconds()}   {run_parameters["grids_save_dt"].total_seconds()} {run_parameters["properties_save_dt"].total_seconds()}
 * GRABAR_RESULTADOS(1:SI,0:NO) _PARTICULAS _MALLA _PROPIEDADES
 {int(run_parameters["save_particles"])}  {int(run_parameters["save_grids"])}   {int(run_parameters["save_properties"])}
 """
 
     with open(path, "w", encoding="utf-8") as f:
         f.write(run_txt)
```

### Comparing `pyteseo-0.0.6/pyteseo/io/substances.py` & `pyteseo-0.0.7/pyteseo/io/substances.py`

 * *Files 24% similar despite different names*

```diff
@@ -53,7 +53,27 @@
     substance_type = substance_type.lower()
     xlsx_path = Path(SUBSTANCES_OFFLINE_PATH, substance_type + ".xlsx")
     if not xlsx_path.exists():
         raise FileNotFoundError(f"{substance_type} not in path ({xlsx_path})")
 
     df = pd.read_excel(xlsx_path)
     return df.name.to_list()
+
+
+def generate_substances_df(json_response: list) -> pd.DataFrame:
+    """convert json substance response from TESEO.Apistore to pd.DataFrame
+
+    Args:
+        json_response (dict): TESEO.apistore json response
+
+    Returns:
+        pd.DataFrame: substances data
+    """
+
+    [
+        substance["data"].update({"name": substance["name"]})
+        for substance in json_response
+    ]
+    dfs = [pd.DataFrame(substance["data"], index=[0]) for substance in json_response]
+    df_substances = pd.concat(dfs).reset_index(drop=True)
+
+    return df_substances
```

### Comparing `pyteseo-0.0.6/pyteseo/io/utils.py` & `pyteseo-0.0.7/pyteseo/io/utils.py`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/plot/animations.py` & `pyteseo-0.0.7/pyteseo/plot/animations.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import matplotlib.animation as animation
 from matplotlib import pyplot as plt
 
 from pyteseo.io.coastline import coastline_df_to_gdf, read_coastline
 from pyteseo.io.forcings import read_forcing
 from pyteseo.io.grid import read_grid
-from pyteseo.io.results import read_particles_results
+from pyteseo.io.results import read_particles
 from pyteseo.plot.basics import (
     _plot_currents_extent,
     _plot_coastline,
     _plot_grid_extent,
     _plot_grid_land_mask,
     _plot_winds_extent,
 )
@@ -23,15 +23,15 @@
         0: {"label": "Particle @ coastline", "marker": ".", "color": "m"},
         1: {"label": "Particle @ water surface", "marker": ".", "color": "b"},
         5: {"label": "Particle @ water column", "marker": ",", "color": "c"},
         -1: {"label": "Particle @ seafloor", "marker": "2", "color": "m"},
         -2: {"label": "Particle outside domain", "marker": "x", "color": "r"},
     }
 
-    df_particles = read_particles_results(results_path)
+    df_particles = read_particles(results_path)
     gdf_coastline = coastline_df_to_gdf(read_coastline(coastline_path))
     df_grid = read_grid(grid_path)
     # df_grid["depth"] = np.where(df_grid["depth"] <= 0, np.nan, df_grid["depth"])
 
     def update(df_group):
         t, df_t = df_group
```

### Comparing `pyteseo-0.0.6/pyteseo/plot/basics.py` & `pyteseo-0.0.7/pyteseo/plot/basics.py`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/plot/figures.py` & `pyteseo-0.0.7/pyteseo/plot/figures.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     currents_path: str,
     winds_path: str,
     waves_path: str,
     ax=None,
     show=True,
 ) -> Figure:
     if not ax:
-        fig, ax = plt.subplots(figsize=(16, 9))
+        fig, ax = plt.subplots()
 
     grid_df = read_grid(grid_path)
     gdf_coastline = coastline_df_to_gdf(read_coastline(coastline_path))
     currents_df = read_forcing(currents_path, "currents")
     winds_df = read_forcing(winds_path, "winds")
     waves_df = read_forcing(waves_path, "waves")
 
@@ -63,24 +63,25 @@
     Args:
         bathymetry_ds (Dataset): xarray DataFrame of the bathymetry.
         coastline_gdf (GeoDataFrame): closed polygons of the coastline.
     """
     grid_df = read_grid(grid_path)
     gdf_coastline = coastline_df_to_gdf(read_coastline(coastline_path))
 
-    fig, ax = plt.subplots(figsize=(16, 9))
-    _plot_grid_extent(grid_df, ax=ax)
+    fig, ax = plt.subplots()
     _scatter_grid_depth(grid_df, ax=ax)
+    # _plot_grid_extent(grid_df, ax=ax)
     _plot_coastline(gdf_coastline, ax=ax)
     if land_mask:
         _plot_grid_land_mask(grid_df, ax=ax)
 
     ax.set_xlabel("Longitude (º)")
     ax.set_ylabel("Latitude (º)")
     ax.set_title("Model domain")
     plt.grid()
     plt.legend()
+    plt.tight_layout()
 
     if show:
         plt.show()
 
     return fig
```

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000000.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000000.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000005.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000005.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000010.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000010.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000015.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000015.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000020.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000020.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000025.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000025.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000030.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000030.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000035.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000035.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000040.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000040.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000045.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000045.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000050.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000050.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000055.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000055.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000060.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000060.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000065.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000065.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000070.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000070.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000075.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000075.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000080.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000080.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000085.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000085.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_001_000090.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_001_000090.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000000.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000000.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000005.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000005.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000010.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000010.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000015.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000015.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000020.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000020.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000025.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000025.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000030.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000030.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000035.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000035.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000040.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000040.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000045.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000045.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000050.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000050.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000055.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000055.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000060.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000060.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000065.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000065.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000070.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000070.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000075.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000075.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000080.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000080.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000085.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000085.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_grid_002_000090.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_grid_002_000090.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000000.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000000.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000005.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000005.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000010.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000010.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000015.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000015.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000020.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000020.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000025.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000025.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000030.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000030.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000035.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000035.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000040.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000040.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000045.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000045.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000050.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000050.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000055.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000055.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000060.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000060.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000065.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000065.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000070.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000070.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000075.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000075.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000080.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000080.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000085.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000085.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_particles_000090.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_particles_000090.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_properties_001.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_properties_001.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/cas1_properties_002.txt` & `pyteseo-0.0.7/pyteseo/tests/data/cas1_properties_002.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/coastline.dat` & `pyteseo-0.0.7/pyteseo/tests/data/coastline.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/coastline_error_range.dat` & `pyteseo-0.0.7/pyteseo/tests/data/coastline_error_range.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/coastline_othernanformat.dat` & `pyteseo-0.0.7/pyteseo/tests/data/coastline_othernanformat.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/costa_poligono1.dat` & `pyteseo-0.0.7/pyteseo/tests/data/costa_poligono1.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/costa_poligono2.dat` & `pyteseo-0.0.7/pyteseo/tests/data/costa_poligono2.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/costa_poligono3.dat` & `pyteseo-0.0.7/pyteseo/tests/data/costa_poligono3.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/costa_poligono4.dat` & `pyteseo-0.0.7/pyteseo/tests/data/costa_poligono4.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/currents.nc` & `pyteseo-0.0.7/pyteseo/tests/data/currents.nc`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/currents_000h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/currents_000h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/currents_001h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/currents_001h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/currents_002h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/currents_002h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/currents_003h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/currents_003h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1.cfg` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1.cfg`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1.run` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1.run`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000060.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_grid_001_000060.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000120.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_grid_001_000120.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000180.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_grid_001_000180.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000240.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_grid_001_000240.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000300.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_grid_001_000300.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000360.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_grid_001_000360.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000420.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_grid_001_000420.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_001_000480.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_grid_001_000480.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_grid_002_000060.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_grid_002_000060.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000060.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000060.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000120.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000120.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000180.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000180.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000240.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000240.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000300.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000300.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000360.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000360.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000420.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000420.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000480.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000480.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000540.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000540.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000600.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000600.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000660.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000660.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000720.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000720.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000780.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000780.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000840.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000840.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_particles_000900.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_particles_000900.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_properties_001.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_properties_001.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/cas1_properties_002.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/cas1_properties_002.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/grid_coordinates.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/grid_coordinates.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa.dat` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono1.dat` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono1.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono2.dat` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono2.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono3.dat` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono3.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono4.dat` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono4.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono6.dat` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono6.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono7.dat` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono7.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/costa_poligono9.dat` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/costa_poligono9.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_000h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_000h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_001h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_001h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_002h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_002h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_003h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_003h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_004h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_004h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_005h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_005h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_006h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_006h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_007h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_007h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_008h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_008h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_009h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_009h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_010h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_010h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_011h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_011h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_012h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_012h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_013h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_013h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_014h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_014h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/currents_015h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/currents_015h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/grid.dat` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/grid.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_000h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_000h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_001h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_001h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_002h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_002h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_003h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_003h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_004h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_004h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_005h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_005h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_006h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_006h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_007h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_007h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_008h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_008h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_009h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_009h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_010h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_010h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_011h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_011h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/input/winds_012h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/input/winds_012h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/grids_001.nc` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/output/grids_001.nc`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/grids_002.nc` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/output/grids_002.nc`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/particles_001.csv` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/output/particles_001.csv`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/particles_001.geojson` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/output/particles_001.geojson`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/particles_002.csv` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/output/particles_002.csv`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/particles_002.geojson` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/output/particles_002.geojson`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/properties_001.csv` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/output/properties_001.csv`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/properties_001.json` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/output/properties_001.json`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/properties_002.csv` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/output/properties_002.csv`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/drift_simulation/output/properties_002.json` & `pyteseo-0.0.7/pyteseo/tests/data/drift_simulation/output/properties_002.json`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/grid.dat` & `pyteseo-0.0.7/pyteseo/tests/data/grid.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/grid_coordinates.txt` & `pyteseo-0.0.7/pyteseo/tests/data/grid_coordinates.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/grid_error_var.dat` & `pyteseo-0.0.7/pyteseo/tests/data/grid_error_var.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1.cfg` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1.cfg`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1.run` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1.run`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_grid_001_000120.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_grid_001_000120.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_grid_001_000180.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_grid_001_000180.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_grid_002_000120.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_grid_002_000120.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000060.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000060.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000120.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000120.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000180.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000180.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000240.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000240.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000300.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000300.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000360.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000360.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000420.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000420.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000480.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000480.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000540.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000540.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_particles_000600.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_particles_000600.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_properties_001.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_properties_001.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/cas1_properties_002.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/cas1_properties_002.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/grid_coordinates.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/grid_coordinates.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/cas1_HNS.calib` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/cas1_HNS.calib`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa.dat` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono1.dat` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono1.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono2.dat` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono2.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono3.dat` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono3.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono4.dat` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono4.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono6.dat` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono6.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono7.dat` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono7.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/costa_poligono9.dat` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/costa_poligono9.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_000h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_000h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_001h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_001h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_002h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_002h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_003h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_003h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_004h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_004h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_005h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_005h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_006h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_006h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_007h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_007h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_008h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_008h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_009h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_009h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/currents_010h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/currents_010h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/grid.dat` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/grid.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_000h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_000h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_001h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_001h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_002h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_002h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_003h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_003h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_004h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_004h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_005h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_005h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_006h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_006h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_007h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_007h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_008h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_008h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_009h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_009h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/input/winds_010h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/input/winds_010h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/grids_001.nc` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/output/grids_001.nc`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/grids_002.nc` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/output/grids_002.nc`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/particles_001.csv` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/output/particles_001.csv`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/particles_001.geojson` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/output/particles_001.geojson`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/particles_002.csv` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/output/particles_002.csv`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/particles_002.geojson` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/output/particles_002.geojson`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/properties_001.csv` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/output/properties_001.csv`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/properties_001.json` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/output/properties_001.json`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/properties_002.csv` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/output/properties_002.csv`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/hns_simulation/output/properties_002.json` & `pyteseo-0.0.7/pyteseo/tests/data/hns_simulation/output/properties_002.json`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa.dat` & `pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono1.dat` & `pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono1.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono2.dat` & `pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono2.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono3.dat` & `pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono3.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono4.dat` & `pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono4.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono6.dat` & `pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono6.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono7.dat` & `pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono7.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/costa_poligono9.dat` & `pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/costa_poligono9.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/ibiza_domain/grid.dat` & `pyteseo-0.0.7/pyteseo/tests/data/ibiza_domain/grid.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1.cfg` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1.cfg`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1.run` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1.run`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_grid_001_000120.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_grid_001_000120.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_grid_001_000180.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_grid_001_000180.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000060.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000060.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000120.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000120.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000180.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000180.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000240.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000240.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000300.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000300.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000360.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000360.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000420.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000420.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000480.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000480.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000540.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000540.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_particles_000600.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_particles_000600.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_properties_001.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_properties_001.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/cas1_properties_002.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/cas1_properties_002.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/grid_coordinates.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/grid_coordinates.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa.dat` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono1.dat` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono1.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono2.dat` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono2.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono3.dat` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono3.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono4.dat` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono4.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono6.dat` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono6.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono7.dat` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono7.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/costa_poligono9.dat` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/costa_poligono9.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_000h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_000h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_001h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_001h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_002h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_002h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_003h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_003h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_004h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_004h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_005h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_005h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_006h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_006h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_007h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_007h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_008h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_008h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_009h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_009h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/currents_010h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/currents_010h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/grid.dat` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/grid.dat`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_000h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_000h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_001h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_001h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_002h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_002h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_003h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_003h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_004h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_004h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_005h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_005h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_006h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_006h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_007h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_007h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_008h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_008h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_009h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_009h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/input/winds_010h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/input/winds_010h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/grids_001.nc` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/output/grids_001.nc`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/grids_002.nc` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/output/grids_002.nc`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/particles_001.csv` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/output/particles_001.csv`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/particles_001.geojson` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/output/particles_001.geojson`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/particles_002.csv` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/output/particles_002.csv`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/particles_002.geojson` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/output/particles_002.geojson`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/properties_001.csv` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/output/properties_001.csv`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/properties_001.json` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/output/properties_001.json`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/properties_002.csv` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/output/properties_002.csv`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/oil_simulation/output/properties_002.json` & `pyteseo-0.0.7/pyteseo/tests/data/oil_simulation/output/properties_002.json`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/shapefile_cantabria/Cantabria.shp` & `pyteseo-0.0.7/pyteseo/tests/data/shapefile_cantabria/Cantabria.shp`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/shapefile_cantabria/Cantabria.shp.xml` & `pyteseo-0.0.7/pyteseo/tests/data/shapefile_cantabria/Cantabria.shp.xml`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/waves_003h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/waves_003h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/winds.nc` & `pyteseo-0.0.7/pyteseo/tests/data/winds.nc`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/winds_000h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/winds_000h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/winds_001h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/winds_001h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/winds_002h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/winds_002h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/data/winds_003h.txt` & `pyteseo-0.0.7/pyteseo/tests/data/winds_003h.txt`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/integration/test_simulation_cte_forcing.py` & `pyteseo-0.0.7/pyteseo/tests/integration/test_simulation_cte_forcing.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,14 @@
         tmp_path.mkdir()
     yield
     if tmp_path.exists():
         rmtree(tmp_path)
 
 
 def test_drifter_cte_forcings_without_coastline(setup_teardown):
-
     input_files = [
         "grid.dat",
         "lstcurr_UVW_cte.pre",
         "lstwinds_cte.pre",
         "lstwaves_cte.pre",
     ]
     input_files_dst = [
@@ -51,15 +50,15 @@
     job.load_domain(job.input_dir)
     job.load_forcings()
 
     parameters = {
         "mode": "2d",
         "motion": "forward",
         "substance_type": "drifter",
-        "forcing_init_datetime": datetime(2023, 1, 1, 0, 0, 0),
+        "forcings_init_time": datetime(2023, 1, 1, 0, 0, 0),
         "duration": timedelta(hours=3),
         "timestep": timedelta(minutes=1),
         "use_coastline": False,
         "spill_points": [
             {
                 "release_time": datetime(2023, 1, 1, 0, 0, 0) + timedelta(minutes=32),
                 "lon": -3.8,
@@ -90,15 +89,14 @@
     )
     assert len([str(path) for path in list(Path(job.output_dir).glob("*.csv"))]) > 0
     assert len([str(path) for path in list(Path(job.output_dir).glob("*.json"))]) > 0
     assert len([str(path) for path in list(Path(job.output_dir).glob("*.nc"))]) > 0
 
 
 def test_drifter_cte_forcings_with_coastline(setup_teardown):
-
     input_files = [
         "grid.dat",
         "coastline.dat",
         "costa_poligono1.dat",
         "costa_poligono2.dat",
         "costa_poligono3.dat",
         "costa_poligono4.dat",
@@ -127,15 +125,15 @@
     job.load_domain(job.input_dir)
     job.load_forcings()
 
     parameters = {
         "mode": "2d",
         "motion": "forward",
         "substance_type": "drifter",
-        "forcing_init_datetime": datetime(2023, 1, 1, 0, 0, 0),
+        "forcings_init_time": datetime(2023, 1, 1, 0, 0, 0),
         "duration": timedelta(hours=3),
         "timestep": timedelta(minutes=1),
         "spill_points": [
             {
                 "release_time": datetime(2023, 1, 1, 0, 0, 0) + timedelta(minutes=32),
                 "lon": -3.8,
                 "lat": 43.44,
@@ -160,15 +158,14 @@
     assert len([str(path) for path in list(Path(job.path).glob("*_grid_*.txt"))]) > 0
     assert (
         len([str(path) for path in list(Path(job.path).glob("*_properties_*.txt"))]) > 0
     )
 
 
 def test_oil_cte_forcings_with_coastline(setup_teardown):
-
     input_files = [
         "grid.dat",
         "coastline.dat",
         "costa_poligono1.dat",
         "costa_poligono2.dat",
         "costa_poligono3.dat",
         "costa_poligono4.dat",
@@ -197,15 +194,15 @@
     job.load_domain(job.input_dir)
     job.load_forcings()
 
     parameters = {
         "mode": "2d",
         "motion": "forward",
         "substance_type": "oil",
-        "forcing_init_datetime": datetime(2023, 1, 1, 0, 0, 0),
+        "forcings_init_time": datetime(2023, 1, 1, 0, 0, 0),
         "duration": timedelta(hours=3),
         "timestep": timedelta(minutes=1),
         "spill_points": [
             {
                 "release_time": datetime(2023, 1, 1, 0, 0, 0) + timedelta(minutes=32),
                 "lon": -3.8,
                 "lat": 43.44,
@@ -236,15 +233,14 @@
     assert len([str(path) for path in list(Path(job.path).glob("*_grid_*.txt"))]) > 0
     assert (
         len([str(path) for path in list(Path(job.path).glob("*_properties_*.txt"))]) > 0
     )
 
 
 def test_hns_cte_forcings_with_coastline(setup_teardown):
-
     input_files = [
         "grid.dat",
         "coastline.dat",
         "costa_poligono1.dat",
         "costa_poligono2.dat",
         "costa_poligono3.dat",
         "costa_poligono4.dat",
@@ -273,15 +269,15 @@
     job.load_domain(job.input_dir)
     job.load_forcings()
 
     parameters = {
         "mode": "2d",
         "motion": "forward",
         "substance_type": "hns",
-        "forcing_init_datetime": datetime(2023, 1, 1, 0, 0, 0),
+        "forcings_init_time": datetime(2023, 1, 1, 0, 0, 0),
         "duration": timedelta(hours=3),
         "timestep": timedelta(minutes=1),
         "spill_points": [
             {
                 "release_time": datetime(2023, 1, 1, 0, 0, 0) + timedelta(minutes=32),
                 "lon": -3.8,
                 "lat": 43.44,
```

### Comparing `pyteseo-0.0.6/pyteseo/tests/unit/test_cfg.py` & `pyteseo-0.0.7/pyteseo/tests/unit/test_cfg.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 @pytest.mark.parametrize(
     "user_parameters",
     [
         (
             {
-                "forcing_init_datetime": datetime.utcnow().replace(
+                "forcings_init_time": datetime.utcnow().replace(
                     minute=0, second=0, microsecond=0
                 ),
                 "duration": timedelta(hours=12),
                 "spill_points": [
                     {
                         "release_time": datetime.utcnow().replace(
                             second=0, microsecond=0
@@ -47,15 +47,15 @@
                     },
                 ],
             }
         ),
         (
             {
                 "substance_type": "drifter",
-                "forcing_init_datetime": datetime.utcnow().replace(
+                "forcings_init_time": datetime.utcnow().replace(
                     minute=0, second=0, microsecond=0
                 ),
                 "duration": timedelta(hours=12),
                 "spill_points": [
                     {
                         "release_time": datetime.utcnow().replace(
                             second=0, microsecond=0
@@ -66,15 +66,15 @@
                     },
                 ],
             }
         ),
         (
             {
                 "substance_type": "drifter",
-                "forcing_init_datetime": datetime.utcnow().replace(
+                "forcings_init_time": datetime.utcnow().replace(
                     minute=0, second=0, microsecond=0
                 ),
                 "duration": timedelta(hours=12),
                 "spill_point": [
                     {
                         "release_time": datetime.utcnow().replace(
                             second=0, microsecond=0
@@ -86,15 +86,15 @@
                     },
                 ],
             }
         ),
         (
             {
                 "substance_type": "drifter",
-                "forcing_init_datetime": datetime.utcnow().replace(
+                "forcings_init_time": datetime.utcnow().replace(
                     minute=0, second=0, microsecond=0
                 ),
                 "spill_points": [
                     {
                         "release_time": datetime.utcnow().replace(
                             second=0, microsecond=0
                         ),
```

### Comparing `pyteseo-0.0.6/pyteseo/tests/unit/test_clasess.py` & `pyteseo-0.0.7/pyteseo/tests/unit/test_clasess.py`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/unit/test_export.py` & `pyteseo-0.0.7/pyteseo/tests/unit/test_export.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 import pytest
 
 from pyteseo.__init__ import __version__ as v
 from pyteseo.export.grids import export_grids
 from pyteseo.export.particles import export_particles
 from pyteseo.export.properties import export_properties
 from pyteseo.io.results import (
-    read_grids_results,
-    read_particles_results,
-    read_properties_results,
+    read_grids,
+    read_particles,
+    read_properties,
 )
 
 # data_path = Path(__file__).parent.parent / "data"
 # data_path = Path(__file__).parent.parent / "data/drift_simulation"
 data_path = Path(__file__).parent.parent / "data/oil_simulation"
 # data_path = Path(__file__).parent.parent / "data/hns_simulation"
 tmp_path = Path(f"./tmp_pyteseo_{v}_tests")
@@ -35,34 +35,34 @@
         ("csv", tmp_path, None),
         ("json", tmp_path, None),
         ("geojson", tmp_path, None),
         ("netcdf", tmp_path, "bad_format"),
     ],
 )
 def test_export_particles(file_format, output_dir, error, setup_teardown):
-    df = read_particles_results(data_path)
+    df = read_particles(data_path)
 
     if error == "bad_format":
         with pytest.raises(ValueError):
             export_particles(df, file_format, output_dir)
     else:
         files = export_particles(df, file_format, output_dir)
         assert all([file.exists() for file in files])
 
 
 @pytest.mark.parametrize(
     "file_format, output_dir, error",
     [
         ("csv", tmp_path, None),
         ("json", tmp_path, None),
-        ("netcdf", tmp_path, "bad_format"),
+        ("nc", tmp_path, "bad_format"),
     ],
 )
 def test_export_properties(file_format, output_dir, error, setup_teardown):
-    df = read_properties_results(data_path)
+    df = read_properties(data_path)
 
     if error == "bad_format":
         with pytest.raises(ValueError):
             export_properties(df, file_format, output_dir)
     elif error == "not_implemented":
         with pytest.raises(NotImplementedError):
             export_properties(df, file_format, output_dir)
@@ -72,20 +72,21 @@
 
 
 @pytest.mark.parametrize(
     "file_format, output_dir, error",
     [
         ("csv", tmp_path, None),
         ("json", tmp_path, None),
+        ("netcdf", tmp_path, "None"),
         ("nc", tmp_path, "None"),
         ("geojson", tmp_path, "bad_format"),
     ],
 )
 def test_export_grids(file_format, output_dir, error, setup_teardown):
-    df = read_grids_results(data_path)
+    df = read_grids(data_path)
 
     if error == "bad_format":
         with pytest.raises(ValueError):
             export_grids(df, file_format, output_dir)
     elif error == "not_implemented":
         with pytest.raises(NotImplementedError):
             export_grids(df, file_format, output_dir)
```

### Comparing `pyteseo-0.0.6/pyteseo/tests/unit/test_io_coastline.py` & `pyteseo-0.0.7/pyteseo/tests/unit/test_io_coastline.py`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/unit/test_io_forcings.py` & `pyteseo-0.0.7/pyteseo/tests/unit/test_io_forcings.py`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/unit/test_io_grid.py` & `pyteseo-0.0.7/pyteseo/tests/unit/test_io_grid.py`

 * *Files identical despite different names*

### Comparing `pyteseo-0.0.6/pyteseo/tests/unit/test_io_results.py` & `pyteseo-0.0.7/pyteseo/tests/unit/test_io_results.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from shutil import rmtree
 
 import pandas as pd
 import pytest
 
 from pyteseo.__init__ import __version__ as v
 from pyteseo.io.results import (
-    read_grids_results,
-    read_particles_results,
-    read_properties_results,
+    read_grids,
+    read_particles,
+    read_properties,
 )
 
 # data_path = Path(__file__).parent.parent / "data"
 # data_path = Path(__file__).parent.parent / "data/drift_simulation"
 # data_path = Path(__file__).parent.parent / "data/oil_simulation"
 data_path = Path(__file__).parent.parent / "data/hns_simulation"
 tmp_path = Path(f"./tmp_pyteseo_{v}_tests")
@@ -25,34 +25,33 @@
     yield
     if tmp_path.exists():
         rmtree(tmp_path)
 
 
 @pytest.mark.parametrize("error", [(None), ("no_match")])
 def test_read_particles_results(error):
-
     if error == "no_match":
         with pytest.raises(FileNotFoundError):
-            df = read_particles_results(dir_path="data_path")
+            df = read_particles(dir_path="data_path")
 
-    df = read_particles_results(dir_path=data_path)
+    df = read_particles(dir_path=data_path)
     assert isinstance(df, pd.DataFrame)
 
 
 @pytest.mark.parametrize("error", [(None), ("no_match")])
 def test_read_properties_results(error):
     if error == "no_match":
         with pytest.raises(FileNotFoundError):
-            df = read_properties_results(dir_path="data_path")
+            df = read_properties(dir_path="data_path")
 
-    df = read_properties_results(dir_path=data_path)
+    df = read_properties(dir_path=data_path)
     assert isinstance(df, pd.DataFrame)
 
 
 @pytest.mark.parametrize("error", [(None), ("no_match")])
 def test_read_grids_results(error):
     if error == "no_match":
         with pytest.raises(FileNotFoundError):
-            df = read_grids_results(dir_path="data_path")
+            df = read_grids(dir_path="data_path")
 
-    df = read_grids_results(dir_path=data_path)
+    df = read_grids(dir_path=data_path)
     assert isinstance(df, pd.DataFrame)
```

### Comparing `pyteseo-0.0.6/pyteseo/tests/unit/test_plot.py` & `pyteseo-0.0.7/pyteseo/tests/unit/test_plot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from shutil import rmtree
 
 import pytest
 
 # from matplotlib import pyplot as plt
 
-from pyteseo.io.results import read_properties_results
+from pyteseo.io.results import read_properties
 from pyteseo.plot.animations import animate_forcings, animate_particles
 from pyteseo.plot.basics import _plot_properties
 from pyteseo.plot.figures import plot_domain, plot_extents
 
 # Domain
 coastline_path = "pyteseo/tests/data/ibiza_domain/costa.dat"
 grid_path = "pyteseo/tests/data/ibiza_domain/grid.dat"
@@ -18,15 +18,15 @@
 currents_lst_path = "pyteseo/tests/data/hns_simulation/input/lstcurr_UVW.pre"
 winds_lst_path = "pyteseo/tests/data/hns_simulation/input/lstwinds.pre"
 waves_lst_path = "pyteseo/tests/data/hns_simulation/input/lstwaves.pre"
 
 # TESEO results
 results_path = "pyteseo/tests/data/hns_simulation"
 
-properties_df = read_properties_results(results_path)
+properties_df = read_properties(results_path)
 
 tmp_path = Path("tests_plots")
 
 
 @pytest.fixture
 def setup_teardown():
     if not tmp_path.exists():
@@ -73,7 +73,8 @@
         winds_lst_path,
         coastline_path,
         grid_path,
         scale=15,
         show=False,
         gif_path=Path(tmp_path, "forcings.gif"),
     )
+    assert True
```

### Comparing `pyteseo-0.0.6/pyteseo/wrapper.py` & `pyteseo-0.0.7/pyteseo/wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+"""Main module where the main class to centralice simulation management is declared"""
+
 from __future__ import annotations
 
 import os
 import subprocess
 from pathlib import Path
 from shutil import copy2
 
+import pandas as pd
 
 from pyteseo.classes import Coastline, Currents, Grid, Waves, Winds
 from pyteseo.defaults import (
     CFG_MAIN_MANDATORY_KEYS,
     CFG_SPILL_POINT_MANDATORY_KEYS,
     DIRECTORY_NAMES,
     FILE_NAMES,
@@ -17,21 +20,20 @@
 from pyteseo.export.grids import export_grids
 from pyteseo.export.particles import export_particles
 from pyteseo.export.properties import export_properties
 from pyteseo.io.cfg import generate_parameters_for_cfg, write_cfg
 from pyteseo.io.forcings import write_null_forcing
 from pyteseo.io.hns_calib import write_hns_calib
 from pyteseo.io.results import (
-    read_grids_results,
-    read_particles_results,
-    read_properties_results,
+    read_grids,
+    read_particles,
+    read_properties,
 )
 from pyteseo.io.run import generate_parameters_for_run, write_run
 
-
 TESEO_PATH = os.environ.get("TESEO_PATH")
 
 
 class TeseoWrapper:
     def __init__(self, dir_path: str, simulation_keyword: str = "cas1"):
         """wrapper of configuration, execution and postprocess of a TESEO's simulation
 
@@ -52,25 +54,25 @@
         particles_file_formats=["geojson", "csv"],
         properties_file_formats=["json", "csv"],
         grids_file_formats=["nc"],
     ):
         print("\nPostprocessing results...\n")
         for k, v in {
             "particles": {
-                "read": read_particles_results,
+                "read": read_particles,
                 "export": export_particles,
                 "file_formats": particles_file_formats,
             },
             "properties": {
-                "read": read_properties_results,
+                "read": read_properties,
                 "export": export_properties,
                 "file_formats": properties_file_formats,
             },
             "grids": {
-                "read": read_grids_results,
+                "read": read_grids,
                 "export": export_grids,
                 "file_formats": grids_file_formats,
             },
         }.items():
             print(f"reading {k}...")
             df = v["read"](self.path)
 
@@ -164,70 +166,98 @@
         else:
             print("No waves defined, creating null waves...")
             write_null_forcing(input_dir, forcing_type="waves")
             self.waves = Waves(Path(input_dir, FILE_NAMES["waves"]), waves_dt_cte)
 
         print("DONE!\n")
 
-    def setup(self, user_parameters: dict[str, any]):
+    def setup(
+        self, user_parameters: dict[str, any], df_substances: pd.Dataframe = None
+    ):
         """create TESEO's configuration files (cfg and run)
 
         Args:
             user_parameters (dict[str, any]): parameters definde by the user to configure the simulation
         """
         check_user_minimum_parameters(user_parameters)
         print("Setting up TESEO's cfg-file...")
-        cfg_parameters = generate_parameters_for_cfg(user_parameters)
+        self._cfg_parameters = generate_parameters_for_cfg(user_parameters)
         forcing_parameters = self._forcing_parameters
         file_parameters = self._file_parameters
 
         self.cfg_path = str(
             Path(self.path, FILE_PATTERNS["cfg"].replace("*", self.simulation_keyword))
         )
         write_cfg(
             output_path=self.cfg_path,
             filename_parameters=file_parameters,
             forcing_parameters=forcing_parameters,
-            simulation_parameters=cfg_parameters,
+            simulation_parameters=self._cfg_parameters,
+            df_substances=df_substances,
         )
         print("cfg-file created\n")
         print("Setting up TESEO's cfg-file...")
-        if "first_time_saved" not in user_parameters.keys():
-            first_time_saved = min(
-                [
-                    spill_point["release_time"]
-                    for spill_point in cfg_parameters["spill_points"]
-                ]
-            )
-        else:
-            first_time_saved = user_parameters["first_time_saved"]
 
-        run_parameters = generate_parameters_for_run(user_parameters)
+        user_parameters["first_time_saved"] = user_parameters["forcings_init_time"]
+
+        # FIXME - Problematic to use initial release datetime as initial of the savings. force to be multiple to dt is complex
+        # if "first_time_saved" not in user_parameters.keys():
+        #     user_parameters["first_time_saved"] = min(
+        #         [
+        #             spill_point["release_time"]
+        #             for spill_point in self._cfg_parameters["spill_points"]
+        #         ]
+        #     )
+
+        self._run_parameters = generate_parameters_for_run(user_parameters)
         if "coastline" in dir(self):
             n_coastal_polygons = self.coastline.n_polygons
         else:
             n_coastal_polygons = 0
         self.run_path = str(
             Path(self.path, FILE_PATTERNS["run"].replace("*", self.simulation_keyword))
         )
         write_run(
             path=self.run_path,
-            run_parameters=run_parameters,
-            first_time_saved=first_time_saved,
+            run_parameters=self._run_parameters,
+            first_time_saved=user_parameters["first_time_saved"],
             n_coastal_polygons=n_coastal_polygons,
         )
         print("run-file created\n")
 
         if user_parameters["substance_type"] == "hns":
             print("Setting up TESEO's hns calibration-file")
             write_hns_calib(
                 dir_path=self.input_dir, simulation_keyword=self.simulation_keyword
             )
             print("hns calibration-file created\n")
-        print("DONE!")
+        self._user_parameters = user_parameters
+        self.print_summary()
+
+    def print_summary(self):
+        print(
+            f"""
+            --------------- SIMULATION SUMMARY ---------------
+            Simulation init:        {min([spill_point["release_time"] for spill_point in self._user_parameters["spill_points"]]).isoformat()}
+            Forcing initial time:   {self._cfg_parameters['forcings_init_time'].isoformat()}
+            Spills' release times:  {[sp['release_time'].isoformat() for sp in self._cfg_parameters["spill_points"]]}
+            First time saved:       {self._run_parameters["first_time_saved"].isoformat()}
+             - - - - - - - - - - - - - - - - - - - - - - - - -
+            particles save dt:      {int(self._cfg_parameters["particles_save_dt"].total_seconds()/60)} minutes
+            properties save dt:     {int(self._cfg_parameters["properties_save_dt"].total_seconds()/60)} minutes
+            grids save dt:          {int(self._cfg_parameters["grids_save_dt"].total_seconds()/60)} minutes
+            simulation dt:          {int(self._cfg_parameters["timestep"].total_seconds()/60)} minutes
+             - - - - - - - - - - - - - - - - - - - - - - - - -
+             simulation mode:       {self._cfg_parameters["mode"]}
+             motion:                {self._cfg_parameters["motion"]}
+             release type:          {self._cfg_parameters["release_type"]}
+             n_particles:           {int(self._run_parameters["n_particles"])} particles
+            ---------------------------------------------------\n
+            """
+        )
 
     def run(self):
         """run TESEO simulation"""
         self.check_files()
         if not TESEO_PATH:
             raise NameError("TESEO_PATH environment variable is not defined")
         self.prepare_teseo_binary(TESEO_PATH)
@@ -315,23 +345,23 @@
             old_path.rename(new_path)
             del hotfix_02
             self.currents_depthavg_path = str(new_path)
         # ------------------------------------------------------------------------
 
     @property
     def load_particles(self):
-        read_particles_results(self.path)
+        read_particles(self.path)
 
     @property
     def load_properties(self):
-        read_properties_results(self.path)
+        read_properties(self.path)
 
     @property
     def load_grids(self):
-        read_grids_results(self.path)
+        read_grids(self.path)
 
     @property
     def _file_parameters(self) -> dict:
         d = {}
         d["inputs_directory"] = DIRECTORY_NAMES["input"] + "/"
         d["grid_filename"] = Path(self.grid.path).name
         return d
```

### Comparing `pyteseo-0.0.6/PKG-INFO` & `pyteseo-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: pyteseo
-Version: 0.0.6
-Summary: Python package developed to simplify and facilitate the setup and processing of TESEO simulations (https://ihcantabria.com/en/specialized-software/teseo/)
+Version: 0.0.7
+Summary: Python package developed to simplify and facilitate the setup and postprocessing of TESEO(v1.2.8) simulations (https://ihcantabria.com/en/specialized-software/teseo/)
 Author-email: German Aragon Caminero <german.aragon@unican.es>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: geopandas
 Requires-Dist: owslib
 Requires-Dist: xarray
 Requires-Dist: dask
-Requires-Dist: netcdf4<=1.5.8
+Requires-Dist: netcdf4
 Requires-Dist: bottleneck
 Requires-Dist: ipykernel
 Requires-Dist: matplotlib
 Requires-Dist: geojson
 Requires-Dist: pytest >=7
 Requires-Dist: lxml
 Requires-Dist: scipy
@@ -64,77 +65,83 @@
 
 
 **pyTESEO** is a python package developed by [IHCantabria](https://ihcantabria.com/en/) to simplify and facilitate the setup and processing of [TESEO](https://ihcantabria.com/en/specialized-software/teseo/) simulations *(TESEO is a lagrangian numerical model also developed by IHCantabria.)*
 
 
 ---
 
-## :computer: Installation
+## 💻 Installation
 
-1 - Install the python library using pip:
+1. Install pyTESEO library:
 
-```bash
-# From pypi repository
-pip install pyteseo
-
-# Or directly from github repository
-pip install git+https://github.com/IHCantabria/pyteseo
-```
-
-2 - Install TESEO model binary (**Not available yet!**):
-- Get access to the binary: https://github.com/IHCantabria/TESEO/blob/main/bin
-- Set up environment variable "TESEO_PATH" with the path to the model executable. You can use the command following CLI command after activate the python environement (python-dotenv library)
+    [Pip package manager](https://pip.pypa.io/en/stable/) is needed to install the library and
+    it is recommended to be installed from [IHCantabria/pyteseo](https://github.com/IHCantabria/    pyteseo) repository:
+    ```bash
+    pip install git+https://github.com/IHCantabria/pyteseo
+    ```
 
+    *Alternatively, you can install it from pypi but you will need also install some direct dependencies     that are not publish in pipy repositories:*
     ```bash
-        dotenv set TESEO_PATH /path/to/teseo_executable
+    pip install pyteseo
+
+    # direct dependencies:
+    pip install "datahub @ https://github.com/IHCantabria/datahub.client/archive/refs/tags/v0.9.4.zip"
     ```
-3 - Opendap connection to some [CMEMS products](https://data.marine.copernicus.eu/products) is available at the library `pyteseo/connections/cmems.py` but needs authetication through the following environement variables:
-```bash
-dotenv set CMEMS_username your_username_at_CMEMS
-```
-```bash
-dotenv set CMEMS_password your_password_at_CMEMS
-```
+
+2. Install TESEO model binary (**Not available yet!**):
+
+    - Get access to the binary @ (https://github.com/IHCantabria/TESEO/blob/main/bin)
+    - Set up environment variable "TESEO_PATH" with the path to the model executable. You can use the   command following CLI command after activate the python environement (python-dotenv library)
+
+        ```bash
+            dotenv set TESEO_PATH /path/to/teseo_executable
+        ```
+
+3. Online data providers require to stablish opendap connections, and in some cases aditional configurations:
+
+    * [CMEMS products](https://data.marine.copernicus.eu/products) requires authentication. You should set up the environment variables `CMEMS_username` and `CMEMS_password`.
+        ```bash
+        dotenv set CMEMS_username your_username_at_CMEMS
+        ```
+        ```bash
+        dotenv set CMEMS_password your_password_at_CMEMS
+        ```
+
+    * [IHCantabria products](https://discoverymap.ihcantabria.com/) requires connection to IHCantabria datahub API. You should set up the environment variable `DATAHUB_API_URL`.
+        ```bash
+        DATAHUB_API_URL = "https://datahub.ihcantabria.com"
+        ```
 
 ---
 
-## :heavy_check_mark: Tests
+## ✔️ Tests
 Tests are located in `pyteseo/tests/` and data required for tests are located in `pyteseo/tests/data/`.
 Tests have been developed using [pytest](https://docs.pytest.org/).
 
 Run tests to verify your package installation:
 ```bash
 pyteseo-test        # Run tests and prompt pytest-report
 ```
 
-If you have cloned the repository, you also can run `coverage.py` functionalities based on current `pytproyect.toml` configuration from your terminal command line interface:
-```bash
-# Commands should be executed from the root directory of the repo
-
-coverage run        # For run tests and generate ".coverage" file
-coverage report     # For prompt results from ".coverage" file
-coverage html       # For generate html report on "htmlcov" folder
-```
-
 ---
 
-## :recycle: Continuous integration (CI)
+## ♻️ Continuous integration (CI)
 
 * Build and deploy documentation on Github Pages in [.github/workflows/docs.yml](.github/workflows/docs.yml)
 * Install and test package in diferent environments in [.github/workflows/tests.yml](.github/workflows/tests.yml)
 * Precommit hooks for formats and linting in [.pre-commit-config.yaml](.pre-commit-config.yaml)
 
 *For Linux, Windows, MacOS and compatible python versions defined in installation section*
 
 ---
 
-## :books: Documentation
+## 📚 Documentation
 
 Documentation is available at https://ihcantabria.github.io/pyteseo
 
 ---
 
-## :copyright: Credits
-Developed and maintained by :man_technologist: [German Aragon](https://github.com/aragong) @ :office: [IHCantabria](https://github.com/IHCantabria).
+## ©️ Credits
+Developed and maintained by 👨‍💻 [German Aragon](https://github.com/aragong) @ 🏢 [IHCantabria](https://github.com/IHCantabria).
 
 ---
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

