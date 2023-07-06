# Comparing `tmp/dp4plus_app-0.1.11.tar.gz` & `tmp/dp4plus_app-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dp4plus_app-0.1.11.tar", last modified: Fri Jun 30 13:15:07 2023, max compression
+gzip compressed data, was "dp4plus_app-0.1.12.tar", last modified: Thu Jul  6 18:05:30 2023, max compression
```

## Comparing `dp4plus_app-0.1.11.tar` & `dp4plus_app-0.1.12.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 13:15:07.276606 dp4plus_app-0.1.11/
--rw-rw-rw-   0        0        0     1092 2023-03-10 18:45:01.000000 dp4plus_app-0.1.11/LICENCE
--rw-rw-rw-   0        0        0     8527 2023-06-30 13:15:07.274653 dp4plus_app-0.1.11/PKG-INFO
--rw-rw-rw-   0        0        0     7924 2023-06-29 17:07:45.000000 dp4plus_app-0.1.11/README.md
--rw-rw-rw-   0        0        0       42 2023-06-30 13:15:07.276606 dp4plus_app-0.1.11/setup.cfg
--rw-rw-rw-   0        0        0     2022 2023-06-30 13:12:52.000000 dp4plus_app-0.1.11/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-30 13:15:03.176418 dp4plus_app-0.1.11/src/
-drwxrwxrwx   0        0        0        0 2023-06-30 13:15:03.852211 dp4plus_app-0.1.11/src/dp4plus_app/
-drwxrwxrwx   0        0        0        0 2023-06-30 13:15:04.127607 dp4plus_app-0.1.11/src/dp4plus_app/UserGuide/
--rw-rw-rw-   0        0        0  1984200 2023-06-29 19:09:47.000000 dp4plus_app-0.1.11/src/dp4plus_app/UserGuide/UserGuide.docx
--rw-rw-rw-   0        0        0  2043916 2023-06-29 19:10:06.000000 dp4plus_app-0.1.11/src/dp4plus_app/UserGuide/UserGuide.pdf
--rw-rw-rw-   0        0        0   839144 2023-06-29 17:31:33.000000 dp4plus_app-0.1.11/src/dp4plus_app/UserGuide/UserGuideFigures.pptx
--rw-rw-rw-   0        0        0        0 2023-03-23 20:21:29.000000 dp4plus_app-0.1.11/src/dp4plus_app/__init__.py
--rw-rw-rw-   0        0        0     9508 2023-06-02 17:21:15.000000 dp4plus_app-0.1.11/src/dp4plus_app/bugs_a_warning_module.py
--rw-rw-rw-   0        0        0     9896 2023-06-07 19:08:21.000000 dp4plus_app-0.1.11/src/dp4plus_app/correlation_module.py
--rw-rw-rw-   0        0        0    18721 2023-06-28 19:16:22.000000 dp4plus_app-0.1.11/src/dp4plus_app/custom_gui_module.py
--rw-rw-rw-   0        0        0     8774 2023-06-28 17:11:40.000000 dp4plus_app-0.1.11/src/dp4plus_app/custom_module.py
--rw-rw-rw-   0        0        0    18712 2023-06-28 17:26:01.000000 dp4plus_app-0.1.11/src/dp4plus_app/data_base_Custom.xlsx
--rw-rw-rw-   0        0        0    61121 2023-05-16 14:51:37.000000 dp4plus_app-0.1.11/src/dp4plus_app/data_base_MM.xlsx
--rw-rw-rw-   0        0        0    42509 2023-02-28 18:07:42.000000 dp4plus_app-0.1.11/src/dp4plus_app/data_base_QM.xlsx
--rw-rw-rw-   0        0        0     7269 2023-05-30 17:36:59.000000 dp4plus_app-0.1.11/src/dp4plus_app/dp4_module.py
--rw-rw-rw-   0        0        0    49515 2023-06-28 16:54:34.000000 dp4plus_app-0.1.11/src/dp4plus_app/logo_CONICET.png
--rw-rw-rw-   0        0        0    73256 2023-06-29 14:53:02.000000 dp4plus_app-0.1.11/src/dp4plus_app/logo_DP4app.png
--rw-rw-rw-   0        0        0    21045 2023-03-07 17:09:01.000000 dp4plus_app-0.1.11/src/dp4plus_app/logo_INGEBIO.png
--rw-rw-rw-   0        0        0     4449 2023-06-28 18:57:00.000000 dp4plus_app-0.1.11/src/dp4plus_app/main.py
--rw-rw-rw-   0        0        0    19301 2023-06-28 18:51:53.000000 dp4plus_app-0.1.11/src/dp4plus_app/main_gui_module.py
-drwxrwxrwx   0        0        0        0 2023-06-30 13:15:04.273120 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/
--rw-rw-rw-   0        0        0    36815 2023-05-31 14:49:36.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/Data_traning_set.xlsx
--rw-rw-rw-   0        0        0    67105 2023-03-14 13:31:40.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/custom_molecules_set.docx
-drwxrwxrwx   0        0        0        0 2023-06-30 13:15:04.640315 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/
--rw-rw-rw-   0        0        0      588 2023-03-09 17:59:12.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/0_Custom_nmr_TMS_optB.gjc
--rw-rw-rw-   0        0        0      529 2023-03-09 17:59:12.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/1_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1057 2023-03-09 17:59:12.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/2_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1539 2023-03-09 17:59:12.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1537 2023-03-15 13:03:00.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_002_optB.gjc
--rw-rw-rw-   0        0        0     1531 2023-03-09 17:59:12.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1530 2023-03-15 13:03:00.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_002_optB.gjc
--rw-rw-rw-   0        0        0      750 2023-03-09 17:59:12.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/5_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1032 2023-03-09 17:59:12.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/6_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1368 2023-03-09 17:59:12.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1372 2023-03-15 13:03:00.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_002_optB.gjc
--rw-rw-rw-   0        0        0     1374 2023-03-15 13:03:00.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_003_optB.gjc
--rw-rw-rw-   0        0        0     1384 2023-03-15 13:03:00.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_004_optB.gjc
--rw-rw-rw-   0        0        0     1716 2023-03-09 17:59:12.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_001_optB.gjc
--rw-rw-rw-   0        0        0     1725 2023-03-15 13:03:00.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_002_optB.gjc
-drwxrwxrwx   0        0        0        0 2023-06-30 13:15:05.090521 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/
--rw-rw-rw-   0        0        0      588 2022-10-04 14:19:04.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/0_Custom_nmr_TMS_MMFF.gjc
--rw-rw-rw-   0        0        0      529 2022-10-04 14:19:04.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/1_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1057 2022-10-04 14:19:04.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/2_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1539 2022-10-04 14:19:04.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1536 2022-10-04 14:19:04.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_002_MMFF.gjc
--rw-rw-rw-   0        0        0     1534 2022-10-04 14:19:06.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1529 2022-10-04 14:19:06.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_002_MMFF.gjc
--rw-rw-rw-   0        0        0      749 2022-10-04 14:19:04.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/5_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1030 2022-10-04 14:19:16.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/6_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1369 2022-10-04 14:19:08.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1372 2022-10-04 14:19:08.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_002_MMFF.gjc
--rw-rw-rw-   0        0        0     1376 2022-10-04 14:19:08.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_003_MMFF.gjc
--rw-rw-rw-   0        0        0     1382 2022-10-04 14:19:08.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_004_MMFF.gjc
--rw-rw-rw-   0        0        0     1712 2022-10-04 14:19:10.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_001_MMFF.gjc
--rw-rw-rw-   0        0        0     1724 2022-10-04 14:19:10.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_002_MMFF.gjc
-drwxrwxrwx   0        0        0        0 2023-06-30 13:15:07.270746 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/
--rw-rw-rw-   0        0        0    16107 2023-03-13 19:26:08.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a - copia.xlsx
--rw-rw-rw-   0        0        0    62190 2022-05-17 17:47:26.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_001_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62202 2022-05-17 17:59:17.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_002_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62133 2022-05-17 18:10:35.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_003_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62150 2022-05-17 18:21:10.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_004_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62411 2022-05-17 18:31:50.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_005_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62149 2022-05-17 18:42:51.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_006_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62608 2022-05-17 18:54:27.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_007_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62119 2022-05-17 19:06:23.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_008_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62121 2022-05-17 19:17:42.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_009_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62114 2022-05-17 19:29:29.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_010_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62393 2022-05-17 19:40:13.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_011_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62174 2022-05-17 19:51:50.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_012_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62373 2022-05-17 20:02:41.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_013_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62105 2022-05-17 20:14:06.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_014_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62116 2022-05-17 20:24:59.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_015_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62115 2022-05-17 20:35:55.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_016_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62446 2022-05-17 20:46:44.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_017_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62187 2022-05-17 20:57:46.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_018_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62154 2022-05-17 21:08:39.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_019_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62493 2022-05-17 18:10:10.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_020_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62148 2022-05-17 18:40:52.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_021_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62142 2022-05-17 19:11:10.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_022_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62196 2022-05-17 19:40:30.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_023_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62042 2022-05-17 20:09:33.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_024_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62182 2022-05-17 20:38:31.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_025_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62183 2022-05-17 21:08:56.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_026_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62120 2022-05-17 21:39:48.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_027_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62186 2022-05-17 22:10:41.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_028_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62172 2022-05-17 22:41:37.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_029_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62078 2022-05-17 23:14:34.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_030_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62352 2022-05-17 23:49:30.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_031_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62156 2022-05-18 00:18:50.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_032_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62159 2022-05-18 00:52:59.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_033_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62114 2022-05-18 01:23:09.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_001_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62635 2022-05-18 01:55:00.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_002_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62125 2022-05-18 02:27:45.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_003_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62530 2022-05-18 02:58:42.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_004_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62375 2022-05-18 03:34:04.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_005_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62140 2022-05-17 18:21:07.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_006_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62059 2022-05-17 18:56:41.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_007_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    61990 2022-05-17 19:26:23.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_008_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62108 2022-05-17 19:53:58.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_009_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62035 2022-05-17 20:19:33.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_010_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62125 2022-05-17 20:47:31.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_011_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62189 2022-05-17 21:16:05.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_012_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62289 2022-05-17 21:40:37.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_013_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62204 2022-05-17 22:05:51.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_014_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62168 2022-05-17 22:33:21.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_015_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62204 2022-05-17 23:01:32.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_016_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62373 2022-05-17 23:36:01.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_017_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62132 2022-05-18 00:05:25.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_018_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62094 2022-05-18 00:41:01.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_019_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62003 2022-05-18 01:14:58.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_020_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62114 2022-05-18 01:51:51.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_021_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62174 2022-05-18 02:25:20.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_022_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62111 2022-05-18 03:04:33.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_023_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62153 2022-05-18 03:34:21.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_024_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62159 2022-05-17 18:26:26.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_025_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62110 2022-05-17 18:32:41.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_026_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62223 2022-05-17 18:39:11.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_027_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62314 2022-05-17 18:46:00.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_028_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62290 2022-05-17 18:52:29.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_029_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62120 2022-05-17 18:59:07.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_030_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62387 2022-05-17 19:05:40.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_031_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62437 2022-05-17 19:12:26.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_032_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62096 2022-05-17 19:18:31.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_033_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    66884 2022-05-17 19:25:09.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_034_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62111 2022-05-17 19:31:38.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_035_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62040 2022-05-17 19:37:41.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_036_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62317 2022-05-17 19:44:23.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_037_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62120 2022-05-17 19:51:02.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_038_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62010 2022-05-17 19:57:03.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_039_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62101 2022-05-17 20:03:32.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_040_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    62045 2022-05-17 20:10:05.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_041_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    63152 2022-05-17 20:16:50.000000 dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_042_WB9_B_SMD_nmr.log
--rw-rw-rw-   0        0        0    10912 2023-06-28 17:08:03.000000 dp4plus_app-0.1.11/src/dp4plus_app/output_module.py
--rw-rw-rw-   0        0        0     5375 2023-06-02 17:47:02.000000 dp4plus_app-0.1.11/src/dp4plus_app/validation_module.py
-drwxrwxrwx   0        0        0        0 2023-06-30 13:15:03.914714 dp4plus_app-0.1.11/src/dp4plus_app.egg-info/
--rw-rw-rw-   0        0        0     8527 2023-06-30 13:15:02.000000 dp4plus_app-0.1.11/src/dp4plus_app.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7079 2023-06-30 13:15:02.000000 dp4plus_app-0.1.11/src/dp4plus_app.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 13:15:02.000000 dp4plus_app-0.1.11/src/dp4plus_app.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      107 2023-06-30 13:15:02.000000 dp4plus_app-0.1.11/src/dp4plus_app.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      132 2023-06-30 13:15:02.000000 dp4plus_app-0.1.11/src/dp4plus_app.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-30 13:15:02.000000 dp4plus_app-0.1.11/src/dp4plus_app.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 18:05:30.749682 dp4plus_app-0.1.12/
+-rw-rw-rw-   0        0        0     1092 2023-03-10 18:45:01.000000 dp4plus_app-0.1.12/LICENCE
+-rw-rw-rw-   0        0        0     8527 2023-07-06 18:05:30.702805 dp4plus_app-0.1.12/PKG-INFO
+-rw-rw-rw-   0        0        0     7924 2023-06-29 17:07:45.000000 dp4plus_app-0.1.12/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 18:05:30.749682 dp4plus_app-0.1.12/setup.cfg
+-rw-rw-rw-   0        0        0     2022 2023-07-06 18:04:12.000000 dp4plus_app-0.1.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:05:26.029313 dp4plus_app-0.1.12/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 18:05:26.904341 dp4plus_app-0.1.12/src/dp4plus_app/
+drwxrwxrwx   0        0        0        0 2023-07-06 18:05:27.107475 dp4plus_app-0.1.12/src/dp4plus_app/UserGuide/
+-rw-rw-rw-   0        0        0  1984200 2023-06-29 19:09:47.000000 dp4plus_app-0.1.12/src/dp4plus_app/UserGuide/UserGuide.docx
+-rw-rw-rw-   0        0        0  2043916 2023-06-29 19:10:06.000000 dp4plus_app-0.1.12/src/dp4plus_app/UserGuide/UserGuide.pdf
+-rw-rw-rw-   0        0        0   839144 2023-06-29 17:31:33.000000 dp4plus_app-0.1.12/src/dp4plus_app/UserGuide/UserGuideFigures.pptx
+-rw-rw-rw-   0        0        0        0 2023-03-23 20:21:29.000000 dp4plus_app-0.1.12/src/dp4plus_app/__init__.py
+-rw-rw-rw-   0        0        0     9508 2023-06-02 17:21:15.000000 dp4plus_app-0.1.12/src/dp4plus_app/bugs_a_warning_module.py
+-rw-rw-rw-   0        0        0     9896 2023-06-07 19:08:21.000000 dp4plus_app-0.1.12/src/dp4plus_app/correlation_module.py
+-rw-rw-rw-   0        0        0    18721 2023-06-28 19:16:22.000000 dp4plus_app-0.1.12/src/dp4plus_app/custom_gui_module.py
+-rw-rw-rw-   0        0        0     8774 2023-06-28 17:11:40.000000 dp4plus_app-0.1.12/src/dp4plus_app/custom_module.py
+-rw-rw-rw-   0        0        0    18712 2023-06-28 17:26:01.000000 dp4plus_app-0.1.12/src/dp4plus_app/data_base_Custom.xlsx
+-rw-rw-rw-   0        0        0    61121 2023-05-16 14:51:37.000000 dp4plus_app-0.1.12/src/dp4plus_app/data_base_MM.xlsx
+-rw-rw-rw-   0        0        0    42509 2023-02-28 18:07:42.000000 dp4plus_app-0.1.12/src/dp4plus_app/data_base_QM.xlsx
+-rw-rw-rw-   0        0        0     7269 2023-05-30 17:36:59.000000 dp4plus_app-0.1.12/src/dp4plus_app/dp4_module.py
+-rw-rw-rw-   0        0        0    49515 2023-06-28 16:54:34.000000 dp4plus_app-0.1.12/src/dp4plus_app/logo_CONICET.png
+-rw-rw-rw-   0        0        0    73256 2023-06-29 14:53:02.000000 dp4plus_app-0.1.12/src/dp4plus_app/logo_DP4app.png
+-rw-rw-rw-   0        0        0    21045 2023-03-07 17:09:01.000000 dp4plus_app-0.1.12/src/dp4plus_app/logo_INGEBIO.png
+-rw-rw-rw-   0        0        0     4432 2023-07-06 18:03:05.000000 dp4plus_app-0.1.12/src/dp4plus_app/main.py
+-rw-rw-rw-   0        0        0    19301 2023-06-28 18:51:53.000000 dp4plus_app-0.1.12/src/dp4plus_app/main_gui_module.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:05:27.232477 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/
+-rw-rw-rw-   0        0        0    36815 2023-05-31 14:49:36.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/Data_traning_set.xlsx
+-rw-rw-rw-   0        0        0    67105 2023-03-14 13:31:40.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/custom_molecules_set.docx
+drwxrwxrwx   0        0        0        0 2023-07-06 18:05:27.685616 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/
+-rw-rw-rw-   0        0        0      588 2023-03-09 17:59:12.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/0_Custom_nmr_TMS_optB.gjc
+-rw-rw-rw-   0        0        0      529 2023-03-09 17:59:12.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/1_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1057 2023-03-09 17:59:12.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/2_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1539 2023-03-09 17:59:12.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1537 2023-03-15 13:03:00.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_002_optB.gjc
+-rw-rw-rw-   0        0        0     1531 2023-03-09 17:59:12.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1530 2023-03-15 13:03:00.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_002_optB.gjc
+-rw-rw-rw-   0        0        0      750 2023-03-09 17:59:12.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/5_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1032 2023-03-09 17:59:12.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/6_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1368 2023-03-09 17:59:12.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1372 2023-03-15 13:03:00.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_002_optB.gjc
+-rw-rw-rw-   0        0        0     1374 2023-03-15 13:03:00.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_003_optB.gjc
+-rw-rw-rw-   0        0        0     1384 2023-03-15 13:03:00.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_004_optB.gjc
+-rw-rw-rw-   0        0        0     1716 2023-03-09 17:59:12.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_001_optB.gjc
+-rw-rw-rw-   0        0        0     1725 2023-03-15 13:03:00.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_002_optB.gjc
+drwxrwxrwx   0        0        0        0 2023-07-06 18:05:28.216887 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/
+-rw-rw-rw-   0        0        0      588 2022-10-04 14:19:04.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/0_Custom_nmr_TMS_MMFF.gjc
+-rw-rw-rw-   0        0        0      529 2022-10-04 14:19:04.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/1_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1057 2022-10-04 14:19:04.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/2_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1539 2022-10-04 14:19:04.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1536 2022-10-04 14:19:04.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_002_MMFF.gjc
+-rw-rw-rw-   0        0        0     1534 2022-10-04 14:19:06.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1529 2022-10-04 14:19:06.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_002_MMFF.gjc
+-rw-rw-rw-   0        0        0      749 2022-10-04 14:19:04.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/5_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1030 2022-10-04 14:19:16.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/6_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1369 2022-10-04 14:19:08.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1372 2022-10-04 14:19:08.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_002_MMFF.gjc
+-rw-rw-rw-   0        0        0     1376 2022-10-04 14:19:08.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_003_MMFF.gjc
+-rw-rw-rw-   0        0        0     1382 2022-10-04 14:19:08.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_004_MMFF.gjc
+-rw-rw-rw-   0        0        0     1712 2022-10-04 14:19:10.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_001_MMFF.gjc
+-rw-rw-rw-   0        0        0     1724 2022-10-04 14:19:10.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_002_MMFF.gjc
+drwxrwxrwx   0        0        0        0 2023-07-06 18:05:30.687181 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/
+-rw-rw-rw-   0        0        0    16107 2023-03-13 19:26:08.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a - copia.xlsx
+-rw-rw-rw-   0        0        0    62190 2022-05-17 17:47:26.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_001_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62202 2022-05-17 17:59:17.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_002_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62133 2022-05-17 18:10:35.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_003_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62150 2022-05-17 18:21:10.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_004_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62411 2022-05-17 18:31:50.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_005_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62149 2022-05-17 18:42:51.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_006_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62608 2022-05-17 18:54:27.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_007_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62119 2022-05-17 19:06:23.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_008_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62121 2022-05-17 19:17:42.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_009_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62114 2022-05-17 19:29:29.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_010_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62393 2022-05-17 19:40:13.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_011_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62174 2022-05-17 19:51:50.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_012_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62373 2022-05-17 20:02:41.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_013_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62105 2022-05-17 20:14:06.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_014_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62116 2022-05-17 20:24:59.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_015_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62115 2022-05-17 20:35:55.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_016_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62446 2022-05-17 20:46:44.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_017_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62187 2022-05-17 20:57:46.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_018_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62154 2022-05-17 21:08:39.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_019_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62493 2022-05-17 18:10:10.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_020_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62148 2022-05-17 18:40:52.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_021_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62142 2022-05-17 19:11:10.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_022_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62196 2022-05-17 19:40:30.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_023_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62042 2022-05-17 20:09:33.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_024_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62182 2022-05-17 20:38:31.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_025_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62183 2022-05-17 21:08:56.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_026_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62120 2022-05-17 21:39:48.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_027_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62186 2022-05-17 22:10:41.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_028_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62172 2022-05-17 22:41:37.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_029_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62078 2022-05-17 23:14:34.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_030_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62352 2022-05-17 23:49:30.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_031_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62156 2022-05-18 00:18:50.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_032_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62159 2022-05-18 00:52:59.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_033_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62114 2022-05-18 01:23:09.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_001_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62635 2022-05-18 01:55:00.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_002_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62125 2022-05-18 02:27:45.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_003_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62530 2022-05-18 02:58:42.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_004_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62375 2022-05-18 03:34:04.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_005_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62140 2022-05-17 18:21:07.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_006_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62059 2022-05-17 18:56:41.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_007_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    61990 2022-05-17 19:26:23.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_008_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62108 2022-05-17 19:53:58.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_009_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62035 2022-05-17 20:19:33.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_010_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62125 2022-05-17 20:47:31.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_011_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62189 2022-05-17 21:16:05.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_012_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62289 2022-05-17 21:40:37.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_013_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62204 2022-05-17 22:05:51.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_014_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62168 2022-05-17 22:33:21.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_015_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62204 2022-05-17 23:01:32.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_016_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62373 2022-05-17 23:36:01.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_017_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62132 2022-05-18 00:05:25.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_018_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62094 2022-05-18 00:41:01.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_019_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62003 2022-05-18 01:14:58.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_020_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62114 2022-05-18 01:51:51.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_021_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62174 2022-05-18 02:25:20.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_022_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62111 2022-05-18 03:04:33.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_023_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62153 2022-05-18 03:34:21.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_024_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62159 2022-05-17 18:26:26.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_025_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62110 2022-05-17 18:32:41.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_026_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62223 2022-05-17 18:39:11.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_027_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62314 2022-05-17 18:46:00.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_028_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62290 2022-05-17 18:52:29.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_029_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62120 2022-05-17 18:59:07.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_030_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62387 2022-05-17 19:05:40.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_031_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62437 2022-05-17 19:12:26.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_032_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62096 2022-05-17 19:18:31.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_033_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    66884 2022-05-17 19:25:09.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_034_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62111 2022-05-17 19:31:38.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_035_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62040 2022-05-17 19:37:41.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_036_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62317 2022-05-17 19:44:23.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_037_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62120 2022-05-17 19:51:02.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_038_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62010 2022-05-17 19:57:03.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_039_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62101 2022-05-17 20:03:32.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_040_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    62045 2022-05-17 20:10:05.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_041_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    63152 2022-05-17 20:16:50.000000 dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_042_WB9_B_SMD_nmr.log
+-rw-rw-rw-   0        0        0    10912 2023-06-28 17:08:03.000000 dp4plus_app-0.1.12/src/dp4plus_app/output_module.py
+-rw-rw-rw-   0        0        0     5375 2023-06-02 17:47:02.000000 dp4plus_app-0.1.12/src/dp4plus_app/validation_module.py
+drwxrwxrwx   0        0        0        0 2023-07-06 18:05:26.966844 dp4plus_app-0.1.12/src/dp4plus_app.egg-info/
+-rw-rw-rw-   0        0        0     8527 2023-07-06 18:05:25.000000 dp4plus_app-0.1.12/src/dp4plus_app.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7079 2023-07-06 18:05:25.000000 dp4plus_app-0.1.12/src/dp4plus_app.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 18:05:25.000000 dp4plus_app-0.1.12/src/dp4plus_app.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      107 2023-07-06 18:05:25.000000 dp4plus_app-0.1.12/src/dp4plus_app.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      132 2023-07-06 18:05:25.000000 dp4plus_app-0.1.12/src/dp4plus_app.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-06 18:05:25.000000 dp4plus_app-0.1.12/src/dp4plus_app.egg-info/top_level.txt
```

### Comparing `dp4plus_app-0.1.11/LICENCE` & `dp4plus_app-0.1.12/LICENCE`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/PKG-INFO` & `dp4plus_app-0.1.12/src/dp4plus_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dp4plus_app
-Version: 0.1.11
+Name: dp4plus-app
+Version: 0.1.12
 Summary: A tool to simplify your DP4+ calculations
 Home-page: https://github.com/RosarioCCLab/DP4plus-App
 Author: Bruno A. Franco
 Author-email: bruno.agustin.franco@gmail.com
 License: MIT
 Keywords: nmr
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dp4plus_app-0.1.11/README.md` & `dp4plus_app-0.1.12/README.md`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/setup.py` & `dp4plus_app-0.1.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 with open('README.md') as file:         #sirve para incluir el REEDME
     long_description = file.read()
 
 short_description = 'A tool to simplify your DP4+ calculations'
 
 setup(
     name='dp4plus_app',
-    version='0.1.11',
+    version='0.1.12',
     
     author='Bruno A. Franco',
     author_email='bruno.agustin.franco@gmail.com',
     url='https://github.com/RosarioCCLab/DP4plus-App',
     description =short_description	,
     long_description = long_description,
     long_description_content_type ="text/markdown",
```

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/UserGuide/UserGuide.docx` & `dp4plus_app-0.1.12/src/dp4plus_app/UserGuide/UserGuide.docx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/UserGuide/UserGuide.pdf` & `dp4plus_app-0.1.12/src/dp4plus_app/UserGuide/UserGuide.pdf`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/UserGuide/UserGuideFigures.pptx` & `dp4plus_app-0.1.12/src/dp4plus_app/UserGuide/UserGuideFigures.pptx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/bugs_a_warning_module.py` & `dp4plus_app-0.1.12/src/dp4plus_app/bugs_a_warning_module.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/correlation_module.py` & `dp4plus_app-0.1.12/src/dp4plus_app/correlation_module.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/custom_gui_module.py` & `dp4plus_app-0.1.12/src/dp4plus_app/custom_gui_module.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/custom_module.py` & `dp4plus_app-0.1.12/src/dp4plus_app/custom_module.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/data_base_Custom.xlsx` & `dp4plus_app-0.1.12/src/dp4plus_app/data_base_Custom.xlsx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/data_base_MM.xlsx` & `dp4plus_app-0.1.12/src/dp4plus_app/data_base_MM.xlsx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/data_base_QM.xlsx` & `dp4plus_app-0.1.12/src/dp4plus_app/data_base_QM.xlsx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/dp4_module.py` & `dp4plus_app-0.1.12/src/dp4plus_app/dp4_module.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/logo_CONICET.png` & `dp4plus_app-0.1.12/src/dp4plus_app/logo_CONICET.png`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/logo_DP4app.png` & `dp4plus_app-0.1.12/src/dp4plus_app/logo_DP4app.png`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/logo_INGEBIO.png` & `dp4plus_app-0.1.12/src/dp4plus_app/logo_INGEBIO.png`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/main.py` & `dp4plus_app-0.1.12/src/dp4plus_app/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     GUI.attributes('-topmost',False)
     GUI.wm_title("DP4+App")
     title = tk.Label(GUI, text= 'Welcome to',
                      font = ("Times", "25", "bold"))
     title.pack()
     
     image1 = Image.open((Path(__file__).parent / 'logo_DP4app.png').as_posix())
-    image1 = image1.resize((192, 237), Image.ANTIALIAS)
+    image1 = image1.resize((192, 237))
     test = ImageTk.PhotoImage(image1)
     label1 = tk.Label(image=test)
     label1.image = test
     label1.pack()
     
     #--------------------------------------------------------------------
     mode, inputs = gui.gui_input()
```

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/main_gui_module.py` & `dp4plus_app-0.1.12/src/dp4plus_app/main_gui_module.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/Data_traning_set.xlsx` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/Data_traning_set.xlsx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/custom_molecules_set.docx` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/custom_molecules_set.docx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/0_Custom_nmr_TMS_optB.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/0_Custom_nmr_TMS_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/1_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/1_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/2_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/2_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_002_optB.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/3_Custom_nmr_002_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_002_optB.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/4_Custom_nmr_002_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/5_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/5_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/6_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/6_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_002_optB.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_002_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_003_optB.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_003_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_004_optB.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/7_Custom_nmr_004_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_001_optB.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_001_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_002_optB.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_B3LYP/8_Custom_nmr_002_optB.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/0_Custom_nmr_TMS_MMFF.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/0_Custom_nmr_TMS_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/1_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/1_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/2_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/2_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_002_MMFF.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/3_Custom_nmr_002_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_002_MMFF.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/4_Custom_nmr_002_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/5_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/5_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/6_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/6_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_002_MMFF.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_002_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_003_MMFF.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_003_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_004_MMFF.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/7_Custom_nmr_004_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_001_MMFF.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_001_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_002_MMFF.gjc` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_custom/opt_MMFF/8_Custom_nmr_002_MMFF.gjc`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a - copia.xlsx` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a - copia.xlsx`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_001_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_001_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_002_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_002_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_003_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_003_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_004_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_004_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_005_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_005_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_006_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_006_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_007_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_007_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_008_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_008_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_009_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_009_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_010_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_010_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_011_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_011_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_012_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_012_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_013_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_013_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_014_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_014_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_015_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_015_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_016_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_016_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_017_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_017_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_018_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_018_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_019_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_019_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_020_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_020_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_021_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_021_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_022_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_022_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_023_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_023_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_024_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_024_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_025_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_025_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_026_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_026_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_027_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_027_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_028_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_028_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_029_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_029_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_030_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_030_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_031_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_031_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_032_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_032_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73a_033_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73a_033_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_001_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_001_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_002_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_002_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_003_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_003_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_004_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_004_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_005_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_005_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_006_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_006_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_007_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_007_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_008_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_008_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_009_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_009_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_010_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_010_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_011_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_011_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_012_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_012_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_013_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_013_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_014_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_014_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_015_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_015_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_016_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_016_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_017_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_017_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_018_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_018_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_019_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_019_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_020_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_020_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_021_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_021_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_022_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_022_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_023_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_023_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_024_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_024_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_025_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_025_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_026_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_026_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_027_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_027_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_028_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_028_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_029_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_029_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_030_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_030_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_031_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_031_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_032_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_032_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_033_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_033_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_034_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_034_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_035_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_035_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_036_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_036_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_037_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_037_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_038_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_038_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_039_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_039_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_040_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_040_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_041_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_041_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/nmr_examples/73b_042_WB9_B_SMD_nmr.log` & `dp4plus_app-0.1.12/src/dp4plus_app/nmr_examples/73b_042_WB9_B_SMD_nmr.log`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/output_module.py` & `dp4plus_app-0.1.12/src/dp4plus_app/output_module.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app/validation_module.py` & `dp4plus_app-0.1.12/src/dp4plus_app/validation_module.py`

 * *Files identical despite different names*

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app.egg-info/PKG-INFO` & `dp4plus_app-0.1.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: dp4plus-app
-Version: 0.1.11
+Name: dp4plus_app
+Version: 0.1.12
 Summary: A tool to simplify your DP4+ calculations
 Home-page: https://github.com/RosarioCCLab/DP4plus-App
 Author: Bruno A. Franco
 Author-email: bruno.agustin.franco@gmail.com
 License: MIT
 Keywords: nmr
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dp4plus_app-0.1.11/src/dp4plus_app.egg-info/SOURCES.txt` & `dp4plus_app-0.1.12/src/dp4plus_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

