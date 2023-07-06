# Comparing `tmp/c4p-2023.7.1.23.tar.gz` & `tmp/c4p-2023.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4p-2023.7.1.23.tar", last modified: Sun Jul  2 05:23:07 2023, max compression
+gzip compressed data, was "c4p-2023.7.6.tar", last modified: Thu Jul  6 12:20:11 2023, max compression
```

## Comparing `c4p-2023.7.1.23.tar` & `c4p-2023.7.6.tar`

### file list

```diff
@@ -1,53 +1,59 @@
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-02 05:23:07.586722 c4p-2023.7.1.23/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1065 2023-05-22 19:27:41.000000 c4p-2023.7.1.23/LICENSE
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       27 2023-07-02 05:18:20.000000 c4p-2023.7.1.23/MANIFEST.in
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      544 2023-07-02 05:23:07.586281 c4p-2023.7.1.23/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       94 2023-07-02 04:04:59.000000 c4p-2023.7.1.23/README.md
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-02 05:23:07.557286 c4p-2023.7.1.23/c4p/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      240 2023-06-01 04:08:45.000000 c4p-2023.7.1.23/c4p/__init__.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1074 2023-07-02 04:08:18.000000 c4p-2023.7.1.23/c4p/case.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7947 2023-07-02 04:54:01.000000 c4p-2023.7.1.23/c4p/runoff.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-02 05:23:07.552427 c4p-2023.7.1.23/c4p/src/
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-02 05:23:07.577201 c4p-2023.7.1.23/c4p/src/rof/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      885 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/Makefile
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    11024 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/check_inf_loop.F90
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2633 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/create-topo_0.5x0.5deg.ncl
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1861 2023-07-02 02:20:03.000000 c4p-2023.7.1.23/c4p/src/rof/create-topo_1x1deg.ncl
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1700 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/create-topo_2x2deg.ncl
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    12241 2023-07-02 04:22:06.000000 c4p-2023.7.1.23/c4p/src/rof/create_ESMF_map.sh
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     5321 2023-07-02 02:42:46.000000 c4p-2023.7.1.23/c4p/src/rof/plot_rdirc.ncl
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1613 2023-07-02 02:44:45.000000 c4p-2023.7.1.23/c4p/src/rof/plotrdirc.csh
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3122 2023-07-02 02:45:04.000000 c4p-2023.7.1.23/c4p/src/rof/rdirc_template.csh
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2620 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/rtm_ncdf.pro
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      543 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/runoff_map.1x1.template.nml
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)  7760296 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/runoff_map_0.5deg
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)  7760360 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/runoff_map_1deg
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-02 05:23:07.577756 c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      580 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/build.cheyenne.csh
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-02 05:23:07.585172 c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      725 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/Macros.cheyenne
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     6226 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/Makefile
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    14995 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/fixroff_mod.F90
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1094 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/kind_mod.F90
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     9525 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/main.F90
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    94808 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/map_mod.F90
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    94853 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/map_mod_0.5deg.F90.save
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    94808 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/map_mod_1deg.F90.save
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    36063 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/mapsort_mod.F90
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1242 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/shr_kind_mod.F90
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    12114 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/shr_sys_mod.F90
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    14025 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/shr_timer_mod.F90
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    60912 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/smooth_mod.F90
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-02 05:23:07.585724 c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/tools/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    12359 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/tools/makdep.c
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    22122 2023-07-02 02:10:44.000000 c4p-2023.7.1.23/c4p/src/rof/topo2rdirc_sed.F90
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1718 2023-07-02 02:31:49.000000 c4p-2023.7.1.23/c4p/utils.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-02 05:23:07.560139 c4p-2023.7.1.23/c4p.egg-info/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      544 2023-07-02 05:23:07.558092 c4p-2023.7.1.23/c4p.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1440 2023-07-02 05:23:07.558518 c4p-2023.7.1.23/c4p.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-07-02 05:23:07.558930 c4p-2023.7.1.23/c4p.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-06-01 04:07:36.000000 c4p-2023.7.1.23/c4p.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       47 2023-07-02 05:23:07.559826 c4p-2023.7.1.23/c4p.egg-info/requires.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2023-07-02 05:23:07.560235 c4p-2023.7.1.23/c4p.egg-info/top_level.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2023-07-02 05:23:07.586825 c4p-2023.7.1.23/setup.cfg
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      915 2023-07-02 05:20:29.000000 c4p-2023.7.1.23/setup.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-06 12:20:11.362035 c4p-2023.7.6/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1065 2023-05-22 19:27:41.000000 c4p-2023.7.6/LICENSE
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       27 2023-07-02 05:18:20.000000 c4p-2023.7.6/MANIFEST.in
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      541 2023-07-06 12:20:11.361341 c4p-2023.7.6/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       94 2023-07-02 04:04:59.000000 c4p-2023.7.6/README.md
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-06 12:20:11.077462 c4p-2023.7.6/c4p/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      240 2023-06-01 04:08:45.000000 c4p-2023.7.6/c4p/__init__.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1301 2023-07-06 11:39:15.000000 c4p-2023.7.6/c4p/case.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3790 2023-07-06 12:17:20.000000 c4p-2023.7.6/c4p/mapping.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7954 2023-07-05 20:44:40.000000 c4p-2023.7.6/c4p/rof.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-06 12:20:11.069399 c4p-2023.7.6/c4p/src/
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-06 12:20:11.177185 c4p-2023.7.6/c4p/src/cime_mapping/
+-rwxr-xr-x   0 fengzhu  (40317) ncar      (1000)    12240 2023-07-06 11:09:27.000000 c4p-2023.7.6/c4p/src/cime_mapping/create_ESMF_map.sh
+-rwxr-xr-x   0 fengzhu  (40317) ncar      (1000)    15746 2023-07-06 11:43:56.000000 c4p-2023.7.6/c4p/src/cime_mapping/gen_cesm_maps.ncpu36.sh
+-rwxr-xr-x   0 fengzhu  (40317) ncar      (1000)    15728 2023-07-05 21:44:35.000000 c4p-2023.7.6/c4p/src/cime_mapping/gen_cesm_maps.sh
+-rwxr-xr-x   0 fengzhu  (40317) ncar      (1000)   875456 2023-07-06 12:14:46.000000 c4p-2023.7.6/c4p/src/cime_mapping/gen_domain
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-06 12:20:11.222944 c4p-2023.7.6/c4p/src/rof/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      885 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/Makefile
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    11024 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/check_inf_loop.F90
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2633 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/create-topo_0.5x0.5deg.ncl
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1861 2023-07-02 02:20:03.000000 c4p-2023.7.6/c4p/src/rof/create-topo_1x1deg.ncl
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1700 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/create-topo_2x2deg.ncl
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    12241 2023-07-02 04:22:06.000000 c4p-2023.7.6/c4p/src/rof/create_ESMF_map.sh
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     5321 2023-07-02 02:42:46.000000 c4p-2023.7.6/c4p/src/rof/plot_rdirc.ncl
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1613 2023-07-02 02:44:45.000000 c4p-2023.7.6/c4p/src/rof/plotrdirc.csh
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3122 2023-07-02 02:45:04.000000 c4p-2023.7.6/c4p/src/rof/rdirc_template.csh
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2620 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/rtm_ncdf.pro
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      543 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map.1x1.template.nml
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)  7760296 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_0.5deg
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)  7760360 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_1deg
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-06 12:20:11.224670 c4p-2023.7.6/c4p/src/rof/runoff_map_src/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      580 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/build.cheyenne.csh
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-06 12:20:11.357580 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      725 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/Macros.cheyenne
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     6226 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/Makefile
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    14995 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/fixroff_mod.F90
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1094 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/kind_mod.F90
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     9525 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/main.F90
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    94808 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/map_mod.F90
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    94853 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/map_mod_0.5deg.F90.save
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    94808 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/map_mod_1deg.F90.save
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    36063 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/mapsort_mod.F90
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1242 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/shr_kind_mod.F90
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    12114 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/shr_sys_mod.F90
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    14025 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/shr_timer_mod.F90
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    60912 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/smooth_mod.F90
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-06 12:20:11.359989 c4p-2023.7.6/c4p/src/rof/runoff_map_src/tools/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    12359 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/tools/makdep.c
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    22122 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/topo2rdirc_sed.F90
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2252 2023-07-06 11:40:09.000000 c4p-2023.7.6/c4p/utils.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-06 12:20:11.174154 c4p-2023.7.6/c4p.egg-info/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      541 2023-07-06 12:20:10.000000 c4p-2023.7.6/c4p.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1591 2023-07-06 12:20:10.000000 c4p-2023.7.6/c4p.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-07-06 12:20:10.000000 c4p-2023.7.6/c4p.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-06-01 04:07:36.000000 c4p-2023.7.6/c4p.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       47 2023-07-06 12:20:10.000000 c4p-2023.7.6/c4p.egg-info/requires.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2023-07-06 12:20:10.000000 c4p-2023.7.6/c4p.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2023-07-06 12:20:11.362151 c4p-2023.7.6/setup.cfg
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      912 2023-07-06 12:19:16.000000 c4p-2023.7.6/setup.py
```

### Comparing `c4p-2023.7.1.23/LICENSE` & `c4p-2023.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/PKG-INFO` & `c4p-2023.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4p
-Version: 2023.7.1.23
+Version: 2023.7.6
 Summary: c4p: CESM for Paleo
 Home-page: https://github.com/fzhu2e/cesm4paleo
 Author: Feng Zhu, Jiang Zhu
 Author-email: fengzhu@ucar.edu, jiangzhu@ucar.edu
 License: MIT
 Keywords: CESM,paleoclimate
 Classifier: Natural Language :: English
```

### Comparing `c4p-2023.7.1.23/c4p/case.py` & `c4p-2023.7.6/c4p/case.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 import os
+from datetime import date
 
 from . import utils
-from .runoff import Runoff
+from .rof import ROF
+from .mapping import Mapping
 
+cwd = os.path.dirname(__file__)
 
 class PaleoCase:
-    def __init__(self, casename=None, work_dirpath=None, esmfbin_path=None, lib_netcdf=None, inc_netcdf=None):
+    def __init__(self, casename=None, work_dirpath=None, esmfbin_path=None, netcdf_lib_path=None, netcdf_inc_path=None, account=None):
         self.casename = casename
+        self.account = account
         self.work_dirpath = work_dirpath
         self.esmfbin_path = '/glade/u/apps/derecho/23.06/spack/opt/spack/esmf/8.4.2/cray-mpich/8.1.25/oneapi/2023.0.0/fslf/bin' if esmfbin_path is None else esmfbin_path
-        self.lib_netcdf = '/glade/u/apps/derecho/23.06/spack/opt/spack/netcdf/4.9.2/oneapi/2023.0.0/iijr/lib' if lib_netcdf is None else lib_netcdf
-        self.inc_netcdf = '/glade/u/apps/derecho/23.06/spack/opt/spack/netcdf/4.9.2/oneapi/2023.0.0/iijr/include' if inc_netcdf is None else inc_netcdf
+        self.netcdf_lib_path = '/glade/u/apps/derecho/23.06/spack/opt/spack/netcdf/4.9.2/oneapi/2023.0.0/iijr/lib' if netcdf_lib_path is None else netcdf_lib_path
+        self.netcdf_inc_path = '/glade/u/apps/derecho/23.06/spack/opt/spack/netcdf/4.9.2/oneapi/2023.0.0/iijr/include' if netcdf_inc_path is None else netcdf_inc_path
         if not os.path.exists(work_dirpath):
             os.makedirs(work_dirpath, exist_ok=True)
             utils.p_success(f'>>> {work_dirpath} created')
         os.chdir(work_dirpath)
         utils.p_success(f'>>> Current directory switched to: {work_dirpath}')
 
+    def mapping(self):
+        return Mapping(**self.__dict__)
+
     def setup_runoff(self):
-        return Runoff(**self.__dict__)
+        return ROF(**self.__dict__)
```

### Comparing `c4p-2023.7.1.23/c4p/runoff.py` & `c4p-2023.7.6/c4p/rof.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import date
 import xarray as xr
 
 from . import utils
 
 cwd = os.path.dirname(__file__)
 
-class Runoff:
+class ROF:
     def __init__(self, grids_dirpath=None, path_create_ESMF_map_sh=None, **kwargs):
         for k, v in kwargs.items():
             self.__dict__[k] = v
 
         self.grids_dirpath='/glade/p/cesmdata/inputdata/share/scripgrids' if grids_dirpath is None else grids_dirpath
         self.path_create_ESMF_map_sh=os.path.join(cwd, './src/rof/create_ESMF_map.sh') if path_create_ESMF_map_sh is None else path_create_ESMF_map_sh
 
@@ -56,16 +56,16 @@
             },
         )
 
         fpath = utils.copy(path_Makefile)
         utils.replace_str(
             fpath,
             {
-                'LIB_NETCDF = -L/glade/apps/opt/netcdf/4.2/intel/default/lib -lnetcdf': f'LIB_NETCDF = -L{self.lib_netcdf} -lnetcdff',
-                'INC_NETCDF = -I/glade/apps/opt/netcdf/4.2/intel/default/include': f'INC_NETCDF = -I{self.inc_netcdf}',
+                'LIB_NETCDF = -L/glade/apps/opt/netcdf/4.2/intel/default/lib -lnetcdf': f'LIB_NETCDF = -L{self.netcdf_lib_path} -lnetcdff',
+                'INC_NETCDF = -I/glade/apps/opt/netcdf/4.2/intel/default/include': f'INC_NETCDF = -I{self.netcdf_inc_path}',
             },
         )
         utils.exec_script(fpath_new)
 
     def plot_runoff(self, topo_path,
             path_plotrdirc_csh=os.path.join(cwd, './src/rof/plotrdirc.csh'),
             path_plotrdirc_ncl=os.path.join(cwd, './src/rof/plot_rdirc.ncl'),
```

### Comparing `c4p-2023.7.1.23/c4p/src/rof/Makefile` & `c4p-2023.7.6/c4p/src/rof/Makefile`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/check_inf_loop.F90` & `c4p-2023.7.6/c4p/src/rof/check_inf_loop.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/create-topo_0.5x0.5deg.ncl` & `c4p-2023.7.6/c4p/src/rof/create-topo_0.5x0.5deg.ncl`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/create-topo_1x1deg.ncl` & `c4p-2023.7.6/c4p/src/rof/create-topo_1x1deg.ncl`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/create-topo_2x2deg.ncl` & `c4p-2023.7.6/c4p/src/rof/create-topo_2x2deg.ncl`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/create_ESMF_map.sh` & `c4p-2023.7.6/c4p/src/rof/create_ESMF_map.sh`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/plot_rdirc.ncl` & `c4p-2023.7.6/c4p/src/rof/plot_rdirc.ncl`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/plotrdirc.csh` & `c4p-2023.7.6/c4p/src/rof/plotrdirc.csh`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/rdirc_template.csh` & `c4p-2023.7.6/c4p/src/rof/rdirc_template.csh`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/rtm_ncdf.pro` & `c4p-2023.7.6/c4p/src/rof/rtm_ncdf.pro`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/runoff_map.1x1.template.nml` & `c4p-2023.7.6/c4p/src/rof/runoff_map.1x1.template.nml`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/runoff_map_0.5deg` & `c4p-2023.7.6/c4p/src/rof/runoff_map_0.5deg`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/runoff_map_1deg` & `c4p-2023.7.6/c4p/src/rof/runoff_map_1deg`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/build.cheyenne.csh` & `c4p-2023.7.6/c4p/src/rof/runoff_map_src/build.cheyenne.csh`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/Macros.cheyenne` & `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/Macros.cheyenne`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/Makefile` & `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/Makefile`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/fixroff_mod.F90` & `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/fixroff_mod.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/kind_mod.F90` & `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/kind_mod.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/main.F90` & `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/main.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/map_mod.F90` & `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/map_mod.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/map_mod_0.5deg.F90.save` & `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/map_mod_0.5deg.F90.save`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/map_mod_1deg.F90.save` & `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/map_mod_1deg.F90.save`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/mapsort_mod.F90` & `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/mapsort_mod.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/shr_kind_mod.F90` & `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/shr_kind_mod.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/shr_sys_mod.F90` & `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/shr_sys_mod.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/shr_timer_mod.F90` & `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/shr_timer_mod.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/src/smooth_mod.F90` & `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/smooth_mod.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/runoff_map_src/tools/makdep.c` & `c4p-2023.7.6/c4p/src/rof/runoff_map_src/tools/makdep.c`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/src/rof/topo2rdirc_sed.F90` & `c4p-2023.7.6/c4p/src/rof/topo2rdirc_sed.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.1.23/c4p/utils.py` & `c4p-2023.7.6/c4p/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -57,13 +57,32 @@
 def copy(src, dst=None):
     if dst is None:
         dst = os.path.basename(src)
 
     shutil.copyfile(src, dst)
     return dst
 
-def exec_script(fpath, args=None, timeout=None):
-    run_shell(f'chmod +x {fpath}')
+def exec_script(fpath, args=None, timeout=None, chmod_add_x=True):
+    if chmod_add_x:
+        run_shell(f'chmod +x {fpath}')
+
     if args is None:
-        run_shell(f'./{fpath}', timeout=timeout)
+        cmd = fpath
     else:
-        run_shell(f'./{fpath} {args}', timeout=timeout)
+        cmd = f'{fpath} {args}'
+
+    run_shell(cmd, timeout=timeout)
+
+def qsub_script(fpath, args=None, name='test', queue='main', select=1, ncpus=36, mpiprocs=36, mem=64, walltime='06:00:00', account=None):
+    if account is None:
+        raise ValueError('account must be specified')
+
+    if args is None:
+        cmd = fpath
+    else:
+        cmd = f'{fpath} {args}'
+
+    l1 = f'select={select}:ncpus={ncpus}:mpiprocs={mpiprocs}:mem={mem}GB'
+    l2 = f'walltime={walltime}'
+    
+    run_shell(f'echo -e {cmd} | qsub -N {name} -q {queue} -l {l1} -l {l2} -A {account}')
+
```

### Comparing `c4p-2023.7.1.23/c4p.egg-info/PKG-INFO` & `c4p-2023.7.6/c4p.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4p
-Version: 2023.7.1.23
+Version: 2023.7.6
 Summary: c4p: CESM for Paleo
 Home-page: https://github.com/fzhu2e/cesm4paleo
 Author: Feng Zhu, Jiang Zhu
 Author-email: fengzhu@ucar.edu, jiangzhu@ucar.edu
 License: MIT
 Keywords: CESM,paleoclimate
 Classifier: Natural Language :: English
```

### Comparing `c4p-2023.7.1.23/c4p.egg-info/SOURCES.txt` & `c4p-2023.7.6/c4p.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 ./c4p/__init__.py
 ./c4p/case.py
-./c4p/runoff.py
 ./c4p/utils.py
 c4p/__init__.py
 c4p/case.py
-c4p/runoff.py
+c4p/mapping.py
+c4p/rof.py
 c4p/utils.py
 c4p.egg-info/PKG-INFO
 c4p.egg-info/SOURCES.txt
 c4p.egg-info/dependency_links.txt
 c4p.egg-info/not-zip-safe
 c4p.egg-info/requires.txt
 c4p.egg-info/top_level.txt
+c4p/src/cime_mapping/create_ESMF_map.sh
+c4p/src/cime_mapping/gen_cesm_maps.ncpu36.sh
+c4p/src/cime_mapping/gen_cesm_maps.sh
+c4p/src/cime_mapping/gen_domain
 c4p/src/rof/Makefile
 c4p/src/rof/check_inf_loop.F90
 c4p/src/rof/create-topo_0.5x0.5deg.ncl
 c4p/src/rof/create-topo_1x1deg.ncl
 c4p/src/rof/create-topo_2x2deg.ncl
 c4p/src/rof/create_ESMF_map.sh
 c4p/src/rof/plot_rdirc.ncl
```

### Comparing `c4p-2023.7.1.23/setup.py` & `c4p-2023.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='c4p',  # required
-    version='2023.7.1.23',
+    version='2023.7.6',
     description='c4p: CESM for Paleo',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Jiang Zhu',
     author_email='fengzhu@ucar.edu, jiangzhu@ucar.edu',
     url='https://github.com/fzhu2e/cesm4paleo',
     packages=find_packages(),
```

