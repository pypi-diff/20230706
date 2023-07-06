# Comparing `tmp/feloopy-0.2.5.tar.gz` & `tmp/feloopy-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feloopy-0.2.5.tar", last modified: Sat May 27 17:33:22 2023, max compression
+gzip compressed data, was "feloopy-0.2.6.tar", last modified: Thu Jul  6 10:24:10 2023, max compression
```

## Comparing `feloopy-0.2.5.tar` & `feloopy-0.2.6.tar`

### file list

```diff
@@ -1,170 +1,183 @@
-drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:22.083867 feloopy-0.2.5/
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1094 2023-05-11 14:53:22.000000 feloopy-0.2.5/LICENSE
--rw-rw-r--   0 keivan    (1000) keivan    (1000)    10791 2023-05-27 17:33:22.079867 feloopy-0.2.5/PKG-INFO
--rw-rw-r--   0 keivan    (1000) keivan    (1000)    10001 2023-05-27 17:30:23.000000 feloopy-0.2.5/README.md
-drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:21.999867 feloopy-0.2.5/feloopy/
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     9762 2023-05-26 17:18:32.000000 feloopy-0.2.5/feloopy/__init__.py
-drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:21.999867 feloopy-0.2.5/feloopy/algorithms/
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-17 08:47:59.000000 feloopy-0.2.5/feloopy/algorithms/__init__.py
-drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:21.999867 feloopy-0.2.5/feloopy/algorithms/constraint/
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 18:18:46.000000 feloopy-0.2.5/feloopy/algorithms/constraint/__init__.py
-drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:21.999867 feloopy-0.2.5/feloopy/algorithms/exact/
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 17:22:32.000000 feloopy-0.2.5/feloopy/algorithms/exact/__init__.py
-drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:22.003867 feloopy-0.2.5/feloopy/algorithms/heuristic/
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3302 2023-05-17 08:43:08.000000 feloopy-0.2.5/feloopy/algorithms/heuristic/DE.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3471 2023-05-17 08:43:29.000000 feloopy-0.2.5/feloopy/algorithms/heuristic/GA.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2644 2023-05-12 20:25:18.000000 feloopy-0.2.5/feloopy/algorithms/heuristic/GWO.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     4030 2023-05-12 20:25:25.000000 feloopy-0.2.5/feloopy/algorithms/heuristic/SA.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2085 2023-05-12 20:25:30.000000 feloopy-0.2.5/feloopy/algorithms/heuristic/TS.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 17:22:42.000000 feloopy-0.2.5/feloopy/algorithms/heuristic/__init__.py
-drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:22.015867 feloopy-0.2.5/feloopy/algorithms/mcdm/
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      957 2023-05-15 18:09:12.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/__init__.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1861 2023-05-26 15:27:35.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/ahp.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2666 2023-05-26 15:29:14.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/aras.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2366 2023-05-26 15:31:12.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/borda.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2620 2023-05-26 15:35:07.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/bwm.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2821 2023-05-26 15:37:07.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/codas.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2670 2023-05-26 15:39:44.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/copras.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1989 2023-05-26 15:42:38.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/critic.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3512 2023-05-26 15:48:36.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/dematel.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1192 2023-05-15 17:53:51.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/edas.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3349 2023-05-26 16:25:52.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/elecre_i.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2215 2023-05-15 17:48:22.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/electre_i_s.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3438 2023-05-15 17:48:29.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/electre_i_v.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3029 2023-05-15 17:48:33.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/electre_ii.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3518 2023-05-15 17:49:14.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/electre_iii.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2145 2023-05-15 17:49:14.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/electre_iv.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3047 2023-05-15 17:49:14.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/electre_tri.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2273 2023-05-15 17:49:03.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/fahp.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2828 2023-05-15 17:56:01.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/fdematel.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1341 2023-05-15 17:54:40.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/fedeas.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1180 2023-05-15 17:49:14.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/ftopsis.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2647 2023-05-15 17:52:09.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/fvikor.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1381 2023-05-15 17:50:08.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/gra.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1478 2023-05-15 17:55:13.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/idocriw.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1247 2023-05-15 17:55:23.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/mabac.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1648 2023-05-15 17:55:33.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/maut.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1668 2023-05-15 17:55:40.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/moora.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2252 2023-05-15 17:50:26.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/moosra.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2049 2023-05-15 17:49:15.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/multimoora.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1905 2023-05-15 17:52:20.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_gaia.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1329 2023-05-15 17:49:14.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_i.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3258 2023-05-15 17:49:14.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_ii.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3141 2023-05-15 17:49:14.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_iii.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3000 2023-05-15 18:23:05.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_iv.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2878 2023-05-15 17:57:18.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_v.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2398 2023-05-15 17:57:13.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_vi.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1356 2023-05-15 17:57:05.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/saw.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1664 2023-05-15 17:56:55.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/smart.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1468 2023-05-15 17:56:48.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/topsis.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2277 2023-05-15 17:56:41.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/vikor.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2628 2023-05-15 17:51:32.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/waspas.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2193 2023-05-15 17:51:36.000000 feloopy-0.2.5/feloopy/algorithms/mcdm/wings.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)   150152 2023-05-27 15:34:30.000000 feloopy-0.2.5/feloopy/feloopy.py
-drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:22.019867 feloopy-0.2.5/feloopy/generators/
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      421 2023-05-12 17:33:41.000000 feloopy-0.2.5/feloopy/generators/__init__.py
-drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:22.031867 feloopy-0.2.5/feloopy/generators/model/
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 17:24:04.000000 feloopy-0.2.5/feloopy/generators/model/__init__.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      431 2023-05-17 15:20:21.000000 feloopy-0.2.5/feloopy/generators/model/cplex_cp_model_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      426 2023-05-26 16:26:32.000000 feloopy-0.2.5/feloopy/generators/model/cplex_model_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      420 2023-05-12 17:24:33.000000 feloopy-0.2.5/feloopy/generators/model/cvxpy_model_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      440 2023-05-12 17:24:39.000000 feloopy-0.2.5/feloopy/generators/model/cylp_model_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3717 2023-05-27 17:31:47.000000 feloopy-0.2.5/feloopy/generators/model/feloopy_model_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      435 2023-05-12 17:25:19.000000 feloopy-0.2.5/feloopy/generators/model/gekko_model_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      421 2023-05-12 17:25:23.000000 feloopy-0.2.5/feloopy/generators/model/gurobi_model_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      392 2023-05-12 17:25:27.000000 feloopy-0.2.5/feloopy/generators/model/linopy_model_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)    26915 2023-05-12 17:29:08.000000 feloopy-0.2.5/feloopy/generators/model/mealpy_model_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      427 2023-05-26 16:28:01.000000 feloopy-0.2.5/feloopy/generators/model/mip_model_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      425 2023-05-26 16:28:05.000000 feloopy-0.2.5/feloopy/generators/model/ortools_cp_model_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      447 2023-05-26 16:28:10.000000 feloopy-0.2.5/feloopy/generators/model/ortools_model_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      423 2023-05-12 17:29:23.000000 feloopy-0.2.5/feloopy/generators/model/picos_model_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      444 2023-05-12 17:29:28.000000 feloopy-0.2.5/feloopy/generators/model/pulp_model_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      415 2023-05-12 17:29:36.000000 feloopy-0.2.5/feloopy/generators/model/pymprog_model_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      437 2023-05-12 17:29:40.000000 feloopy-0.2.5/feloopy/generators/model/pyomo_model_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      421 2023-05-12 17:29:44.000000 feloopy-0.2.5/feloopy/generators/model/xpress_model_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2687 2023-05-26 10:39:58.000000 feloopy-0.2.5/feloopy/generators/model_generator.py
-drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:22.047867 feloopy-0.2.5/feloopy/generators/result/
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 17:29:52.000000 feloopy-0.2.5/feloopy/generators/result/__init__.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      680 2023-05-12 17:29:58.000000 feloopy-0.2.5/feloopy/generators/result/cplex_cp_result_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      745 2023-05-12 17:30:09.000000 feloopy-0.2.5/feloopy/generators/result/cplex_result_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      751 2023-05-12 17:30:13.000000 feloopy-0.2.5/feloopy/generators/result/cvxpy_result_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      751 2023-05-12 17:30:17.000000 feloopy-0.2.5/feloopy/generators/result/cylp_result_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      860 2023-05-12 17:30:22.000000 feloopy-0.2.5/feloopy/generators/result/gekko_result_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1448 2023-05-12 17:30:26.000000 feloopy-0.2.5/feloopy/generators/result/gurobi_result_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      736 2023-05-12 17:30:31.000000 feloopy-0.2.5/feloopy/generators/result/linopy_result_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      674 2023-05-12 17:30:34.000000 feloopy-0.2.5/feloopy/generators/result/mip_result_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      855 2023-05-12 17:30:38.000000 feloopy-0.2.5/feloopy/generators/result/ortools_cp_result_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      930 2023-05-12 17:30:46.000000 feloopy-0.2.5/feloopy/generators/result/ortools_result_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      692 2023-05-12 17:30:50.000000 feloopy-0.2.5/feloopy/generators/result/picos_result_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      796 2023-05-12 17:30:55.000000 feloopy-0.2.5/feloopy/generators/result/pulp_result_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      778 2023-05-12 17:30:58.000000 feloopy-0.2.5/feloopy/generators/result/pymprog_result_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      747 2023-05-12 17:31:02.000000 feloopy-0.2.5/feloopy/generators/result/pyomo_result_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      711 2023-05-12 17:31:06.000000 feloopy-0.2.5/feloopy/generators/result/xpress_result_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     6520 2023-05-12 17:33:49.000000 feloopy-0.2.5/feloopy/generators/result_generator.py
-drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:22.051867 feloopy-0.2.5/feloopy/generators/solution/
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 17:31:12.000000 feloopy-0.2.5/feloopy/generators/solution/__init__.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2294 2023-05-26 16:32:33.000000 feloopy-0.2.5/feloopy/generators/solution/cplex_cp_solution_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     4247 2023-05-12 17:31:21.000000 feloopy-0.2.5/feloopy/generators/solution/cplex_solution_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3241 2023-05-12 17:31:26.000000 feloopy-0.2.5/feloopy/generators/solution/cvxpy_solution_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2255 2023-05-12 17:31:30.000000 feloopy-0.2.5/feloopy/generators/solution/cylp_solution_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3182 2023-05-12 17:31:34.000000 feloopy-0.2.5/feloopy/generators/solution/feloopy_solution_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2935 2023-05-12 17:31:37.000000 feloopy-0.2.5/feloopy/generators/solution/gekko_solution_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2984 2023-05-12 17:31:41.000000 feloopy-0.2.5/feloopy/generators/solution/gurobi_solution_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2372 2023-05-12 17:31:45.000000 feloopy-0.2.5/feloopy/generators/solution/linopy_solution_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     4607 2023-05-26 22:10:18.000000 feloopy-0.2.5/feloopy/generators/solution/mealpy_solution_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2186 2023-05-12 17:31:54.000000 feloopy-0.2.5/feloopy/generators/solution/mip_solution_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2976 2023-05-12 17:31:58.000000 feloopy-0.2.5/feloopy/generators/solution/ortools_cp_solution_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3311 2023-05-12 17:32:03.000000 feloopy-0.2.5/feloopy/generators/solution/ortools_solution_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2570 2023-05-12 17:32:06.000000 feloopy-0.2.5/feloopy/generators/solution/picos_solution_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3558 2023-05-12 20:06:11.000000 feloopy-0.2.5/feloopy/generators/solution/pulp_solution_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2349 2023-05-12 17:32:17.000000 feloopy-0.2.5/feloopy/generators/solution/pymprog_solution_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     5347 2023-05-27 17:00:58.000000 feloopy-0.2.5/feloopy/generators/solution/pymultiobjective_solution_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     5733 2023-05-12 17:32:27.000000 feloopy-0.2.5/feloopy/generators/solution/pyomo_solution_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2240 2023-05-12 17:32:31.000000 feloopy-0.2.5/feloopy/generators/solution/xpress_solution_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3090 2023-05-17 15:57:15.000000 feloopy-0.2.5/feloopy/generators/solution_generator.py
-drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:22.059867 feloopy-0.2.5/feloopy/generators/variable/
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 17:32:36.000000 feloopy-0.2.5/feloopy/generators/variable/__init__.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3123 2023-05-27 16:01:05.000000 feloopy-0.2.5/feloopy/generators/variable/cplex_cp_variable_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3433 2023-05-12 17:32:45.000000 feloopy-0.2.5/feloopy/generators/variable/cplex_variable_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     6293 2023-05-19 19:26:03.000000 feloopy-0.2.5/feloopy/generators/variable/cvxpy_variable_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3158 2023-05-12 17:32:53.000000 feloopy-0.2.5/feloopy/generators/variable/cylp_variable_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3072 2023-05-12 17:32:57.000000 feloopy-0.2.5/feloopy/generators/variable/gekko_variable_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     8216 2023-05-12 17:33:01.000000 feloopy-0.2.5/feloopy/generators/variable/gurobi_variable_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2420 2023-05-12 17:33:04.000000 feloopy-0.2.5/feloopy/generators/variable/linopy_variable_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2955 2023-05-12 17:33:08.000000 feloopy-0.2.5/feloopy/generators/variable/mip_variable_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3742 2023-05-12 17:33:12.000000 feloopy-0.2.5/feloopy/generators/variable/ortools_cp_variable_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3957 2023-05-12 17:33:17.000000 feloopy-0.2.5/feloopy/generators/variable/ortools_variable_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3295 2023-05-12 17:33:21.000000 feloopy-0.2.5/feloopy/generators/variable/picos_variable_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3661 2023-05-12 17:33:25.000000 feloopy-0.2.5/feloopy/generators/variable/pulp_variable_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3508 2023-05-12 17:33:30.000000 feloopy-0.2.5/feloopy/generators/variable/pymprog_variable_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     2705 2023-05-12 17:33:34.000000 feloopy-0.2.5/feloopy/generators/variable/pyomo_variable_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     4232 2023-05-12 17:33:37.000000 feloopy-0.2.5/feloopy/generators/variable/xpress_variable_generator.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3022 2023-05-12 17:34:00.000000 feloopy-0.2.5/feloopy/generators/variable_generator.py
-drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:22.063867 feloopy-0.2.5/feloopy/helpers/
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 17:34:12.000000 feloopy-0.2.5/feloopy/helpers/__init__.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1494 2023-05-12 17:34:17.000000 feloopy-0.2.5/feloopy/helpers/empty.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)       49 2023-05-27 11:55:10.000000 feloopy-0.2.5/feloopy/helpers/error.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      132 2023-05-27 14:39:24.000000 feloopy-0.2.5/feloopy/helpers/formatter.py
-drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:22.079867 feloopy-0.2.5/feloopy/operators/
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      384 2023-05-12 20:17:53.000000 feloopy-0.2.5/feloopy/operators/__init__.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)    11270 2023-05-12 17:54:44.000000 feloopy-0.2.5/feloopy/operators/common.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      772 2023-05-12 17:34:37.000000 feloopy-0.2.5/feloopy/operators/count_operators.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)        0 2023-05-12 20:47:21.000000 feloopy-0.2.5/feloopy/operators/epsilon.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      380 2023-05-12 17:34:41.000000 feloopy-0.2.5/feloopy/operators/exact.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      560 2023-05-26 22:23:23.000000 feloopy-0.2.5/feloopy/operators/fix_operators.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      474 2023-05-12 17:34:53.000000 feloopy-0.2.5/feloopy/operators/heuristic.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     3656 2023-05-12 17:34:49.000000 feloopy-0.2.5/feloopy/operators/heuristic_operators.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1569 2023-05-25 13:29:00.000000 feloopy-0.2.5/feloopy/operators/math_operators.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)    15154 2023-05-26 16:39:30.000000 feloopy-0.2.5/feloopy/operators/metric_operators.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)        0 2023-05-26 10:16:57.000000 feloopy-0.2.5/feloopy/operators/pareto.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      476 2023-05-12 17:35:00.000000 feloopy-0.2.5/feloopy/operators/random_operators.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      576 2023-05-26 16:39:45.000000 feloopy-0.2.5/feloopy/operators/set_operators.py
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1932 2023-05-26 16:39:50.000000 feloopy-0.2.5/feloopy/operators/update_operators.py
-drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-05-27 17:33:21.999867 feloopy-0.2.5/feloopy.egg-info/
--rw-rw-r--   0 keivan    (1000) keivan    (1000)    10791 2023-05-27 17:33:21.000000 feloopy-0.2.5/feloopy.egg-info/PKG-INFO
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     6493 2023-05-27 17:33:21.000000 feloopy-0.2.5/feloopy.egg-info/SOURCES.txt
--rw-rw-r--   0 keivan    (1000) keivan    (1000)        1 2023-05-27 17:33:21.000000 feloopy-0.2.5/feloopy.egg-info/dependency_links.txt
--rw-rw-r--   0 keivan    (1000) keivan    (1000)      270 2023-05-27 17:33:21.000000 feloopy-0.2.5/feloopy.egg-info/requires.txt
--rw-rw-r--   0 keivan    (1000) keivan    (1000)        8 2023-05-27 17:33:21.000000 feloopy-0.2.5/feloopy.egg-info/top_level.txt
--rw-rw-r--   0 keivan    (1000) keivan    (1000)       38 2023-05-27 17:33:22.083867 feloopy-0.2.5/setup.cfg
--rw-rw-r--   0 keivan    (1000) keivan    (1000)     1809 2023-05-17 08:50:20.000000 feloopy-0.2.5/setup.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-07-06 10:24:10.907938 feloopy-0.2.6/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1094 2023-05-11 14:53:22.000000 feloopy-0.2.6/LICENSE
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)    10918 2023-07-06 10:24:10.907938 feloopy-0.2.6/PKG-INFO
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)    10128 2023-07-06 09:42:16.000000 feloopy-0.2.6/README.md
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-07-06 10:24:10.831937 feloopy-0.2.6/feloopy/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     9762 2023-05-26 17:18:32.000000 feloopy-0.2.6/feloopy/__init__.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-07-06 10:24:10.831937 feloopy-0.2.6/feloopy/algorithms/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-17 08:47:59.000000 feloopy-0.2.6/feloopy/algorithms/__init__.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-07-06 10:24:10.831937 feloopy-0.2.6/feloopy/algorithms/constraint/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      294 2023-07-06 09:28:42.000000 feloopy-0.2.6/feloopy/algorithms/constraint/__init__.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-07-06 10:24:10.831937 feloopy-0.2.6/feloopy/algorithms/exact/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      295 2023-07-06 09:28:53.000000 feloopy-0.2.6/feloopy/algorithms/exact/__init__.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      294 2023-07-06 09:28:57.000000 feloopy-0.2.6/feloopy/algorithms/exact/benders.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-07-06 10:24:10.835937 feloopy-0.2.6/feloopy/algorithms/heuristic/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3303 2023-07-06 09:29:13.000000 feloopy-0.2.6/feloopy/algorithms/heuristic/DE.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3471 2023-07-06 09:29:22.000000 feloopy-0.2.6/feloopy/algorithms/heuristic/GA.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2645 2023-07-06 09:29:29.000000 feloopy-0.2.6/feloopy/algorithms/heuristic/GWO.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     4030 2023-07-06 09:29:36.000000 feloopy-0.2.6/feloopy/algorithms/heuristic/SA.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2115 2023-07-06 09:29:43.000000 feloopy-0.2.6/feloopy/algorithms/heuristic/TS.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      294 2023-07-06 09:29:07.000000 feloopy-0.2.6/feloopy/algorithms/heuristic/__init__.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-07-06 10:24:10.847937 feloopy-0.2.6/feloopy/algorithms/mcdm/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      957 2023-05-15 18:09:12.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/__init__.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1862 2023-07-06 09:30:01.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/ahp.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2666 2023-05-26 15:29:14.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/aras.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2366 2023-05-26 15:31:12.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/borda.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2620 2023-05-26 15:35:07.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/bwm.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2821 2023-05-26 15:37:07.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/codas.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2670 2023-05-26 15:39:44.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/copras.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1989 2023-05-26 15:42:38.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/critic.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3512 2023-05-26 15:48:36.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/dematel.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1192 2023-05-15 17:53:51.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/edas.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3349 2023-05-26 16:25:52.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/elecre_i.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2215 2023-05-15 17:48:22.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/electre_i_s.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3438 2023-05-15 17:48:29.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/electre_i_v.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3029 2023-05-15 17:48:33.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/electre_ii.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3518 2023-05-15 17:49:14.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/electre_iii.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2145 2023-05-15 17:49:14.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/electre_iv.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3047 2023-05-15 17:49:14.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/electre_tri.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2273 2023-05-15 17:49:03.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/fahp.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2828 2023-05-15 17:56:01.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/fdematel.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1341 2023-05-15 17:54:40.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/fedeas.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1180 2023-05-15 17:49:14.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/ftopsis.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2647 2023-05-15 17:52:09.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/fvikor.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1381 2023-05-15 17:50:08.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/gra.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1478 2023-05-15 17:55:13.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/idocriw.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1247 2023-05-15 17:55:23.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/mabac.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1648 2023-05-15 17:55:33.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/maut.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1668 2023-05-15 17:55:40.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/moora.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2252 2023-05-15 17:50:26.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/moosra.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2049 2023-05-15 17:49:15.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/multimoora.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1905 2023-05-15 17:52:20.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/promethee_gaia.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1329 2023-05-15 17:49:14.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/promethee_i.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3258 2023-05-15 17:49:14.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/promethee_ii.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3141 2023-05-15 17:49:14.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/promethee_iii.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3000 2023-05-15 18:23:05.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/promethee_iv.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2878 2023-05-15 17:57:18.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/promethee_v.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2398 2023-05-15 17:57:13.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/promethee_vi.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1356 2023-05-15 17:57:05.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/saw.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1664 2023-05-15 17:56:55.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/smart.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1468 2023-05-15 17:56:48.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/topsis.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2277 2023-05-15 17:56:41.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/vikor.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2628 2023-05-15 17:51:32.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/waspas.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2193 2023-05-15 17:51:36.000000 feloopy-0.2.6/feloopy/algorithms/mcdm/wings.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)   191735 2023-07-06 10:06:42.000000 feloopy-0.2.6/feloopy/feloopy.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-07-06 10:24:10.847937 feloopy-0.2.6/feloopy/generators/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      421 2023-05-12 17:33:41.000000 feloopy-0.2.6/feloopy/generators/__init__.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-07-06 10:24:10.855937 feloopy-0.2.6/feloopy/generators/model/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 17:24:04.000000 feloopy-0.2.6/feloopy/generators/model/__init__.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      430 2023-07-03 09:43:08.000000 feloopy-0.2.6/feloopy/generators/model/cplex_cp_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      426 2023-05-26 16:26:32.000000 feloopy-0.2.6/feloopy/generators/model/cplex_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      420 2023-05-12 17:24:33.000000 feloopy-0.2.6/feloopy/generators/model/cvxpy_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      440 2023-05-12 17:24:39.000000 feloopy-0.2.6/feloopy/generators/model/cylp_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3717 2023-05-27 17:31:47.000000 feloopy-0.2.6/feloopy/generators/model/feloopy_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      435 2023-05-12 17:25:19.000000 feloopy-0.2.6/feloopy/generators/model/gekko_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      421 2023-05-12 17:25:23.000000 feloopy-0.2.6/feloopy/generators/model/gurobi_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      392 2023-05-12 17:25:27.000000 feloopy-0.2.6/feloopy/generators/model/linopy_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      488 2023-07-06 07:08:47.000000 feloopy-0.2.6/feloopy/generators/model/localsolver_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)    14135 2023-07-06 09:09:45.000000 feloopy-0.2.6/feloopy/generators/model/mealpy_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      427 2023-05-26 16:28:01.000000 feloopy-0.2.6/feloopy/generators/model/mip_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      425 2023-07-03 09:44:37.000000 feloopy-0.2.6/feloopy/generators/model/ortools_cp_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      447 2023-05-26 16:28:10.000000 feloopy-0.2.6/feloopy/generators/model/ortools_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      423 2023-05-12 17:29:23.000000 feloopy-0.2.6/feloopy/generators/model/picos_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      444 2023-05-12 17:29:28.000000 feloopy-0.2.6/feloopy/generators/model/pulp_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      415 2023-05-12 17:29:36.000000 feloopy-0.2.6/feloopy/generators/model/pymprog_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      437 2023-05-12 17:29:40.000000 feloopy-0.2.6/feloopy/generators/model/pyomo_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      443 2023-06-02 16:15:25.000000 feloopy-0.2.6/feloopy/generators/model/rsome_dro_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      415 2023-06-02 16:15:31.000000 feloopy-0.2.6/feloopy/generators/model/rsome_ro_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      421 2023-05-12 17:29:44.000000 feloopy-0.2.6/feloopy/generators/model/xpress_model_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3183 2023-07-06 06:58:59.000000 feloopy-0.2.6/feloopy/generators/model_generator.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-07-06 10:24:10.867937 feloopy-0.2.6/feloopy/generators/result/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 17:29:52.000000 feloopy-0.2.6/feloopy/generators/result/__init__.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      679 2023-06-03 12:29:13.000000 feloopy-0.2.6/feloopy/generators/result/cplex_cp_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1015 2023-07-06 07:07:41.000000 feloopy-0.2.6/feloopy/generators/result/cplex_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1045 2023-06-03 14:24:23.000000 feloopy-0.2.6/feloopy/generators/result/cvxpy_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      751 2023-05-12 17:30:17.000000 feloopy-0.2.6/feloopy/generators/result/cylp_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      927 2023-06-18 11:53:44.000000 feloopy-0.2.6/feloopy/generators/result/gekko_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1448 2023-05-12 17:30:26.000000 feloopy-0.2.6/feloopy/generators/result/gurobi_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      736 2023-05-12 17:30:31.000000 feloopy-0.2.6/feloopy/generators/result/linopy_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      942 2023-07-06 07:09:11.000000 feloopy-0.2.6/feloopy/generators/result/localsolver_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      674 2023-05-12 17:30:34.000000 feloopy-0.2.6/feloopy/generators/result/mip_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      959 2023-06-18 11:52:33.000000 feloopy-0.2.6/feloopy/generators/result/ortools_cp_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1109 2023-06-18 11:53:36.000000 feloopy-0.2.6/feloopy/generators/result/ortools_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      692 2023-05-12 17:30:50.000000 feloopy-0.2.6/feloopy/generators/result/picos_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1934 2023-06-04 16:00:26.000000 feloopy-0.2.6/feloopy/generators/result/pulp_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      778 2023-05-12 17:30:58.000000 feloopy-0.2.6/feloopy/generators/result/pymprog_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1033 2023-06-03 13:11:24.000000 feloopy-0.2.6/feloopy/generators/result/pyomo_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      560 2023-06-02 17:59:25.000000 feloopy-0.2.6/feloopy/generators/result/rsome_dro_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      549 2023-06-02 17:59:20.000000 feloopy-0.2.6/feloopy/generators/result/rsome_ro_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      733 2023-07-06 06:53:59.000000 feloopy-0.2.6/feloopy/generators/result/xpress_result_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     7843 2023-07-06 07:13:00.000000 feloopy-0.2.6/feloopy/generators/result_generator.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-07-06 10:24:10.879938 feloopy-0.2.6/feloopy/generators/solution/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 17:31:12.000000 feloopy-0.2.6/feloopy/generators/solution/__init__.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2278 2023-06-20 07:27:00.000000 feloopy-0.2.6/feloopy/generators/solution/cplex_cp_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     4329 2023-06-03 13:59:21.000000 feloopy-0.2.6/feloopy/generators/solution/cplex_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3447 2023-06-05 14:37:17.000000 feloopy-0.2.6/feloopy/generators/solution/cvxpy_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2281 2023-06-03 14:25:38.000000 feloopy-0.2.6/feloopy/generators/solution/cylp_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3191 2023-06-18 14:01:23.000000 feloopy-0.2.6/feloopy/generators/solution/feloopy_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2934 2023-06-05 14:18:06.000000 feloopy-0.2.6/feloopy/generators/solution/gekko_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2984 2023-05-12 17:31:41.000000 feloopy-0.2.6/feloopy/generators/solution/gurobi_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2552 2023-06-05 15:09:05.000000 feloopy-0.2.6/feloopy/generators/solution/linopy_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1015 2023-07-06 07:22:31.000000 feloopy-0.2.6/feloopy/generators/solution/localsolver_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     4644 2023-06-18 14:29:47.000000 feloopy-0.2.6/feloopy/generators/solution/mealpy_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2311 2023-07-03 10:40:07.000000 feloopy-0.2.6/feloopy/generators/solution/mip_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2976 2023-05-12 17:31:58.000000 feloopy-0.2.6/feloopy/generators/solution/ortools_cp_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3577 2023-06-05 14:28:56.000000 feloopy-0.2.6/feloopy/generators/solution/ortools_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2570 2023-05-12 17:32:06.000000 feloopy-0.2.6/feloopy/generators/solution/picos_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3697 2023-06-05 14:04:16.000000 feloopy-0.2.6/feloopy/generators/solution/pulp_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     4744 2023-07-04 16:01:03.000000 feloopy-0.2.6/feloopy/generators/solution/pymoo_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2379 2023-07-03 10:51:25.000000 feloopy-0.2.6/feloopy/generators/solution/pymprog_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     5327 2023-07-05 07:30:19.000000 feloopy-0.2.6/feloopy/generators/solution/pymultiobjective_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     6260 2023-06-05 14:04:35.000000 feloopy-0.2.6/feloopy/generators/solution/pyomo_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3127 2023-06-02 17:50:49.000000 feloopy-0.2.6/feloopy/generators/solution/rsome_dro_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3155 2023-06-02 17:50:43.000000 feloopy-0.2.6/feloopy/generators/solution/rsome_ro_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2318 2023-07-06 06:55:51.000000 feloopy-0.2.6/feloopy/generators/solution/xpress_solution_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3671 2023-07-06 07:13:52.000000 feloopy-0.2.6/feloopy/generators/solution_generator.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-07-06 10:24:10.895938 feloopy-0.2.6/feloopy/generators/variable/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 17:32:36.000000 feloopy-0.2.6/feloopy/generators/variable/__init__.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3123 2023-05-27 16:01:05.000000 feloopy-0.2.6/feloopy/generators/variable/cplex_cp_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3433 2023-05-12 17:32:45.000000 feloopy-0.2.6/feloopy/generators/variable/cplex_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     4246 2023-07-06 10:08:27.000000 feloopy-0.2.6/feloopy/generators/variable/cvxpy_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3694 2023-06-05 13:39:32.000000 feloopy-0.2.6/feloopy/generators/variable/cylp_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     4188 2023-06-05 14:43:14.000000 feloopy-0.2.6/feloopy/generators/variable/gekko_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     7600 2023-06-05 13:41:32.000000 feloopy-0.2.6/feloopy/generators/variable/gurobi_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3746 2023-06-05 13:50:53.000000 feloopy-0.2.6/feloopy/generators/variable/linopy_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2355 2023-07-06 07:03:39.000000 feloopy-0.2.6/feloopy/generators/variable/localsolver_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2955 2023-05-12 17:33:08.000000 feloopy-0.2.6/feloopy/generators/variable/mip_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3742 2023-05-12 17:33:12.000000 feloopy-0.2.6/feloopy/generators/variable/ortools_cp_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3957 2023-05-12 17:33:17.000000 feloopy-0.2.6/feloopy/generators/variable/ortools_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3295 2023-05-12 17:33:21.000000 feloopy-0.2.6/feloopy/generators/variable/picos_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3661 2023-05-12 17:33:25.000000 feloopy-0.2.6/feloopy/generators/variable/pulp_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3508 2023-05-12 17:33:30.000000 feloopy-0.2.6/feloopy/generators/variable/pymprog_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     2705 2023-05-12 17:33:34.000000 feloopy-0.2.6/feloopy/generators/variable/pyomo_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     4882 2023-06-02 13:17:59.000000 feloopy-0.2.6/feloopy/generators/variable/rsome_dro_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     4905 2023-06-02 14:10:39.000000 feloopy-0.2.6/feloopy/generators/variable/rsome_ro_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     4232 2023-05-12 17:33:37.000000 feloopy-0.2.6/feloopy/generators/variable/xpress_variable_generator.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     3540 2023-07-06 07:14:43.000000 feloopy-0.2.6/feloopy/generators/variable_generator.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-07-06 10:24:10.899938 feloopy-0.2.6/feloopy/helpers/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      293 2023-05-12 17:34:12.000000 feloopy-0.2.6/feloopy/helpers/__init__.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1494 2023-05-12 17:34:17.000000 feloopy-0.2.6/feloopy/helpers/empty.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)       96 2023-06-26 08:19:13.000000 feloopy-0.2.6/feloopy/helpers/error.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     8718 2023-07-06 06:52:49.000000 feloopy-0.2.6/feloopy/helpers/formatter.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-07-06 10:24:10.907938 feloopy-0.2.6/feloopy/operators/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      384 2023-05-12 20:17:53.000000 feloopy-0.2.6/feloopy/operators/__init__.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)    11267 2023-07-06 10:14:38.000000 feloopy-0.2.6/feloopy/operators/common.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)        0 2023-06-07 15:13:19.000000 feloopy-0.2.6/feloopy/operators/epsilon.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      380 2023-05-12 17:34:41.000000 feloopy-0.2.6/feloopy/operators/exact.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      472 2023-06-18 16:30:35.000000 feloopy-0.2.6/feloopy/operators/fix_operators.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      473 2023-06-18 16:29:46.000000 feloopy-0.2.6/feloopy/operators/heuristic.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     5436 2023-07-05 18:56:21.000000 feloopy-0.2.6/feloopy/operators/heuristic_operators.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1114 2023-06-18 16:25:00.000000 feloopy-0.2.6/feloopy/operators/math_operators.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1056 2023-06-07 10:52:56.000000 feloopy-0.2.6/feloopy/operators/metric_operators.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)        0 2023-07-04 20:58:08.000000 feloopy-0.2.6/feloopy/operators/pareto.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      471 2023-06-18 16:29:31.000000 feloopy-0.2.6/feloopy/operators/random_operators.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      575 2023-06-18 16:25:13.000000 feloopy-0.2.6/feloopy/operators/set_operators.py
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1907 2023-06-22 15:51:56.000000 feloopy-0.2.6/feloopy/operators/update_operators.py
+drwxrwxr-x   0 keivan    (1000) keivan    (1000)        0 2023-07-06 10:24:10.831937 feloopy-0.2.6/feloopy.egg-info/
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)    10918 2023-07-06 10:24:10.000000 feloopy-0.2.6/feloopy.egg-info/PKG-INFO
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     7242 2023-07-06 10:24:10.000000 feloopy-0.2.6/feloopy.egg-info/SOURCES.txt
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)        1 2023-07-06 10:24:10.000000 feloopy-0.2.6/feloopy.egg-info/dependency_links.txt
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)      328 2023-07-06 10:24:10.000000 feloopy-0.2.6/feloopy.egg-info/requires.txt
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)        8 2023-07-06 10:24:10.000000 feloopy-0.2.6/feloopy.egg-info/top_level.txt
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)       38 2023-07-06 10:24:10.907938 feloopy-0.2.6/setup.cfg
+-rw-rw-r--   0 keivan    (1000) keivan    (1000)     1856 2023-06-27 09:42:23.000000 feloopy-0.2.6/setup.py
```

### Comparing `feloopy-0.2.5/LICENSE` & `feloopy-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/PKG-INFO` & `feloopy-0.2.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,13 @@
-Metadata-Version: 2.1
-Name: feloopy
-Version: 0.2.5
-Summary: FelooPy: An integrated optimization environment for automated operations research in Python.
-Home-page: https://github.com/ktafakkori/feloopy
-Download-URL: https://github.com/ktafakkori/feloopy/releases
-Author: Keivan Tafakkori
-Author-email: k.tafakkori@gmail.com
-Maintainer: Keivan Tafakkori
-Maintainer-email: k.tafakkori@gmail.com
-License: MIT
-Keywords: optimization,machine learning,simulation,operations research,computer science,data science,management science,industrial engineering,supply chain,operations management
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: all_solvers
-Provides-Extra: gurobi
-Provides-Extra: cplex
-Provides-Extra: xpress
-Provides-Extra: linux
-License-File: LICENSE
-
 ### **Introduction**
 
-| FelooPy                                            | [![version code](https://img.shields.io/badge/version-0.2.5-darkgreen.svg)](https://github.com/ktafakkori/feloopy/releases) [![number of users](https://static.pepy.tech/personalized-badge/feloopy?period=total&units=international_system&left_color=grey&right_color=darkgreen&left_text=users)](https://pepy.tech/project/feloopy) ![release date](https://img.shields.io/github/release-date/ktafakkori/feloopy?color=blue) [![monthly Downloads](https://static.pepy.tech/personalized-badge/feloopy?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20downloads%20)](https://pepy.tech/project/feloopy) [![license type](https://img.shields.io/badge/license-MIT-darkred.svg)](https://opensource.org/licenses/MIT) |
+| FelooPy                                            | [![version code](https://img.shields.io/badge/version-0.2.6-darkgreen.svg)](https://github.com/ktafakkori/feloopy/releases) [![number of users](https://static.pepy.tech/personalized-badge/feloopy?period=total&units=international_system&left_color=grey&right_color=darkgreen&left_text=users)](https://pepy.tech/project/feloopy) ![release date](https://img.shields.io/github/release-date/ktafakkori/feloopy?color=blue) [![monthly Downloads](https://static.pepy.tech/personalized-badge/feloopy?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20downloads%20)](https://pepy.tech/project/feloopy) [![license type](https://img.shields.io/badge/license-MIT-darkred.svg)](https://opensource.org/licenses/MIT) |
 | :------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | ![Image description](miscellaneous/logo/logo1.png) | FelooPy (pronounced /fɛlupaɪ/) is a free and open-source Python library for automated operations research that serves as both a hyper-optimization interface and an integrated optimization environment. The name comes from the idea of suggesting practical and applicable solutions for systems, industries, and supply chains, and it also references the importance of loops in programming and algorithm development, and draws similarities to the name "Floppy" to highlight memory efficiency. FelooPy helps operations research scientists achieve their goals using various target, representor, and learner models. In simple words, FelooPy is a unified framework for optimization algorithms, decision-making methods, and modeling and analytical tools. |
-| News                                               | 🎉 _Version 0.2.5 is out: Added new features!_ 🎉                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
+| News                                               | 🎉 _Version 0.2.6 is out: Robustness and stability!_ 🎉                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
 
 ### **Installation**
 
 FelooPy can be installed on Linux-based distributions, Windows, or macOS. It has a few dependencies that should work on all these platforms.
 
 <div align="center">
 
@@ -46,53 +25,53 @@
 <td> Python >= 3.10 </td>
 </tr>
 
 <tr>
 <td> PyPI </td>
 <td>
     
-`pip install feloopy==0.2.5`
+`pip install feloopy==0.2.6`
 </td>
 <td> Python >= 3.10 </td>
 </tr>
 
 <tr>
 <td> Command </td>
 <td>
     
-`!pip install feloopy==0.2.5`
+`!pip install feloopy==0.2.6`
 </td>
 <td> Python >= 3.10 </td>
 </tr>
 
 <tr>
 <td> Script </td>
 <td>
     
 ```python
 import pip
 
 def install(package):
-if hasattr(pip, 'main'):
-pip.main(['install','-U', package])
-else:
-pip._internal.main(['install','-U', package])
+  if hasattr(pip, 'main'):
+    pip.main(['install','-U', package])
+  else:
+    pip._internal.main(['install','-U', package])
 
-install('feloopy')
+install('feloopy==0.2.6')
 
 ````
 </td>
 <td> Python >= 3.10 </td>
 </tr>
 
 <tr>
 <td> Local </td>
 <td>
 
-1. Download the [feloopy-0.2.5.zip][c] file.
+1. Download the [feloopy-0.2.6.zip][c] file.
 2. Extract it into a specific directory.
 3. Open a terminal in that directory.
 4. Type: `pip install .`
 
 </td>
 
 <td> Python >= 3.10 </td>
@@ -110,15 +89,15 @@
 !bash ./py310.sh -b -f -p /usr/local
 !python -m ipykernel install --name "py310" --user
 ````
 
 2. Run this cell and reload (CTRL + R):
 
 ```python
-!pip install feloopy==0.2.5
+!pip install feloopy==0.2.6
 ```
 
 </td>
 
 <td> Python >= 3.10 </td>
 
 </tr>
@@ -143,42 +122,46 @@
 
 ```
 conda create --name feloopy python=3.10
 conda activate feloopy
 pip install feloopy
 ```
 
-FelooPy (v0.2.5) has a few optional dependencies that can be installed using the following commands:
+FelooPy (v0.2.6) has a few optional dependencies that can be installed using the following commands:
 
 * All solvers: `pip install feloopy[all_solvers]`
 * Gurobi: `pip install feloopy[gurobi]`
-* CPLEX: `pip install feloopy[cplex]`
-* XPRESS: `pip install feloopy[xpress]`
-* Linux: `pip install feloopy[linux]` (for multi-objective optimization)
+* Cplex: `pip install feloopy[cplex]`
+* Xpress: `pip install feloopy[xpress]`
+* Linux: `pip install feloopy[linux]` (better support for multi-objective optimization)
 
-For multi-objective optimization, you should use the linux command for installation. However, please note that the optional dependencies for Linux might not work on other operating systems. As a workaround, you can use a Conda-based Python 3.10 interpreter to ensure that optional dependencies for multi-objective optimization are installed correctly.
+For multi-objective optimization, you should use the linux command for installation. However, please note that the optional dependencies for Linux kernel might not work on some operating systems. As a workaround, you can use a Conda-based Python 3.10 interpreter to ensure that optional dependencies for multi-objective optimization are installed correctly.
 
 ### **Features**
 
 FelooPy offers the following key features:
 
 * **Simplest optimization programming language**: Designed to be easy to use, even for those with little or no programming experience.
 * **Modeling, solving and analyzing optimization problems**: Provides a complete suite of tools for modeling, solving and analyzing a wide range of optimization problems.
 * **Exact optimization algorithms**: Supports *107* exact optimization algorithms that guarantee the optimal solution to your problem.
 * **Heuristic optimization algorithms**: Supports *197* heuristic optimization algorithms that can find best possible solutions to complex problems.
 * **Convex optimization algorithms**: Supports *20* convex optimization algorithms that ease tensor- and matrix-form modeling, primarily for convex problems.
 * **Constraint optimization algorithms**: Supports *2* constraint optimization algorithms that can handle a wide range of complex constraints for operational and time-dependent decisions.
-* **Multi-objective optimization algorithms**: Supports *17* multi-objective optimization algorithms, in which objectives might be contradicting or with different numerical units.
+* **Multi-objective optimization algorithms**: Supports *17* multi-objective optimization algorithms, in which objectives might be conflicting or with different numerical units.
 * **Multi-critera decision-making methods**: Supports *41* MCDM algorithms to solve decision problems with expert-based inputs without mathematical modeling.
 * **Solver configurations**: Lets you configure the solver to meet specific requirements.
 * **Auto-encoders for general purpose programming**: Provides auto-encoders to simplify general-purpose programming tasks.
 * **Auto-linearizers for linear programming conversions**: Provides auto-linearizers that can handle mixed-integer non-linear programming problems.
 * **Auto-logic for modeling special constraints**: Provides auto-logic to help you model and solve problems with special constraints.
 * **Auto-sensitivity for analyzing the impact of key parameters**: Provides auto-sensitivity tools to help you analyze the impact of key parameters on your optimization problem.
 
+### **Documentation**
+
+Please refer to https://feloopy.readthedocs.io/en/latest/.
+
 ### **Contributions**
 
 We welcome your contributions to this project, such as reporting bugs, submitting pull requests, testing changes, providing examples, and so on.
 ### **Support FelooPy**
 
 We are committed to continuing the development of FelooPy and would greatly appreciate your support. You can help us by:
 
@@ -214,8 +197,8 @@
 [c]: https://github.com/ktafakkori/feloopy/releases
 [support]: https://ktafakkori.github.io/support/
 
 ### **License**
 
 FelooPy is completely free and open-source and licensed under the [MIT][08] license.
 
-[08]: https://github.com/ktafakkori/feloopy/blob/main/LICENSE
+[08]: https://github.com/ktafakkori/feloopy/blob/main/LICENSE
```

### Comparing `feloopy-0.2.5/README.md` & `feloopy-0.2.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,34 @@
+Metadata-Version: 2.1
+Name: feloopy
+Version: 0.2.6
+Summary: FelooPy: An integrated optimization environment for automated operations research in Python.
+Home-page: https://github.com/ktafakkori/feloopy
+Download-URL: https://github.com/ktafakkori/feloopy/releases
+Author: Keivan Tafakkori
+Author-email: k.tafakkori@gmail.com
+Maintainer: Keivan Tafakkori
+Maintainer-email: k.tafakkori@gmail.com
+License: MIT
+Keywords: optimization,machine learning,simulation,operations research,computer science,data science,management science,industrial engineering,supply chain,operations management
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: all_solvers
+Provides-Extra: gurobi
+Provides-Extra: cplex
+Provides-Extra: xpress
+Provides-Extra: linux
+License-File: LICENSE
+
 ### **Introduction**
 
-| FelooPy                                            | [![version code](https://img.shields.io/badge/version-0.2.5-darkgreen.svg)](https://github.com/ktafakkori/feloopy/releases) [![number of users](https://static.pepy.tech/personalized-badge/feloopy?period=total&units=international_system&left_color=grey&right_color=darkgreen&left_text=users)](https://pepy.tech/project/feloopy) ![release date](https://img.shields.io/github/release-date/ktafakkori/feloopy?color=blue) [![monthly Downloads](https://static.pepy.tech/personalized-badge/feloopy?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20downloads%20)](https://pepy.tech/project/feloopy) [![license type](https://img.shields.io/badge/license-MIT-darkred.svg)](https://opensource.org/licenses/MIT) |
+| FelooPy                                            | [![version code](https://img.shields.io/badge/version-0.2.6-darkgreen.svg)](https://github.com/ktafakkori/feloopy/releases) [![number of users](https://static.pepy.tech/personalized-badge/feloopy?period=total&units=international_system&left_color=grey&right_color=darkgreen&left_text=users)](https://pepy.tech/project/feloopy) ![release date](https://img.shields.io/github/release-date/ktafakkori/feloopy?color=blue) [![monthly Downloads](https://static.pepy.tech/personalized-badge/feloopy?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20downloads%20)](https://pepy.tech/project/feloopy) [![license type](https://img.shields.io/badge/license-MIT-darkred.svg)](https://opensource.org/licenses/MIT) |
 | :------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | ![Image description](miscellaneous/logo/logo1.png) | FelooPy (pronounced /fɛlupaɪ/) is a free and open-source Python library for automated operations research that serves as both a hyper-optimization interface and an integrated optimization environment. The name comes from the idea of suggesting practical and applicable solutions for systems, industries, and supply chains, and it also references the importance of loops in programming and algorithm development, and draws similarities to the name "Floppy" to highlight memory efficiency. FelooPy helps operations research scientists achieve their goals using various target, representor, and learner models. In simple words, FelooPy is a unified framework for optimization algorithms, decision-making methods, and modeling and analytical tools. |
-| News                                               | 🎉 _Version 0.2.5 is out: Added new features!_ 🎉                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
+| News                                               | 🎉 _Version 0.2.6 is out: Robustness and stability!_ 🎉                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
 
 ### **Installation**
 
 FelooPy can be installed on Linux-based distributions, Windows, or macOS. It has a few dependencies that should work on all these platforms.
 
 <div align="center">
 
@@ -25,53 +46,53 @@
 <td> Python >= 3.10 </td>
 </tr>
 
 <tr>
 <td> PyPI </td>
 <td>
     
-`pip install feloopy==0.2.5`
+`pip install feloopy==0.2.6`
 </td>
 <td> Python >= 3.10 </td>
 </tr>
 
 <tr>
 <td> Command </td>
 <td>
     
-`!pip install feloopy==0.2.5`
+`!pip install feloopy==0.2.6`
 </td>
 <td> Python >= 3.10 </td>
 </tr>
 
 <tr>
 <td> Script </td>
 <td>
     
 ```python
 import pip
 
 def install(package):
-if hasattr(pip, 'main'):
-pip.main(['install','-U', package])
-else:
-pip._internal.main(['install','-U', package])
+  if hasattr(pip, 'main'):
+    pip.main(['install','-U', package])
+  else:
+    pip._internal.main(['install','-U', package])
 
-install('feloopy')
+install('feloopy==0.2.6')
 
 ````
 </td>
 <td> Python >= 3.10 </td>
 </tr>
 
 <tr>
 <td> Local </td>
 <td>
 
-1. Download the [feloopy-0.2.5.zip][c] file.
+1. Download the [feloopy-0.2.6.zip][c] file.
 2. Extract it into a specific directory.
 3. Open a terminal in that directory.
 4. Type: `pip install .`
 
 </td>
 
 <td> Python >= 3.10 </td>
@@ -89,15 +110,15 @@
 !bash ./py310.sh -b -f -p /usr/local
 !python -m ipykernel install --name "py310" --user
 ````
 
 2. Run this cell and reload (CTRL + R):
 
 ```python
-!pip install feloopy==0.2.5
+!pip install feloopy==0.2.6
 ```
 
 </td>
 
 <td> Python >= 3.10 </td>
 
 </tr>
@@ -122,42 +143,46 @@
 
 ```
 conda create --name feloopy python=3.10
 conda activate feloopy
 pip install feloopy
 ```
 
-FelooPy (v0.2.5) has a few optional dependencies that can be installed using the following commands:
+FelooPy (v0.2.6) has a few optional dependencies that can be installed using the following commands:
 
 * All solvers: `pip install feloopy[all_solvers]`
 * Gurobi: `pip install feloopy[gurobi]`
-* CPLEX: `pip install feloopy[cplex]`
-* XPRESS: `pip install feloopy[xpress]`
-* Linux: `pip install feloopy[linux]` (for multi-objective optimization)
+* Cplex: `pip install feloopy[cplex]`
+* Xpress: `pip install feloopy[xpress]`
+* Linux: `pip install feloopy[linux]` (better support for multi-objective optimization)
 
-For multi-objective optimization, you should use the linux command for installation. However, please note that the optional dependencies for Linux might not work on other operating systems. As a workaround, you can use a Conda-based Python 3.10 interpreter to ensure that optional dependencies for multi-objective optimization are installed correctly.
+For multi-objective optimization, you should use the linux command for installation. However, please note that the optional dependencies for Linux kernel might not work on some operating systems. As a workaround, you can use a Conda-based Python 3.10 interpreter to ensure that optional dependencies for multi-objective optimization are installed correctly.
 
 ### **Features**
 
 FelooPy offers the following key features:
 
 * **Simplest optimization programming language**: Designed to be easy to use, even for those with little or no programming experience.
 * **Modeling, solving and analyzing optimization problems**: Provides a complete suite of tools for modeling, solving and analyzing a wide range of optimization problems.
 * **Exact optimization algorithms**: Supports *107* exact optimization algorithms that guarantee the optimal solution to your problem.
 * **Heuristic optimization algorithms**: Supports *197* heuristic optimization algorithms that can find best possible solutions to complex problems.
 * **Convex optimization algorithms**: Supports *20* convex optimization algorithms that ease tensor- and matrix-form modeling, primarily for convex problems.
 * **Constraint optimization algorithms**: Supports *2* constraint optimization algorithms that can handle a wide range of complex constraints for operational and time-dependent decisions.
-* **Multi-objective optimization algorithms**: Supports *17* multi-objective optimization algorithms, in which objectives might be contradicting or with different numerical units.
+* **Multi-objective optimization algorithms**: Supports *17* multi-objective optimization algorithms, in which objectives might be conflicting or with different numerical units.
 * **Multi-critera decision-making methods**: Supports *41* MCDM algorithms to solve decision problems with expert-based inputs without mathematical modeling.
 * **Solver configurations**: Lets you configure the solver to meet specific requirements.
 * **Auto-encoders for general purpose programming**: Provides auto-encoders to simplify general-purpose programming tasks.
 * **Auto-linearizers for linear programming conversions**: Provides auto-linearizers that can handle mixed-integer non-linear programming problems.
 * **Auto-logic for modeling special constraints**: Provides auto-logic to help you model and solve problems with special constraints.
 * **Auto-sensitivity for analyzing the impact of key parameters**: Provides auto-sensitivity tools to help you analyze the impact of key parameters on your optimization problem.
 
+### **Documentation**
+
+Please refer to https://feloopy.readthedocs.io/en/latest/.
+
 ### **Contributions**
 
 We welcome your contributions to this project, such as reporting bugs, submitting pull requests, testing changes, providing examples, and so on.
 ### **Support FelooPy**
 
 We are committed to continuing the development of FelooPy and would greatly appreciate your support. You can help us by:
 
@@ -193,8 +218,8 @@
 [c]: https://github.com/ktafakkori/feloopy/releases
 [support]: https://ktafakkori.github.io/support/
 
 ### **License**
 
 FelooPy is completely free and open-source and licensed under the [MIT][08] license.
 
-[08]: https://github.com/ktafakkori/feloopy/blob/main/LICENSE
+[08]: https://github.com/ktafakkori/feloopy/blob/main/LICENSE
```

### Comparing `feloopy-0.2.5/feloopy/__init__.py` & `feloopy-0.2.6/feloopy/__init__.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/heuristic/DE.py` & `feloopy-0.2.6/feloopy/algorithms/heuristic/DE.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 '''
  # @ Author: Keivan Tafakkori
  # @ Created: 2023-05-11
- # @ Modified: 2023-05-12
+ # @ Modified: 2023-07-06
  # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
 
+
 import numpy as np
 import warnings as wn
 
 wn.filterwarnings("ignore")
 
 
 class DE:
```

### Comparing `feloopy-0.2.5/feloopy/algorithms/heuristic/GA.py` & `feloopy-0.2.6/feloopy/algorithms/heuristic/GA.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
  # @ Author: Keivan Tafakkori
  # @ Created: 2023-05-11
- # @ Modified: 2023-05-12
+ # @ Modified: 2023-07-06
  # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
```

### Comparing `feloopy-0.2.5/feloopy/algorithms/heuristic/GWO.py` & `feloopy-0.2.6/feloopy/algorithms/heuristic/GWO.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 '''
  # @ Author: Keivan Tafakkori
  # @ Created: 2023-05-11
- # @ Modified: 2023-05-12
+ # @ Modified: 2023-07-06
  # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
+
 import numpy as np
 import warnings as wn
 
 wn.filterwarnings("ignore")
 
 
 class GWO:
```

### Comparing `feloopy-0.2.5/feloopy/algorithms/heuristic/SA.py` & `feloopy-0.2.6/feloopy/algorithms/heuristic/SA.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
  # @ Author: Keivan Tafakkori
  # @ Created: 2023-05-11
- # @ Modified: 2023-05-12
+ # @ Modified: 2023-07-06
  # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
 import numpy as np
```

### Comparing `feloopy-0.2.5/feloopy/algorithms/heuristic/TS.py` & `feloopy-0.2.6/feloopy/algorithms/heuristic/TS.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
  # @ Author: Keivan Tafakkori
  # @ Created: 2023-05-11
- # @ Modified: 2023-05-12
+ # @ Modified: 2023-07-06
  # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
 import numpy as np
@@ -24,14 +24,15 @@
         self.s = s
         self.t = t
         self.c = c
         self.features_cols = [0, self.f]
         self.status_col = [-2]
         self.reward_col = [-1]
         self.single_objective_tot = self.f + 1 + 1
+        self.solve = self.run
 
     def run(self, evaluate):
 
         self.evaluate = evaluate
         self.initialize()
         for self.it_no in range(0, self.s):
             self.update()
```

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/__init__.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/__init__.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/ahp.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/ahp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 '''
  # @ Author: Keivan Tafakkori
  # @ Created: 2023-05-15
- # @ Modified: 2023-05-15
+ # @ Modified: 2023-07-06
  # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
+
 from typing import Dict
 import numpy as np
 
 
 def mcdm_ahp(dataset: np.ndarray, weight_derivation: str, verbose: bool = False) -> Dict[str, np.ndarray]:
     """
     Computes weights for a set of criteria using the Analytic Hierarchy Process (AHP).
```

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/aras.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/aras.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/borda.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/borda.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/bwm.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/bwm.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/codas.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/codas.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/copras.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/copras.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/critic.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/critic.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/dematel.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/dematel.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/edas.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/edas.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/elecre_i.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/elecre_i.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/electre_i_s.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/electre_i_s.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/electre_i_v.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/electre_i_v.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/electre_ii.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/electre_ii.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/electre_iii.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/electre_iii.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/electre_iv.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/electre_iv.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/electre_tri.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/electre_tri.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/fahp.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/fahp.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/fdematel.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/fdematel.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/fedeas.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/fedeas.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/ftopsis.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/ftopsis.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/fvikor.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/fvikor.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/gra.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/gra.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/idocriw.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/idocriw.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/mabac.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/mabac.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/maut.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/maut.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/moora.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/moora.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/moosra.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/moosra.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/multimoora.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/multimoora.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_gaia.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/promethee_gaia.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_i.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/promethee_i.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_ii.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/promethee_ii.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_iii.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/promethee_iii.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_iv.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/promethee_iv.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_v.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/promethee_v.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/promethee_vi.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/promethee_vi.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/saw.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/saw.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/smart.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/smart.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/topsis.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/topsis.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/vikor.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/vikor.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/waspas.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/waspas.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/algorithms/mcdm/wings.py` & `feloopy-0.2.6/feloopy/algorithms/mcdm/wings.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/feloopy.py` & `feloopy-0.2.6/feloopy/feloopy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,358 +1,439 @@
 '''
  # @ Author: Keivan Tafakkori
- # @ Created: 2023-05-11
- # @ Modified: 2023-05-25
+ # @ Created: 2023-06-28
+ # @ Modified: 2023-07-02
  # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
 from .helpers.empty import *
 from .helpers.error import *
 from .helpers.formatter import *
 from .operators.set_operators import *
 from .operators.math_operators import *
-from .operators.count_operators import *
 from .operators.update_operators import *
 from .operators.random_operators import *
 from .operators.heuristic_operators import *
 from .operators.fix_operators import *
 from .operators.epsilon import *
 from .operators.metric_operators import *
 from collections import defaultdict
-        
 
 import warnings
 import itertools as it
 import math as mt
 import numpy as np
 from tabulate import tabulate as tb
 from typing import List, Tuple, Optional
 import sys
 
+
+
 warnings.filterwarnings("ignore")
 
 avar = defaultdict()
 
 class Model:
 
-    # Method for the modeling envrionment.
+    def __init__(self, solution_method, model_name, interface_name, agent=None, scens=1, no_agents= None, key=None):
 
-    def __init__(self, solution_method, model_name, interface_name, agent=None, key=None):
         """
         Creates and returns the modeling environment.
 
         Args:
             solution_method (str): Desired solution (optimization) method.
             model_name (str): Name of this model.
             interface_name (str): Desired interface name.
             agent (X, optional): Input of the representor model. Default: None. 
+            scens (int, optional): Number of uncertainty scenarios, which can also be an array containing scenario indices. Default: 1.
             key (number, optional): Key for the random number generator. Default: None.
         """
 
-        if solution_method == 'constraint': solution_method = 'exact'
-        self.binary_variable = self.add_binary_variable = self.boolean_variable = self.add_boolean_variable = self.bvar
-        self.positive_variable = self.add_positive_variable = self.pvar
-        self.integer_variable = self.add_integer_variable = self.ivar
-        self.free_variable = self.add_free_variable = self.fvar
-        self.sequential_variable = self.add_sequential_variable = self.svar
-        self.positive_tensor_variable = self.add_positive_tensor_variable = self.ptvar
-        self.binary_tensor_variable = self.add_binary_tensor_variable = self.add_boolean_tensor_variable = self.boolean_tensor_variable = self.btvar
-        self.integer_tensor_variable = self.add_integer_tensor_variable = self.itvar
-        self.free_tensor_variable = self.add_free_tensor_variable = self.ftvar
-        self.dependent_variable = self.add_dependent_variable = self.dvar
-        self.objective = self.reward = self.hypothesis = self.fitness = self.goal = self.add_objective = self.obj
-        self.constraint = self.equation = self.add_constraint = self.add_equation = self.con
+        self.binary_variable = self.binary = self.bool = self.add_bool = self.add_binary = self.add_binary_variable = self.boolean_variable = self.add_boolean_variable = self.bvar
+        self.positive_variable = self.positive = self.add_positive = self.add_positive_variable = self.pvar
+        self.integer_variable = self.integer = self.add_integer =  self.add_integer_variable = self.ivar
+        self.free_variable = self.free = self.float = self.add_free = self.add_float = self.real = self.add_real = self.add_free_variable = self.fvar
+        self.sequential_variable = self.sequence = self.sequential = self.add_sequence = self.add_sequential = self.add_sequential_variable = self.svar
+        self.positive_tensor_variable = self.positive_tensor = self.add_positive_tensor = self.add_positive_tensor_variable = self.ptvar
+        self.binary_tensor_variable = self.binary_tensor = self.add_binary_tensor = self.add_binary_tensor_variable = self.add_boolean_tensor_variable = self.boolean_tensor_variable = self.btvar
+        self.integer_tensor_variable = self.integer_tensor = self.add_integer_tensor = self.add_integer_tensor_variable = self.itvar
+        self.free_tensor_variable = self.free_tensor = self.float_tensor = self.add_free_tensor = self.add_float_tensor = self.add_free_tensor_variable = self.ftvar
+        self.random_variable = self.add_random_variable = self.rvar
+        self.random_tensor_variable = self.add_random_tensor_variable = self.rtvar
+        self.dependent_variable = self.array = self.add_array = self.add_dependent_variable = self.dvar
+        self.objective = self.reward = self.hypothesis = self.fitness = self.goal = self.add_objective = self.loss = self.gain = self.obj 
+        self.constraint = self.equation = self.add_constraint = self.add_equation = self.st = self.subject_to = self.cb = self.computed_by = self.penalize = self.pen = self.eq = self.con
         self.solve = self.implement = self.run = self.optimize = self.sol
         self.get_obj = self.get_objective
         self.get_stat = self.get_status
         self.get_var = self.value = self.get = self.get_variable
         self.dis = self.dis_var = self.display = self.show = self.print = self.display_variable = self.dis_variable
         self.status = self.show_status = self.dis_status
         self.objective_value = self.show_objective = self.display_objective = self.dis_obj
+            
         self.random = create_random_number_generator(key)
-        self.avar= self.coll()
+        self.avar = self.coll()
 
-        match solution_method:
-            case 'exact':
-                self.features = {
-                    'solution_method': 'exact',
-                    'model_name': model_name,
-                    'interface_name': interface_name,
-                    'solver_name': None,
-                    'constraints': [],
-                    'constraint_labels': [],
-                    'objectives': [],
-                    'objective_labels': [],
-                    'directions': [],
-                    'positive_variable_counter': [0, 0],
-                    'integer_variable_counter': [0, 0],
-                    'binary_variable_counter': [0, 0],
-                    'free_variable_counter': [0, 0],
-                    'total_variable_counter': [0, 0],
-                    'objective_counter': [0, 0],
-                    'constraint_counter': [0, 0],
-                    'objective_being_optimized': 0,
+        self.no_agents = no_agents
+
+        if interface_name == 'rsome_ro':
+            from rsome import ro as robust_tools
+        
+        if interface_name == 'rsome_dro':
+            from rsome import dro as robust_tools
+
+        if solution_method == 'constraint':
+
+            if interface_name == 'cplex_cp':
+                import docplex.cp.model as constraint_tools
+            if interface_name == 'ortools_cp':
+                import ortools.sat.python.cp_model as constraint_tools
+            self.solution_method_was = 'constraint'
+            solution_method = 'exact'
+
+        elif solution_method == 'convex':
+
+            if interface_name == 'cvxpy':
+                import cvxpy as convex_tools
+            if interface_name == 'gurobi':
+                import gurobipy as convex_tools
+            self.solution_method_was = 'convex'
+            solution_method = 'exact'
+        else:
+            self.solution_method_was=None
+
+        self.features = {
+            'solution_method': solution_method,
+            'model_name': model_name,
+            'interface_name': interface_name,
+            'solver_name': None,
+            'constraints': [],
+            'constraint_labels': [],
+            'objectives': [],
+            'objective_labels': [],
+            'directions': [],
+            'positive_variable_counter': [0, 0],
+            'integer_variable_counter': [0, 0],
+            'binary_variable_counter': [0, 0],
+            'free_variable_counter': [0, 0],
+            'event_variable_counter': [0, 0],
+            'sequential_variable_counter': [0,0],
+            'dependent_variable_counter': [0,0],
+            'total_variable_counter': [0, 0],
+            'objective_counter': [0, 0],
+            'constraint_counter': [0, 0],
+            'objective_being_optimized': 0,
+            'scens': scens,
+        }
+
+        if solution_method == 'heuristic':
+
+            self.agent = agent
+
+            self.features.update(
+                {
+                'agent_status': self.agent[0],
+                'variable_spread': self.agent[2] if self.agent[0] != 'idle' else dict(),
+                'variable_type': dict() if self.agent[0] == 'idle' else None,
+                'variable_bound': dict() if self.agent[0] == 'idle' else None,
+                'variable_dim': dict() if self.agent[0] == 'idle' else None,
+                'pop_size': 1 if self.agent[0] == 'idle' else len(self.agent[1]),
+                'penalty_coefficient': 0 if self.agent[0] == 'idle' else self.agent[3],
+                'vectorized': None,
                 }
-                self.mainvars = self.coll()
-                self.maindims = self.coll()
-                from .generators import model_generator
-                self.model = model_generator.generate_model(self.features)
-                self.sm = self.model
-            case 'heuristic':
-                self.agent = agent
-                if self.agent[0] == 'idle':
-                    self.features = {
-                        'agent_status': 'idle',
-                        'solution_method': 'heuristic',
-                        'model_name': model_name,
-                        'interface_name': interface_name,
-                        'solver_name': None,
-                        'constraints': [],
-                        'constraint_labels': [],
-                        'objectives': [],
-                        'objective_labels': [],
-                        'directions': [],
-                        'positive_variable_counter': [0, 0],
-                        'integer_variable_counter': [0, 0],
-                        'binary_variable_counter': [0, 0],
-                        'free_variable_counter': [0, 0],
-                        'total_variable_counter': [0, 0],
-                        'objective_counter': [0, 0],
-                        'constraint_counter': [0, 0],
-                        'variable_spread': dict(),
-                        'variable_type': dict(),
-                        'variable_bound': dict(),
-                        'variable_dim': dict(),
-                        'pop_size': 1,
-                        'penalty_coefficient': 0,
-                        'vectorized': None,
-                        'objective_being_optimized': 0,
-                    }
-                elif self.agent[0] == 'feasibility_check':
-                    self.features = {
-                        'agent_status': 'feasibility_check',
-                        'solution_method': 'heuristic',
-                        'constraints': [],
-                        'objectives': [],
-                        'objective_counter': [0, 0],
-                        'interface_name': interface_name,
-                        'variable_spread': self.agent[2],
-                        'pop_size': len(self.agent[1]),
-                        'penalty_coefficient': self.agent[3],
-                        'vectorized': None,
-                        'objective_being_optimized': 0,
-                        'directions': []
-                    }
-                    self.agent = self.agent[1].copy()
-                else:
-                    self.features = {
-                        'agent_status': 'active',
-                        'solution_method': 'heuristic',
-                        'constraints': [],
-                        'objectives': [],
-                        'objective_counter': [0, 0],
-                        'interface_name': interface_name,
-                        'variable_spread': self.agent[2],
-                        'pop_size': len(self.agent[1]),
-                        'penalty_coefficient': self.agent[3],
-                        'vectorized': None,
-                        'objective_being_optimized': 0,
-                        'directions': []
-                    }
-                    self.agent = self.agent[1].copy()
-                match self.features['interface_name']:
-                    case 'mealpy': self.features['vectorized'] = False
-                    case 'pymultiobjective': self.features['vectorized'] = False
-                    case 'feloopy': self.features['vectorized'] = True
+            )
+
+            self.features['vectorized'] = interface_name in ['feloopy', 'pymoo']
+
+            if self.agent[0] != 'idle':
+
+                self.agent = self.agent[1].copy()
+
+        if solution_method == 'exact':
+
+            self.mainvars = self.coll()
+            self.maindims = self.coll()
+
+            from .generators import model_generator
+            self.model = model_generator.generate_model(self.features)
+            self.sm = self.link_to_interface = self.lti = self.model
 
     def __getitem__(self, agent):
+
         """
         Returns the required features of the model object.
 
         Args:
             agent (X): Input of the representor model/instance.
         """
 
-        if self.features['agent_status'] == 'idle':
+        agent_status = self.features['agent_status']
+        vectorized = self.features['vectorized']
+        interface_name = self.features['interface_name']
+
+        if agent_status == 'idle':
             return self
-        elif self.features['agent_status'] == 'feasibility_check':
-            if self.features['penalty_coefficient'] == 0:
-                return 'feasible (unconstrained)'
-            else:
-                if self.penalty > 0:
-                    return 'infeasible (constrained)'
-                else:
-                    return 'feasible (constrained)'
+        elif agent_status == 'feasibility_check':
+            return self.feasibility_check()
         else:
-            if self.features['vectorized']:
-                return self.agent
-            else:
-                return self.response
+            return self.get_result(vectorized, interface_name)
+
+    def feasibility_check(self):
+
+        if self.features['penalty_coefficient'] == 0:
+            return 'feasible (unconstrained)'
+        else:
+            return 'infeasible (constrained)' if self.penalty > 0 else 'feasible (constrained)'
+
+    def get_result(self, vectorized, interface_name):
+
+        if vectorized:
+            return self.agent if interface_name == 'feloopy' else self.sing_result
+        else:
+            return self.response
 
     # Methods for variables definitions.
 
     def coll(dim):
+
         """
+
         Creates and returns an empty collection (dictionary) of variables.
+
         """
+
         from collections import defaultdict
         return defaultdict()
 
-    def btvar(self, name, dim=0, bound=[0, 1]):
+    #Tensors
+
+    def ftvar(self, name, shape=0, bound=[None, None]):
         """
-        Creates and returns a tensor-like binary variable.
+        Creates and returns a tensor-like free variable.
 
         Args:
             name (str): Name of this variable.
-            dim (list, optional): Dimensions of this variable. Default: 0.
-            bound (list, optional): Bounds of this variable. Default: [0, 1].
+            shape (list, optional): Shape of this variable. Default: 0.
+            bound (list, optional): Bounds of this variable. Default: [None, None].
         """
-        
-        dim = fix_dims(dim)
-        self.features = update_variable_features(
-            name, dim, bound, 'binary_variable_counter', self.features)
-
-        match self.features['solution_method']:
-
-            case 'exact':
-
-                from .generators import variable_generator
-                self.mainvars[("btvar",name)] = variable_generator.generate_variable(self.features['interface_name'], self.model, 'btvar', name, bound, dim)
-                self.maindims[name] = dim
-                return self.mainvars[("btvar",name)]
+        dim = fix_dims(shape)
+        self.features = update_variable_features(name, dim, bound, 'free_variable_counter', self.features)
+        if self.features['solution_method'] == 'exact':
+            
+            from .generators import variable_generator
+            self.mainvars[("ftvar", name)] = variable_generator.generate_variable(self.features['interface_name'], self.model, 'ftvar', name, bound, dim)
+            self.maindims[name] = dim
+            return self.mainvars[("ftvar", name)]
 
-    def ptvar(self, name, dim=0, bound=[0, None]):
+    def ptvar(self, name, shape=0, bound=[0, None]):
         """
         Creates and returns a tensor-like positive variable.
 
         Args:
             name (str): Name of this variable.
-            dim (list, optional): Dimensions of this variable. Default: 0.
+            shape (list, optional): Shape of this variable. Default: 0.
             bound (list, optional): Bounds of this variable. Default: [0, None].
         """
+        dim = fix_dims(shape)
+        self.features = update_variable_features(name, dim, bound, 'positive_variable_counter', self.features)
+        if self.features['solution_method'] == 'exact':
+            from .generators import variable_generator
+            self.mainvars[("ptvar", name)] = variable_generator.generate_variable(self.features['interface_name'], self.model, 'ptvar', name, bound, dim)
+            self.maindims[name] = dim
+            if self.features['interface_name'] in ['rsome_ro', 'rsome_dro', 'cvxpy']:
+                self.con(self.mainvars[("ptvar", name)] >= 0)
+                if bound[1]!=None:
+                    self.con(self.mainvars[("ptvar", name)] <= bound[1])
+            return self.mainvars[("ptvar", name)]
 
-        dim = fix_dims(dim)
-        self.features = update_variable_features(
-            name, dim, bound, 'positive_variable_counter', self.features)
-
-        match self.features['solution_method']:
-
-            case 'exact':
-
-                from .generators import variable_generator
-                self.mainvars[("ptvar",name)] = variable_generator.generate_variable(self.features['interface_name'], self.model, 'ptvar', name, bound, dim)
-                self.maindims[name] = dim
-                return self.mainvars[("ptvar",name)]
-
-    def itvar(self, name, dim=0, bound=[0, None]):
+    def itvar(self, name, shape=0, bound=[0, None]):
         """
         Creates and returns a tensor-like integer variable.
 
         Args:
             name (str): Name of this variable.
-            dim (list, optional): Dimensions of this variable. Default: 0.
+            shape (list, optional): Shape of this variable. Default: 0.
             bound (list, optional): Bounds of this variable. Default: [0, None].
         """
-
-        dim = fix_dims(dim)
-        self.features = update_variable_features(
-            name, dim, bound, 'integer_variable_counter', self.features)
-
-        match self.features['solution_method']:
-
-            case 'exact':
-
-                from .generators import variable_generator
-                self.mainvars[("ptvar",name)] = variable_generator.generate_variable(self.features['interface_name'], self.model, 'itvar', name, bound, dim)
-                self.maindims[name] = dim
-                return self.mainvars[("ptvar",name)]
-
-        return self.vars[name]
-
-    def ftvar(self, name, dim=0, bound=[None, None]):
+        dim = fix_dims(shape)
+        self.features = update_variable_features(name, dim, bound, 'integer_variable_counter', self.features)
+        if self.features['solution_method'] == 'exact':
+            from .generators import variable_generator
+            self.mainvars[("itvar", name)] = variable_generator.generate_variable(self.features['interface_name'], self.model, 'itvar', name, bound, dim)
+            self.maindims[name] = dim
+            return self.mainvars[("itvar", name)]
+              
+    def btvar(self, name, shape=0, bound=[0, 1]):
         """
-        Creates and returns a tensor-like free variable.
-
+        Creates and returns a tensor-like binary variable.
         Args:
             name (str): Name of this variable.
-            dim (list, optional): Dimensions of this variable. Default: 0.
-            bound (list, optional): Bounds of this variable. Default: [None, None].
+            shape (list, optional): Shape of this variable. Default: 0.
+            bound (list, optional): Bounds of this variable. Default: [0, 1].
         """
+        dim = fix_dims(shape)
+        self.features = update_variable_features(name, dim, bound, 'binary_variable_counter', self.features)
+        if self.features['solution_method'] == 'exact':
+            from .generators import variable_generator
+            self.mainvars[("btvar", name)] = variable_generator.generate_variable(self.features['interface_name'], self.model, 'btvar', name, bound, dim)
+            self.maindims[name] = dim
+            return self.mainvars[("btvar", name)]
 
-        dim = fix_dims(dim)
-        self.features = update_variable_features(
-            name, dim, bound, 'free_variable_counter', self.features)
+    # Tensor collections
 
-        match self.features['solution_method']:
+    def cftvar(self, name, indices, shape=0, bound=[None,None]):
+        """
+        This method creates a dictionary of free (float) tensor variables with given names and indices.
+        
+        Parameters:
+            name (str): The base name for the variables.
+            indices (list): The indices for the variables.
+            shape (dict): The shapes for the variables. Defaults to 0 for all indices if not provided as a dictionary.
+            bound (dict): The bounds for the variables. Defaults to [None, None] for all indices if not provided as a dictionary.
+
+        Returns:
+            dict: A dictionary where each key is an index from 'indices' and the corresponding value is a float tensor variable with the name derived from 'name' and the index.
+        """
+        if type(bound)!=dict: bound = {i: bound for i in indices}
+        if type(shape)!=dict: shape = {i: shape for i in indices}
+        return {i: self.ftvar(name+f"[{i}]".replace("(", "").replace(")", ""), shape=shape[i], bound=bound[i]) for i in indices}
 
-            case 'exact':
+    def cptvar(self, name, indices, shape=0, bound=[0, None]):
+        """
+        This method creates a dictionary of positive tensor variables with given names and indices.
+        
+        Parameters:
+            name (str): The base name for the variables.
+            indices (list): The indices for the variables.
+            shape (dict): The shapes for the variables. Defaults to 0 for all indices if not provided as a dictionary.
+            bound (dict): The bounds for the variables. Defaults to [0, None] for all indices if not provided as a dictionary.
+
+        Returns:
+            dict: A dictionary where each key is an index from 'indices' and the corresponding value is a positive tensor variable with the name derived from 'name' and the index.
+        """
+        if type(bound)!=dict: bound = {i: bound for i in indices}
+        if type(shape)!=dict: shape = {i: shape for i in indices}
+        return {i: self.ptvar(name+f"[{i}]".replace("(", "").replace(")", ""), shape=shape[i], bound=bound[i]) for i in indices}
 
-                from .generators import variable_generator
-                self.mainvars[("ftvar",name)] = variable_generator.generate_variable(self.features['interface_name'], self.model, 'ftvar', name, bound, dim)
-                self.maindims[name] = dim
-                return self.mainvars[("ftvar",name)]
+    def citvar(self, name, indices, shape=0, bound=[0, None]):
+        """
+        This method creates a dictionary of integer tensor variables with given names and indices.
+        
+        Parameters:
+            name (str): The base name for the variables.
+            indices (list): The indices for the variables.
+            shape (dict): The shapes for the variables. Defaults to 0 for all indices if not provided as a dictionary.
+            bound (dict): The bounds for the variables. Defaults to [0, None] for all indices if not provided as a dictionary.
+
+        Returns:
+            dict: A dictionary where each key is an index from 'indices' and the corresponding value is an integer tensor variable with the name derived from 'name' and the index.
+        """
+        if type(bound)!=dict: bound = {i: bound for i in indices}
+        if type(shape)!=dict: shape = {i: shape for i in indices}
+        return {i: self.itvar(name+f"[{i}]".replace("(", "").replace(")", ""), shape=shape[i], bound=bound[i]) for i in indices}
 
-    def bvar(self, name, dim=0, bound=[0, 1]):
+    def cbtvar(self, name, indices, shape=0, bound=[0,1]):
         """
-        Creates and returns a binary variable.
+        This method creates a dictionary of binary tensor variables with given names and indices.
+        
+        Parameters:
+            name (str): The base name for the variables.
+            indices (list): The indices for the variables.
+            shape (dict): The shapes for the variables. Defaults to 0 for all indices if not provided as a dictionary.
+            bound (dict): The bounds for the variables. Defaults to [0, 1] for all indices if not provided as a dictionary.
+
+        Returns:
+            dict: A dictionary where each key is an index from 'indices' and the corresponding value is a binary tensor variable with the name derived from 'name' and the index.
+        """
+        if type(bound)!=dict: bound = {i: bound for i in indices}
+        if type(shape)!=dict: shape = {i: shape for i in indices}
+        return {i: self.btvar(name+f"[{i}]".replace("(", "").replace(")", ""), shape=shape[i], bound=bound[i]) for i in indices}
+       
+    # Normal variables
 
-        Args:
-            name (str): Name of this variable.
-            dim (list, optional): Dimensions of this variable. Default: 0.
-            bound (list, optional): Bounds of this variable. Default: [0, 1].
+    def fvar(self, name, dim=0, bound=[None, None]):
+
+        """
+        `fvar` method is used to create and return a free variable.
+
+        Parameters:
+        - name (str): Name.
+        - dim (list, optional): Dimensions. Default is 0.
+        - bound (list, optional): Lower and upper bounds. Default is [None, None]. Required for heuristic optimization.
+
+        Returns:
+        - variable: A free variable.
         """
 
         dim = fix_dims(dim)
-        self.features = update_variable_features(
-            name, dim, bound, 'binary_variable_counter', self.features)
+
+        self.features = update_variable_features(name, dim, bound, 'free_variable_counter', self.features)
 
         match self.features['solution_method']:
 
             case 'exact':
 
                 from .generators import variable_generator
-                self.mainvars[("bvar",name)] = variable_generator.generate_variable(self.features['interface_name'], self.model, 'bvar', name, bound, dim)
+                self.mainvars[("fvar",name)] = variable_generator.generate_variable(self.features['interface_name'], self.model, 'fvar', name, bound, dim)
                 self.maindims[name] = dim
-                return self.mainvars[("bvar",name)]
+                return self.mainvars[("fvar",name)]
 
             case 'heuristic':
-
-                return generate_heuristic_variable(self.features, 'bvar', name, dim, bound, self.agent)
-
+                
+                return generate_heuristic_variable(self.features, 'fvar', name, dim, bound, self.agent,self.no_agents)
+            
     def pvar(self, name, dim=0, bound=[0, None]):
+
         """
         Creates and returns a positive variable.
 
         Args:
             name (str): Name of this variable.
             dim (list, optional): Dimensions of this variable. Default: 0.
             bound (list, optional): Bounds of this variable. Default: [0, None].
         """
 
         dim = fix_dims(dim)
-        self.features = update_variable_features(
-            name, dim, bound, 'positive_variable_counter', self.features)
+        self.features = update_variable_features(name, dim, bound, 'positive_variable_counter', self.features)
 
         match self.features['solution_method']:
 
             case 'exact':
 
                 from .generators import variable_generator
                 self.mainvars[("pvar",name)] = variable_generator.generate_variable(self.features['interface_name'], self.model, 'pvar', name, bound, dim)
                 self.maindims[name] = dim
+
+                if self.features['interface_name'] in ['rsome_ro', 'rsome_dro', 'cvxpy']:
+                    if dim==0:
+                        self.con(self.mainvars[("pvar",name)]>=0)
+                        if bound[1]!=None:
+                            self.con(self.mainvars[("pvar",name)]<=bound[1])
+                    elif len(dim)==1:
+                        for i in dim[0]:
+                            self.con(self.mainvars[("pvar",name)][i]>=0)
+                            if bound[1]!=None:
+                                self.con(self.mainvars[("pvar",name)][i]<=bound[1])
+                    else:
+                        for i in it.product(*tuple(dim)):
+                            self.con(self.mainvars[("pvar",name)][i]>=0)
+                            if bound[1]!=None:
+                                self.con(self.mainvars[("pvar",name)][i]<=bound[1])
+
                 return self.mainvars[("pvar",name)]
 
             case 'heuristic':
 
-                return generate_heuristic_variable(self.features, 'pvar', name, dim, bound, self.agent)
+                return generate_heuristic_variable(self.features, 'pvar', name, dim, bound, self.agent,self.no_agents)
 
     def ivar(self, name, dim=0, bound=[0, None]):
+
         """
         Creates and returns an integer variable.
 
         Args:
             name (str): Name of this variable.
             dim (list, optional): Dimensions of this variable. Default: 0.
             bound (list, optional): Bounds of this variable. Default: [0, None].
@@ -364,310 +445,644 @@
         match self.features['solution_method']:
 
             case 'exact':
 
                 from .generators import variable_generator
                 self.mainvars[("ivar",name)] = variable_generator.generate_variable(self.features['interface_name'], self.model, 'ivar', name, bound, dim)
                 self.maindims[name] = dim
+
+                if self.features['interface_name'] in ['rsome_ro', 'rsome_dro', 'cvxpy']:
+                    if dim==0:
+                        self.con(self.mainvars[("ivar",name)]>=0)
+                        if bound[1]!=None:
+                            self.con(self.mainvars[("ivar",name)]<=bound[1])
+                    elif len(dim)==1:
+                        for i in dim[0]:
+                            self.con(self.mainvars[("ivar",name)][i]>=0)
+                            if bound[1]!=None:
+                                self.con(self.mainvars[("ivar",name)][i]<=bound[1])
+                    else:
+                        for i in it.product(*tuple(dim)):
+                            self.con(self.mainvars[("ivar",name)][i]>=0)
+                            if bound[1]!=None:
+                                self.con(self.mainvars[("ivar",name)][i]<=bound[1])
+
                 return self.mainvars[("ivar",name)]
 
             case 'heuristic':
+                return generate_heuristic_variable(self.features, 'ivar', name, dim, bound, self.agent,self.no_agents)
+                   
+    def bvar(self, name, dim=0, bound=[0, 1]):
 
-                return generate_heuristic_variable(self.features, 'ivar', name, dim, bound, self.agent)
-
-    def fvar(self, name, dim=0, bound=[None, None]):
         """
-        Creates and returns a free variable.
+        Creates and returns a binary variable.
 
         Args:
             name (str): Name of this variable.
             dim (list, optional): Dimensions of this variable. Default: 0.
-            bound (list, optional): Bounds of this variable. Default: [None, None].
+            bound (list, optional): Bounds of this variable. Default: [0, 1].
         """
 
         dim = fix_dims(dim)
-        self.features = update_variable_features(
-            name, dim, bound, 'free_variable_counter', self.features)
+        self.features = update_variable_features(name, dim, bound, 'binary_variable_counter', self.features)
 
-        match self.features['solution_method']:
+        if self.features['solution_method'] == 'exact':
 
-            case 'exact':
+            from .generators import variable_generator
+            self.mainvars[("bvar", name)] = variable_generator.generate_variable(self.features['interface_name'], self.model, 'bvar', name, bound, dim)
+            self.maindims[name] = dim
 
-                from .generators import variable_generator
-                self.mainvars[("fvar",name)] = variable_generator.generate_variable(self.features['interface_name'], self.model, 'fvar', name, bound, dim)
-                self.maindims[name] = dim
-                return self.mainvars[("fvar",name)]
+            if self.features['interface_name'] in ['cvxpy']:
+                if dim == 0:
+                    self.con(self.mainvars[("bvar", name)] >= 0)
+                    self.con(self.mainvars[("bvar", name)] <= 1)
+                elif len(dim) == 1:
+                    for i in dim[0]:
+                        self.con(self.mainvars[("bvar", name)][i] >= 0)
+                        self.con(self.mainvars[("bvar", name)][i] <= 1)
+                else:
+                    for i in it.product(*tuple(dim)):
+                        self.con(self.mainvars[("bvar", name)][i] >= 0)
+                        self.con(self.mainvars[("bvar", name)][i] <= 1)
+            return self.mainvars[("bvar", name)]
 
-            case 'heuristic':
+        elif self.features['solution_method'] == 'heuristic':
+            return generate_heuristic_variable(self.features, 'bvar', name, dim, bound, self.agent,self.no_agents)
+    
+    def cfvar(self, name, indices, dim=0, bound=[None, None]):
+
+        """
+        This method creates a dictionary of free (continuous) variables with given names and indices.
+        
+        Parameters:
+            name (str): The base name for the variables.
+            indices (list): The indices for the variables.
+            dim (dict): The dimensions for the variables. Defaults to 0 for all indices if not provided as a dictionary.
+            bound (dict): The bounds for the variables. Defaults to [None, None] for all indices if not provided as a dictionary.
+
+        Returns:
+            dict: A dictionary where each key is an index from 'indices' and the corresponding value is a continuous variable with the name derived from 'name' and the index.
+        """
+
+        if type(bound)!=dict: bound = {i: bound for i in indices}
+        if type(dim)!=dict: dim = {i: dim for i in indices}
+        return {i: self.fvar(name+f"[{i}]".replace("(", "").replace(")", ""), dim =dim[i], bound=bound[i]) for i in indices}
+
+    def cpvar(self, name, indices, dim=0, bound=[0, None]):
+
+        """
+        This method creates a dictionary of positive continuous variables with given names and indices.
+        
+        Parameters:
+            name (str): The base name for the variables.
+            indices (list): The indices for the variables.
+            dim (dict): The dimensions for the variables. Defaults to 0 for all indices if not provided as a dictionary.
+            bound (dict): The bounds for the variables. Defaults to [0, None] for all indices if not provided as a dictionary.
+
+        Returns:
+            dict: A dictionary where each key is an index from 'indices' and the corresponding value is a positive continuous variable with the name derived from 'name' and the index.
+        """
+
+        if type(bound)!=dict: bound = {i: bound for i in indices}
+        if type(dim)!=dict: dim = {i: dim for i in indices}
+        return {i: self.pvar(name+f"[{i}]".replace("(", "").replace(")", ""), dim =dim[i], bound=bound[i]) for i in indices}
+
+    def civar(self, name, indices, dim=0, bound= [0, None]):
+
+        """
+        This method creates a dictionary of integer variables with given names and indices.
+        
+        Parameters:
+            name (str): The base name for the variables.
+            indices (list): The indices for the variables.
+            dim (dict): The dimensions for the variables. Defaults to 0 for all indices if not provided as a dictionary.
+            bound (dict): The bounds for the variables. Defaults to [0, None] for all indices if not provided as a dictionary.
+
+        Returns:
+            dict: A dictionary where each key is an index from 'indices' and the corresponding value is an integer variable with the name derived from 'name' and the index.
+        """
+
+        if type(bound)!=dict: bound = {i: bound for i in indices}
+        if type(dim)!=dict: dim = {i: dim for i in indices}
+        return {i: self.ivar(name+f"[{i}]".replace("(", "").replace(")", ""), dim =dim[i], bound=bound[i]) for i in indices}
+
+    def cbvar(self, name, indices, dim=0, bound=[0,1]):
+
+        """
+        This method creates a dictionary of binary variables with given names and indices.
+        
+        Parameters:
+            name (str): The base name for the variables.
+            indices (list): The indices for the variables.
+            dim (dict): The dimensions for the variables. Defaults to 0 for all indices if not provided as a dictionary.
+            bound (dict): The bounds for the variables. Defaults to [0, None] for all indices if not provided as a dictionary.
+
+        Returns:
+            dict: A dictionary where each key is an index from 'indices' and the corresponding value is a binary variable with the name derived from 'name' and the index.
+        """
 
-                return generate_heuristic_variable(self.features, 'fvar', name, dim, bound, self.agent)
+        if type(bound)!=dict: bound = {i: bound for i in indices}
+        if type(dim)!=dict: dim = {i: dim for i in indices}
+        return {i: self.bvar(name+f"[{i}]".replace("(", "").replace(")", ""), dim =dim[i], bound=bound[i]) for i in indices}
 
     def dvar(self, name, dim=0):
+        
         """
         Creates and returns a dependent variable.
 
         Args:
             name (str): Name of this variable.
             dim (list, optional): Dimensions of this variable. Default: 0.
         """
 
         dim = fix_dims(dim)
 
-        if self.features['agent_status'] == 'idle':
-            if self.features['vectorized']:
-                if dim == 0:
-                    return 0
-                else:
-                    return np.random.rand(*tuple([50]+[len(dims) for dims in dim]))
-            else:
-                if dim == 0:
-                    return 0
-                else:
-                    return np.zeros([len(dims) for dims in dim])
+        if self.no_agents!=None:
+            default_pop= self.no_agents
         else:
-            if self.features['vectorized']:
-                if dim == 0:
-                    return np.zeros(self.features['pop_size'])
-                else:
-                    return np.zeros([self.features['pop_size']]+[len(dims) for dims in dim])
-            else:
-                if dim == 0:
-                    return 0
+            default_pop = 100
+
+        match self.features['solution_method']:
+
+            case 'exact':
+
+                return np.zeros([len(dims) for dims in dim])
+            
+            case 'heuristic':
+
+                if self.features['agent_status'] == 'idle':
+                    if self.features['vectorized']:
+                        if dim == 0:
+                            return 0
+                        else:
+                            return np.random.rand(*tuple([default_pop]+[len(dims) for dims in dim]))
+                    else:
+                        if dim == 0:
+                            return 0
+                        else:
+                            return np.zeros([len(dims) for dims in dim])
                 else:
-                    return np.zeros([len(dims) for dims in dim])
+                    if self.features['vectorized']:
+                        if dim == 0:
+                            return np.zeros(self.features['pop_size'])
+                        else:
+                            return np.zeros([self.features['pop_size']]+[len(dims) for dims in dim])
+                    else:
+                        if dim == 0:
+                            return 0
+                        else:
+                            return np.zeros([len(dims) for dims in dim])
 
-    def svar(self, name, dim=0):
+    def cdvar(self, name, indices, dim = 0):
         """
-        Creates and returns a sequential variable.
+        This method creates a dictionary of dependent variables with specific names and dimensions.
+
+        Parameters:
+            name (str): The base name for the variables.
+            indices (list): The indices for the variables.
+            dim (dict, optional): The dimensions for the variables. Defaults to 0 for all indices if not provided as a dictionary.
+
+        Returns:
+            dict: A dictionary where each key is an index from 'indices' and the corresponding value is a dependent variable with the name derived from 'name' and the index, and dimensions specified by 'dim'.
+        """
+        if type(dim)!=dict: dim = {i: dim for i in indices}
+        return {i: self.dvar(name+f"[{i}]".replace("(", "").replace(")", ""), dim =dim[i]) for i in indices}
+
+    def rvar(self, name, dim=0):
+        """
+        Creates and returns a random variable.
 
         Args:
             name (str): Name of this variable.
             dim (list, optional): Dimensions of this variable. Default: 0.
         """
+        dim = fix_dims(dim)
+        from .generators import variable_generator
+        return variable_generator.generate_variable(self.features['interface_name'], self.model, 'rvar', name, [None, None], dim)
+
+    def crvar(self, name, indices, dim=0):
+        """
+        Creates a dictionary of random variables with specific names and dimensions.
+
+        Args:
+            name (str): Base name for the variables.
+            indices (list): Indices for the variables.
+            dim (dict, optional): Dimensions for the variables. Defaults to None.
+
+        Returns:
+            dict: A dictionary where each key is an index from 'indices' and the corresponding value is a random variable with the name derived from 'name' and the index.
+        """
+        if type(dim)!=dict: dim = {i: dim for i in indices}
+        return {i: self.rvar(name+f"[{i}]".replace("(", "").replace(")", ""), dim =dim[i]) for i in indices}
+
+    def rtvar(self, name, shape=0):
+
+        """
+        Creates and returns a tensor-like random variable.
+
+        Args:
+            name (str): Name of this variable.
+            shape (list, optional): Shape of this variable. Default: 0.
+        """
+
+        dim = fix_dims(shape)
+        from .generators import variable_generator
+        return variable_generator.generate_variable(self.features['interface_name'], self.model, 'rtvar', name, [None, None], dim)
+        
+    def crtvar(self, name, indices, shape=0):
+
+        """
+        Creates a dictionary of tensor-like random variables with specific names and shapes.
 
-        self.features = update_variable_features(
-            name, dim, [0, 1], 'integer_variable_counter', self.features)
+        Args:
+            name (str): Base name for the variables.
+            indices (list): Indices for the variables.
+            shape (dict, optional): Shapes for the variables. Defaults to None.
+
+        Returns:
+            dict: A dictionary where each key is an index from 'indices' and the corresponding value is a tensor-like random variable with the name derived from 'name' and the index, and shape specified by 'shape'.
+        """
+
+        if type(shape)!=dict: shape = {i: shape for i in indices}
+        return {i: self.rtvar(name+f"[{i}]".replace("(", "").replace(")", ""), shape =shape[i]) for i in indices}
+
+    def svar(self, name, length=1):
+        """
+        Creates and returns a sequential variable.
+
+        Args:
+            name (str): Name of this variable.
+            length (int, optional): Length of this variable. Default: 1.
+            
+        Returns:
+            A sequential variable with the given name and length.
+        """
+        dim = fix_dims([length])
+        self.features = update_variable_features(name, dim, [0, 1], 'integer_variable_counter', self.features)
         self.features['variable_type'][name] = 'svar'
+        return generate_heuristic_variable(self.features, 'svar', name, dim, [0, 1], self.agent, self.no_agents)
 
-        return generate_heuristic_variable(self.features, 'svar', name, dim, [0, 1], self.agent)
+    def csvar(self, name, indices, length=1):
+        """
+        Creates a dictionary of sequential variables with specific names and lengths.
+
+        Args:
+            name (str): Base name for the variables.
+            indices (list): Indices for the variables.
+            length (dict, optional): Lengths for the variables. Defaults to None.
+
+        Returns:
+            dict: A dictionary where each key is an index from 'indices' and the corresponding value is a sequential variable with the name derived from 'name' and the index, and length specified by 'length'.
+        """
+        if type(length)!=dict: length = {i: length for i in indices}
+        return {i: self.svar(name+f"[{i}]".replace("(", "").replace(")", ""), length =length[i]) for i in indices}
+
+    def evar(self, name, interval=[None, None, None], dim=0, optional=False):
 
-    def evar(self, name, interval=[None, None, None], dim=0, is_present=False):
         """        
         Creates and returns an event (interval) variable.
 
         Args:
             name: Name of this variable.
             interval: [size, start, end]. 
             dim (list, optional): Dimensions of this variable. Default: 0.
         """
 
-        if len(interval) == 1:
-            interval = [interval[0], None, None]
+        self.features = update_variable_features(name, dim, None, 'event_variable_counter', self.features)
+
+        if len(interval) == 1: interval = [interval[0], None, None]
 
         if dim == 0:
 
             if self.features['interface_name'] == 'cplex_cp':
-                return self.model.interval_var(start=interval[1], size=interval[0], end=interval[2], name=name, optional=is_present)
+
+                self.mainvars[("evar",name)] = self.model.interval_var(start=interval[1], size=interval[0], end=interval[2], name=name, optional=optional)
+                self.maindims[name] = dim
+
+                return self.mainvars[("evar",name)]
+            
             if self.features['interface_name'] == 'ortools_cp':
-                return self.model.NewOptionalIntervalVar(start=interval[1], size=interval[0], end=interval[2], name=name, is_present=is_present)
+                self.mainvars[("evar",name)] = self.model.NewOptionalIntervalVar(start=interval[1], size=interval[0], end=interval[2], name=name, is_present=optional)
+                self.maindims[name] = dim
+
+                return self.mainvars[("evar",name)]
         else:
+
             if self.features['interface_name'] == 'cplex_cp':
+
                 if len(dim) == 1:
-                    return {key: self.model.interval_var(start=interval[1], size=interval[0], end=interval[2], name=f"{name}{key}", optional=is_present) for key in dim[0]}
+                    self.mainvars[("evar",name)] = {key: self.model.interval_var(start=interval[1], size=interval[0], end=interval[2], name=f"{name}{key}", optional=optional) for key in dim[0]}
+                    self.maindims[name] = dim
+                    return self.mainvars[("evar",name)] 
+                
                 else:
-                    return {key: self.model.interval_var(start=interval[1], size=interval[0], end=interval[2], name=f"{name}{key}", optional=is_present) for key in sets(*dim)}
+                    self.mainvars[("evar",name)]  = {key: self.model.interval_var(start=interval[1], size=interval[0], end=interval[2], name=f"{name}{key}", optional=optional) for key in sets(*dim)}
+                    self.maindims[name] = dim
+                    return  self.mainvars[("evar",name)] 
 
             if self.features['interface_name'] == 'ortools_cp':
 
                 if len(dim) == 1:
-                    return {key: self.model.NewOptionalIntervalVar(start=interval[1], size=interval[0], end=interval[2], name=f"{name}{key}", is_present=is_present) for key in dim[0]}
+                    self.mainvars[("evar",name)] = {key: self.model.NewOptionalIntervalVar(start=interval[1], size=interval[0], end=interval[2], name=f"{name}{key}", is_present=optional) for key in dim[0]}
+                    self.maindims[name] = dim
+                    return self.mainvars[("evar",name)]
+                
                 else:
-                    return {key: self.model.NewOptionalIntervalVar(start=interval[1], size=interval[0], end=interval[2], name=f"{name}{key}", is_present=is_present) for key in sets(*dim)}
-
+                    self.mainvars[("evar",name)]  = {key: self.model.NewOptionalIntervalVar(start=interval[1], size=interval[0], end=interval[2], name=f"{name}{key}", is_present=optional) for key in sets(*dim)}
+                    self.maindims[name] = dim
+                    return self.mainvars[("evar",name)] 
+
+    def cevar(self, name, indices, interval=[None, None, None], dim=0, optional=False):
+
+        if type(interval)!=dict: interval = {i: interval for i in indices}
+        if type(dim)!=dict: dim = {i: dim for i in indices}
+        if type(optional)!=dict: optional = {i: optional for i in indices}
+        return {i: self.evar(name+f"[{i}]".replace("(", "").replace(")", ""), interval=interval[i], dim=dim[i], optional=optional[i]) for i in indices}
+                
     # Methods for handling special automation operations
+    
     def scon_exactly_one_one(self, list_of_binary_variables):
+        """
+        This method adds a constraint to the model such that exactly one variable in the list of binary variables is equal to 1.
+
+        Parameters:
+            list_of_binary_variables (list): List of binary variables.
+        """
         self.con(sum(list_of_binary_variables[i] for i in range(len(list_of_binary_variables)))==1)
 
     def scon_max_one_one(self, list_of_binary_variables):
+        """
+        This method adds a constraint to the model such that at most one variable in the list of binary variables is equal to 1.
+
+        Parameters:
+            list_of_binary_variables (list): List of binary variables.
+        """
         self.con(sum(list_of_binary_variables[i] for i in range(len(list_of_binary_variables)))<=1)
 
     def scon_min_one_one(self, list_of_binary_variables):
+        """
+        This method adds a constraint to the model such that at least one variable in the list of binary variables is equal to 1.
+
+        Parameters:
+            list_of_binary_variables (list): List of binary variables.
+        """
         self.con(sum(list_of_binary_variables[i] for i in range(len(list_of_binary_variables)))>=1)
 
     def scon_exactly_m_one(self, list_of_binary_variables, m):
+        """
+        This method adds a constraint to the model such that exactly 'm' variables in the list of binary variables are equal to 1.
+
+        Parameters:
+            list_of_binary_variables (list): List of binary variables.
+            m (int): The exact number of variables that should be equal to 1.
+        """
         self.con(sum(list_of_binary_variables[i] for i in range(len(list_of_binary_variables)))==m)
 
     def scon_max_m_one(self, list_of_binary_variables, m):
+        """
+        This method adds a constraint to the model such that at most 'm' variables in the list of binary variables are equal to 1.
+
+        Parameters:
+            list_of_binary_variables (list): List of binary variables.
+            m (int): The maximum number of variables that should be equal to 1.
+        """
         self.con(sum(list_of_binary_variables[i] for i in range(len(list_of_binary_variables)))<=m)
 
     def scon_min_m_one(self, list_of_binary_variables, m):
+        """
+        This method adds a constraint to the model such that at least 'm' variables in the list of binary variables are equal to 1.
+
+        Parameters:
+            list_of_binary_variables (list): List of binary variables.
+            m (int): The minimum number of variables that should be equal to 1.
+        """
         self.con(sum(list_of_binary_variables[i] for i in range(len(list_of_binary_variables)))>=m)
 
     def scon_only_one_of_the_values(self, variable, list_of_values):
+        """
+        This method adds a constraint to the model such that the variable can only take one value from the list of values.
+
+        Parameters:
+            variable (variable): The variable that should take a value from the list.
+            list_of_values (list): List of potential values for the variable.
+        """
         try:
             for i in range(len(list_of_values)):
                 self.features['indicators'].append(self.features['indicators'][-1]+1)
         except:
             self.features['indicators'] = []
             for i in range(len(list_of_values)):
                 self.features['indicators'].append(i)
         z = self.bvar(f"indicator{self.features['indicators'][-1]}",[range(len(list_of_values))])
         self.con(variable==sum(list_of_values[i]*z[i] for i in range(len(list_of_values))))
         self.con(sum(z[i] for i in range(len(list_of_values)))==1)
 
     def scon_only_one_of_the_values_or_zero(self, variable, list_of_values):
+        """
+        This method adds a constraint to the model such that the variable can either take one value from the list of values or be zero.
+
+        Parameters:
+            variable (variable): The variable that should take a value from the list or be zero.
+            list_of_values (list): List of potential values for the variable.
+        """
         try:
             for i in range(len(list_of_values)):
                 self.features['indicators'].append(self.features['indicators'][-1]+1)
         except:
             self.features['indicators'] = []
             for i in range(len(list_of_values)):
                 self.features['indicators'].append(i)
         z = self.bvar(f"indicator{self.features['indicators'][-1]}",[range(len(list_of_values))])
         self.con(variable==sum(list_of_values[i]*z[i] for i in range(len(list_of_values))))
         self.con(sum(z[i] for i in range(len(list_of_values)))<=1)
 
     def scon_this_depends_on_that(self, this, that):
-        self.con(this<=that)
+        """
+        This method adds a constraint to the model such that the 'this' variable should be less than or equal to the 'that' variable.
 
-    def scon_this_indeed_that(self, this, that):
+        Parameters:
+            this (variable): The dependent variable.
+            that (variable): The variable that 'this' is dependent on.
+        """
         self.con(this<=that)
 
-    def scon_strict_indicator_leq(self,indicator, expr, rhs, big_m=10e9, epsilon=10e-9):
-        """
-        Either expr<=rhs or expr>rhs should be true (1), using the user-provided indicator (0,1).
+    def scon_this_indeed_that(self, this, that):
         """
-        self.con(expr<=rhs+(1-indicator)*big_m)
-        self.con(expr>=rhs-indicator*big_m+epsilon)
+        This method adds a constraint to the model such that the 'this' variable should be less than or equal to the 'that' variable.
 
-    def scon_strict_indicator_geq(self,indicator, expr, rhs, big_m=10e9, epsilon=10e-9):
+        Parameters:
+            this (variable): The dependent variable.
+            that (variable): The variable that 'this' is dependent on.
         """
-        Either expr>=rhs or expr<rhs should be true (1), using the user-provided indicator (0,1).
-        """
-        self.con(expr>=rhs-(1-indicator)*big_m)
-        self.con(expr<=rhs+indicator*big_m-epsilon)
+        self.con(this<=that)
 
     def scon_soft_indicator_leq(self,indicator, expr, rhs, big_m=10e9):
         """
-        expr<=rhs might be true (1) or not (0).
+        This method adds a soft constraint to the model. It relaxes the constraint expr <= rhs by allowing it to be false. The indicator variable decides whether the constraint should be enforced (1) or not (0).
+
+        Parameters:
+            indicator (variable): The binary variable that indicates whether the constraint should be enforced or not.
+            expr (expression): The left-hand side of the constraint.
+            rhs (number): The right-hand side of the constraint.
+            big_m (number): A large positive number used for relaxation. Default is 10e9.
         """
         self.con(expr<=rhs+(1-indicator)*big_m)
 
     def scon_soft_indicator_geq(self,indicator, expr, rhs, big_m=10e9):
         """
-        expr>=rhs might be true (1) or not (0).
+        This method adds a soft constraint to the model. It relaxes the constraint expr >= rhs by allowing it to be false. The indicator variable decides whether the constraint should be enforced (1) or not (0).
+
+        Parameters:
+            indicator (variable): The binary variable that indicates whether the constraint should be enforced or not.
+            expr (expression): The left-hand side of the constraint.
+            rhs (number): The right-hand side of the constraint.
+            big_m (number): A large positive number used for relaxation. Default is 10e9.
         """
         self.con(expr>=rhs-(1-indicator)*big_m)
 
     def scon_this_or_that(self,this,rhs_this,that,rhs_that,big_m=10e9):
         """
-        Adds two constraints and one indicator variable, to find if this<=rhs_this or that<=rhs_that.
+        Adds two constraints and one indicator variable to the model. The constraints ensure that either 'this' is less than or equal to 'rhs_this' or 'that' is less than or equal to 'rhs_that'.
+        Note: Variables can also be expressions.
+
+        Parameters:
+            this (variable): The first variable.
+            rhs_this (number): The upper limit for the 'this' variable.
+            that (variable): The second variable.
+            rhs_that (number): The upper limit for the 'that' variable.
+            big_m (number): A large positive number used for relaxation. Default is 10e9.
         """
+
         try:
-            self.features['indicators'].append(
-                self.features['indicators'][-1]+1)
-        except:
+            self.features['indicators'].append(self.features['indicators'][-1]+1)
 
+        except:
             self.features['indicators'] = [0]
 
         z = self.bvar(f"indicator{self.features['indicators'][-1]}")
+
         self.con(this<=rhs_this+z*big_m)
         self.con(that<=rhs_that+(1-z)*big_m)
 
     def scon_if_then(self, this, rhs_this, that, rhs_that, big_m=10e9, epsilon=10e-9):
         """
-        Adds two constraints and one indicator variable, to find if this<=rhs_this then that<=rhs_that.
-        """
+        Adds two constraints and one indicator variable to the model. If 'this' is less than or equal to 'rhs_this', then 'that' should be less than or equal to 'rhs_that'.
+        Note: Variables can also be expressions.
 
+        Parameters:
+            this (variable): The condition variable.
+            rhs_this (number): The upper limit for the 'this' variable.
+            that (variable): The dependent variable.
+            rhs_that (number): The upper limit for the 'that' variable.
+            big_m (number): A large positive number used for relaxation. Default is 10e9.
+            epsilon (number): A small positive number to ensure strict inequality. Default is 10e-9.
+        """
         try:
-            self.features['indicators'].append(
-                self.features['indicators'][-1]+1)
+            self.features['indicators'].append(self.features['indicators'][-1]+1)
         except:
-
             self.features['indicators'] = [0]
-
         z = self.bvar(f"indicator{self.features['indicators'][-1]}")
-
         self.con(this >= rhs_this + epsilon - z*big_m)
         self.con(that <= rhs_that + (1-z)*big_m)
 
     def scon_viol_leq(self,expr,rhs=0):
         """
+        Adds a constraint to the model that represents the amount of violation for soft constraints of type less than or equal to (<=).
+
+        Parameters:
+            expr (expression): The expression that should be less than or equal to 'rhs'.
+            rhs (number): The right-hand side of the constraint. Default is 0.
         
-        Returns the amount of violation for soft constraints of type less than or equal (<=).
-        
+        Returns:
+            z (variable): The variable representing the amount of violation.
         """
         try:
-            self.features['indicators'].append(
-                self.features['indicators'][-1]+1)
+            self.features['indicators'].append(self.features['indicators'][-1]+1)
         except:
-
             self.features['indicators'] = [0]
-        
         z = self.pvar(f"indicator{self.features['indicators'][-1]}")
         self.con(expr<=rhs+z)
         return z
-    
+
     def scon_viol_geq(self,expr,rhs=0):
         """
-        Returns the amount of violation for soft constraints of type greater than or equal (>=).
+        Adds a constraint to the model that represents the amount of violation for soft constraints of type greater than or equal to (>=).
+
+        Parameters:
+            expr (expression): The expression that should be greater than or equal to 'rhs'.
+            rhs (number): The right-hand side of the constraint. Default is 0.
         
+        Returns:
+            z (variable): The variable representing the amount of violation.
         """
         try:
-            self.features['indicators'].append(
-                self.features['indicators'][-1]+1)
+            self.features['indicators'].append(self.features['indicators'][-1]+1)
         except:
-
             self.features['indicators'] = [0]
-        
         z = self.pvar(f"indicator{self.features['indicators'][-1]}")
         self.con(expr>=rhs-z)
         return z 
-    
+
     def scon_slack_leq(self,expr,rhs=0):
+        """
+        Adds a slack variable to the model for a less than or equal to (<=) constraint. The slack variable represents the difference between the left-hand side expression and the right-hand side.
+
+        Parameters:
+            expr (expression): The expression that should be less than or equal to 'rhs'.
+            rhs (number): The right-hand side of the constraint. Default is 0.
+        
+        Returns:
+            z (variable): The slack variable.
+        """
         try:
-            self.features['indicators'].append(
-                self.features['indicators'][-1]+1)
+            self.features['indicators'].append(self.features['indicators'][-1]+1)
         except:
-
             self.features['indicators'] = [0]
-        
         z = self.pvar(f"indicator{self.features['indicators'][-1]}")
         self.con(expr+z==rhs)
         return z 
 
     def scon_surplus_leq(self,expr,rhs=0):
+        """
+        Adds a surplus variable to the model for a greater than or equal to (>=) constraint. The surplus variable represents the difference between the left-hand side expression and the right-hand side.
+
+        Parameters:
+            expr (expression): The expression that should be greater than or equal to 'rhs'.
+            rhs (number): The right-hand side of the constraint. Default is 0.
+        
+        Returns:
+            z (variable): The surplus variable.
+        """
         try:
-            self.features['indicators'].append(
-                self.features['indicators'][-1]+1)
+            self.features['indicators'].append(self.features['indicators'][-1]+1)
         except:
-
             self.features['indicators'] = [0]
-        
-        z = self.pvar(f"indicator{self.features['indicators'][-1]}")
+        z = self.nvar(f"indicator{self.features['indicators'][-1]}")
         self.con(expr-z==rhs)
         return z
 
-    def lin_piecewise(self, slopes, intercepts, breakpoints):
+    def scon_viol_eq(self,expr,rhs=0):
+        """
+        Adds two constraints to the model that represent the amount of violation for soft constraints of type equal to (==).
 
+        Parameters:
+            expr (expression): The expression that should be equal to 'rhs'.
+            rhs (number): The right-hand side of the constraint. Default is 0.
+        
+        Returns:
+            z (variable): The variable representing the amount of violation.
+        """
         try:
-            for i in range(len(breakpoints)):
-                self.features['indicators'].append(self.features['indicators'][-1]+1)
+            self.features['indicators'].append(self.features['indicators'][-1]+1)
         except:
-            self.features['indicators'] = []
-            for i in range(len(breakpoints)):
-                self.features['indicators'].append(0)
-
-        x = self.pvar(f"indicatorr{self.features['indicators'][-1]}",[range(len(breakpoints))])
-        y = self.bvar(f"indicatorr{self.features['indicators'][-1]}",[range(len(breakpoints))])
-        for i in range(len(breakpoints)):
-            if i!=len(breakpoints)-1:
-                self.scon_in_bound(x[i], lb= (breakpoints[i+1]-breakpoints[i])*y[i], ub=(breakpoints[i+1]-breakpoints[i])*y[i])
-
-        return sum(slopes[i]*x[i]+intercepts[i] for i in range(len(breakpoints)-1))
+            self.features['indicators'] = [0]
+        z = self.pvar(f"indicator{self.features['indicators'][-1]}")
+        self.con(expr<=rhs+z)
+        self.con(expr>=rhs-z)
+        return z
 
     def scon_in_bound(self, expr, lb=None, ub=None, label=None):
         """
         Creates upper and/or lower bounds on the given variable in the optimization model.
         """
         if lb is not None:
             self.con(expr >= lb, label=label)
@@ -697,37 +1112,96 @@
             f"abs_geq_linearizer{self.features['abs_geq_linearizers'][-1]}")
         
         self.scon_this_or_that()
 
         self.con(expr >= rhs-z*big_m)
         self.con(expr <= -1*rhs+(1-z)*big_m)
 
+    def lin_piecewise(self, slopes, intercepts, breakpoints):
+        """
+        This method implements a piecewise linear function in the context of mathematical programming.
+
+        Parameters:
+            slopes (list): A list of slopes for each piece of the function.
+            intercepts (list): A list of intercepts for each piece of the function.
+            breakpoints (list): A list of breakpoints that define the domain of each piece of the function.
+
+        Returns:
+            The piecewise linear function represented as a sum of linear functions, each multiplied by a binary variable.
+
+        Note:
+            The function is represented as a sum of linear functions, each multiplied by a binary variable that indicates whether that piece of the function is active. The constraints ensure that only one piece is active at any point in the domain.
+        """
+        try:
+            self.features['indicators'].append(self.features['indicators'][-1]+1)
+        except:
+            self.features['indicators'] = [0]
+
+        x = self.pvar(f"indicatorr{self.features['indicators'][-1]}", range(len(breakpoints)))
+        y = self.bvar(f"indicatorr{self.features['indicators'][-1]}", range(len(breakpoints)))
+
+        for i in range(len(breakpoints) - 1):
+            self.con((breakpoints[i+1] - breakpoints[i])*y[i] <= x[i])
+            self.con(x[i] <= (breakpoints[i+1] - breakpoints[i])*y[i+1])
+
+        self.con(sum(y[i] for i in range(len(breakpoints))) == 1)
+
+        return sum((slopes[i]*x[i] + intercepts[i])*y[i] for i in range(len(breakpoints)))
+
+    def lin_approx(self, f, x, x_range, num_breakpoints):
+        """
+        This method implements a piecewise linear approximation of a non-linear function in the context of mathematical programming.
+
+        Parameters:
+            f (function): The non-linear function to be approximated.
+            x (variable): The variable of the non-linear function.
+            x_range (tuple): A tuple of two numbers representing the minimum and maximum values of x.
+            num_breakpoints (int): The number of breakpoints to use in the approximation.
+
+        Returns:
+            The piecewise linear approximation of the non-linear function.
+        """
+        breakpoints = np.linspace(x_range[0], x_range[1], num_breakpoints)
+        slopes = [(f(breakpoints[i+1]) - f(breakpoints[i])) / (breakpoints[i+1] - breakpoints[i]) for i in range(len(breakpoints)-1)]
+        intercepts = [f(breakpoints[i]) - slopes[i] * breakpoints[i] for i in range(len(breakpoints)-1)]
+        
+        return self.lin_piecewise(slopes, intercepts, breakpoints)
+    
     def lin_abs_in_obj(self, expr, method=0, dir_obj=None):
         """
         Linearizes an |a| expression inside the objective function.
 
-        * method 0: +2 pvars and +1 constraint (for min and max)
-        * method 1: +1 pvar and + 2 constraints (+1 bvar for max) (for min or max, requires user input)
-        * method 2: +1 pvar and +1 constraint (only for min, does not require user input)
-        """
+        Parameters:
+            expr: The absolute value expression to be linearized.
+            method (int): The method to use for linearization.
+                - method 0: Uses +2 pvars and +1 constraint (for min and max).
+                - method 1: Uses +1 pvar and +2 constraints (+1 bvar for max) (for min or max, requires user input).
+                - method 2: Uses +1 pvar and +1 constraint (only for min, does not require user input).
+            dir_obj (str): The direction of the objective function. Required for method 1 when linearizing for max.
+
+        Returns:
+            The linearized expression.
 
+        Note:
+            The linearization is performed based on the chosen method and the direction of the objective function.
+        """
         if method == 0:
             try:
                 self.features['abs_obj_linearizers'].append(
                     self.features['abs_obj_linearizers'][-1]+1)
                 self.features['abs_obj_linearizers'].append(
                     self.features['abs_obj_linearizers'][-1]+1)
             except:
                 self.features['abs_obj_linearizers'] = [0, 1]
             z1 = self.pvar(
                 f"abs_obj_linearizer{self.features['abs_obj_linearizers'][-1]}")
             z2 = self.pvar(
                 f"abs_obj_linearizer{self.features['abs_obj_linearizers'][-2]}")
-            self.con(expr == z1-z2)
-            return z1+z2
+            self.con(expr == z1 - z2)
+            return z1 + z2
 
         if method == 1:
             if dir_obj == 'min':
                 try:
                     self.features['abs_obj_linearizers'].append(
                         self.features['abs_obj_linearizers'][-1]+1)
                 except:
@@ -751,23 +1225,33 @@
             try:
                 self.features['abs_obj_linearizers'].append(
                     self.features['abs_obj_linearizers'][-1]+1)
             except:
                 self.features['abs_obj_linearizers'] = [0]
             z = self.pvar(
                 f"abs_obj_linearizer{self.features['abs_obj_linearizers'][-1]}")
-            self.con(expr+z >= 0)
-            return expr + 2*z
+            self.con(expr + z >= 0)
+            return expr + 2 * z
 
     def lin_max(self, input_list, type_max, ub_max):
         """
         Linearizes the max function.
+
+        Parameters:
+            input_list (list): The list of expressions to be linearized.
+            type_max (str): The type of variable to use for linearization.
+            ub_max: The upper bound for the linearized expression (optional).
+
+        Returns:
+            The linearized expression.
+
+        Note:
+            The linearization is performed based on the type of variable chosen for linearization and the upper bound, if provided.
         """
         if self.features['solution_method'] == 'exact':
-
             try:
                 self.features['max_linearizers'].append(
                     self.features['max_linearizers'][-1]+1)
             except:
                 self.features['max_linearizers'] = [0]
 
             if type_max == 'bvar':
@@ -781,22 +1265,35 @@
                     f"max_linearizer{self.features['max_linearizers'][-1]}")
             if type_max == 'fvar':
                 z = self.fvar(
                     f"max_linearizer{self.features['max_linearizers'][-1]}")
 
             for item in input_list:
                 self.con(z >= item)
-            if ub_max != None:
+            if ub_max is not None:
                 self.con(z <= ub_max)
             return z
 
     def lin_min(self, input_list, type_min, lb_min=None):
+
         """
         Linearizes the min function.
+
+        Parameters:
+            input_list (list): The list of expressions to be linearized.
+            type_min (str): The type of variable to use for linearization.
+            lb_min: The lower bound for the linearized expression (optional).
+
+        Returns:
+            The linearized expression.
+
+        Note:
+            The linearization is performed based on the type of variable chosen for linearization and the lower bound, if provided.
         """
+
         try:
             self.features['min_linearizers'].append(
                 self.features['min_linearizers'][-1]+1)
         except:
             self.features['min_linearizers'] = [0]
 
         if type_min == 'bvar':
@@ -810,539 +1307,658 @@
                 f"min_linearizer{self.features['min_linearizers'][-1]}")
         elif type_min == 'fvar':
             z = self.fvar(
                 f"min_linearizer{self.features['min_linearizers'][-1]}")
 
         for item in input_list:
             self.con(z <= item)
-        if lb_min != None:
+        if lb_min is not None:
             self.con(z >= lb_min)
         return z
 
     def lin_prod_bb(self, binary1, binary2):
         """
         Linearizes a Binary * Binary product.
 
-        constraints: +3
-        positive variables: +1
+        Returns:
+            The linearized expression.
+
+        Note:
+            The linearization requires +3 constraints and +1 positive variable.
         """
 
         try:
             self.features['bb_linearizers'].append(
                 self.features['bb_linearizers'][-1]+1)
         except:
-
             self.features['bb_linearizers'] = [0]
 
         z = self.pvar(f"bb_linearizer{self.features['bb_linearizers'][-1]}")
         self.con(z <= binary1)
         self.con(z <= binary2)
         self.con(z >= binary1 + binary2 - 1)
         return z
-
+    
     def lin_prod_bp(self, binary, positive, ub_positive=10e9):
         """
         Linearizes a Binary * Positive product.
 
-        constraints: +3
-        positive variables: +1
+        Returns:
+            The linearized expression.
+
+        Note:
+            The linearization requires +3 constraints and +1 positive variable.
         """
         try:
             self.features['bp_linearizers'].append(
                 self.features['bp_linearizers'][-1]+1)
         except:
             self.features['bp_linearizers'] = [0]
 
         z = self.pvar(f"bp_linearizer{self.features['bp_linearizers'][-1]}")
         self.con(z <= positive)
-        self.con(z <= binary*ub_positive)
-        self.con(z >= positive - ub_positive*(1-binary))
+        self.con(z <= binary * ub_positive)
+        self.con(z >= positive - ub_positive * (1 - binary))
         return z
 
     def lin_prod_bi(self, binary, integer, ub_integer=10e9):
         """
         Linearizes a Binary * Integer product.
 
-        constraints: +3
-        positive variables: +1
+        Returns:
+            The linearized expression.
+
+        Note:
+            The linearization requires +3 constraints and +1 positive variable.
         """
         try:
             self.features['bi_linearizers'].append(
                 self.features['bi_linearizers'][-1]+1)
         except:
             self.features['bi_linearizers'] = [0]
 
         z = self.pvar(f"bi_linearizer{self.features['bi_linearizers'][-1]}")
         self.con(z <= integer)
-        self.con(z <= binary*ub_integer)
-        self.con(z >= integer - ub_integer*(1-binary))
+        self.con(z <= binary * ub_integer)
+        self.con(z >= integer - ub_integer * (1 - binary))
         return z
 
+
     def lin_prod_ip(self, integer, positive, ub_integer, ub_positive):
         """
         Linearizes a Integer * Positive product.
 
-        constraints: +1+3*(mt.ceil(mt.log2(ub_integer + 1)))
-        positive variables: +(mt.ceil(mt.log2(ub_integer + 1)))
-        binary variables: +(mt.ceil(mt.log2(ub_integer + 1)))
-        """
+        Returns:
+            The linearized expression.
 
+        Note:
+            The linearization requires +1 + 3 * (mt.ceil(mt.log2(ub_integer + 1))) constraints, +(mt.ceil(mt.log2(ub_integer + 1))) positive variables, and +(mt.ceil(mt.log2(ub_integer + 1))) binary variables.
+        """
         try:
             self.features['ip_linearizers'].append(
                 self.features['ip_linearizers'][-1]+1)
         except:
             self.features['ip_linearizers'] = [0]
 
         z = self.pvar(f"ip_linearizer{self.features['ip_linearizers'][-1]}", [
-                      range(mt.ceil(mt.log2(ub_integer + 1)))])
+                    range(mt.ceil(mt.log2(ub_integer + 1)))])
         x = self.bvar(f"ip_binary_convert{self.features['ip_linearizers'][-1]}", [
-                      range(mt.ceil(mt.log2(ub_integer + 1)))])
+                    range(mt.ceil(mt.log2(ub_integer + 1)))])
 
         self.con(integer == sum(
             2**i * x[i] for i in range(mt.ceil(mt.log2(ub_integer + 1)))))
 
         for i in range(mt.ceil(mt.log2(ub_integer + 1))):
-
             self.con(z[i] <= positive)
-            self.con(z[i] <= x[i]*ub_positive)
-            self.con(z[i] >= positive - ub_positive*(1-x[i]))
+            self.con(z[i] <= x[i] * ub_positive)
+            self.con(z[i] >= positive - ub_positive * (1 - x[i]))
 
         return sum(2**i * z[i] for i in range(mt.ceil(mt.log2(ub_integer + 1))))
 
     def lin_prod_ii(self, integer1, integer2, ub_integer1, ub_integer2):
         """
         Linearizes a Integer * Integer product.
 
-        constraints: +1+3*(mt.ceil(mt.log2(ub_integer + 1)))
-        positive variables: +(mt.ceil(mt.log2(ub_integer + 1)))
-        binary variables: +(mt.ceil(mt.log2(ub_integer + 1)))
+        Returns:
+            The linearized expression.
+
+        Note:
+            The linearization requires +1 + 3 * (mt.ceil(mt.log2(ub_integer + 1))) constraints, +(mt.ceil(mt.log2(ub_integer + 1))) positive variables, and +(mt.ceil(mt.log2(ub_integer + 1))) binary variables.
         """
         try:
             self.features['ii_linearizers'].append(
                 self.features['ii_linearizers'][-1]+1)
         except:
             self.features['ii_linearizers'] = [0]
 
         z = self.pvar(f"ii_linearizer{self.features['ii_linearizers'][-1]}", [
-                      range(mt.ceil(mt.log2(ub_integer1 + 1)))])
+                    range(mt.ceil(mt.log2(ub_integer1 + 1)))])
         x = self.bvar(f"ii_binary_convert{self.features['ii_linearizers'][-1]}", [
-                      range(mt.ceil(mt.log2(ub_integer1 + 1)))])
+                    range(mt.ceil(mt.log2(ub_integer1 + 1)))])
 
         self.con(integer1 == sum(
             2**i * x[i] for i in range(mt.ceil(mt.log2(ub_integer1 + 1)))))
 
         for i in range(mt.ceil(mt.log2(ub_integer1 + 1))):
-
             self.con(z[i] <= integer2)
-            self.con(z[i] <= x[i]*ub_integer2)
-            self.con(z[i] >= integer2 - ub_integer2*(1-x[i]))
+            self.con(z[i] <= x[i] * ub_integer2)
+            self.con(z[i] >= integer2 - ub_integer2 * (1 - x[i]))
 
         return sum(2**i * z[i] for i in range(mt.ceil(mt.log2(ub_integer1 + 1))))
 
     # Methods for constraint programming
 
     def start_of(self, interval_variable, absent_value=None):
         """
+        Returns the start time of an interval_variable.
 
-        Returns the start of an interval_variable. 
-        If it was absent, the absent_value is returned, which is by default equal to 0.
+        If the interval_variable is absent in the solution, the absent_value is returned. 
+        The default absent_value is 0.
 
-        """
+        Parameters:
+        interval_variable: The interval variable whose start time is to be returned.
+        absent_value: The value to be returned if the interval_variable is absent in the solution.
 
+        Returns:
+        The start time of the interval_variable or the absent_value if the interval_variable is absent in the solution.
+        """
         if self.features['interface_name'] == 'cplex_cp':
             return self.model.start_of(interval_variable, absent_value)
         if self.features['interface_name'] == 'ortools_cp':
             return interval_variable.StartExpr()
 
     def end_of(self, interval_variable, absent_value=None):
         """
-        Returns the end of an interval_variable. 
-        If it was absent, the absent_value is returned, which is by default equal to 0.
-        """
+        Returns the end time of an interval_variable.
 
+        If the interval_variable is absent in the solution, the absent_value is returned. 
+        The default absent_value is 0.
+
+        Parameters:
+        interval_variable: The interval variable whose end time is to be returned.
+        absent_value: The value to be returned if the interval_variable is absent in the solution.
+
+        Returns:
+        The end time of the interval_variable or the absent_value if the interval_variable is absent in the solution.
+        """
         if self.features['interface_name'] == 'cplex_cp':
             return self.model.end_of(interval_variable, absent_value)
         if self.features['interface_name'] == 'ortools_cp':
             return interval_variable.EndExpr()
 
     def length_of(self, interval_variable, absent_value=None):
         """
+        Returns the length of an interval_variable.
 
-        Returns the length of an interval_variable. 
-        If it was absent, the absent_value is returned, which is by default equal to 0.
+        If the interval_variable is absent in the solution, the absent_value is returned. 
+        The default absent_value is 0.
 
-        """
+        Parameters:
+        interval_variable: The interval variable whose length is to be returned.
+        absent_value: The value to be returned if the interval_variable is absent in the solution.
 
+        Returns:
+        The length of the interval_variable or the absent_value if the interval_variable is absent in the solution.
+        """
         if self.features['interface_name'] == 'cplex_cp':
             return self.model.length_of(interval_variable, absent_value)
         if self.features['interface_name'] == 'ortools_cp':
             return interval_variable.EndExpr() - interval_variable.StartExpr()
 
     def size_of(self, interval_variable, absent_value=None):
         """
+        Returns the size of an interval_variable.
 
-        Returns the size of an interval_variable. 
-        If it was absent, the absent_value is returned, which is by default equal to 0.
+        If the interval_variable is absent in the solution, the absent_value is returned. 
+        The default absent_value is 0.
 
-        """
+        Parameters:
+        interval_variable: The interval variable whose size is to be returned.
+        absent_value: The value to be returned if the interval_variable is absent in the solution.
 
+        Returns:
+        The size of the interval_variable or the absent_value if the interval_variable is absent in the solution.
+        """
         if self.features['interface_name'] == 'cplex_cp':
             return self.model.size_of(interval_variable, absent_value)
         if self.features['interface_name'] == 'ortools_cp':
             return interval_variable.SizeExpr()
 
     def presence_of(self, interval_variable):
         """
-
         Returns the presence (1) or absence (0) of an interval_variable. 
-        Can be used for assignments.
 
+        This method can be used to check whether the interval_variable is present in the solution.
+
+        Parameters:
+        interval_variable: The interval variable whose presence is to be checked.
+
+        Returns:
+        1 if the interval_variable is present in the solution, 0 otherwise.
         """
         if self.features['interface_name'] == 'cplex_cp':
-
             return self.model.presence_of(interval_variable)
-
         if self.features['interface_name'] == 'ortools_cp':
+            return interval_variable.IsPresent().Value()
 
-            return 1
-
-    def prec_start_at_start(self, one, two, delay=None):
+    def prec_start_at_start(self, one, two, delay=0):
         """
-        start(one) + delay == start(two)
+        Returns a boolean expression that checks if the start time of interval variable 'one' 
+        plus a specified delay equals the start time of interval variable 'two'.
         """
-
         if self.features['interface_name'] == 'cplex_cp':
             return self.model.start_at_start(one, two, delay)
         if self.features['interface_name'] == 'ortools_cp':
             return one.StartExpr() + delay == two.StartExpr()
 
-    def prec_start_at_end(self, one, two, delay=None):
+    def prec_start_at_end(self, one, two, delay=0):
         """
-        start(one) + delay == end(two)
+        Returns a boolean expression that checks if the start time of interval variable 'one' 
+        plus a specified delay equals the end time of interval variable 'two'.
         """
-
         if self.features['interface_name'] == 'cplex_cp':
             return self.model.start_at_end(one, two, delay)
         if self.features['interface_name'] == 'ortools_cp':
             return one.StartExpr() + delay == two.EndExpr()
 
-    def prec_start_before_start(self, one, two, delay=None):
+    def prec_start_before_start(self, one, two, delay=0):
         """
-        start(one) + delay <= start(two)
+        Returns a boolean expression that checks if the start time of interval variable 'one' 
+        plus a specified delay is less than or equal to the start time of interval variable 'two'.
         """
-
         if self.features['interface_name'] == 'cplex_cp':
             return self.model.start_before_start(one, two, delay)
         if self.features['interface_name'] == 'ortools_cp':
             return one.StartExpr() + delay <= two.StartExpr()
 
-    def prec_start_before_end(self, one, two, delay=None):
+    def prec_start_before_end(self, one, two, delay=0):
         """
-        start(one) + delay <= end(two)
+        Returns a boolean expression that checks if the start time of interval variable 'one' 
+        plus a specified delay is less than or equal to the end time of interval variable 'two'.
         """
-
         if self.features['interface_name'] == 'cplex_cp':
             return self.model.start_before_end(one, two, delay)
         if self.features['interface_name'] == 'ortools_cp':
             return one.StartExpr() + delay <= two.EndExpr()
 
-    def prec_end_at_start(self, one, two, delay=None):
+    def prec_end_at_start(self, one, two, delay=0):
         """
-        end(one) + delay == start(two)
+        Returns a boolean expression that checks if the end time of interval variable 'one' 
+        plus a specified delay equals the start time of interval variable 'two'.
         """
-
         if self.features['interface_name'] == 'cplex_cp':
             return self.model.end_at_start(one, two, delay)
         if self.features['interface_name'] == 'ortools_cp':
             return one.EndExpr() + delay == two.StartExpr()
 
-    def prec_end_at_end(self, one, two, delay=None):
+    def prec_end_at_end(self, one, two, delay=0):
         """
-        end(one) + delay == end(two)
+        Returns a boolean expression that checks if the end time of interval variable 'one' 
+        plus a specified delay equals the end time of interval variable 'two'.
         """
-
         if self.features['interface_name'] == 'cplex_cp':
             return self.model.end_at_end(one, two, delay)
         if self.features['interface_name'] == 'ortools_cp':
             return one.EndExpr() + delay == two.EndExpr()
 
-    def prec_end_before_start(self, one, two, delay=None):
+    def prec_end_before_start(self, one, two, delay=0):
         """
-        end(one) + delay <= start(two)
+        Returns a boolean expression that checks if the end time of interval variable 'one' 
+        plus a specified delay is less than or equal to the start time of interval variable 'two'.
         """
-
         if self.features['interface_name'] == 'cplex_cp':
             return self.model.end_before_start(one, two, delay)
         if self.features['interface_name'] == 'ortools_cp':
             return one.EndExpr() + delay <= two.StartExpr()
 
-    def prec_end_before_end(self, one, two, delay=None):
+    def prec_end_before_end(self, one, two, delay=0):
         """
-        end(one) + delay <= end(two)
+        Returns a boolean expression that checks if the end time of interval variable 'one' 
+        plus a specified delay is less than or equal to the end time of interval variable 'two'.
         """
-
         if self.features['interface_name'] == 'cplex_cp':
             return self.model.end_before_end(one, two, delay)
         if self.features['interface_name'] == 'ortools_cp':
             return one.EndExpr() + delay <= two.EndExpr()
 
     def forbid_start(self, interval, function):
         """
-
         Forbids an interval variable to start during specified regions.
 
+        Parameters:
+        interval (IntervalVar): The interval variable.
+        function (function): The function that specifies forbidden regions.
+
         """
 
         if self.features['interface_name'] == 'cplex_cp':
-
             return self.model.forbid_start(interval, function)
 
         if self.features['interface_name'] == 'ortools_cp':
-
-            ""
+            forbidden_domains = function(interval)
+            for domain in forbidden_domains:
+                self.model.Add(interval.StartExpr() < domain[0])
+                self.model.Add(interval.StartExpr() > domain[1])
 
     def forbid_end(self, interval, function):
         """
-
         Forbids an interval variable to end during specified regions.
 
+        Parameters:
+        interval (IntervalVar): The interval variable.
+        function (function): The function that specifies forbidden regions.
+
         """
 
         if self.features['interface_name'] == 'cplex_cp':
-
             return self.model.forbid_end(interval, function)
 
         if self.features['interface_name'] == 'ortools_cp':
-
-            ""
+            forbidden_domains = function(interval)
+            for domain in forbidden_domains:
+                self.model.Add(interval.EndExpr() < domain[0])
+                self.model.Add(interval.EndExpr() > domain[1])
 
     def forbid_overlap(self, interval_variables, transition_matrix=None):
         """
-
         Forbids overlapping of interval variables.
 
+        Parameters:
+        interval_variables (list of IntervalVar): The list of interval variables.
+        transition_matrix (list of list of bool, optional): Transition matrix. Defaults to None.
+
         """
 
         if self.features['interface_name'] == 'cplex_cp':
-
             if transition_matrix == None:
-
                 return self.model.no_overlap(interval_variables)
-
             else:
-
                 return self.model.no_overlap(interval_variables, transition_matrix)
 
         if self.features['interface_name'] == 'ortools_cp':
-
             return self.model.AddNoOverlap(interval_variables)
 
     def forbid_extent(self, interval, function):
         """
-
         Forbid an interval variable to overlap with specified regions.
 
+        Parameters:
+        interval (IntervalVar): The interval variable.
+        function (function): The function that specifies forbidden regions.
+
         """
 
         if self.features['interface_name'] == 'cplex_cp':
-
             return self.model.forbid_extent(interval, function)
 
         if self.features['interface_name'] == 'ortools_cp':
-
-            ""
+            forbidden_domains = function(interval)
+            for domain in forbidden_domains:
+                self.model.Add(interval.EndExpr() < domain[0])
+                self.model.Add(interval.StartExpr() > domain[1])
 
     def overlap_length(self, interval_variable1, interval_variable2, absent_value=None):
         """
         To get the length of the overlap of two interval variables.
         """
 
         if self.features['interface_name'] == 'cplex_cp':
-
             return self.model.overlap_length(interval_variable1, interval_variable2, absent_value)
 
         if self.features['interface_name'] == 'ortools_cp':
-
-            ""
+            overlap_start = self.model.NewIntVar(0, self.model.Horizon(), "")
+            overlap_end = self.model.NewIntVar(0, self.model.Horizon(), "")
+            self.model.Add(overlap_start <= interval_variable1.EndExpr())
+            self.model.Add(overlap_end >= interval_variable1.StartExpr())
+            return overlap_end - overlap_start
 
     def start_eval(self, interval, function, absent_value=None):
         """
         To evaluate a segmented function at the start of an interval variable
         """
 
         if self.features['interface_name'] == 'cplex_cp':
-
             return self.model.start_eval(interval, function, absent_value)
 
         if self.features['interface_name'] == 'ortools_cp':
-
-            ""
+            return function(interval.StartExpr().Value())
 
     def end_eval(self, interval, function, absent_value=None):
         """
         To evaluate a segmented function at the end of an interval variable
         """
 
         if self.features['interface_name'] == 'cplex_cp':
-
             return self.model.end_eval(interval, function, absent_value)
 
         if self.features['interface_name'] == 'ortools_cp':
-
-            ""
+            return function(interval.EndExpr().Value())
 
     def size_eval(self, interval, function, absent_value=None):
         """
         To evaluate a segmented function on the size of an interval variable
         """
-
         if self.features['interface_name'] == 'cplex_cp':
-
             return self.model.size_eval(interval, function, absent_value)
 
         if self.features['interface_name'] == 'ortools_cp':
-
-            ""
+            return function(interval.SizeExpr().Value())
 
     def length_eval(self, interval, function, absent_value=None):
         """
         To evaluate a segmented function on the length of an interval variable
         """
 
         if self.features['interface_name'] == 'cplex_cp':
-
             return self.model.length_eval(interval, function, absent_value)
 
         if self.features['interface_name'] == 'ortools_cp':
-
-            ""
+            return function(interval.SizeExpr().Value())
 
     def span(self, interval, function, absent_value=None):
         """
         Forces that one interval variable must exactly cover a set of interval variables.
         """
 
         if self.features['interface_name'] == 'cplex_cp':
             return self.model.span(interval, function, absent_value)
-        if self.features['interface_name'] == 'ortools_cp':
 
-            ""
+        if self.features['interface_name'] == 'ortools_cp':
+            intervals = function(interval)
+            for i in intervals:
+                self.model.Add(interval.StartExpr() <= i.StartExpr())
+                self.model.Add(interval.EndExpr() >= i.EndExpr())
 
-    def always_equal(self, state_fucntion, input1, input2):
+    def always_equal(self, state_function, input1, input2):
         """
-
         Creates an equality constraint between two expressions.
-
         """
 
         if self.features['interface_name'] == 'cplex_cp':
-
-            return self.model.always_equal(state_fucntion, input1, input2)
+            return self.model.always_equal(state_function, input1, input2)
 
         if self.features['interface_name'] == 'ortools_cp':
-
-            ""
+            return self.model.Add(input1 == input2)
 
     def alternative(self, interval, array, cardinality=None):
         """
         Create an alternative constraint between interval variables.
         """
 
         if self.features['interface_name'] == 'cplex_cp':
-
             return self.model.alternative(interval, array, cardinality)
 
         if self.features['interface_name'] == 'ortools_cp':
-
-            ""
+            self.model.Add(sum([self.model.NewBoolVar('') for _ in array]) == 1)
 
     def all_dist_above(self, exprs, value):
+        """
+        All expressions should be greater than or equal to the specified value.
+        """
 
         if self.features['interface_name'] == 'cplex_cp':
-
             return self.model.all_min_distance(exprs, value)
 
-        else:
-
-            return abs(exprs) >= value
+        if self.features['interface_name'] == 'ortools_cp':
+            for expr in exprs:
+                self.model.Add(expr >= value)
 
     def sum(self, input):
 
-        return self.model.sum(input)
+        """
+        Sum of all values in the input.
+        """
+
+        return self.model.Sum(input)
 
     def if_then(self, input1, input2):
+        """
+        If input1 is true, then return input2.
+        """
 
         if self.features['interface_name'] == 'cplex_cp':
-
             return self.model.if_then(input1, input2)
 
-        else:
-
+        if self.features['interface_name'] == 'ortools_cp':
             if input1:
-
                 return input2
 
-    def control_resource(self, *args, function='pulse'):
+    def synchronize(self, interval, array):
+        """
+        Synchronizes an interval variable interval and a set of interval variables in array.
         """
-        Creates and returns a dynamic resource usage control function.
 
-        A cumulative function expression can be modified with the atomic demand functions:
+        return self.model.synchronize(interval,array)
 
-        function = 'step', change resource level by a given amount at a given time.
-        function = 'pulse', change resource level by a given amount based on the length of a given interval variable or fixed interval.
-        function = 'start', change resource level by a given amount based on the start of a given interval variable.
-        function = 'end', change resource level by by a given amount at the end of a given interval variable.
+    def control_resource(self, *args, function='pulse'):
+        """
+        Creates and returns a dynamic resource usage control function.
         """
 
         if function == 'pulse':
             return self.model.pulse(*args)
         if function == 'step':
             return self.model.step(*args)
         if function == 'start':
             return self.model.step_at_start(*args)
         if function == 'end':
             return self.model.step_at_end(*args)
 
-    # Methods for modeling and solving.
+    def circuit(self, nodes):
+        """
+        Creates a circuit constraint.
 
-    def obj(self, expression, direction=None, label=None):
+        The circuit constraint ensures that there is a Hamiltonian circuit on the nodes.
         """
-        Objective Function Definition
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-        To define an objective function.
+        if self.features['interface_name'] == 'cplex_cp':
+            return self.model.circuit(nodes)
 
-        Args:
-            expression (formula): what are the terms of this objective?
-            direction (str, optional): what is the direction for optimizing this objective?. Defaults to None.
+        if self.features['interface_name'] == 'ortools_cp':
+            return self.model.AddCircuit(nodes)
+
+    def allowed_assignments(self, variables, tuples):
         """
+        Creates an allowed assignments constraint.
 
-        match self.features['solution_method']:
+        The allowed assignments constraint ensures that the values assigned to the variables are in the list of tuples.
+        """
+        if self.features['interface_name'] == 'cplex_cp':
+            return self.model.allowed_assignments(variables, tuples)
 
-            case 'exact':
+        if self.features['interface_name'] == 'ortools_cp':
+            return self.model.AddAllowedAssignments(variables, tuples)
 
-                self.features['directions'].append(direction)
-                self.features['objectives'].append(expression)
-                self.features['objective_labels'].append(label)
-                self.features['objective_counter'][0] += 1
-                self.features['objective_counter'][1] += 1
+    def inverse(self, variables, inverse_variables):
+        """
+        Creates an inverse constraint.
 
-            case 'heuristic':
+        The inverse constraint ensures that if variables[i] = j then inverse_variables[j] = i and vice versa.
+        """
+        if self.features['interface_name'] == 'cplex_cp':
+            return self.model.inverse(variables, inverse_variables)
 
-                if self.features['agent_status'] == 'idle':
+        if self.features['interface_name'] == 'ortools_cp':
+            return self.model.AddInverse(variables, inverse_variables)
+
+    def logical_and(self, expr1, expr2):
+        """
+        Creates a logical AND constraint.
+        """
+        if self.features['interface_name'] == 'cplex_cp':
+            return self.model.logical_and(expr1, expr2)
 
-                    self.features['directions'].append(direction)
-                    self.features['objectives'].append(expression)
-                    self.features['objective_labels'].append(label)
-                    self.features['objective_counter'][0] += 1
-                    self.features['objective_counter'][1] += 1
+        if self.features['interface_name'] == 'ortools_cp':
+            return self.model.AddBoolAnd([expr1, expr2])
 
-                else:
-                    self.features['directions'].append(direction)
-                    self.features['objective_counter'][0] += 1
-                    self.features['objectives'].append(expression)
+    def logical_or(self, expr1, expr2):
+        """
+        Creates a logical OR constraint.
+        """
+        if self.features['interface_name'] == 'cplex_cp':
+            return self.model.logical_or(expr1, expr2)
+            
+        if self.features['interface_name'] == 'ortools_cp':
+            return self.model.AddBoolOr([expr1, expr2])
+
+    def logical_not(self, expr):
+        """
+        Creates a logical NOT constraint.
+        """
+        if self.features['interface_name'] == 'cplex_cp':
+            return self.model.logical_not(expr)
+            
+        if self.features['interface_name'] == 'ortools_cp':
+            return self.model.Not(expr)
+
+    def less_than(self, expr1, expr2):
+        """
+        Creates a less than constraint.
+        """
+        if self.features['interface_name'] == 'cplex_cp':
+            return self.model.less_than(expr1, expr2)
+            
+        if self.features['interface_name'] == 'ortools_cp':
+            return self.model.Add(expr1 < expr2)
+
+    def greater_than(self, expr1, expr2):
+        """
+        Creates a greater than constraint.
+        """
+        if self.features['interface_name'] == 'cplex_cp':
+            return self.model.greater_than(expr1, expr2)
+            
+        if self.features['interface_name'] == 'ortools_cp':
+            return self.model.Add(expr1 > expr2)
+
+    # Methods for modeling and solving.
+
+    def obj(self, expression=0, direction=None, label=None):
+        """
+        Defines an objective function for the optimization problem.
+
+        Args:
+            expression (formula): The terms of the objective function.
+            direction (str, optional): The direction for optimizing this objective ("min" or "max"). Defaults to None.
+            label (str, optional): The label for this objective function. Defaults to None.
+        """
+
+        if self.features['solution_method'] == 'exact' or (self.features['solution_method'] == 'heuristic' and self.features['agent_status'] == 'idle'):
+
+            self.features['directions'].append(direction)
+            self.features['objectives'].append(expression)
+            self.features['objective_labels'].append(label)
+
+            self.features['objective_counter'][0] += 1
+            self.features['objective_counter'][1] += 1
+
+        elif self.features['solution_method'] == 'heuristic' and self.features['agent_status'] != 'idle':
+
+            self.features['directions'].append(direction)
+            self.features['objectives'].append(expression)
+            self.features['objective_counter'][0] += 1
 
     def con(self, expression, label=None):
         """
         Constraint Definition
         ~~~~~~~~~~~~~~~~~~~~~
         To define a constraint.
 
@@ -1382,85 +1998,113 @@
 
                         self.features['constraints'].append(
                             np.reshape(expression, [np.shape(self.agent)[0], 1]))
 
                     else:
                         self.features['constraints'].append(expression)
 
-    def sol(self, directions=None, solver_name=None, solver_options=dict(), objective_id=0, email=None, debug=False, time_limit=None, cpu_threads=None, absolute_gap=None, relative_gap=None, show_log=False, save_log=False, save_model=False, max_iterations=None):
+    def sol(self, directions=None, solver_name=None, solver_options=dict(), obj_id=0, email=None, debug=False, time_limit=None, cpu_threads=None, absolute_gap=None, relative_gap=None, show_log=False, save_log=False, save_model=False, max_iterations=None, obj_operators=[]):
         """
         Solve Command Definition
         ~~~~~~~~~~~~~~~~~~~~~~~~
         To define solver and its settings to solve the problem.
 
         Args:
             directions (list, optional): please set the optimization directions of the objectives, if not provided before. Defaults to None.
             solver_name (_type_, optional): please set the solver_name. Defaults to None.
             solver_options (dict, optional): please set the solver options using a dictionary with solver specific keys. Defaults to None.
-            objective_id (int, optional): please provide the objective id (number) that you wish to optimize. Defaults to 0.
+            obj_id (int, optional): please provide the objective id (number) that you wish to optimize. Defaults to 0.
             email (_type_, optional): please provide your email address if you wish to use cloud solvers (e.g., NEOS server). Defaults to None.
             debug (bool, optional): please state if the model should be checked for feasibility or logical bugs. Defaults to False.
             time_limit (seconds, optional): please state if the model should be solved under a specific timelimit. Defaults to None.
             cpu_threads (int, optional): please state if the solver should use a specific number of cpu threads. Defaults to None.
             absolute_gap (value, optional): please state an abolute gap to find the optimal objective value. Defaults to None.
             relative_gap (%, optional): please state a releative gap (%) to find the optimal objective value. Defaults to None.
         """
 
-        if len(directions)<len(self.features['objectives']):
+        if self.no_agents!=None:
+            if self.features['interface_name'] in ['mealpy' , 'feloopy']:
+                solver_options['pop_size'] = self.no_agents
+        
+        if len(self.features['objectives']) !=0 and len(directions)!=len(self.features['objectives']):
             raise MultiObjectivityError("The number of directions and the provided objectives do not match.")
 
-        self.features['objective_being_optimized'] = objective_id
-        self.features['solver_name'] = solver_name
+        self.features['objective_being_optimized'] = obj_id
         self.features['solver_options'] = solver_options
         self.features['debug_mode'] = debug
         self.features['time_limit'] = time_limit
         self.features['thread_count'] = cpu_threads
         self.features['absolute_gap'] = absolute_gap
         self.features['relative_gap'] = relative_gap
         self.features['log'] = show_log
         self.features['write_model_file'] = save_model
         self.features['save_solver_log'] = save_log
         self.features['email_address'] = email
         self.features['max_iterations'] = max_iterations
+        self.features['obj_operators'] = obj_operators
+        self.features['solver_name'] = solver_name
 
-        if type(objective_id) != str and directions != None:
+        try:
+            if type(obj_id) != str and directions != None:
 
-            if self.features['directions'][objective_id] == None:
+                if self.features['directions'][obj_id] == None:
 
-                self.features['directions'][objective_id] = directions[objective_id]
+                    self.features['directions'][obj_id] = directions[obj_id]
 
-            for i in range(len(self.features['objectives'])):
+                for i in range(len(self.features['objectives'])):
 
-                if i != objective_id:
+                    if i != obj_id:
 
-                    del self.features['directions'][i]
+                        del self.features['directions'][i]
 
-                    del directions[i]
+                        del directions[i]
 
-                    del self.features['objectives'][i]
+                        del self.features['objectives'][i]
 
-            objective_id = 0
+                obj_id = 0
 
-            self.features['objective_counter'] = [1, 1]
+                self.features['objective_counter'] = [1, 1]
 
-        else:
+            else:
 
-            for i in range(len(self.features['directions'])):
+                for i in range(len(self.features['directions'])):
 
-                self.features['directions'][i] = directions[i]
+                    self.features['directions'][i] = directions[i]
+        except:
+            pass
 
         match self.features['solution_method']:
 
             case 'exact':
 
                 self.features['model_object_before_solve'] = self.model
 
                 from .generators import solution_generator
-                self.solution = solution_generator.generate_solution(
-                    self.features)
+
+                try:
+                    if len(self.features['objectives'])==0:
+                        self.obj()
+                        self.features['objective_counter'][1] = 0
+                        self.features['directions'] = ["nan"]
+                        self.features['solver_name'] = directions
+        
+                    self.solution = solution_generator.generate_solution(
+                        self.features)
+                
+                except:
+
+                    if len(self.features['objectives'])==0:
+                        self.obj()
+                        self.features['objective_counter'][1] = 0
+                        self.features['directions'] = ["min"]
+                        self.features['solver_name'] = directions
+        
+                    self.solution = solution_generator.generate_solution(self.features)
+                    
+
 
                 try:
                     self.obj_val = self.get_objective()
                     self.status = self.get_status()
                     self.cpt = self.get_time()*10**6
 
                 except:
@@ -1472,88 +2116,126 @@
 
                     "Do nothing"
 
                 else:
 
                     if self.features['vectorized']:
 
-                        self.penalty = np.zeros(np.shape(self.agent)[0])
+                        if self.features['interface_name']=='feloopy':
 
-                        if self.features['penalty_coefficient'] != 0 and len(self.features['constraints']) == 1:
+                            self.penalty = np.zeros(np.shape(self.agent)[0])
 
-                            self.features['constraints'][0] = np.reshape(
-                                self.features['constraints'][0], [np.shape(self.agent)[0], 1])
-                            self.features['constraints'].append(
-                                np.zeros(shape=(np.shape(self.agent)[0], 1)))
-                            self.penalty = np.amax(np.concatenate(
-                                self.features['constraints'], axis=1), axis=1)
-
-                            self.agent[np.where(self.penalty == 0), -2] = 1
-                            self.agent[np.where(self.penalty > 0), -2] = -1
-
-                        if self.features['penalty_coefficient'] != 0 and len(self.features['constraints']) > 1:
-
-                            self.features['constraints'].append(
-                                np.zeros(shape=(np.shape(self.agent)[0], 1)))
-                            self.penalty = np.amax(np.concatenate(
-                                self.features['constraints'], axis=1), axis=1)
-                            self.agent[np.where(self.penalty == 0), -2] = 1
-                            self.agent[np.where(self.penalty > 0), -2] = -1
+                            if self.features['penalty_coefficient'] != 0 and len(self.features['constraints']) == 1:
 
-                        else:
+                                self.features['constraints'][0] = np.reshape(
+                                    self.features['constraints'][0], [np.shape(self.agent)[0], 1])
+                                self.features['constraints'].append(
+                                    np.zeros(shape=(np.shape(self.agent)[0], 1)))
+                                self.penalty = np.amax(np.concatenate(
+                                    self.features['constraints'], axis=1), axis=1)
+
+                                self.agent[np.where(self.penalty == 0), -2] = 1
+                                self.agent[np.where(self.penalty > 0), -2] = -1
+
+                            if self.features['penalty_coefficient'] != 0 and len(self.features['constraints']) > 1:
+
+                                self.features['constraints'].append(
+                                    np.zeros(shape=(np.shape(self.agent)[0], 1)))
+                                self.penalty = np.amax(np.concatenate(
+                                    self.features['constraints'], axis=1), axis=1)
+                                self.agent[np.where(self.penalty == 0), -2] = 1
+                                self.agent[np.where(self.penalty > 0), -2] = -1
 
-                            self.agent[:, -2] = 2
+                            else:
+
+                                self.agent[:, -2] = 2
+
+                            if type(obj_id) != str:
+
+                                if directions[obj_id] == 'max':
+                                    self.agent[:, -1] = np.reshape(self.features['objectives'][obj_id], [self.agent.shape[0],]) - np.reshape(
+                                        self.features['penalty_coefficient'] * (self.penalty)**2, [self.agent.shape[0],])
+
+                                if directions[obj_id] == 'min':
+                                    self.agent[:, -1] = np.reshape(self.features['objectives'][obj_id], [self.agent.shape[0],]) + np.reshape(
+                                        self.features['penalty_coefficient'] * (self.penalty)**2, [self.agent.shape[0],])
+
+                            else:
+
+                                self.agent[:, -1] = 0
+
+                                total_obj = self.features['objective_counter'][0]
+                                
+                                self.features['objectives'] = np.array(self.features['objectives']).T
 
-                        if type(objective_id) != str:
+                                print(self.features['objectives'])
 
-                            if directions[objective_id] == 'max':
-                                self.agent[:, -1] = np.reshape(self.features['objectives'][objective_id], [self.agent.shape[0],]) - np.reshape(
-                                    self.features['penalty_coefficient'] * (self.penalty)**2, [self.agent.shape[0],])
+                                for i in range(self.features['objective_counter'][0]):
 
-                            if directions[objective_id] == 'min':
-                                self.agent[:, -1] = np.reshape(self.features['objectives'][objective_id], [self.agent.shape[0],]) + np.reshape(
-                                    self.features['penalty_coefficient'] * (self.penalty)**2, [self.agent.shape[0],])
+                                    if directions[i] == 'max':
+                                        self.agent[:, -2-total_obj+i] = self.features['objectives'][:,i] - self.features['penalty_coefficient'] * (self.penalty)**2
 
+                                    if directions[i] == 'min':
+                                        self.agent[:, -2-total_obj+i] = self.features['objectives'][:,i] + self.features['penalty_coefficient'] * (self.penalty)**2
                         else:
 
-                            self.agent[:, -1] = 0
+                            self.penalty = np.zeros(np.shape(self.agent)[0])
 
-                            total_obj = self.features['objective_counter'][0]
+                            if self.features['penalty_coefficient'] != 0 and len(self.features['constraints']) == 1:
 
-                            self.features['objectives'] = np.array(
-                                self.features['objectives']).T[0]
+                                self.features['constraints'][0] = np.reshape(self.features['constraints'][0], [np.shape(self.agent)[0], 1])
+                                self.features['constraints'].append(np.zeros(shape=(np.shape(self.agent)[0], 1)))
+                                self.penalty = np.amax(np.concatenate(self.features['constraints'], axis=1), axis=1)
 
-                            for i in range(self.features['objective_counter'][0]):
+                            if self.features['penalty_coefficient'] != 0 and len(self.features['constraints']) > 1:
 
-                                if directions[i] == 'max':
-                                    self.agent[:, -2-total_obj+i] = self.features['objectives'][:,
-                                                                                                i] - self.features['penalty_coefficient'] * (self.penalty)**2
+                                self.features['constraints'].append(np.zeros(shape=(np.shape(self.agent)[0], 1)))
+                                self.penalty = np.amax(np.concatenate(self.features['constraints'], axis=1), axis=1)
 
-                                if directions[i] == 'min':
-                                    self.agent[:, -2-total_obj+i] = self.features['objectives'][:,
-                                                                                                i] + self.features['penalty_coefficient'] * (self.penalty)**2
+                            if type(obj_id) != str:
 
+                                if directions[obj_id] == 'max':
+                                    self.sing_result = np.reshape(self.features['objectives'][obj_id], [self.agent.shape[0],]) - np.reshape(self.features['penalty_coefficient'] * (self.penalty)**2, [self.agent.shape[0],])
+
+                                if directions[obj_id] == 'min':
+                                    self.sing_result = np.reshape(self.features['objectives'][obj_id], [self.agent.shape[0],]) + np.reshape(self.features['penalty_coefficient'] * (self.penalty)**2, [self.agent.shape[0],])
+
+                            else:
+
+                                total_obj = self.features['objective_counter'][0]
+
+                                self.sing_result = []
+                                
+
+                                for i in range(self.features['objective_counter'][0]):
+
+                                    
+                                    if directions[i] == 'max':
+                                        self.sing_result.append(self.features['objectives'][i] - self.features['penalty_coefficient'] * (self.penalty)**2)
+
+                                    if directions[i] == 'min':
+                                        self.sing_result.append(self.features['objectives'][i] + self.features['penalty_coefficient'] * (self.penalty)**2)
                     else:
 
                         self.penalty = 0
 
                         if len(self.features['constraints']) >= 1:
 
                             self.penalty = np.amax(
                                 np.array([0]+self.features['constraints'], dtype=object))
 
-                        if type(objective_id) != str:
+                        if type(obj_id) != str:
 
-                            if directions[objective_id] == 'max':
-                                self.response = self.features['objectives'][objective_id] - \
+                            if directions[obj_id] == 'max':
+                                self.response = self.features['objectives'][obj_id] - \
                                     self.features['penalty_coefficient'] * \
                                     (self.penalty-0)**2
 
-                            if directions[objective_id] == 'min':
-                                self.response = self.features['objectives'][objective_id] + \
+                            if directions[obj_id] == 'min':
+                                self.response = self.features['objectives'][obj_id] + \
                                     self.features['penalty_coefficient'] * \
                                     (self.penalty-0)**2
 
                         else:
 
                             total_obj = self.features['objective_counter'][0]
 
@@ -1573,14 +2255,22 @@
                                         self.features['penalty_coefficient'] * \
                                         (self.penalty)**2
 
     def get_variable(self, variable_with_index):
         from .generators import result_generator
         return result_generator.get(self.features, self.model, self.solution, 'variable', variable_with_index)
 
+    def get_dual(self, constraint_label_with_index):
+        from .generators import result_generator
+        return result_generator.get(self.features, self.model, self.solution, 'dual', constraint_label_with_index)
+
+    def get_slack(self, constraint_label_with_index):
+        from .generators import result_generator
+        return result_generator.get(self.features, self.model, self.solution, 'slack', constraint_label_with_index)
+    
     def get_objective(self):
         from .generators import result_generator
         return result_generator.get(self.features, self.model, self.solution, 'objective', None)
 
     def get_status(self):
         from .generators import result_generator
         return result_generator.get(self.features, self.model, self.solution, 'status', None)
@@ -1589,21 +2279,24 @@
         from .generators import result_generator
         return result_generator.get(self.features, self.model, self.solution, 'time', None)
 
     def get_start(self, invterval_variable):
 
         if self.features['interface_name'] == 'cplex_cp':
             return self.solution[0].get_var_solution(invterval_variable).get_start()
+        
         if self.features['interface_name'] == 'ortools_cp':
+
             ""
 
     def get_interval(self, invterval_variable):
 
         if self.features['interface_name'] == 'cplex_cp':
             return self.solution[0].get_var_solution(invterval_variable)
+        
         if self.features['interface_name'] == 'ortools_cp':
             ""
 
     def get_end(self, invterval_variable):
 
         if self.features['interface_name'] == 'cplex_cp':
             return self.solution[0].get_var_solution(invterval_variable).get_end()
@@ -1648,191 +2341,245 @@
         hour = round((self.get_time()), 3) % (24 * 3600) // 3600
         min = round((self.get_time()), 3) % (24 * 3600) % 3600 // 60
         sec = round((self.get_time()), 3) % (24 * 3600) % 3600 % 60
 
         print(f"cpu time [{self.features['interface_name']}]: ", self.get_time(
         )*10**6, '(microseconds)', "%02d:%02d:%02d" % (hour, min, sec), '(h, m, s)')
 
-    def inf(self):
+    def scen_probs(self):
+        """
+        Returns an array of scenario probabilities
+        """
+        if self.features['interface_name'] in ['rsome_ro', 'rsome_dro']:
+            return self.model.p
+
+    def exval(self,expr):
 
-        data = {"info": ["model", "interface", "solver", "direction", "method"], "detail": [self.features['model_name'], self.features['interface_name'], self.features['solver_name'], self.features['directions'], self.features['solution_method']], "variable": ["positive", "binary", "integer", "free", "tot"], "count [cat,tot]": [str(self.features['positive_variable_counter']), str(
-            self.features['binary_variable_counter']), str(self.features['integer_variable_counter']), str(self.features['free_variable_counter']), str(self.features['total_variable_counter'])], "other": ["objective", "constraint"], "count [cat,tot] ": [self.features['objective_counter'], self.features['constraint_counter']]}
+        """
+        Expected Value
+        --------------
+        1) Returns the expected value of random variables if the uncertainty set of expectations is being determined.
+        2) Returns the worst case expected values of an expression that has random variables inside.
+
+        """
+        if self.features['interface_name'] in ['rsome_ro', 'rsome_dro']:
+            from rsome import E
+            return E(expr)
+
+    def norm(self,expr_or_1D_array_of_variables, degree):
+        
+        """
+        Returns the first, second, or infinity norm of a 1-D array.
+        """
 
-        A = tb(data, headers="keys", tablefmt="github")
+        if self.features['interface_name'] in ['rsome_ro', 'rsome_dro']:
+            from rsome import norm
+            return norm(expr_or_1D_array_of_variables, degree)
+    
+    def sumsqr(self,expr_or_1D_array_of_variables):
 
-        print("~~~~~~~~~~~~\nPROBLEM INFO\n~~~~~~~~~~~~")
-        print(A)
-        print("~~~~~~~~~~~~\n")
 
-        return A
+        if self.features['interface_name'] in ['rsome_ro', 'rsome_dro']:
+        
+            from rsome import sumsqr
+            return sumsqr(expr_or_1D_array_of_variables)
+    
 
     def state_function(self):
         """
 
         Creates and returns a state function.
 
         """
 
         return self.model.state_function()
 
-    def report(self):
-        print()
+    def report(self, all_metrics: bool = False, feloopy_info: bool = True, sys_info: bool = False, model_info: bool = True, sol_info: bool = True, obj_values: bool = True, dec_info: bool = True, metric_info: bool = True, ideal_pareto: Optional[np.ndarray] = [], ideal_point: Optional[np.array] = [], save=None):
+
+        self.interface_name = self.features['interface_name']
+        if self.solution_method_was==None:
+            self.solution_method = self.features['solution_method']
+        else:
+            self.solution_method = self.solution_method_was
+        self.model_name = self.features['model_name']
+        self.solver_name = self.features['solver_name']
+        self.model_constraints = self.features['constraints']
+        self.model_objectives = self.features['objectives']
+        self.objectives_directions = self.features['directions']
+        self.pos_var_counter = self.features['positive_variable_counter']
+        self.bin_var_counter = self.features['binary_variable_counter']
+        self.int_var_counter = self.features['integer_variable_counter']
+        self.free_var_counter = self.features['free_variable_counter']
+        self.event_var_counter = self.features['event_variable_counter']
+        self.tot_counter = self.features['total_variable_counter']
+        self.con_counter = self.features['constraint_counter']
+        self.obj_counter = self.features['objective_counter']
+
+        if save is not None:
+            stdout_origin = sys.stdout
+            sys.stdout = open(save, "w")
 
-        self.InterfaceName = self.features['interface_name']
-        self.SolutionMethod = self.features['solution_method']
-        self.ModelName = self.features['model_name']
-        self.SolverName = self.features['solver_name']
-        self.ModelConstraints = self.features['constraints']
-        self.ModelObjectives = self.features['objectives']
-        self.ObjectivesDirections = self.features['directions']
-        self.PositiveVariableCounter = self.features['positive_variable_counter']
-        self.BinaryVariableCounter = self.features['binary_variable_counter']
-        self.IntegerVariableCounter = self.features['integer_variable_counter']
-        self.FreeVariableCounter = self.features['free_variable_counter']
-        self.ToTalVariableCounter = self.features['total_variable_counter']
-        self.ConstraintsCounter = self.features['constraint_counter']
-        self.ObjectivesCounter = self.features['objective_counter']
-
-
-        import datetime
-        now = datetime.datetime.now()
-        date_str = now.strftime("Date: %Y-%m-%d")
-        time_str = now.strftime("Time: %H:%M:%S")
+        status = self.get_status()
+        hour, min, sec = calculate_time_difference(length=self.get_time())
+
+        if len(str(status)) == 0:
+            status = ['infeasible (constrained)']
 
         box_width = 80
-        padding = box_width - len(date_str) - len(time_str) - 2
+        vspace()
 
-        print("+" + "-"*box_width + "+")
-        print("|" + " " + "FelooPy v0.2.5".center(box_width-2) + " " + "|")
-        print("+" + "-"*box_width + "+")
-        print("| " + date_str + " "*padding + time_str + " |")
-        padding = box_width - len("Solver: "+ self.SolverName) - len("Interface: "+ self.InterfaceName) - 2
-        print("| " + "Interface: " + self.InterfaceName + " "*padding + "Solver: "+ self.SolverName + " |")
-        print("+" + "-"*box_width + "+")
-        print("|" + " " + "Model Information".center(box_width-2) + " " + "|")
-        print("+" + "-"*box_width + "+")
-
-        self.ModelName, self.InterfaceName, self.SolverName, self.ObjectivesDirections, self.SolutionMethod
-        # determine the maximum length of variables
-        ModelName = "The '" + self.ModelName + "' model has:"
-        print("|" + " " + ModelName.center(box_width-2) + " " + "|")
-        if self.PositiveVariableCounter[0]>0:
-            P_report = str(self.PositiveVariableCounter[1]) + " positive variable(s) in " + str(self.PositiveVariableCounter[0]) + " class(es)."
-            print("|" + " " + P_report.center(box_width-2) + " " + "|")
-        if self.BinaryVariableCounter[0]>0:
-            P_report = str(self.BinaryVariableCounter[1]) + " binary variable(s) in " + str(self.BinaryVariableCounter[0]) + " class(es)."
-            print("|" + " " + P_report.center(box_width-2) + " " + "|")
-        if self.IntegerVariableCounter[0]>0:
-            P_report = str(self.IntegerVariableCounter[1]) + " integer variable(s) in " + str(self.IntegerVariableCounter[0]) + " class(es)."
-            print("|" + " " + P_report.center(box_width-2) + " " + "|")
-        if self.FreeVariableCounter[0]>0:
-            P_report = str(self.FreeVariableCounter[1]) + " free variable(s) in " + str(self.FreeVariableCounter[0]) + " class(es)."
-            print("|" + " " + P_report.center(box_width-2) + " " + "|")
-        if self.ObjectivesCounter[0]>0:
-            P_report = str(self.ObjectivesCounter[1]) + " objective(s)."
-            print("|" + " " + P_report.center(box_width-2) + " " + "|")
-        if self.ConstraintsCounter[0]>0:
-            P_report = str(self.ConstraintsCounter[1]) + " constraint(s) in " + str(self.ConstraintsCounter[0]) + " class(es)."
-            print("|" + " " + P_report.center(box_width-2) + " " + "|")
-        P_report =  "Total number of variables is " + str(self.ToTalVariableCounter[1]) + f" in {self.ToTalVariableCounter[1]} class(es)."
-        print("|" + " " + P_report.center(box_width-2) + " " + "|")
-
-
-        print("+" + "-"*box_width + "+")
-        print("|" + " " + "Solve Information".center(box_width-2) + " " + "|")
-        print("+" + "-"*box_width + "+")
-        padding = box_width - len("Method: "+ self.SolutionMethod) - len("Objective Value(s)") - 2
-        print("| " + "Method: "+ self.SolutionMethod + " "*padding + "Objective Value(s)" + " |")
-        status= self.get_status()
-        if len(self.ObjectivesDirections)!=1:
-            row = "| " + "Status: " + " "*(len(status[0]) - len("Status: ")) + " " * (box_width-9*len(self.ObjectivesDirections) +1 - len(str(status[0])) - 3)
-            for j in range(len(self.ObjectivesDirections)):
-                obj_row = self.ObjectivesDirections[j]
-                row += " " * (8 - len(obj_row)) + obj_row
-            print(row + " |")
-            for i in range(len(status)): 
-                row = "| " + str(status[i]) + " " * (box_width-9*len(self.ObjectivesDirections) +1 - len(str(status[i])) - 3)
-                obj_row = self.get_obj()[i]
-                for j in range(len(obj_row)):
-                    num_str = format_string(obj_row[j])
-                    row += " " * (9 - len(num_str)) + num_str
-                print(row + " |")
-        else:
-            row = "| " + "Status: " + " "*(len(status) - len("Status: ")) + " " * (box_width-9*len(self.ObjectivesDirections) +1 - len(str(status)) - 3)
-            for j in range(len(self.ObjectivesDirections)):
-                obj_row = self.ObjectivesDirections[j]
-                row += " " * (8 - len(obj_row)) + obj_row
-            print(row + " |")
-            row = "| " + str(status) + " " * (box_width-9*len(self.ObjectivesDirections) +1 - len(str(status)) - 3)
-            obj_row = self.get_obj()
-            num_str = format_string(obj_row)
-            row += " " * (9 - len(num_str)) + num_str
-            print(row + " |")
-        print("+" + "-"*box_width + "+")
-        print("|" + " " + "Metric Information".center(box_width-2) + " " + "|")
-        print("+" + "-"*box_width + "+")
-        hour = round((self.get_time()), 3) % (24 * 3600) // 3600
-        min = round((self.get_time()), 3) % (24 * 3600) % 3600 // 60
-        sec = round((self.get_time()), 3) % (24 * 3600) % 3600 % 60
+        if feloopy_info:
+            
+            import datetime
+            now = datetime.datetime.now()
+            date_str = now.strftime("Date: %Y-%m-%d")
+            time_str = now.strftime("Time: %H:%M:%S")
+            tline_text("FelooPy v0.2.6")
+            empty_line()
+            two_column(date_str, time_str)
+            two_column(f"Interface: {self.interface_name}", f"Solver: {self.solver_name}")
+            empty_line()
+            bline()
 
-    
-        if len(self.ObjectivesDirections)!=1:
+        if sys_info:
             try:
+                import psutil
+                import cpuinfo
+                import platform
+                tline_text("System")
+                empty_line()
+                cpu_info = cpuinfo.get_cpu_info()["brand_raw"]
+                cpu_cores = psutil.cpu_count(logical=False)
+                cpu_threads = psutil.cpu_count(logical=True)
+                ram_info = psutil.virtual_memory()
+                ram_total = ram_info.total
+                os_info = platform.system()
+                os_version = platform.version()
+                left_align(f"OS: {os_version} ({os_info})")
+                left_align(f"CPU   Model: {cpu_info}")
+                left_align(f"CPU   Cores: {cpu_cores}")
+                left_align(f"CPU Threads: {cpu_threads}")
                 try:
-                    self.get_indicators()
-                    print("| CPT   (microseconds): ", format_string(self.get_time()*10**6) + " "*(box_width-len("| CPT   (microseconds): " + format_string(self.get_time()*10**6))) + "|")
-                    print("| CPT   (hour:min:sec): ", "%02d:%02d:%02d" % (hour, min, sec)+ " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| GD    (min):          ", format_string(self.calculated_indicators['gd'])+ " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| GDP   (min):          ", format_string(self.calculated_indicators['gdp'])+ " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| IGD   (min):          ", format_string(self.calculated_indicators['igd'])+ " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| IGDP  (min):          ", format_string(self.calculated_indicators['igdp'])+ " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| MS    (max):          ", format_string(self.calculated_indicators['ms']) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| SP    (max):          ", format_string(self.calculated_indicators['sp']) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| HV    (max):          ", format_string(self.calculated_indicators['hv']) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
+                    import GPUtil
+                    gpus = GPUtil.getGPUs()
+                    for gpu in gpus:
+                        left_align(f"GPU   Model: {gpu.name}")
+                        left_align(f"GPU    VRAM: {gpu.memoryTotal / 1024:.2f} GB")
                 except:
-                    print("| CPT   (microseconds): ", format_string(self.get_time()*10**6) + " "*(box_width-len("| CPT   (microseconds): " + format_string(self.get_time()*10**6))) + "|")
-                    print("| GD    (min):          ", format_string(self.calculated_indicators['gd']) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| GDP   (min):          ", format_string(self.calculated_indicators['gdp']) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| IGD   (min):          ", format_string(self.calculated_indicators['igd']) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| IGDP  (min):          ", format_string(self.calculated_indicators['igdp']) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| MS    (max):          ", format_string(self.calculated_indicators['ms']) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| SP    (max):          ", format_string(self.calculated_indicators['sp']) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
+                    pass
+                left_align(f"SYSTEM  RAM: {ram_total / (1024 ** 3):.2f} GB")
             except:
-                print("| CPT   (microseconds): ", format_string(self.get_time()*10**6) + " "*(box_width-len("| CPT   (microseconds): " + format_string(self.get_time()*10**6))) + "|")
-                print("| CPT   (hour:min:sec): ", "%02d:%02d:%02d" % (hour, min, sec) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-        else:
-            print("| CPT   (microseconds): ", format_string(self.get_time()*10**6) + " "*(box_width-len("| CPT   (microseconds): " + format_string(self.get_time()*10**6))) + "|")
-            print("| CPT   (hour:min:sec): ", "%02d:%02d:%02d" % (hour, min, sec) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")     
-        print("+" + "-"*box_width + "+")
-        print("|" + " " + "Decision Information".center(box_width-2) + " " + "|")
-        print("+" + "-"*box_width + "+")
+                pass
+            empty_line()
+            bline()
+
+        if model_info:
+            tline_text("Model")
+            empty_line()
+            left_align(f"Name: {self.model_name}")
+            list_three_column([
+                ("Feature:         ", "Class:", "Total:"),
+                ("Positive variable", self.pos_var_counter[0], self.pos_var_counter[1]),
+                ("Binary variable  ", self.bin_var_counter[0], self.bin_var_counter[1]),
+                ("Integer variable ", self.int_var_counter[0], self.int_var_counter[1]),
+                ("Free variable    ", self.free_var_counter[0], self.free_var_counter[1]), 
+                ("Event variable   ", self.event_var_counter[0], self.event_var_counter[1]),
+                ("Total variables  ", self.tot_counter[0], self.tot_counter[1]), 
+                ("Objective        ", "-", self.obj_counter[1]), 
+                ("Constraint       ", self.con_counter[0], self.con_counter[1]) ])
+            empty_line()
+            bline()
+
+        if sol_info:
+            tline_text("Solve")
+            empty_line()
+            two_column(f"Method: {self.solution_method}", "Objective value")
+            status_row_print(self.objectives_directions, status)
+            if obj_values:
+                if len(self.objectives_directions) != 1:
+                    try:
+                        solution_print(self.objectives_directions, status, self.get_obj(), self.get_payoff())
+                    except:
+                        left_align("Nothing found.")
+                else:
+                    solution_print(self.objectives_directions, status, self.get_obj())
+            empty_line()
+            bline()
+
+        if metric_info:
+            tline_text("Metric")
+            empty_line()
+            self.calculated_indicators = None
+            try:
+                self.get_indicators(ideal_pareto=ideal_pareto, ideal_point=ideal_point)
+            except:
+                pass
+            metrics_print(self.objectives_directions, all_metrics, self.get_obj(), self.calculated_indicators, length=self.get_time())
+            empty_line()
+            bline()
+
+        if dec_info:
+            tline_text("Decision")
+            empty_line()
+            self.decision_information_print(status)
+            empty_line()
+            bline()
+
+        if save is not None:
+            sys.stdout.close()
+            sys.stdout = stdout_origin
+    
+    def decision_information_print(self,status, box_width=80):
+
         for i,j in self.mainvars.keys():
-            if self.maindims[j] == 0:
-                if self.get(self.mainvars[(i,j)]) not in [0, None]:
-                    print(f"| {j} =", self.get(self.mainvars[(i,j)]), " "* (box_width-(len(f"| {j} =") + len(str(self.get(self.mainvars[(i,j)]))))-1) + "|")
-            elif len(self.maindims[j])==1:
-                try:
-                    for k in fix_dims(self.maindims[j])[0]:
-                        if self.get(self.mainvars[(i,j)][k]) not in [0, None]:
-                            print(f"| {j}[{k}] =", self.get(self.mainvars[(i,j)][k]), " "* (box_width-(len(f"| {j}[{k}] =") + len(str(self.get(self.mainvars[(i,j)][k])))) - 1) + "|")
-                except:
-                    for k in fix_dims(self.maindims[j])[0]:
-                        if self.get(self.mainvars[(i,j)])[k] not in [0, None]:
-                            print(f"| {j}[{k}] =", self.get(self.mainvars[(i,j)])[k], " "* (box_width-(len(f"| {j}[{k}] =") + len(str(self.get(self.mainvars[(i,j)])[k]))) - 1) + "|")
+
+            if i!='evar':
+
+                if self.maindims[j] == 0:
+
+                    if self.get(self.mainvars[(i,j)]) not in [0, None]:
+
+                        print(f"| {j} =", self.get(self.mainvars[(i,j)]), " "* (box_width-(len(f"| {j} =") + len(str(self.get(self.mainvars[(i,j)]))))-1) + "|")
+
+                elif len(self.maindims[j])==1:
+                    try:
+                        for k in fix_dims(self.maindims[j])[0]:
+                            if self.get(self.mainvars[(i,j)][k]) not in [0, None]:
+                                print(f"| {j}[{k}] =", self.get(self.mainvars[(i,j)][k]), " "* (box_width-(len(f"| {j}[{k}] =") + len(str(self.get(self.mainvars[(i,j)][k])))) - 1) + "|")
+                    except:
+                        for k in fix_dims(self.maindims[j])[0]:
+                            if self.get(self.mainvars[(i,j)])[k] not in [0, None]:
+                                print(f"| {j}[{k}] =", self.get(self.mainvars[(i,j)])[k], " "* (box_width-(len(f"| {j}[{k}] =") + len(str(self.get(self.mainvars[(i,j)])[k]))) - 1) + "|")
+                else:
+                    try:
+                        for k in it.product(*tuple(fix_dims(self.maindims[j]))):
+                            if self.get(self.mainvars[(i,j)][k]) not in [0, None]:
+                                print(f"| {j}[{k}] =".replace("(", "").replace(")", ""), self.get(self.mainvars[(i,j)][k]), " "* (box_width-(len(f"| {j}[{k}] =".replace("(", "").replace(")", "")) + len(str(self.get(self.mainvars[(i,j)][k])))) - 1) + "|")
+                    except:
+                        for k in it.product(*tuple(fix_dims(self.maindims[j]))):
+                            if self.get(self.mainvars[(i,j)])[k] not in [0, None]:
+                                print(f"| {j}[{k}] =".replace("(", "").replace(")", ""), self.get(self.mainvars[(i,j)])[k], " "* (box_width-(len(f"| {j}[{k}] =".replace("(", "").replace(")", "")) + len(str(self.get(self.mainvars[(i,j)])[k]))) - 1) + "|")
+
             else:
-                try:
-                    for k in it.product(*tuple(fix_dims(self.maindims[j]))):
-                        if self.get(self.mainvars[(i,j)][k]) not in [0, None]:
-                            print(f"| {j}[{k}] =".replace("(", "").replace(")", ""), self.get(self.mainvars[(i,j)][k]), " "* (box_width-(len(f"| {j}[{k}] =".replace("(", "").replace(")", "")) + len(str(self.get(self.mainvars[(i,j)][k])))) - 1) + "|")
-                except:
-                    for k in it.product(*tuple(fix_dims(self.maindims[j]))):
-                        if self.get(self.mainvars[(i,j)])[k] not in [0, None]:
-                            print(f"| {j}[{k}] =".replace("(", "").replace(")", ""), self.get(self.mainvars[(i,j)])[k], " "* (box_width-(len(f"| {j}[{k}] =".replace("(", "").replace(")", "")) + len(str(self.get(self.mainvars[(i,j)])[k]))) - 1) + "|")
 
-        print("+" + "-"*box_width + "+")
+                if self.maindims[j] == 0:
+                        if self.get_start(self.mainvars[(i,j)])!=None:
+                            print(f"| {j} =", [self.get_start(self.mainvars[(i,j)]), self.get_end(self.mainvars[(i,j)])], " "* (box_width-(len(f"| {j} =") + len(str([self.get_start(self.mainvars[(i,j)]), self.get_end(self.mainvars[(i,j)])])))-1) + "|")
+
+
+                elif len(self.maindims[j])==1:                    
+                    for k in fix_dims(self.maindims[j])[0]:
+                        if self.get_start(self.mainvars[(i,j)][k])!=None:
+                            print(f"| {j}[{k}] =", [self.get_start(self.mainvars[(i,j)][k]), self.get_end(self.mainvars[(i,j)][k])], " "* (box_width-(len(f"| {j} =") + len(str([self.get_start(self.mainvars[(i,j)][k]), self.get_end(self.mainvars[(i,j)][k])])))-1) + "|")
+
+                else:                    
+                    for k in it.product(*tuple(fix_dims(self.maindims[j]))):
+                        if self.get_start(self.mainvars[(i,j)][k])!=None:
+                            print(f"| {j}[{k}] =", [self.get_start(self.mainvars[(i,j)][k]), self.get_end(self.mainvars[(i,j)][k])], " "* (box_width-(len(f"| {j} =") + len(str([self.get_start(self.mainvars[(i,j)][k]), self.get_end(self.mainvars[(i,j)][k])])))-1) + "|")
+                    
 
     # Methods to work with input and output data.
 
     def max(self, *args):
 
         if self.features['interface_name'] == 'cplex_cp':
             return self.model.max(*args)
@@ -1842,14 +2589,20 @@
         Set Definition
         ~~~~~~~~~~~~~~
         To define a set.
         """
 
         return range(*size)
 
+    def ambiguity_set(self,*args,**kwds):
+        """
+        Ambiguity set defintion
+        """
+        return self.model.ambiguity(*args,**kwds)
+
     def card(self, set):
         """
         Card Definition
         ~~~~~~~~~~~~~~~~
         To measure size of the set, etc.
         """
 
@@ -1865,14 +2618,40 @@
         dim = fix_dims(parameter_dim)
 
         if dim == 0:
             return self.random.uniform(low=lb, high=ub)
         else:
             return self.random.uniform(low=lb, high=ub, size=([len(i) for i in dim]))
 
+    def uniformlist(self, lb_sample_size, ub_sample_size, candidate_set, parameter_dim=0, fixed_sample_size=None, replace=False, sorted=True):
+
+        dim = fix_dims(parameter_dim)
+
+        if dim==0:
+            if fixed_sample_size==None:
+
+                if sorted:
+
+                    return np.sort(self.random.choice(candidate_set, self.random.integers(lb_sample_size, ub_sample_size), replace=replace))
+                
+                else:
+
+                    return self.random.choice(candidate_set, self.random.integers(lb_sample_size, ub_sample_size), replace=replace)
+        else:
+            if fixed_sample_size==None:
+
+                if sorted:
+
+                    return [np.sort(self.random.choice(candidate_set, self.random.integers(lb_sample_size, ub_sample_size), replace=replace)) for i in dim[0]]
+                
+                else:
+
+                    return [self.random.choice(candidate_set, self.random.integers(lb_sample_size, ub_sample_size), replace=replace) for i in dim[0]]
+
+
     def uniformint(self, lb, ub, parameter_dim=0):
         """
         Uniform Integer Parameter Definition
         ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         To generate an integer parameter using uniform distribution inside a range.
         """
 
@@ -2093,45 +2872,100 @@
         else:
 
             return input1 % input2
 
     def square(self, input):
 
         if self.features['interface_name'] == 'cplex_cp':
-
             return self.model.square(input)
-
+        
+        elif self.features['interface_name'] in ['rsome_ro', 'rsome_dro']:
+            from rsome import square
+            return square(input)
+        
         else:
-
             return input * input
 
+    def quad(self,expr_or_1D_array_of_variables, positive_or_negative_semidefinite_matrix):
+
+        if self.features['interface_name'] in ['rsome_ro', 'rsome_dro']:
+            from rsome import quad
+            return quad(expr_or_1D_array_of_variables,positive_or_negative_semidefinite_matrix)
+
+    def expcone(self,rhs,a,b):
+        """
+        Returns an exponential cone constraint in the form: b*exp(a/b) <= rhs.
+
+        Args
+        rhs : array of variables or affine expression
+        a : Scalar.
+        b : Scalar.
+        """
+
+        if self.features['interface_name'] in ['rsome_ro', 'rsome_dro']:
+            from rsome import expcone
+            return expcone(rhs,a,b)
+
     def power(self, input1, input2):
 
         if self.features['interface_name'] == 'cplex_cp':
 
             return self.model.power(input1, input2)
 
         else:
 
             return input1 ** input2
 
+
+    def kldive(self, input, emprical_rpob, ambiguity_constant):
+
+        """
+        Returns KL divergence
+        
+        input: an 1D array of variables, an affine expression, or probabilities. 
+        emprical_rpob: an 1D array of emprical probabilities.
+        ambiguity_constant: Ambiguity constant.
+        """
+
+        if self.features['interface_name'] in ['rsome_ro', 'rsome_dro']:
+            from rsome import kldiv
+            return kldiv(input, emprical_rpob, ambiguity_constant)
+
+    def entropy(self, input):
+
+        """
+        Returns an entropy expression like sum(input*log(input))
+        """
+
+        if self.features['interface_name'] in ['rsome_ro', 'rsome_dro']:
+
+            from rsome import entropy
+            return entropy(input)
+    
+
+
     def log(self, input):
         """
 
         Natural Logarithm
 
         """
 
         if self.features['interface_name'] in ['cplex_cp']:
 
             return self.model.log(input)
 
         elif self.features['interface_name'] in ['gekko']:
 
             return self.model.log(input)
+        
+        elif self.features['interface_name'] in ['rsome_ro', 'rsome_dro']:
+
+            from rsome import log
+            return log(input)
 
         else:
 
             return np.log(input)
 
     def log10(self, input):
         """
@@ -2211,15 +3045,20 @@
             return self.model.sigmoid(input)
 
     def exponent(self, input):
 
         if self.features['interface_name'] in ['cplex_cp', 'gekko']:
 
             return self.model.exp(input)
+        
+        elif self.features['interface_name'] in ['rsome_ro', 'rsome_dro']:
 
+            from rsome import exp
+            return exp(input)
+    
         else:
 
             return np.exp(input)
 
     def count(self, input, value):
 
         if self.features['interface_name'] == 'cplex_cp':
@@ -2279,200 +3118,251 @@
         else:
 
             return np.round(x)
 
     # Methods to visualize data.
 
     def show_gantt(interval_variables, names, colors='lightblue'):
-
+        """
+        This function visualizes a Gantt chart of interval variables using the IBM DOcplex library.
+        
+        Parameters:
+        interval_variables: A list of interval variables. Each interval variable represents a task.
+        names: A list of strings. Each string is a name corresponding to an interval variable.
+        colors: Either a list of colors (one for each interval variable) or a single color string. 
+                If a single color string is provided, it will be used for all interval variables. 
+                If a list of colors is provided, it should have the same length as interval_variables and names.
+        
+        Returns:
+        None. A Gantt chart is displayed as output.
+        """
+        
         import docplex.cp.utils_visu as visu
         import matplotlib.pyplot as plt
 
-        counter = 0
-        for i in interval_variables:
-            visu.interval(i, colors[counter], names[counter])
-            counter += 1
+        if isinstance(colors, str):
+            colors = [colors] * len(interval_variables)
+        elif len(colors) != len(interval_variables):
+            raise ValueError("Length of colors list must match length of interval_variables list")
+
+        if len(interval_variables) != len(names):
+            raise ValueError("Length of interval_variables list must match length of names list")
+
+        for i, interval in enumerate(interval_variables):
+            visu.interval(interval, colors[i], names[i])
+            
         visu.show()
 
 # Alternatives for defining this class:
 
-
-model = mdl = add_model = create_environment = env = feloopy = representor_model = learner_model = target_model = optimizer = Model
+model = mdl = add_model = deterministic_model = certain_model = create_environment = env = feloopy = representor_model = learner_model = target_model = uncertain_target_model = uncertain_learner_model = uncertain_representor_model = optimizer = uncertain_model = stochastic_model = robust_model = possibilistic_model = Model
 
 warnings.simplefilter(action='ignore', category=FutureWarning)
 
-
 class Implement:
 
     def __init__(self, ModelFunction):
         '''
         Creates and returns an implementor for the representor model.
         '''
 
-        self.ModelInfo = ModelFunction(['idle'])
+        self.model_data = ModelFunction(['idle'])
         self.ModelFunction = ModelFunction
-        self.InterfaceName = self.ModelInfo.features['interface_name']
-        self.SolutionMethod = self.ModelInfo.features['solution_method']
-        self.ModelName = self.ModelInfo.features['model_name']
-        self.SolverName = self.ModelInfo.features['solver_name']
-        self.ModelConstraints = self.ModelInfo.features['constraints']
-        self.ModelObjectives = self.ModelInfo.features['objectives']
-        self.ObjectivesDirections = self.ModelInfo.features['directions']
-        self.PositiveVariableCounter = self.ModelInfo.features['positive_variable_counter']
-        self.BinaryVariableCounter = self.ModelInfo.features['binary_variable_counter']
-        self.IntegerVariableCounter = self.ModelInfo.features['integer_variable_counter']
-        self.FreeVariableCounter = self.ModelInfo.features['free_variable_counter']
-        self.ToTalVariableCounter = self.ModelInfo.features['total_variable_counter']
-        self.ConstraintsCounter = self.ModelInfo.features['constraint_counter']
-        self.ObjectivesCounter = self.ModelInfo.features['objective_counter']
-        self.AlgOptions = self.ModelInfo.features['solver_options']
-        self.VariablesSpread = self.ModelInfo.features['variable_spread']
-        self.VariablesType = self.ModelInfo.features['variable_type']
-        self.ObjectiveBeingOptimized = self.ModelInfo.features['objective_being_optimized']
-        self.VariablesBound = self.ModelInfo.features['variable_bound']
-        self.VariablesDim = self.ModelInfo.features['variable_dim']
+        self.interface_name = self.model_data.features['interface_name']
+        self.solution_method = self.model_data.features['solution_method']
+        self.model_name = self.model_data.features['model_name']
+        self.solver_name = self.model_data.features['solver_name']
+        self.model_constraints = self.model_data.features['constraints']
+        self.model_objectives = self.model_data.features['objectives']
+        self.objectives_directions = self.model_data.features['directions']
+        self.pos_var_counter = self.model_data.features['positive_variable_counter']
+        self.bin_var_counter = self.model_data.features['binary_variable_counter']
+        self.int_var_counter = self.model_data.features['integer_variable_counter']
+        self.free_var_counter = self.model_data.features['free_variable_counter']
+        self.tot_counter = self.model_data.features['total_variable_counter']
+        self.con_counter = self.model_data.features['constraint_counter']
+        self.obj_counter = self.model_data.features['objective_counter']
+        self.AlgOptions = self.model_data.features['solver_options']
+        self.VariablesSpread = self.model_data.features['variable_spread']
+        self.VariablesType = self.model_data.features['variable_type']
+        self.ObjectiveBeingOptimized = self.model_data.features['objective_being_optimized']
+        self.VariablesBound = self.model_data.features['variable_bound']
+        self.VariablesDim = self.model_data.features['variable_dim']
         self.status = 'Not solved'
         self.response = None
         self.AgentProperties = [None, None, None, None]
         self.get_objective = self.get_obj
         self.get_var = self.get_variable = self.get
         self.search = self.solve = self.optimize = self.run = self.sol
 
-        match self.InterfaceName:
+        match self.interface_name:
 
             case 'mealpy':
 
                 from .generators.model import mealpy_model_generator
                 self.ModelObject = mealpy_model_generator.generate_model(
-                    self.SolverName, self.AlgOptions)
+                    self.solver_name, self.AlgOptions)
 
             case 'pymultiobjective':
 
                 self.ModelObject = None
 
+            case 'pymoo':
+
+                self.ModelObject = None
+
             case 'feloopy':
 
                 from .generators.model import feloopy_model_generator
                 self.ModelObject = feloopy_model_generator.generate_model(
-                    self.ToTalVariableCounter[1], self.ObjectivesDirections, self.SolverName, self.AlgOptions)
+                    self.tot_counter[1], self.objectives_directions, self.solver_name, self.AlgOptions)
 
     def remove_infeasible_solutions(self):
 
         self.BestAgent = np.delete(self.BestAgent, self.remove, axis=0)
         self.BestReward = np.delete(self.BestReward, self.remove, axis=0)
 
-    def sol(self, penalty_coefficient=0, number_of_times=1, show_plots=False, save_plots=False):
+    def sol(self, penalty_coefficient=0, number_of_times=1, show_plots=False, save_plots=False, show_log=False):
 
         self.penalty_coefficient = penalty_coefficient
 
-        match self.InterfaceName:
+        match self.interface_name:
 
             case 'mealpy':
 
                 from .generators.solution import mealpy_solution_generator
                 self.BestAgent, self.BestReward, self.start, self.end = mealpy_solution_generator.generate_solution(
-                    self.ModelObject, self.Fitness, self.ToTalVariableCounter, self.ObjectivesDirections, self.ObjectiveBeingOptimized, number_of_times, show_plots, save_plots)
+                    self.ModelObject, self.Fitness, self.tot_counter, self.objectives_directions, self.ObjectiveBeingOptimized, number_of_times, show_plots, save_plots,show_log)
 
             case 'pymultiobjective':
 
                 from .generators.solution import pymultiobjective_solution_generator
                 self.BestAgent, self.BestReward, self.start, self.end = pymultiobjective_solution_generator.generate_solution(
-                    self.SolverName, self.AlgOptions, self.Fitness, self.ToTalVariableCounter, self.ObjectivesDirections, self.ObjectiveBeingOptimized, number_of_times, show_plots, save_plots)
+                    self.solver_name, self.AlgOptions, self.Fitness, self.tot_counter, self.objectives_directions, self.ObjectiveBeingOptimized, number_of_times, show_plots, save_plots,show_log)
                 self.remove = []
+
                 for i in range(np.shape(self.BestReward)[0]):
 
                     if 'infeasible' in self.Check_Fitness(self.BestAgent[i]):
 
                         self.remove.append(i)
 
                 if len(self.remove) != 0:
                     self.remove_infeasible_solutions()
 
+            case 'pymoo':
+
+                from .generators.solution import pymoo_solution_generator
+                self.BestAgent, self.BestReward,self.start, self.end = pymoo_solution_generator.generate_solution(self.solver_name, self.AlgOptions, self.Fitness, self.tot_counter, self.objectives_directions, self.ObjectiveBeingOptimized, number_of_times, show_plots, save_plots, show_log)
+                self.remove = []
+
+                for i in range(np.shape(self.BestReward)[0]):
+
+                    if 'infeasible' in self.Check_Fitness(np.array([self.BestAgent[i]])):
+
+                        self.remove.append(i)
+
+                if len(self.remove) != 0:
+                    self.remove_infeasible_solutions()
+            
             case 'feloopy':
 
                 from .generators.solution import feloopy_solution_generator
                 self.BestAgent, self.BestReward, self.start, self.end, self.status = feloopy_solution_generator.generate_solution(
-                    self.ModelObject, self.Fitness, self.ToTalVariableCounter, self.ObjectivesDirections, self.ObjectiveBeingOptimized, number_of_times, show_plots)
+                    self.ModelObject, self.Fitness, self.tot_counter, self.objectives_directions, self.ObjectiveBeingOptimized, number_of_times, show_plots, show_log)
 
     def dis_plots(self, ideal_pareto: Optional[np.ndarray] = [], step: Optional[tuple] = (0.1,)):
 
         """
         Calculates selected Pareto front metrics and displays the results in a tabulated format.
 
         :param ideal_pareto: An array of shape (n_samples, n_objectives) containing the ideal Pareto front. Default is None.
         """
 
         obtained_pareto = self.BestReward
 
         from pyMultiobjective.util import graphs
-        ObjectivesDirections = [-1 if direction =='max' else 1 for direction in self.ObjectivesDirections]
+        ObjectivesDirections = [-1 if direction =='max' else 1 for direction in self.objectives_directions]
         def f1(X): return ObjectivesDirections[0]*self.Fitness(np.array(X))[0]
         def f2(X): return ObjectivesDirections[1]*self.Fitness(np.array(X))[1]
         def f3(X): return ObjectivesDirections[2]*self.Fitness(np.array(X))[2]
         def f4(X): return ObjectivesDirections[3]*self.Fitness(np.array(X))[3]
         def f5(X): return ObjectivesDirections[4]*self.Fitness(np.array(X))[4]
         def f6(X): return ObjectivesDirections[5]*self.Fitness(np.array(X))[5]
         my_list_of_functions = [f1, f2, f3, f4, f5, f6]
         parameters = dict()
         list_of_functions = []
         for i in range(len(ObjectivesDirections)): list_of_functions.append(my_list_of_functions[i])
         
         solution = np.concatenate((self.BestAgent, self.BestReward*ObjectivesDirections), axis=1)
     
         parameters = {
-        'min_values': (0,)*self.ToTalVariableCounter[1],
-        'max_values': (1,)*self.ToTalVariableCounter[1],
-        'step': step*self.ToTalVariableCounter[1],
+        'min_values': (0,)*self.tot_counter[1],
+        'max_values': (1,)*self.tot_counter[1],
+        'step': step*self.tot_counter[1],
         'solution': solution, 
         'show_pf': True,
         'show_pts': True,
         'show_sol': True,
         'pf_min': True, 
         'custom_pf': ideal_pareto*ObjectivesDirections if type(ideal_pareto) == np.ndarray else [],
         'view': 'browser'
         }
         graphs.plot_mooa_function(list_of_functions = list_of_functions, **parameters)
 
         parameters = {
-            'min_values': (0,)*self.ToTalVariableCounter[1],
-            'max_values': (1,)*self.ToTalVariableCounter[1],
-            'step': step*self.ToTalVariableCounter[1],
+            'min_values': (0,)*self.tot_counter[1],
+            'max_values': (1,)*self.tot_counter[1],
+            'step': step*self.tot_counter[1],
             'solution': solution, 
             'show_pf': True,
             'pf_min': True,  
             'custom_pf': ideal_pareto*ObjectivesDirections if type(ideal_pareto) == np.ndarray else [],
             'view': 'browser'
         }
         graphs.parallel_plot(list_of_functions = list_of_functions, **parameters)
 
     def dis_status(self):
         print('status:', self.get_status())
 
     def get_status(self):
 
-        if self.InterfaceName in ['mealpy', 'pymultiobjective']:
+        if len(self.objectives_directions)==1:
 
-            if self.InterfaceName == 'mealpy':
+            if self.interface_name == 'mealpy':
 
                 return self.Check_Fitness(self.BestAgent)
+        
+            else:
+
+                if self.status[0] == 1:
+                    return 'feasible (constrained)'
+                elif self.status[0] == 2:
+                    return 'feasible (unconstrained)'
+                elif self.status[0] == -1:
+                    return 'infeasible'
+
+        else:
+
+            status = []
+            
+            if self.interface_name in ['feloopy', 'pymoo']:
+
+                for i in range(np.shape(self.BestReward)[0]):
+                    status.append(self.Check_Fitness(np.array([self.BestAgent[i]])))
 
             else:
-                status = []
+
                 for i in range(np.shape(self.BestReward)[0]):
                     status.append(self.Check_Fitness(self.BestAgent[i]))
+            
 
-                return status
+            return status
 
-        else:
-            if self.status[0] == 1:
-                return 'feasible (constrained)'
-            elif self.status[0] == 2:
-                return 'feasible (unconstrained)'
-            elif self.status[0] == -1:
-                return 'infeasible'
+        
 
     def Check_Fitness(self, X):
 
         self.AgentProperties[0] = 'feasibility_check'
         self.AgentProperties[1] = X
         self.AgentProperties[2] = self.VariablesSpread
         self.AgentProperties[3] = self.penalty_coefficient
@@ -2576,29 +3466,29 @@
                 max_episode_obj.append(
                     np.max(m[episode]['epoch_solutions'][epoch][:, -1]))
             std_epoch_obj.append(np.std(max_episode_obj))
         std_epoch_obj = np.array(std_epoch_obj)
 
         axs = fig.add_subplot(1, 5, 4)
         x = np.arange(no_epochs)
-        if self.ObjectivesDirections[self.ObjectiveBeingOptimized] == 'max':
+        if self.objectives_directions[self.ObjectiveBeingOptimized] == 'max':
             axs.plot(x, max_epoch_obj, 'green', alpha=0.4)
             axs.plot(x, ave_epoch_obj, 'green', alpha=0.8)
             axs.plot(x, min_epoch_obj, 'green', alpha=0.4)
             axs.fill_between(x, ave_epoch_obj - std_epoch_obj,
                              ave_epoch_obj + std_epoch_obj, color='green', alpha=0.3)
         else:
             axs.plot(x, max_epoch_obj, 'red', alpha=0.4)
             axs.plot(x, ave_epoch_obj, 'red', alpha=0.8)
             axs.plot(x, min_epoch_obj, 'red', alpha=0.4)
 
             axs.fill_between(x, ave_epoch_obj - std_epoch_obj,
                              ave_epoch_obj + std_epoch_obj, color='red', alpha=0.3)
         axs.set_xlabel('Epoch')
-        if self.ObjectivesDirections[self.ObjectiveBeingOptimized] == 'max':
+        if self.objectives_directions[self.ObjectiveBeingOptimized] == 'max':
             axs.set_ylabel('Maximum reward')
         else:
             axs.set_ylabel('Maximum loss')
         axs.set_xlim(-0.5, no_epochs-1+0.5)
 
         max_epoch_obj = []
         for epoch in range(0, no_epochs):
@@ -2640,15 +3530,15 @@
         x = np.arange(no_epochs)
         axs.plot(x, max_epoch_obj, 'orange', alpha=0.4)
         axs.plot(x, ave_epoch_obj, 'orange', alpha=0.8)
         axs.plot(x, min_epoch_obj, 'orange', alpha=0.4)
         axs.fill_between(x, ave_epoch_obj - std_epoch_obj,
                          ave_epoch_obj + std_epoch_obj, color='orange', alpha=0.3)
         axs.set_xlabel('Epoch')
-        if self.ObjectivesDirections[self.ObjectiveBeingOptimized] == 'max':
+        if self.objectives_directions[self.ObjectiveBeingOptimized] == 'max':
             axs.set_ylabel('Average reward')
         else:
             axs.set_ylabel('Average loss')
         axs.set_xlim(-0.5, no_epochs-1+0.5)
 
         max_epoch_obj = []
         for epoch in range(0, no_epochs):
@@ -2684,39 +3574,39 @@
                 max_episode_obj.append(
                     np.min(m[episode]['epoch_solutions'][epoch][:, -1]))
             std_epoch_obj.append(np.std(max_episode_obj))
         std_epoch_obj = np.array(std_epoch_obj)
 
         axs = fig.add_subplot(1, 5, 2)
         x = np.arange(no_epochs)
-        if self.ObjectivesDirections[self.ObjectiveBeingOptimized] == 'max':
+        if self.objectives_directions[self.ObjectiveBeingOptimized] == 'max':
             axs.plot(x, max_epoch_obj, 'red', alpha=0.4)
             axs.plot(x, ave_epoch_obj, 'red', alpha=0.8)
             axs.plot(x, min_epoch_obj, 'red', alpha=0.4)
             axs.fill_between(x, ave_epoch_obj - std_epoch_obj,
                              ave_epoch_obj + std_epoch_obj, color='red', alpha=0.3)
         else:
             axs.plot(x, max_epoch_obj, 'green', alpha=0.4)
             axs.plot(x, ave_epoch_obj, 'green', alpha=0.8)
             axs.plot(x, min_epoch_obj, 'green', alpha=0.4)
             axs.fill_between(x, ave_epoch_obj - std_epoch_obj,
                              ave_epoch_obj + std_epoch_obj, color='green', alpha=0.3)
         axs.set_xlabel('Epoch')
         axs.set_xlim(-0.5, no_epochs-1+0.5)
-        if self.ObjectivesDirections[self.ObjectiveBeingOptimized] == 'max':
+        if self.objectives_directions[self.ObjectiveBeingOptimized] == 'max':
             axs.set_ylabel('Minimum reward')
         else:
             axs.set_ylabel('Minimum loss')
 
-        if self.ObjectivesDirections[self.ObjectiveBeingOptimized] == 'min':
+        if self.objectives_directions[self.ObjectiveBeingOptimized] == 'min':
             best_min_min = np.inf
             best_min_min_t = []
             best_sol_t = []
             best_per_episode = []
-            no_features = self.ToTalVariableCounter[1]
+            no_features = self.tot_counter[1]
             for epoch in range(0, no_epochs):
                 best_min = []
                 best_sol = []
                 for episode in range(0, no_episodes):
                     best_min.append(
                         np.min(m[episode]['epoch_solutions'][epoch][:, -1]))
                     best_sol.append(m[episode]['epoch_solutions'][epoch][np.argmin(
@@ -2745,15 +3635,15 @@
 
             best_min_min_t = np.array(best_min_min_t)
         else:
             best_min_min = -np.inf
             best_min_min_t = []
             best_sol_t = []
             best_per_episode = []
-            no_features = self.ToTalVariableCounter[1]
+            no_features = self.tot_counter[1]
             for epoch in range(0, no_epochs):
                 best_min = []
                 best_sol = []
                 for episode in range(0, no_episodes):
                     best_min.append(
                         np.max(m[episode]['epoch_solutions'][epoch][:, -1]))
                     best_sol.append(m[episode]['epoch_solutions'][epoch][np.argmax(
@@ -2864,15 +3754,15 @@
         from math import isclose
 
         opt = np.array([opt])
         prob_per_epoch = []
 
         findbest = np.zeros(shape=(no_episodes, no_epochs))
 
-        if self.ObjectivesDirections[self.ObjectiveBeingOptimized] == 'min':
+        if self.objectives_directions[self.ObjectiveBeingOptimized] == 'min':
             for episode in range(0, no_episodes):
                 episode_tracker = []
                 best = np.inf
                 for epoch in range(0, no_epochs):
                     if np.min(m[episode]['epoch_solutions'][epoch][:, -1]) <= best:
                         best = np.min(
                             m[episode]['epoch_solutions'][epoch][:, -1])
@@ -2911,16 +3801,16 @@
 
         prob_per_epoch = [sum(findbest[episode, epoch] for episode in range(
             0, no_episodes))/no_episodes for epoch in range(0, no_epochs)]
 
         return [obj, time, accuracy, prob_per_epoch]
 
     def get(self, *args):
-        if self.ObjectivesCounter[0] == 1:
-            match self.InterfaceName:
+        if self.obj_counter[0] == 1:
+            match self.interface_name:
                 case 'mealpy':
                     for i in args:
                         if len(i) >= 2:
                             match self.VariablesType[i[0]]:
                                 case 'pvar':
                                     if self.VariablesDim[i[0]] == 0:
                                         return (self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))[0]
@@ -2946,18 +3836,18 @@
                                         def var(*args):
                                             self.NewAgentProperties = np.round(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (
                                                 self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
                                             return self.NewAgentProperties[sum(args[k]*mt.prod(len(self.VariablesDim[i[0]][j]) for j in range(k+1, len(self.VariablesDim[i[0]]))) for k in range(len(self.VariablesDim[i[0]])))]
                                         return var(*i[1])
                                 case 'ivar':
                                     if self.VariablesDim[i[0]] == 0:
-                                        return np.floor(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))[0]
+                                        return np.round(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))[0]
                                     else:
                                         def var(*args):
-                                            self.NewAgentProperties = np.floor(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (
+                                            self.NewAgentProperties = np.round(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (
                                                 self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
                                             return self.NewAgentProperties[sum(args[k]*mt.prod(len(self.VariablesDim[i[0]][j]) for j in range(k+1, len(self.VariablesDim[i[0]]))) for k in range(len(self.VariablesDim[i[0]])))]
                                         return var(*i[1])
                                 case 'svar':
                                     return np.argsort(self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]])[i[1]]
 
                         else:
@@ -2965,15 +3855,15 @@
                                 case 'pvar':
                                     return (self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))[0]
                                 case 'fvar':
                                     return (self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))[0]
                                 case 'bvar':
                                     return np.round(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))[0]
                                 case 'ivar':
-                                    return np.floor(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))[0]
+                                    return np.round(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))[0]
                                 case 'svar':
                                     return np.argsort(self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]])
                 case 'feloopy':
                     for i in args:
                         if len(i) >= 2:
                             match self.VariablesType[i[0]]:
                                 case 'pvar':
@@ -2996,30 +3886,30 @@
                                                 self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
                                             return self.NewAgentProperties[sum(args[k]*mt.prod(len(self.VariablesDim[i[0]][j]) for j in range(k+1, len(self.VariablesDim[i[0]]))) for k in range(len(self.VariablesDim[i[0]])))]
 
                                         return var(*i[1])
 
                                 case 'bvar':
                                     if self.VariablesDim[i[0]] == 0:
-                                        return np.floor(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
+                                        return np.round(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
 
                                     else:
                                         def var(*args):
                                             self.NewAgentProperties = np.round(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (
                                                 self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
                                             return self.NewAgentProperties[sum(args[k]*mt.prod(len(self.VariablesDim[i[0]][j]) for j in range(k+1, len(self.VariablesDim[i[0]]))) for k in range(len(self.VariablesDim[i[0]])))]
 
                                         return var(*i[1])
                                 case 'ivar':
                                     if self.VariablesDim[i[0]] == 0:
-                                        return np.floor(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
+                                        return np.round(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
 
                                     else:
                                         def var(*args):
-                                            self.NewAgentProperties = np.floor(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (
+                                            self.NewAgentProperties = np.round(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (
                                                 self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
                                             return self.NewAgentProperties[sum(args[k]*mt.prod(len(self.VariablesDim[i[0]][j]) for j in range(k+1, len(self.VariablesDim[i[0]]))) for k in range(len(self.VariablesDim[i[0]])))]
                                         return var(*i[1])
 
                                 case 'svar':
                                     return np.argsort(self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]])[i[1]]
 
@@ -3029,15 +3919,15 @@
                                 case 'pvar':
                                     return (self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
                                 case 'fvar':
                                     return (self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
                                 case 'bvar':
                                     return np.round(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
                                 case 'ivar':
-                                    return np.floor(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
+                                    return np.round(self.VariablesBound[i[0]][0] + self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
                                 case 'svar':
                                     return np.argsort(self.BestAgent[self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]])
         else:
 
             for i in args:
                 if len(i) >= 2:
 
@@ -3119,138 +4009,88 @@
         :param n_clusters: An integer value for the number of clusters used in the knee point distance metric. Default is 5.
         :param save_path: A string value for the path where the results should be saved. Default is None.
         """
 
 
         self.get_indicators(ideal_pareto, ideal_point, step, epsilon, p, n_clusters, save_path, show_log = True)
 
-    def get_indicators(self, ideal_pareto: Optional[np.ndarray] = [], ideal_point: Optional[np.array] = [], step: Optional[tuple] = (0.1,), epsilon: float = 0.01, p: float = 2.0, n_clusters: int = 5, save_path: Optional[str] = None, show_log: Optional[bool] = False):
+    def get_indicators(self, ideal_pareto: Optional[np.ndarray] = [], ideal_point: Optional[np.array] = [], step: Optional[tuple] = (0.2,), epsilon: float = 0.01, p: float = 2.0, n_clusters: int = 5, save_path: Optional[str] = None, show_log: Optional[bool] = False, normalize_hv: Optional[bool] = False, bypass_limit=False):
 
         """
         Calculates selected Pareto front metrics and displays the results in a tabulated format.
 
         :param ideal_pareto: An array of shape (n_samples, n_objectives) containing the ideal Pareto front. Default is None.
         :param epsilon: A float value for the epsilon value used in the epsilon metric. Default is 0.01.
         :param p: A float value for the power parameter used in the weighted generational distance and weighted inverted generational distance metrics. Default is 2.0.
         :param n_clusters: An integer value for the number of clusters used in the knee point distance metric. Default is 5.
         :param save_path: A string value for the path where the results should be saved. Default is None.
         """
+        if len(self.get_obj())!=0:
 
-        obtained_pareto = self.BestReward
-
-        from pyMultiobjective.util import indicators
-        ObjectivesDirections = [-1 if direction =='max' else 1 for direction in self.ObjectivesDirections]
-        def f1(X): return ObjectivesDirections[0]*self.Fitness(np.array(X))[0]
-        def f2(X): return ObjectivesDirections[1]*self.Fitness(np.array(X))[1]
-        def f3(X): return ObjectivesDirections[2]*self.Fitness(np.array(X))[2]
-        def f4(X): return ObjectivesDirections[3]*self.Fitness(np.array(X))[3]
-        def f5(X): return ObjectivesDirections[4]*self.Fitness(np.array(X))[4]
-        def f6(X): return ObjectivesDirections[5]*self.Fitness(np.array(X))[5]
-        my_list_of_functions = [f1, f2, f3, f4, f5, f6]
-        parameters = dict()
-        list_of_functions = []
-        for i in range(len(ObjectivesDirections)): list_of_functions.append(my_list_of_functions[i])
-        
-        solution = np.concatenate((self.BestAgent, self.BestReward*ObjectivesDirections), axis=1)
-    
-        parameters = {
-            'min_values': (0,)*self.ToTalVariableCounter[1],
-            'max_values': (1,)*self.ToTalVariableCounter[1],
-            'step': step*self.ToTalVariableCounter[1],
-            'solution': solution,
-            'pf_min': True,
-            'custom_pf': ideal_pareto*ObjectivesDirections if type(ideal_pareto) == np.ndarray else []
-        }
+            obtained_pareto = self.BestReward
+            from pyMultiobjective.util import indicators
 
-        self.calculated_indicators = dict()
-        gd = indicators.gd_indicator(list_of_functions=list_of_functions, **parameters)
-        gdp = indicators.gd_plus_indicator(list_of_functions=list_of_functions, **parameters)
-        igd = indicators.igd_indicator(list_of_functions=list_of_functions, **parameters)
-        igdp = indicators.igd_plus_indicator(list_of_functions=list_of_functions, **parameters)
-        ms = indicators.ms_indicator(list_of_functions=list_of_functions, **parameters)
-        sp = indicators.sp_indicator(list_of_functions=list_of_functions, **parameters)
-
-        self.calculated_indicators['gd'] = gd
-        self.calculated_indicators['gdp'] = gdp
-        self.calculated_indicators['igd'] = igd
-        self.calculated_indicators['igdp'] = igdp
-        self.calculated_indicators['ms'] = ms
-        self.calculated_indicators['sp'] = sp
+            ObjectivesDirections = [-1 if direction =='max' else 1 for direction in self.objectives_directions]
 
-        parameters = {
-            'solution': solution,
-            'n_objs': len(ObjectivesDirections),
-            'ref_point': ideal_point,
-        }
-        
-        hypervolume = indicators.hv_indicator(**parameters)
-        self.calculated_indicators['hv'] = hypervolume
-        metrics = []
-
-        if type(ideal_pareto) == np.ndarray:
-            metrics = [
-                ('Additive Epsilon Indicator Metric (min) [0, +inf)',metric_pareto_aem(ideal_pareto, obtained_pareto)),
-                ('Convergence Metric (min) [0,+inf)', metric_pareto_cvm(obtained_pareto, ideal_pareto)),
-                ('Coverage Ratio Metric (max) [0,1]', metric_pareto_crm(ideal_pareto, obtained_pareto)),
-                ('Epsilon Metric (max) [0 or 1]', metric_pareto_epm(obtained_pareto, ideal_pareto, epsilon)),
-                ('F-Ratio Metric (max) [0,1]', metric_pareto_frm(obtained_pareto, ideal_pareto)),
-                ('Generational Distance Metric (min) [0,+inf)', self.calculated_indicators['gd']),
-                ('Hyper Volume Metric (max) [0, +inf)', self.calculated_indicators['hv']),
-                ('Inverted Generational Distance (min) [0, +inf)', self.calculated_indicators['igd']),
-                ('Knee Point Distance Metric (min) [0, +inf)', metric_pareto_kdm(obtained_pareto, ideal_pareto, n_clusters)),
-                ('Maximum Pareto Front Error Metric (min) [0, +inf)',metric_pareto_mem(ideal_pareto, obtained_pareto)),
-                ('Maximum Spread Metric (max) [0, +inf)', self.calculated_indicators['ms']),
-                ('Quantity Metric (max) [0,1]', metric_pareto_qvm(obtained_pareto, ideal_pareto)),
-                ('R2 Metric (max) [0,1]', metric_pareto_r2m(obtained_pareto, ideal_pareto)),
-                ('Spacing Metric (max) [0,+inf)', self.calculated_indicators['sp']),
-                ('Spread Metric (max) [0, +inf)', metric_pareto_rsm(obtained_pareto, ideal_pareto)),
-                ('Generational Distance Metric Plus (min) [0, +inf)', self.calculated_indicators['gdp']),
-                ('Weighted Inverted Generational Distance Plus (min) [0, +inf)', self.calculated_indicators['igdp'])]
-        else:
-
-            metrics = [
-                ('Generational Distance Metric (min) [0,+inf)', self.calculated_indicators['gd']),
-                ('Hyper Volume Metric (max) [0, +inf)', self.calculated_indicators['hv']),
-                ('Inverted Generational Distance (min) [0, +inf)', self.calculated_indicators['igd']),
-                ('Maximum Spread Metric (max) [0, +inf)', self.calculated_indicators['ms']),
-                ('Spacing Metric (max) [0,+inf)', self.calculated_indicators['sp']),
-                ('Generational Distance Metric Plus (min) [0, +inf)', self.calculated_indicators['gdp']),
-                ('Inverted Generational Distance Plus (min) [0, +inf)', self.calculated_indicators['igdp'])]
-
-        headers = ['Metric', 'Value']
-        results = [[metric[0], metric[1]] for metric in metrics]
-        table = tb(results, headers=headers)
-
-        if show_log:
-            print(table)
-
-            mean_values = np.mean(self.BestReward, axis=0)
-            std_values = np.std(self.BestReward, axis=0)
-            min_values = np.min(self.BestReward, axis=0)
-            max_values = np.max(self.BestReward, axis=0)
-
-            table_data = [['Objective']+['Mean', 'Standard Deviation', 'Min', 'Max']]
-            for i in range(len(ObjectivesDirections)):
-                table_data.append([f'Objective {i+1}', mean_values[i], std_values[i], min_values[i], max_values[i]])
-            print()
-            print(tabulate(table_data, headers='firstrow'))
-
-        if save_path is not None:
-            with open(save_path, 'w') as f:
-                f.write(table)
+            def f1(X): return ObjectivesDirections[0]*self.Fitness(np.array(X))[0]
+            def f2(X): return ObjectivesDirections[1]*self.Fitness(np.array(X))[1]
+            def f3(X): return ObjectivesDirections[2]*self.Fitness(np.array(X))[2]
+            def f4(X): return ObjectivesDirections[3]*self.Fitness(np.array(X))[3]
+            def f5(X): return ObjectivesDirections[4]*self.Fitness(np.array(X))[4]
+            def f6(X): return ObjectivesDirections[5]*self.Fitness(np.array(X))[5]
+
+            list_of_functions = [f1, f2, f3, f4, f5, f6]
+
+            solution = np.concatenate((self.BestAgent, self.BestReward*ObjectivesDirections), axis=1)
+            self.calculated_indicators = dict()
+
+            #Does not require the ideal_pareto
+            parameters = {
+                'solution': solution,
+                'n_objs': len(ObjectivesDirections),
+                'ref_point': ideal_point,
+                'normalize': normalize_hv
+            }
+            hypervolume = indicators.hv_indicator(**parameters)
+            self.calculated_indicators['hv'] = hypervolume
+
+            parameters = {
+                'min_values': (0,)*self.tot_counter[1],
+                'max_values': (1,)*self.tot_counter[1],
+                'step': step*self.tot_counter[1],
+                'solution': solution,
+                'pf_min': True,
+                'custom_pf': ideal_pareto*ObjectivesDirections if type(ideal_pareto) == np.ndarray else []
+            }
+
+            sp = indicators.sp_indicator(list_of_functions=list_of_functions, **parameters)
+            self.calculated_indicators['sp'] = sp
+
+            #Computationally efficient only if ideal_pareto exists
+            if self.tot_counter[1]<=3 or ideal_pareto != [] or bypass_limit:
+                gd = indicators.gd_indicator(list_of_functions=list_of_functions, **parameters)
+                gdp = indicators.gd_plus_indicator(list_of_functions=list_of_functions, **parameters)
+                igd = indicators.igd_indicator(list_of_functions=list_of_functions, **parameters)
+                igdp = indicators.igd_plus_indicator(list_of_functions=list_of_functions, **parameters)
+                ms = indicators.ms_indicator(list_of_functions=list_of_functions, **parameters)
+                self.calculated_indicators['gd'] = gd
+                self.calculated_indicators['gdp'] = gdp
+                self.calculated_indicators['igd'] = igd
+                self.calculated_indicators['igdp'] = igdp
+                self.calculated_indicators['ms'] = ms
 
-        return metrics
+            return self.calculated_indicators
 
     def dis_time(self):
 
         hour = round(((self.end-self.start)), 3) % (24 * 3600) // 3600
         min = round(((self.end-self.start)), 3) % (24 * 3600) % 3600 // 60
         sec = round(((self.end-self.start)), 3) % (24 * 3600) % 3600 % 60
 
-        print(f"cpu time [{self.InterfaceName}]: ", (self.end-self.start)*10 **
+        print(f"cpu time [{self.interface_name}]: ", (self.end-self.start)*10 **
               6, '(microseconds)', "%02d:%02d:%02d" % (hour, min, sec), '(h, m, s)')
 
         
     def get_time(self):
         """
 
         Used to get solution time in seconds.
@@ -3269,188 +4109,262 @@
         else:
             print(str(input[0])+': ', self.get(input))
 
     def dis_obj(self):
 
         print('objective: ', self.BestReward)
 
-    def inf(self):
 
-        print()
-        print("~~~~~~~~~~~~\nPROBLEM INFO\n~~~~~~~~~~~~")
+    def get_bound(self, *args):
+
+        for i in args:
+
+            if len(i) >= 2:
+            
+                match self.VariablesType[i[0]]:
+
+                    case 'pvar':
 
-        A = tb(
-            {
-                "info": ["model", "interface", "solver", "direction", "method"],
-                "detail": [self.ModelName, self.InterfaceName, self.SolverName, self.ObjectivesDirections, self.SolutionMethod],
-                "variable": ["positive", "binary", "integer", "free", "tot"],
-                "count [cat,tot]": [str(self.PositiveVariableCounter), str(self.BinaryVariableCounter), str(self.IntegerVariableCounter), str(self.FreeVariableCounter), str(self.ToTalVariableCounter)],
-                "other": ["objective", "constraint"],
-                "count [cat,tot] ": [str(self.ObjectivesCounter), str(self.ConstraintsCounter)]
-            },
-            headers="keys", tablefmt="github"
-        )
-        print(A)
-        print("~~~~~~~~~~~~\n")
+                        if self.VariablesDim[i[0]] == 0:
+                            UB = np.max((self.VariablesBound[i[0]][0] + self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0])))
+                            LB = np.min((self.VariablesBound[i[0]][0] + self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0])))
+                            return [LB,UB]
 
-        return A
+                        else:
+                            def var(*args):
+                                self.NewAgentProperties = (self.VariablesBound[i[0]][0] + self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (
+                                    self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
+                                return self.NewAgentProperties[:,sum(args[k]*mt.prod(len(self.VariablesDim[i[0]][j]) for j in range(k+1, len(self.VariablesDim[i[0]]))) for k in range(len(self.VariablesDim[i[0]])))]
+                            return [np.min(var(*i[1])),np.max(var(*i[1]))]
+
+                    case 'fvar':
+
+                        if self.VariablesDim[i[0]] == 0:
+                            LB = np.min(self.VariablesBound[i[0]][0] + self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
+                            UB = np.max(self.VariablesBound[i[0]][0] + self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
+                            return [LB,UB]
+
+                        else:
+                            def var(*args):
+                                self.NewAgentProperties = (self.VariablesBound[i[0]][0] + self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (
+                                    self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
+                                return self.NewAgentProperties[:,sum(args[k]*mt.prod(len(self.VariablesDim[i[0]][j]) for j in range(k+1, len(self.VariablesDim[i[0]]))) for k in range(len(self.VariablesDim[i[0]])))]
+                            return [np.min(var(*i[1])),np.max(var(*i[1]))]
+
+                    case 'bvar':
+                        if self.VariablesDim[i[0]] == 0:
+                            LB = np.min(np.round(self.VariablesBound[i[0]][0] + self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0])))
+                            UB = np.max(np.round(self.VariablesBound[i[0]][0] + self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0])))
+                            return [LB,UB]
+
+                        else:
+                            def var(*args):
+                                self.NewAgentProperties = np.round(self.VariablesBound[i[0]][0] + self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (
+                                    self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
+                                return self.NewAgentProperties[:,sum(args[k]*mt.prod(len(self.VariablesDim[i[0]][j]) for j in range(k+1, len(self.VariablesDim[i[0]]))) for k in range(len(self.VariablesDim[i[0]])))]
+                            return [np.min(var(*i[1])),np.max(var(*i[1]))]
+                        
+                    case 'ivar':
+                        if self.VariablesDim[i[0]] == 0:
+                            LB = np.min(np.round(self.VariablesBound[i[0]][0] + self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0])))
+                            UB = np.min(np.round(self.VariablesBound[i[0]][0] + self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0])))
+                            return [LB,UB]
+
+                        else:
+                            def var(*args):
+                                self.NewAgentProperties = np.round(self.VariablesBound[i[0]][0] + self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (
+                                    self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
+                                return self.NewAgentProperties[:,sum(args[k]*mt.prod(len(self.VariablesDim[i[0]][j]) for j in range(k+1, len(self.VariablesDim[i[0]]))) for k in range(len(self.VariablesDim[i[0]])))]
+                            return [np.min(var(*i[1])),np.max(var(*i[1]))]
+                        
+                    case 'svar':
+                        return np.argsort(self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]])[i[1]]
+
+            else:
 
+                match self.VariablesType[i[0]]:
+
+                    case 'pvar':
+                        UB = np.max((self.VariablesBound[i[0]][0] + self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0])))
+                        LB = np.min((self.VariablesBound[i[0]][0] + self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0])))
+                        return [LB,UB]
+
+                    case 'fvar':
+                        UB = np.max(self.VariablesBound[i[0]][0] + self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
+                        LB = np.min(self.VariablesBound[i[0]][0] + self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0]))
+                        return [LB,UB]
+
+                    case 'bvar':
+                        UB = np.max(np.round(self.VariablesBound[i[0]][0] + self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0])))
+                        LB = np.min(np.round(self.VariablesBound[i[0]][0] + self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0])))
+                        return [LB,UB]
+
+                    case 'ivar':
+                        UB = np.max(np.round(self.VariablesBound[i[0]][0] + self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0])))
+                        LB= np.min(np.round(self.VariablesBound[i[0]][0] + self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]] * (self.VariablesBound[i[0]][1] - self.VariablesBound[i[0]][0])))
+                        return [UB,LB]
+
+                    case 'svar':
+                        return np.argsort(self.BestAgent[:,self.VariablesSpread[i[0]][0]:self.VariablesSpread[i[0]][1]])
+                    
     def get_payoff(self):
 
         payoff=[]
-        for i in range(len(self.ObjectivesDirections)):
-            if self.ObjectivesDirections[i]=='max':
+        for i in range(len(self.objectives_directions)):
+            if self.objectives_directions[i]=='max':
                 ind =np.argmax(self.get_obj()[:, i])
                 val = self.get_obj()[ind, :]
-            elif self.ObjectivesDirections[i] =='min':
+            elif self.objectives_directions[i] =='min':
                 ind = np.argmin(self.get_obj()[:, i])
                 val = self.get_obj()[ind, :]
             payoff.append(val)
         return np.array(payoff)
 
-    def report(self):
+    def report(self, all_metrics: bool = False, feloopy_info: bool = True, sys_info: bool = False, model_info: bool = True, sol_info: bool = True, obj_values: bool = True, dec_info: bool = True, metric_info: bool = True, ideal_pareto: Optional[np.ndarray] = [], ideal_point: Optional[np.array] = [], save=None):
 
-        print()
+        if save is not None:
+            stdout_origin = sys.stdout
+            sys.stdout = open(save, "w")
+
+        status = self.get_status()
+        hour, min, sec = calculate_time_difference(self.start,self.end)
 
-        import datetime
-        now = datetime.datetime.now()
-        date_str = now.strftime("Date: %Y-%m-%d")
-        time_str = now.strftime("Time: %H:%M:%S")
+        if len(str(status)) == 0:
+            status = ['infeasible (constrained)']
 
         box_width = 80
-        padding = box_width - len(date_str) - len(time_str) - 2
+        vspace()
 
-        print("+" + "-"*box_width + "+")
-        print("|" + " " + "FelooPy v0.2.5".center(box_width-2) + " " + "|")
-        print("+" + "-"*box_width + "+")
-        print("| " + date_str + " "*padding + time_str + " |")
-        padding = box_width - len("Solver: "+ self.SolverName) - len("Interface: "+ self.InterfaceName) - 2
-        print("| " + "Interface: " + self.InterfaceName + " "*padding + "Solver: "+ self.SolverName + " |")
-        print("+" + "-"*box_width + "+")
-        print("|" + " " + "Model Information".center(box_width-2) + " " + "|")
-        print("+" + "-"*box_width + "+")
-
-        self.ModelName, self.InterfaceName, self.SolverName, self.ObjectivesDirections, self.SolutionMethod
-        # determine the maximum length of variables
-        ModelName = "The '" + self.ModelName + "' model has:"
-        print("|" + " " + ModelName.center(box_width-2) + " " + "|")
-        if self.PositiveVariableCounter[0]>0:
-            P_report = str(self.PositiveVariableCounter[1]) + " positive variable(s) in " + str(self.PositiveVariableCounter[0]) + " class(es)."
-            print("|" + " " + P_report.center(box_width-2) + " " + "|")
-        if self.BinaryVariableCounter[0]>0:
-            P_report = str(self.BinaryVariableCounter[1]) + " binary variable(s) in " + str(self.BinaryVariableCounter[0]) + " class(es)."
-            print("|" + " " + P_report.center(box_width-2) + " " + "|")
-        if self.IntegerVariableCounter[0]>0:
-            P_report = str(self.IntegerVariableCounter[1]) + " integer variable(s) in " + str(self.IntegerVariableCounter[0]) + " class(es)."
-            print("|" + " " + P_report.center(box_width-2) + " " + "|")
-        if self.FreeVariableCounter[0]>0:
-            P_report = str(self.FreeVariableCounter[1]) + " free variable(s) in " + str(self.FreeVariableCounter[0]) + " class(es)."
-            print("|" + " " + P_report.center(box_width-2) + " " + "|")
-        if self.ObjectivesCounter[0]>0:
-            P_report = str(self.ObjectivesCounter[1]) + " objective(s)."
-            print("|" + " " + P_report.center(box_width-2) + " " + "|")
-        if self.ConstraintsCounter[0]>0:
-            P_report = str(self.ConstraintsCounter[1]) + " constraint(s) in " + str(self.ConstraintsCounter[0]) + " class(es)."
-            print("|" + " " + P_report.center(box_width-2) + " " + "|")
-        P_report =  "Total number of variables is " + str(self.ToTalVariableCounter[1]) + f" in {self.ToTalVariableCounter[1]} class(es)."
-        print("|" + " " + P_report.center(box_width-2) + " " + "|")
-
-        print("+" + "-"*box_width + "+")
-        print("|" + " " + "Solve Information".center(box_width-2) + " " + "|")
-        print("+" + "-"*box_width + "+")
-        padding = box_width - len("Method: "+ self.SolutionMethod) - len("Objective Value(s)") - 2
-        print("| " + "Method: "+ self.SolutionMethod + " "*padding + "Objective Value(s)" + " |")
-        status= self.get_status()
-        if len(self.ObjectivesDirections)!=1:
-            row = "| " + "Status: " + " "*(len(status[0]) - len("Status: ")) + " " * (box_width-10*len(self.ObjectivesDirections)+1  - len(str(status[0])) - 3)
-            for j in range(len(self.ObjectivesDirections)):
-                obj_row = self.ObjectivesDirections[j]
-                row += " " * (10 - len(obj_row)) + obj_row
-            print(row + " |")
-            for i in range(len(status)): 
-                row = "| " + str(status[i]) + " " * (box_width-10*len(self.ObjectivesDirections) +1 - len(str(status[i])) - 3)
-                obj_row = self.get_obj()[i]
-                for j in range(len(obj_row)):
-                    num_str = format_string(obj_row[j])
-                    row += " " * (10 - len(num_str)) + num_str
-                print(row + " |")
-            for j in range(len(self.ObjectivesDirections)):
-                row = "| " + str(f"payoff {j}") + " " * (box_width-10*len(self.ObjectivesDirections) +1 - len(str(f"payoff {j}")) - 3)
-                for k in range(len(self.ObjectivesDirections)):
-                    num_str = format_string(self.get_payoff()[j,k])
-                    row += " " * (10 - len(num_str)) + num_str
-                print(row + " |")
-        else:
-            row = "| " + "Status: " + " "*(len(status) - len("Status: ")) + " " * (box_width-9*len(self.ObjectivesDirections) +1 - len(str(status)) - 3)
-            for j in range(len(self.ObjectivesDirections)):
-                obj_row = self.ObjectivesDirections[j]
-                row += " " * (9 - len(obj_row)) + obj_row
-            print(row + " |")
-            row = "| " + str(status) + " " * (box_width-9*len(self.ObjectivesDirections) +1 - len(str(status)) - 3)
-            obj_row = self.get_obj()
-            num_str = format_string(obj_row)
-            row += " " * (9 - len(num_str)) + num_str
-            print(row + " |")
-        print("+" + "-"*box_width + "+")
-        print("|" + " " + "Metric Information".center(box_width-2) + " " + "|")
-        print("+" + "-"*box_width + "+")
-        hour = round(((self.end-self.start)), 3) % (24 * 3600) // 3600
-        min = round(((self.end-self.start)), 3) % (24 * 3600) % 3600 // 60
-        sec = round(((self.end-self.start)), 3) % (24 * 3600) % 3600 % 60
-        if len(self.ObjectivesDirections)!=1:
+        if feloopy_info:
+            
+            import datetime
+            now = datetime.datetime.now()
+            date_str = now.strftime("Date: %Y-%m-%d")
+            time_str = now.strftime("Time: %H:%M:%S")
+            tline_text("FelooPy v0.2.6")
+            empty_line()
+            two_column(date_str, time_str)
+            two_column(f"Interface: {self.interface_name}", f"Solver: {self.solver_name}")
+            empty_line()
+            bline()
+
+        if sys_info:
             try:
+                import psutil
+                import cpuinfo
+                import platform
+                tline_text("System")
+                empty_line()
+                cpu_info = cpuinfo.get_cpu_info()["brand_raw"]
+                cpu_cores = psutil.cpu_count(logical=False)
+                cpu_threads = psutil.cpu_count(logical=True)
+                ram_info = psutil.virtual_memory()
+                ram_total = ram_info.total
+                os_info = platform.system()
+                os_version = platform.version()
+                left_align(f"OS: {os_version} ({os_info})")
+                left_align(f"CPU   Model: {cpu_info}")
+                left_align(f"CPU   Cores: {cpu_cores}")
+                left_align(f"CPU Threads: {cpu_threads}")
                 try:
-                    self.get_indicators()
-                    print("| CPT   (microseconds): ", format_string((self.end-self.start)*10 **6) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| CPT   (hour:min:sec): ", "%02d:%02d:%02d" % (hour, min, sec)+ " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| NP    (max):          ", format_string(len((self.get_obj())))+ " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| GD    (min):          ", format_string(self.calculated_indicators['gd'])+ " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| GDP   (min):          ", format_string(self.calculated_indicators['gdp'])+ " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| IGD   (min):          ", format_string(self.calculated_indicators['igd'])+ " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| IGDP  (min):          ", format_string(self.calculated_indicators['igdp'])+ " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    if np.isnan(self.calculated_indicators['ms']):
-                        print("| MS    (max):               ", format_string(self.calculated_indicators['ms']) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    else:
-                        print("| MS    (max):          ", format_string(self.calculated_indicators['ms']) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| SP    (max):          ", format_string(self.calculated_indicators['sp']) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| HV    (max):          ", format_string(self.calculated_indicators['hv']) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
+                    import GPUtil
+                    gpus = GPUtil.getGPUs()
+                    for gpu in gpus:
+                        left_align(f"GPU   Model: {gpu.name}")
+                        left_align(f"GPU    VRAM: {gpu.memoryTotal / 1024:.2f} GB")
                 except:
-                    print("| CPT   (microseconds): ", format_string((self.end-self.start)*10 **6) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| CPT   (hour:min:sec): ", "%02d:%02d:%02d" % (hour, min, sec)+ " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| NP    (max):          ", format_string(len((self.get_obj())))+ " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| GD    (min):          ", format_string(self.calculated_indicators['gd']) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| GDP   (min):          ", format_string(self.calculated_indicators['gdp']) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| IGD   (min):          ", format_string(self.calculated_indicators['igd']) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| IGDP  (min):          ", format_string(self.calculated_indicators['igdp']) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    if np.isnan(self.calculated_indicators['ms']):
-                        print("| MS    (max):               ", format_string(self.calculated_indicators['ms']) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    else:
-                        print("| MS    (max):          ", format_string(self.calculated_indicators['ms']) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                    print("| SP    (max):          ", format_string(self.calculated_indicators['sp']) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
+                    pass
+                left_align(f"SYSTEM  RAM: {ram_total / (1024 ** 3):.2f} GB")
             except:
-                print("| CPT   (microseconds): ", format_string((self.end-self.start)*10 **6) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-                print("| CPT   (hour:min:sec): ", "%02d:%02d:%02d" % (hour, min, sec) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-        else:
-            print("| CPT   (microseconds): ", format_string((self.end-self.start)*10 **6) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")
-            print("| CPT   (hour:min:sec): ", "%02d:%02d:%02d" % (hour, min, sec) + " "*(box_width-len("| CPT   (micro-sec):    ")-8) + "|")     
-        print("+" + "-"*box_width + "+")
+                pass
+            empty_line()
+            bline()
+
+        if model_info:
+            tline_text("Model")
+            empty_line()
+            left_align(f"Name: {self.model_name}")
+            list_three_column([
+                ("Feature:         ", "Class:", "Total:"),
+                ("Positive variable", self.pos_var_counter[0], self.pos_var_counter[1]),
+                ("Binary variable  ", self.bin_var_counter[0], self.bin_var_counter[1]),
+                ("Integer variable ", self.int_var_counter[0], self.int_var_counter[1]),
+                ("Free variable    ", self.free_var_counter[0], self.free_var_counter[1]), 
+                ("Total variables  ", self.tot_counter[0], self.tot_counter[1]), 
+                ("Objective        ", "-", self.obj_counter[1]), 
+                ("Constraint       ", self.con_counter[0], self.con_counter[1]) ])
+            empty_line()
+            bline()
+
+        if sol_info:
+            tline_text("Solve")
+            empty_line()
+            two_column(f"Method: {self.solution_method}", "Objective value")
+            status_row_print(self.objectives_directions, status)
+            if obj_values:
+                if len(self.objectives_directions) != 1:
+                    try:
+                        solution_print(self.objectives_directions, status, self.get_obj(), self.get_payoff())
+                    except:
+                        left_align("Nothing found.")
+                else:
+                    solution_print(self.objectives_directions, status, self.get_obj())
+            empty_line()
+            bline()
+
+        if metric_info:
+            tline_text("Metric")
+            empty_line()
+            self.calculated_indicators = None
+            try:
+                self.get_indicators(ideal_pareto=ideal_pareto, ideal_point=ideal_point)
+            except:
+                pass
+            metrics_print(self.objectives_directions, all_metrics, self.get_obj(), self.calculated_indicators, self.start, self.end)
+            empty_line()
+            bline()
+
+        if dec_info:
+            tline_text("Decision")
+            empty_line()
+            self.decision_information_print(status)
+            empty_line()
+            bline()
+
+        if save is not None:
+            sys.stdout.close()
+            sys.stdout = stdout_origin
+
+    def decision_information_print(self, status, box_width=80):
         if type(status) == str:
-            print("|" + " " + "Decision Information".center(box_width-2) + " " + "|")
-            print("+" + "-"*box_width + "+")
             for i in self.VariablesDim.keys():
                 if self.VariablesDim[i] == 0:
-                    if self.get([i,(0,)])!=0:
-                        print(f"| {i} =", self.get([i,(0,)]), " "* (box_width-(len(f"| {i} =") + len(str(self.get([i,(0,)])))) -1) + "|")
-                elif len(self.VariablesDim[i])==1:
+                    if self.get([i, (0,)]) != 0:
+                        print(f"| {i} =", self.get([i, (0,)]), " " * (box_width - (len(f"| {i} =") + len(str(self.get([i, (0,)])))) - 1) + "|")
+                elif len(self.VariablesDim[i]) == 1:
                     for k in fix_dims(self.VariablesDim[i])[0]:
-                        if self.get([i,(k,)])!=0:
-                            print(f"| {i}[{k}] =", self.get([i,(k,)]), " "* (box_width-(len(f"| {i}[{k}] =") + len(str(self.get([i,(k,)])))) - 1) + "|")
+                        if self.get([i, (k,)]) != 0:
+                            print(f"| {i}[{k}] =", self.get([i, (k,)]), " " * (box_width - (len(f"| {i}[{k}] =") + len(str(self.get([i, (k,)])))) - 1) + "|")
                 else:
                     for k in it.product(*tuple(fix_dims(self.VariablesDim[i]))):
-                        if self.get([i,(*k,)])!=0:
-                            print(f"| {i}[{k}] =".replace("(", "").replace(")", ""), self.get([i,(*k,)]), " "* (box_width-(len(f"| {i}[{k}] =".replace("(", "").replace(")", "")) + len(str(self.get([i,(*k,)])))) - 1) + "|")
-            print("+" + "-"*box_width + "+")
-
-        
+                        if self.get([i, (*k,)]) != 0:
+                            print(f"| {i}[{k}] =".replace("(", "").replace(")", ""), self.get([i, (*k,)]), " " * (box_width - (len(f"| {i}[{k}] =".replace("(", "").replace(")", "")) + len(str(self.get([i, (*k,)])))) - 1) + "|")
+        else:
+            for i in self.VariablesDim.keys():
+                if self.VariablesDim[i] == 0:
+                    if self.get_bound([i, (0,)])!=[0,0]:
+                        print(f"| {i} =", self.get_bound([i, (0,)]), " " * (box_width - (len(f"| {i} =") + len(str(self.get_bound([i, (0,)])))) - 1) + "|")
+                elif len(self.VariablesDim[i]) == 1:
+                    for k in fix_dims(self.VariablesDim[i])[0]:
+                        if self.get_bound([i, (k,)])!= [0,0]:
+                            print(f"| {i}[{k}] =", self.get_bound([i, (k,)]), " " * (box_width - (len(f"| {i}[{k}] =") + len(str(self.get_bound([i, (k,)])))) - 1) + "|")
+                else:
+                    for k in it.product(*tuple(fix_dims(self.VariablesDim[i]))):
+                        if self.get_bound([i, (*k,)]) != [0,0]:
+                            print(f"| {i}[{k}] =".replace("(", "").replace(")", ""), self.get_bound([i, (*k,)]), " " * (box_width - (len(f"| {i}[{k}] =".replace("(", "").replace(")", "")) + len(str(self.get_bound([i, (*k,)])))) - 1) + "|")
+    
 # Alternatives for defining this class:
             
 construct = make_model = implementor = implement = Implement
+
+
+
```

### Comparing `feloopy-0.2.5/feloopy/generators/model/feloopy_model_generator.py` & `feloopy-0.2.6/feloopy/generators/model/feloopy_model_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/generators/model_generator.py` & `feloopy-0.2.6/feloopy/generators/model_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,19 @@
             model_object = pymprog_model_generator.generate_model(features)
 
         case 'cplex':
 
             from .model import cplex_model_generator
             model_object = cplex_model_generator.generate_model(features)
 
+        case 'localsolver':
+
+            from .model import localsolver_model_generator
+            model_object = localsolver_model_generator.generate_model(features)
+
         case 'cplex_cp':
 
             from .model import cplex_cp_model_generator
             model_object = cplex_cp_model_generator.generate_model(features)
 
         case 'gurobi':
 
@@ -84,8 +89,18 @@
             model_object = mip_model_generator.generate_model(features)
 
         case 'linopy':
 
             from .model import linopy_model_generator
             model_object = linopy_model_generator.generate_model(features)
 
+        case 'rsome_ro':
+
+            from .model import rsome_ro_model_generator
+            model_object = rsome_ro_model_generator.generate_model(features)
+
+        case 'rsome_dro':
+
+            from .model import rsome_dro_model_generator
+            model_object = rsome_dro_model_generator.generate_model(features)    
+
     return model_object
```

### Comparing `feloopy-0.2.5/feloopy/generators/result/cplex_cp_result_generator.py` & `feloopy-0.2.6/feloopy/generators/result/cplex_cp_result_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
  # @ Modified: 2023-05-12
  # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
-
 def Get(model_object, result, input1, input2=None):
 
     input1 = input1[0]
 
     match input1:
 
         case 'variable':
```

### Comparing `feloopy-0.2.5/feloopy/generators/result/cplex_result_generator.py` & `feloopy-0.2.6/feloopy/generators/result/picos_result_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,32 +4,31 @@
  # @ Modified: 2023-05-12
  # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
-import cplex
-from docplex.mp.model import Model as CPLEXMODEL
+import picos as picos_interface
 
 
 def Get(model_object, result, input1, input2=None):
 
     input1 = input1[0]
 
     match input1:
 
         case 'variable':
 
-            return input2.solution_value
+            return input2.value
 
         case 'status':
 
-            return model_object.solve_details.status
+            return result[0].claimedStatus
 
         case 'objective':
 
-            return model_object.objective_value
+            return model_object.obj_value()
 
         case 'time':
 
             return (result[1][1]-result[1][0])
```

### Comparing `feloopy-0.2.5/feloopy/generators/result/cvxpy_result_generator.py` & `feloopy-0.2.6/feloopy/generators/result/mip_result_generator.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,34 +4,31 @@
  # @ Modified: 2023-05-12
  # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
+import mip as mip_interface
+
 
 def Get(model_object, result, input1, input2=None):
 
     input1 = input1[0]
 
     match input1:
 
         case 'variable':
 
-            if len(input2.value) == 1:
-
-                return input2.value[0]
-
-            else:
-                return input2.value
+            return input2.x
 
         case 'status':
 
-            return result[0][0].status
+            return result[0]
 
         case 'objective':
 
-            return result[0][0].value
+            return model_object.objective_value
 
         case 'time':
 
             return (result[1][1]-result[1][0])
```

### Comparing `feloopy-0.2.5/feloopy/generators/result/cylp_result_generator.py` & `feloopy-0.2.6/feloopy/generators/result/cylp_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/generators/result/gekko_result_generator.py` & `feloopy-0.2.6/feloopy/generators/result/gekko_result_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,28 +6,30 @@
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
 import gekko as gekko_interface
 
-gekko_status_dict = {0: "not_optimal", 1: "optimal"}
-
+gekko_status_dict = {0: "unknown", 1: "optimal"}
 
 def Get(model_object, result, input1, input2=None):
 
     directions = +1 if input1[1][input1[2]] == 'min' else -1
 
     input1 = input1[0]
 
     match input1:
 
         case 'variable':
 
-            return input2.value[0]
+            try:
+                return input2.value[0]
+            except: 
+                return input2
 
         case 'status':
 
             return gekko_status_dict.get(model_object.options.SOLVESTATUS)
 
         case 'objective':
```

### Comparing `feloopy-0.2.5/feloopy/generators/result/gurobi_result_generator.py` & `feloopy-0.2.6/feloopy/generators/result/gurobi_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/generators/result/linopy_result_generator.py` & `feloopy-0.2.6/feloopy/generators/result/linopy_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/generators/result/mip_result_generator.py` & `feloopy-0.2.6/feloopy/generators/result/xpress_result_generator.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,31 +4,31 @@
  # @ Modified: 2023-05-12
  # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
-import mip as mip_interface
+import xpress as xpress_interface
 
 
 def Get(model_object, result, input1, input2=None):
 
     input1 = input1[0]
 
     match input1:
 
         case 'variable':
 
-            return input2.x
+            return model_object.getSolution(input2)
 
         case 'status':
 
-            return result[0]
+            return model_object.getProbStatusString()
 
         case 'objective':
 
-            return model_object.objective_value
-
+            return model_object.getObjVal()
+        
         case 'time':
 
             return (result[1][1]-result[1][0])
```

### Comparing `feloopy-0.2.5/feloopy/generators/result/ortools_cp_result_generator.py` & `feloopy-0.2.6/feloopy/generators/result/ortools_cp_result_generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,16 +6,21 @@
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
 from ortools.sat.python import cp_model
 
-ortools_status_dict = {cp_model.OPTIMAL: "optimal",
-                       cp_model.FEASIBLE: "feasible"}
+ortools_status_dict = {
+    cp_model.OPTIMAL: "optimal",
+    cp_model.FEASIBLE: "feasible",
+    cp_model.INFEASIBLE: "infeasible",
+    cp_model.MODEL_INVALID: "model_invalid",
+    cp_model.UNKNOWN: "unknown"
+}
 
 
 def Get(model_object, result, input1, input2=None):
 
     input1 = input1[0]
 
     match input1:
```

### Comparing `feloopy-0.2.5/feloopy/generators/result/ortools_result_generator.py` & `feloopy-0.2.6/feloopy/generators/result/ortools_result_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,14 @@
  '''
 
 from ortools.linear_solver import pywraplp as ortools_interface
 
 ortools_status_dict = {0: "optimal", 1: "feasible", 2: "infeasible",
                        3: "unbounded", 4: "abnormal", 5: "model_invalid", 6: "not_solved"}
 
-
 def Get(model_object, result, input1, input2=None):
 
     input1 = input1[0]
 
     match input1:
 
         case 'variable':
@@ -31,7 +30,15 @@
         case 'objective':
 
             return model_object.Objective().Value()
 
         case 'time':
 
             return (result[1][1]-result[1][0])
+        
+        case 'dual':
+
+            return model_object.LookupConstraint(input2).dual_value()
+        
+        case 'slack':
+
+            print('Not supported in ortools.')
```

### Comparing `feloopy-0.2.5/feloopy/generators/result/pymprog_result_generator.py` & `feloopy-0.2.6/feloopy/generators/result/pymprog_result_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/generators/result/pyomo_result_generator.py` & `feloopy-0.2.6/feloopy/generators/result/pyomo_result_generator.py`

 * *Files 25% similar despite different names*

```diff
@@ -28,7 +28,19 @@
         case 'objective':
 
             return pyomo_interface.value(model_object.OBJ)
 
         case 'time':
 
             return (result[1][1]-result[1][0])
+        
+        case 'dual':
+
+            return model_object.dual[model_object.c[input2]]
+
+        case 'slack':
+
+            upper_slack = model_object.c[input2].uslack()
+            lower_slack = model_object.c[input2].lslack()
+
+            return min(upper_slack, lower_slack)
+
```

### Comparing `feloopy-0.2.5/feloopy/generators/result/xpress_result_generator.py` & `feloopy-0.2.6/feloopy/generators/result/cplex_result_generator.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,31 +4,44 @@
  # @ Modified: 2023-05-12
  # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
-import xpress as xpress_interface
+import cplex
+from docplex.mp.model import Model as CPLEXMODEL
 
 
 def Get(model_object, result, input1, input2=None):
 
     input1 = input1[0]
 
     match input1:
 
         case 'variable':
 
-            return model_object.getSolution(input2)
+            return input2.solution_value
 
         case 'status':
 
-            return result[0]
+            return model_object.solve_details.status
 
         case 'objective':
 
-            return model_object.getSolution(result[0])
+            return model_object.objective_value
 
         case 'time':
 
             return (result[1][1]-result[1][0])
+
+        case 'dual':
+
+            return  model_object.get_duals(model_object.get_constraints_by_name(input2))[0]
+        
+        case 'slack':
+
+            return model_object.get_slacks(model_object.get_constraints_by_name(input2))[0]
+        
+
+            
+
```

### Comparing `feloopy-0.2.5/feloopy/generators/result_generator.py` & `feloopy-0.2.6/feloopy/generators/result_generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     InterfaceName = input['interface_name']
 
     indicator = [Thing,
                  input['directions'],
                  input['objective_being_optimized']]
 
-    if indicator[0] == 'variable':
+    if indicator[0] == 'variable' or indicator[0] == 'dual' or indicator[0] == 'slack':
 
         match InterfaceName:
 
             case 'pulp':
 
                 from .result import pulp_result_generator
                 return pulp_result_generator.Get(model_object, model_solution, indicator, variable_name_with_index)
@@ -62,14 +62,19 @@
                 return cylp_result_generator.Get(model_object, model_solution, indicator, variable_name_with_index)
 
             case 'pymprog':
 
                 from .result import pymprog_result_generator
                 return pymprog_result_generator.Get(model_object, model_solution, indicator, variable_name_with_index)
 
+            case 'localsolver':
+
+                from .result import localsolver_result_generator
+                return localsolver_result_generator.Get(model_object, model_solution, indicator, variable_name_with_index)
+
             case 'cplex':
 
                 from .result import cplex_result_generator
                 return cplex_result_generator.Get(model_object, model_solution, indicator, variable_name_with_index)
 
             case 'cplex_cp':
 
@@ -92,14 +97,25 @@
                 return mip_result_generator.Get(model_object, model_solution, indicator, variable_name_with_index)
 
             case 'linopy':
 
                 from .result import linopy_result_generator
                 return linopy_result_generator.Get(model_object, model_solution, indicator, variable_name_with_index)
 
+
+            case 'rsome_ro':
+
+                from .result import rsome_ro_result_generator
+                return rsome_ro_result_generator.Get(model_object, model_solution, indicator, variable_name_with_index)
+
+            case 'rsome_dro':
+
+                from .result import rsome_dro_result_generator
+                return rsome_dro_result_generator.Get(model_object, model_solution, indicator, variable_name_with_index)
+
     elif indicator[0] == 'objective' or indicator[0] == 'status' or indicator[0] == 'time':
 
         match InterfaceName:
 
             case 'pulp':
 
                 from .result import pulp_result_generator
@@ -111,14 +127,19 @@
                 return pyomo_result_generator.Get(model_object, model_solution, indicator)
 
             case 'ortools':
 
                 from .result import ortools_result_generator
                 return ortools_result_generator.Get(model_object, model_solution, indicator)
 
+            case 'localsolver':
+
+                from .result import localsolver_result_generator
+                return localsolver_result_generator.Get(model_object, model_solution, indicator)
+            
             case 'ortools_cp':
 
                 from .result import ortools_cp_result_generator
                 return ortools_cp_result_generator.Get(model_object, model_solution, indicator)
 
             case 'gekko':
 
@@ -170,7 +191,18 @@
                 from .result import mip_result_generator
                 return mip_result_generator.Get(model_object, model_solution, indicator)
 
             case 'linopy':
 
                 from .result import linopy_result_generator
                 return linopy_result_generator.Get(model_object, model_solution, indicator)
+            
+            case 'rsome_ro':
+                    
+                from .result import rsome_ro_result_generator
+                return rsome_ro_result_generator.Get(model_object, model_solution, indicator)
+
+            case 'rsome_dro':
+
+                from .result import rsome_dro_result_generator
+                return rsome_dro_result_generator.Get(model_object, model_solution, indicator)
+
```

### Comparing `feloopy-0.2.5/feloopy/generators/solution/cplex_cp_solution_generator.py` & `feloopy-0.2.6/feloopy/generators/solution/cplex_cp_solution_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,13 +49,13 @@
             elif directions[objective_id] == 'max':
                 model_object.add(model_object.maximize(model_objectives[objective_id]))
 
         for constraint in model_constraints:
             model_object.add(constraint)
 
         time_solve_begin = timeit.default_timer()
-        result = model_object.solve(TimeLimit=time_limit, log_output=log)
+        result = model_object.solve(TimeLimit=time_limit)
         time_solve_end = timeit.default_timer()
 
         generated_solution = [result, [time_solve_begin, time_solve_end]]
 
     return generated_solution
```

### Comparing `feloopy-0.2.5/feloopy/generators/solution/cplex_solution_generator.py` & `feloopy-0.2.6/feloopy/generators/solution/cplex_solution_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,16 +90,18 @@
                     model_object.set_objective(
                         'min', model_objectives[objective_id])
 
                 case 'max':
                     model_object.set_objective(
                         'max', model_objectives[objective_id])
 
+            counter=0
             for constraint in model_constraints:
-                model_object.add_constraint(constraint)
+                model_object.add_constraint(constraint, name=constraint_labels[counter])
+                counter+=1
 
             if save_model != False:
 
                 if '.lp' in save_model:
                     model_object.export_as_lp(path=save_model)
                 if '.mps' in save_model:
                     model_object.export_as_mps(path=save_model)
```

### Comparing `feloopy-0.2.5/feloopy/generators/solution/cvxpy_solution_generator.py` & `feloopy-0.2.6/feloopy/generators/solution/cvxpy_solution_generator.py`

 * *Files 18% similar despite different names*

```diff
@@ -56,42 +56,50 @@
     email = features['email_address']
     max_iterations = features['max_iterations']
     solver_options = features['solver_options']
 
     options = {'solver': cvxpy_solver_selector[solver_name], 'verbose': log,
                'scipy_options': solver_options.get('scipy_options', None)}
 
+    constraint_dict = dict()
+    if len(model_constraints)!=0:
+        if constraint_labels[0]!=None:
+            for i in range(len(model_constraints)):
+                constraint_dict[constraint_labels[i]] = model_constraints[i]
+
     for key in solver_options:
 
         if key != 'scipy_options':
 
             options[key] = solver_options[key]
 
     if solver_name not in cvxpy_solver_selector.keys():
-        raise RuntimeError(
-            "Using solver '%s' is not supported by 'cvxpy'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
+        
+        raise RuntimeError("Using solver '%s' is not supported by 'cvxpy'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
 
     match debug:
 
         case False:
 
             match directions[objective_id]:
 
                 case 'min':
-                    obj = cvxpy_interface.Minimize(
-                        model_objectives[objective_id])
+
+                    obj = cvxpy_interface.Minimize(model_objectives[objective_id])
 
                 case 'max':
-                    obj = cvxpy_interface.Maximize(
-                        model_objectives[objective_id])
 
-            print(options)
+                    obj = cvxpy_interface.Maximize(model_objectives[objective_id])
 
             prob = cvxpy_interface.Problem(obj, model_constraints)
+            
             time_solve_begin = timeit.default_timer()
+            
             result = prob.solve(**options)
+            
             time_solve_end = timeit.default_timer()
+            
             newresult = [prob, result]
-            generated_solution = [newresult, [
-                time_solve_begin, time_solve_end]]
+
+            generated_solution = [[newresult,constraint_dict], [time_solve_begin, time_solve_end]]
 
     return generated_solution
```

### Comparing `feloopy-0.2.5/feloopy/generators/solution/cylp_solution_generator.py` & `feloopy-0.2.6/feloopy/generators/solution/cylp_solution_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
 import cylp as cylp_interface
 from cylp.cy import CyClpSimplex
 import timeit
 
-cylp_solver_selector = {'cbc': 'cbc'}
+cylp_solver_selector = {'cbc': 'cbc', 'clp':'clp', 'cgl':'cgl'}
 
 
 def generate_solution(features):
 
     model_object = features['model_object_before_solve']
     model_objectives = features['objectives']
     model_constraints = features['constraints']
```

### Comparing `feloopy-0.2.5/feloopy/generators/solution/feloopy_solution_generator.py` & `feloopy-0.2.6/feloopy/generators/solution/feloopy_solution_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
  '''
 
 import timeit
 from tabulate import tabulate as tb
 import numpy as np
 
 
-def generate_solution(model_object, fitness_function, total_features, objectives_directions, objective_number, number_of_times, show_plots):
+def generate_solution(model_object, fitness_function, total_features, objectives_directions, objective_number, number_of_times, show_plots,show_log):
 
     if number_of_times == 1:
 
         time_solve_begin = timeit.default_timer()
         x, y, status = model_object.solve(fitness_function)
         time_solve_end = timeit.default_timer()
         return x, y, time_solve_begin, time_solve_end, status
```

### Comparing `feloopy-0.2.5/feloopy/generators/solution/gekko_solution_generator.py` & `feloopy-0.2.6/feloopy/generators/solution/gekko_solution_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import gekko as gekko_interface
 import timeit
 
 gekko_solver_selector = {'apopt': 1,
                          'bpopt': 2,
                          'ipopt': 3}
 
-
 def generate_solution(features):
 
     model_object = features['model_object_before_solve']
     model_objectives = features['objectives']
     model_constraints = features['constraints']
     directions = features['directions']
     constraint_labels = features['constraint_labels']
```

### Comparing `feloopy-0.2.5/feloopy/generators/solution/gurobi_solution_generator.py` & `feloopy-0.2.6/feloopy/generators/solution/gurobi_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/generators/solution/linopy_solution_generator.py` & `feloopy-0.2.6/feloopy/generators/solution/xpress_solution_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,18 @@
  # @ Modified: 2023-05-12
  # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
-from linopy import Model as LINOPYMODEL
+import xpress as xpress_interface
 import timeit
 
-linopy_solver_selector = {'cbc': 'cbc',
-                          'glpk': 'glpk',
-                          'highs': 'highs',
-                          'gurobi': 'gurobi',
-                          'xpress': 'xpress',
-                          'cplex': 'cplex'}
+xpress_solver_selector = {'xpress': 'xpress'}
 
 
 def generate_solution(features):
 
     model_object = features['model_object_before_solve']
     model_objectives = features['objectives']
     model_constraints = features['constraints']
@@ -36,30 +31,39 @@
     log = features['log']
     save = features['save_solver_log']
     save_model = features['write_model_file']
     email = features['email_address']
     max_iterations = features['max_iterations']
     solver_options = features['solver_options']
 
-    if solver_name not in linopy_solver_selector.keys():
+    if log:
+        ""
+    else:
+        model_object.controls.outputlog = 0
+
+    if solver_name not in xpress_solver_selector.keys():
         raise RuntimeError(
-            "Using solver '%s' is not supported by 'linopy'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
+            "Using solver '%s' is not supported by 'xpress'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
 
     match debug:
 
         case False:
 
+            for constraint in model_constraints:
+                model_object.addConstraint(constraint)
+
             match directions[objective_id]:
+
                 case "min":
-                    model_object.add_objective(model_objectives[objective_id])
-                case "max":
-                    model_object.add_objective(-model_objectives[objective_id])
+                    model_object.setObjective(
+                        model_objectives[objective_id], sense=xpress_interface.minimize)
 
-            for constraint in model_constraints:
-                model_object.add_constraints(constraint)
+                case "max":
+                    model_object.setObjective(
+                        model_objectives[objective_id], sense=xpress_interface.maximize)
 
             time_solve_begin = timeit.default_timer()
-            result = model_object.solve(solver_name=solver_name)
+            result = model_object.solve()
             time_solve_end = timeit.default_timer()
             generated_solution = [result, [time_solve_begin, time_solve_end]]
 
     return generated_solution
```

### Comparing `feloopy-0.2.5/feloopy/generators/solution/mealpy_solution_generator.py` & `feloopy-0.2.6/feloopy/generators/solution/mealpy_solution_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,24 @@
 
 import numpy as np
 import timeit
 from tabulate import tabulate as tb
 from mealpy.utils.visualize import *
 
 
-def generate_solution(model_object, fitness_function, total_features, objectives_directions, objective_number, number_of_times, show_plots, save_plots):
+def generate_solution(model_object, fitness_function, total_features, objectives_directions, objective_number, number_of_times, show_plots, save_plots,show_log):
 
     problem = {
         "fit_func": fitness_function,
         "lb": [0, ] * total_features[1],
         "ub": [1, ] * total_features[1],
         "minmax": objectives_directions[objective_number],
         "log_to": None,
         "save_population": False,
+        "verbose": show_log
     }
 
     if number_of_times == 1:
 
         time_solve_begin = timeit.default_timer()
         best_agent, best_reward = model_object.solve(problem)
         time_solve_end = timeit.default_timer()
```

### Comparing `feloopy-0.2.5/feloopy/generators/solution/mip_solution_generator.py` & `feloopy-0.2.6/feloopy/generators/solution/mip_solution_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
 import mip as mip_interface
 import timeit
 
-mip_solver_selector = {'cbc': 'cbc'}
+mip_solver_selector = {'cbc': 'cbc', 'gurobi': 'gurobi', 'cplex': 'cplex', 'glpk': 'glpk'}
 
 
 def generate_solution(features):
 
     model_object = features['model_object_before_solve']
     model_objectives = features['objectives']
     model_constraints = features['constraints']
@@ -34,14 +34,19 @@
     email = features['email_address']
     max_iterations = features['max_iterations']
     solver_options = features['solver_options']
 
     if solver_name not in mip_solver_selector.keys():
         raise RuntimeError(
             "Using solver '%s' is not supported by 'mip'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
+    
+    if log:
+        ""
+    else:
+        model_object.verbose = 0
 
     match debug:
 
         case False:
 
             for constraint in model_constraints:
                 model_object += constraint
```

### Comparing `feloopy-0.2.5/feloopy/generators/solution/ortools_cp_solution_generator.py` & `feloopy-0.2.6/feloopy/generators/solution/ortools_cp_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/generators/solution/ortools_solution_generator.py` & `feloopy-0.2.6/feloopy/generators/solution/ortools_solution_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,16 +62,21 @@
 
                 case "min":
                     model_object.Minimize(model_objectives[objective_id])
 
                 case "max":
                     model_object.Maximize(model_objectives[objective_id])
 
-            for constraint in model_constraints:
-                model_object.Add(constraint)
+            if len(model_constraints)!=0:
+                counter=0
+                for constraint in model_constraints:
+                    if constraint_labels[counter]==None:
+                        constraint_labels[counter]=f"con[{counter}]"
+                    model_object.Add(constraint, name=constraint_labels[counter])
+                    counter+=1
 
             model_object.CreateSolver(ortools_solver_selector[solver_name])
             solverParams = ortools_interface.MPSolverParameters()
 
             if time_limit != None:
                 model_object.set_time_limit(time_limit)
```

### Comparing `feloopy-0.2.5/feloopy/generators/solution/picos_solution_generator.py` & `feloopy-0.2.6/feloopy/generators/solution/picos_solution_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/generators/solution/pulp_solution_generator.py` & `feloopy-0.2.6/feloopy/generators/solution/pulp_solution_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,16 +85,19 @@
 
                 case "min":
                     model_object += model_objectives[objective_id]
 
                 case "max":
                     model_object += -model_objectives[objective_id]
 
-            for constraint in model_constraints:
-                model_object += constraint
+            if len(model_constraints)!=0:
+                counter = 0
+                for constraint in model_constraints:
+                    model_object += (constraint, constraint_labels[counter])
+                    counter+=1
 
             time_solve_begin = timeit.default_timer()
             result = model_object.solve(
                 solver=pulp_solver_selector[solver_name])
             time_solve_end = timeit.default_timer()
             generated_solution = [result, [time_solve_begin, time_solve_end]]
```

### Comparing `feloopy-0.2.5/feloopy/generators/solution/pymprog_solution_generator.py` & `feloopy-0.2.6/feloopy/generators/solution/pymprog_solution_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 
     else:
 
         msg_lev = pymprog_interface.glpk.GLP_MSG_OFF
 
     if time_limit != None:
         tmlim = time_limit
+    else:
+        tmlim= None
 
     if solver_name not in pymprog_solver_selector.keys():
         raise RuntimeError(
             "Using solver '%s' is not supported by 'pymprog'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
 
     match debug:
```

### Comparing `feloopy-0.2.5/feloopy/generators/solution/pymultiobjective_solution_generator.py` & `feloopy-0.2.6/feloopy/generators/solution/pymultiobjective_solution_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,51 +8,51 @@
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
 import numpy as np
 import timeit
 
 
-def generate_solution(solver_name, AlgOptions, Fitness, ToTalVariableCounter, ObjectivesDirections, ObjectiveBeingOptimized, number_of_times, show_plots, save_plots):
+def generate_solution(solver_name, AlgOptions, Fitness, ToTalVariableCounter, ObjectivesDirections, ObjectiveBeingOptimized, number_of_times, show_plots, save_plots,show_log):
 
-    ObjectivesDirections = [-1 if direction ==
-                            'max' else 1 for direction in ObjectivesDirections]
+    ObjectivesDirections = [-1 if direction =='max' else 1 for direction in ObjectivesDirections]
 
     def f1(X): return ObjectivesDirections[0]*Fitness(np.array(X))[0]
     def f2(X): return ObjectivesDirections[1]*Fitness(np.array(X))[1]
     def f3(X): return ObjectivesDirections[2]*Fitness(np.array(X))[2]
     def f4(X): return ObjectivesDirections[3]*Fitness(np.array(X))[3]
     def f5(X): return ObjectivesDirections[4]*Fitness(np.array(X))[4]
     def f6(X): return ObjectivesDirections[5]*Fitness(np.array(X))[5]
 
     my_list_of_functions = [f1, f2, f3, f4, f5, f6]
 
     parameters = dict()
-    parameters['verbose'] = False
+    parameters['verbose'] = show_log
 
     for key in AlgOptions:
 
         if key == 'epoch':
             parameters['generations'] = AlgOptions[key]
+
         elif key == 'show_log':
             parameters['verbose'] = AlgOptions[key]
+
         else:
             parameters[key] = AlgOptions[key]
 
     parameters['min_values'] = (0,)*ToTalVariableCounter[1]
     parameters['max_values'] = (1,)*ToTalVariableCounter[1]
 
     list_of_functions = []
     list_of_directions = ObjectivesDirections
 
     for i in range(len(ObjectivesDirections)):
 
         list_of_functions.append(my_list_of_functions[i])
 
-
     match solver_name:
 
         case "c-ns-ga-ii":
 
             from pyMultiobjective.algorithm import clustered_non_dominated_sorting_genetic_algorithm_II
             solver = clustered_non_dominated_sorting_genetic_algorithm_II
 
@@ -136,9 +136,8 @@
             from pyMultiobjective.algorithm import unified_non_dominated_sorting_genetic_algorithm_III
             solver = unified_non_dominated_sorting_genetic_algorithm_III
 
     time_solve_begin = timeit.default_timer()
     sol = solver(list_of_functions=list_of_functions, **parameters)
     time_solve_end = timeit.default_timer()
 
-   
     return sol[:, :ToTalVariableCounter[1]], list_of_directions*sol[:, ToTalVariableCounter[1]:], time_solve_begin, time_solve_end
```

### Comparing `feloopy-0.2.5/feloopy/generators/solution/pyomo_solution_generator.py` & `feloopy-0.2.6/feloopy/generators/solution/pyomo_solution_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -113,19 +113,26 @@
                     model_object.OBJ = pyomo_interface.Objective(
                         expr=model_objectives[objective_id], sense=pyomo_interface.minimize)
 
                 case "max":
                     model_object.OBJ = pyomo_interface.Objective(
                         expr=model_objectives[objective_id], sense=pyomo_interface.maximize)
 
-            model_object.constraint = pyomo_interface.ConstraintList()
-
-            for element in model_constraints:
-
-                model_object.constraint.add(expr=element)
+            if len(model_constraints)!=0:
+                if constraint_labels[0]==None:
+                    model_object.constraint = pyomo_interface.ConstraintList()
+                    for element in model_constraints:
+                        model_object.constraint.add(expr=element)
+                else:         
+                    model_object.dual = pyomo_interface.Suffix(direction=pyomo_interface.Suffix.IMPORT)
+                    model_object.c = pyomo_interface.Constraint(pyomo_interface.Any)
+                    counter=0
+                    for element in model_constraints:
+                        model_object.c[constraint_labels[counter]] = element
+                        counter+=1
 
             if 'online' not in solver_name:
 
                 if solver_name not in pyomo_offline_solver_selector.keys():
 
                     raise RuntimeError(
                         "Using solver '%s' is not supported by 'pyomo'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
```

### Comparing `feloopy-0.2.5/feloopy/generators/solution/xpress_solution_generator.py` & `feloopy-0.2.6/feloopy/generators/solution/linopy_solution_generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,18 +4,24 @@
  # @ Modified: 2023-05-12
  # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
-import xpress as xpress_interface
+from linopy import Model as LINOPYMODEL
+from linopy import LinearExpression
 import timeit
 
-xpress_solver_selector = {'xpress': 'xpress'}
+linopy_solver_selector = {'cbc': 'cbc',
+                          'glpk': 'glpk',
+                          'highs': 'highs',
+                          'gurobi': 'gurobi',
+                          'xpress': 'xpress',
+                          'cplex': 'cplex'}
 
 
 def generate_solution(features):
 
     model_object = features['model_object_before_solve']
     model_objectives = features['objectives']
     model_constraints = features['constraints']
@@ -31,34 +37,33 @@
     log = features['log']
     save = features['save_solver_log']
     save_model = features['write_model_file']
     email = features['email_address']
     max_iterations = features['max_iterations']
     solver_options = features['solver_options']
 
-    if solver_name not in xpress_solver_selector.keys():
+    if solver_name not in linopy_solver_selector.keys():
         raise RuntimeError(
-            "Using solver '%s' is not supported by 'xpress'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
+            "Using solver '%s' is not supported by 'linopy'! \nPossible fixes: \n1) Check the solver name. \n2) Use another interface. \n" % (solver_name))
 
     match debug:
 
         case False:
 
-            for constraint in model_constraints:
-                model_object.addConstraint(constraint)
-
             match directions[objective_id]:
-
                 case "min":
-                    model_object.setObjective(
-                        model_objectives[objective_id], sense=xpress_interface.minimize)
-
+                    print(model_objectives[objective_id])
+                    print(type(model_objectives[objective_id]))
+                    model_object.add_objective(model_objectives[objective_id])
+                    
                 case "max":
-                    model_object.setObjective(
-                        model_objectives[objective_id], sense=xpress_interface.maximize)
+                    model_object.add_objective(-1*model_objectives[objective_id])
+
+            for constraint in model_constraints:
+                model_object.add_constraint(constraint)
 
             time_solve_begin = timeit.default_timer()
-            result = model_object.solve()
+            result = model_object.solve(solver_name=solver_name)
             time_solve_end = timeit.default_timer()
             generated_solution = [result, [time_solve_begin, time_solve_end]]
 
     return generated_solution
```

### Comparing `feloopy-0.2.5/feloopy/generators/solution_generator.py` & `feloopy-0.2.6/feloopy/generators/solution_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,16 +64,20 @@
             from .solution import pymprog_solution_generator
             ModelSolution = pymprog_solution_generator.generate_solution(
                 features)
 
         case 'cplex':
 
             from .solution import cplex_solution_generator
-            ModelSolution = cplex_solution_generator.generate_solution(
-                features)
+            ModelSolution = cplex_solution_generator.generate_solution(features)
+            
+        case 'localsolver':
+
+            from .solution import localsolver_solution_generator
+            ModelSolution = localsolver_solution_generator.generate_solution(features)
 
         case 'cplex_cp':
 
             from .solution import cplex_cp_solution_generator
             ModelSolution = cplex_cp_solution_generator.generate_solution(
                 features)
 
@@ -96,8 +100,20 @@
 
         case 'linopy':
 
             from .solution import linopy_solution_generator
             ModelSolution = linopy_solution_generator.generate_solution(
                 features)
 
+        case 'rsome_ro':
+
+            from .solution import rsome_ro_solution_generator
+            ModelSolution = rsome_ro_solution_generator.generate_solution(
+                features)
+
+        case 'rsome_dro':
+
+            from .solution import rsome_dro_solution_generator
+            ModelSolution = rsome_dro_solution_generator.generate_solution(
+                features)
+                     
     return ModelSolution
```

### Comparing `feloopy-0.2.5/feloopy/generators/variable/cplex_cp_variable_generator.py` & `feloopy-0.2.6/feloopy/generators/variable/cplex_cp_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/generators/variable/cplex_variable_generator.py` & `feloopy-0.2.6/feloopy/generators/variable/cplex_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/generators/variable/cvxpy_variable_generator.py` & `feloopy-0.2.6/feloopy/generators/variable/cvxpy_variable_generator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,231 +1,87 @@
 '''
  # @ Author: Keivan Tafakkori
  # @ Created: 2023-05-11
- # @ Modified: 2023-05-12
+ # @ Modified: 2023-06-05
  # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
 import cvxpy as cvxpy_interface
 import itertools as it
 import warnings
 warnings.filterwarnings("ignore")
 
 sets = it.product
-
 VariableGenerator = cvxpy_interface.Variable
 
-
 def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
 
     match variable_type:
-
         case 'pvar':
-
-            '''
-
-            Positive Variable Generator
-
-
-            '''
-
             if variable_dim == 0:
-
-                generated_variable = VariableGenerator(
-                    1, integer=False,  nonneg=True, name=variable_name)
-
+                generated_variable = VariableGenerator(1, integer=False, nonneg=True, name=variable_name)
             else:
-
                 if len(variable_dim) == 1:
-
-                    generated_variable = {key: VariableGenerator(
-                        1, integer=False,  nonneg=True, name=f"{variable_name}{key}") for key in variable_dim[0]}
-
+                    generated_variable = {key: VariableGenerator(1, integer=False, nonneg=True, name=f"{variable_name}_{key}") for key in variable_dim[0]}
                 else:
-
-                    generated_variable = {key: VariableGenerator(
-                        1, integer=False,  nonneg=True, name=f"{variable_name}{key}") for key in sets(*variable_dim)}
+                    generated_variable = {key: VariableGenerator(1, integer=False, nonneg=True, name=f"{variable_name}_{key}") for key in sets(*variable_dim)}
 
         case 'bvar':
-
-            '''
-
-            Binary Variable Generator
-
-
-            '''
-
             if variable_dim == 0:
-
-                generated_variable = VariableGenerator(
-                    1,  nonneg=True, integer=True, name=variable_name)
-
+                generated_variable = VariableGenerator(1, nonneg=True, integer=True, name=variable_name)
             else:
-
                 if len(variable_dim) == 1:
-
-                    generated_variable = {key: VariableGenerator(
-                        1, integer=True, nonneg=True, name=f"{variable_name}{key}") for key in variable_dim[0]}
-
+                    generated_variable = {key: VariableGenerator(1, integer=True, nonneg=True, name=f"{variable_name}_{key}") for key in variable_dim[0]}
                 else:
-
-                    generated_variable = {key: VariableGenerator(
-                        1, integer=True, nonneg=True, name=f"{variable_name}{key}") for key in sets(*variable_dim)}
+                    generated_variable = {key: VariableGenerator(1, integer=True, nonneg=True, name=f"{variable_name}_{key}") for key in sets(*variable_dim)}
 
         case 'ivar':
-
-            '''
-
-            Integer Variable Generator
-
-
-            '''
-
             if variable_dim == 0:
-
-                generated_variable = VariableGenerator(
-                    1,  nonneg=True, integer=True, name=variable_name)
-
+                generated_variable = VariableGenerator(1, nonneg=True, integer=True, name=variable_name)
             else:
-
                 if len(variable_dim) == 1:
-
-                    generated_variable = {key: VariableGenerator(
-                        1,  nonneg=True, integer=True, name=f"{variable_name}{key}") for key in variable_dim[0]}
-
+                    generated_variable = {key: VariableGenerator(1, nonneg=True, integer=True, name=f"{variable_name}_{key}") for key in variable_dim[0]}
                 else:
-
-                    generated_variable = {key: VariableGenerator(
-                        1,  nonneg=True, integer=True, name=f"{variable_name}{key}") for key in sets(*variable_dim)}
+                    generated_variable = {key: VariableGenerator(1, nonneg=True, integer=True, name=f"{variable_name}_{key}") for key in sets(*variable_dim)}
 
         case 'fvar':
-
-            '''
-
-            Free Variable Generator
-
-
-            '''
-
             if variable_dim == 0:
-
-                generated_variable = VariableGenerator(
-                    1, integer=False,  nonneg=False, name=variable_name)
-
+                generated_variable = VariableGenerator(1, integer=False, nonneg=False, name=variable_name)
             else:
-
                 if len(variable_dim) == 1:
-
-                    generated_variable = {key: VariableGenerator(
-                        1, integer=False,  nonneg=False, name=f"{variable_name}{key}") for key in variable_dim[0]}
-
+                    generated_variable = {key: VariableGenerator(1, integer=False, nonneg=False, name=f"{variable_name}_{key}") for key in variable_dim[0]}
                 else:
-
-                    generated_variable = {key: VariableGenerator(
-                        1, integer=False,  nonneg=False, name=f"{variable_name}{key}") for key in sets(*variable_dim)}
+                    generated_variable = {key: VariableGenerator(1, integer=False, nonneg=False, name=f"{variable_name}_{key}") for key in sets(*variable_dim)}
 
         case 'ftvar':
 
-            '''
-
-            Free Tensor Variable Generator
-
-            '''
-
             if variable_dim == 0:
-
-                generated_variable = VariableGenerator(
-                    1, integer=False, name=variable_name)
-
+                generated_variable = VariableGenerator(1, integer=False, nonneg=False, name=variable_name)
             else:
-
-                if len(variable_dim) == 1:
-
-                    generated_variable = VariableGenerator(
-                        len(variable_dim[0]), integer=False, name=variable_name)
-
-                if len(variable_dim) == 2:
-
-                    generated_variable = VariableGenerator(
-                        len(variable_dim[0]), len(variable_dim[1]), integer=False)
+                dims = tuple(len(dim) for dim in variable_dim)
+                generated_variable = VariableGenerator(dims, integer=False, name=variable_name)
 
         case 'ptvar':
-
-            '''
-
-            Positive Tensor Variable Generator
-
-            '''
-
-            if variable_dim == 0:
-
-                generated_variable = VariableGenerator(
-                    1, integer=False,  nonneg=True, name=variable_name)
-
+            if variable_dim ==0:
+                generated_variable = VariableGenerator(1, integer=False, nonneg=True, name=variable_name)
             else:
-
-                if len(variable_dim) == 1:
-
-                    generated_variable = VariableGenerator(
-                        len(variable_dim[0]), integer=False,  nonneg=True, name=variable_name)
-
-                if len(variable_dim) == 2:
-
-                    generated_variable = VariableGenerator(len(variable_dim[0]), len(
-                        variable_dim[1]), integer=False,  nonneg=True, name=variable_name)
+                dims = tuple(len(dim) for dim in variable_dim)
+                generated_variable = VariableGenerator(dims, integer=False, nonneg=True, name=variable_name)
 
         case 'itvar':
-
-            '''
-
-            Integer Tensor Variable Generator
-
-            '''
-
-            if variable_dim == 0:
-
-                generated_variable = VariableGenerator(
-                    1, integer=True,  nonneg=True, name=variable_name)
-
+            if variable_dim ==0:
+                generated_variable = VariableGenerator(1, nonneg=True, integer=True, name=variable_name)
             else:
-
-                if len(variable_dim) == 1:
-
-                    generated_variable = VariableGenerator(
-                        len(variable_dim[0]), integer=True,  nonneg=True, name=variable_name)
-
-                if len(variable_dim) == 2:
-
-                    generated_variable = VariableGenerator(len(variable_dim[0]), len(
-                        variable_dim[1]), integer=True,  nonneg=True, name=variable_name)
+                dims = tuple(len(dim) for dim in variable_dim)
+                generated_variable = VariableGenerator(dims, integer=True, nonneg=True, name=variable_name)
 
         case 'btvar':
-
-            '''
-
-            Binary Tensor Variable Generator
-
-            '''
-
-            if variable_dim == 0:
-
-                generated_variable = VariableGenerator(
-                    1, integer=True,  nonneg=True, name=variable_name)
-
+            if variable_dim ==0:
+                generated_variable = VariableGenerator(1, nonneg=True, integer=True, name=variable_name)
             else:
-
-                if len(variable_dim) == 1:
-
-                    print('i am here', len(variable_dim[0]))
-
-                    generated_variable = VariableGenerator(
-                        len(variable_dim[0]), integer=True,  nonneg=True, name=variable_name)
-
-                if len(variable_dim) == 2:
-
-                    generated_variable = VariableGenerator(len(variable_dim[0]), len(
-                        variable_dim[1]), integer=True,  nonneg=True, name=variable_name)
+                dims = tuple(len(dim) for dim in variable_dim)
+                generated_variable = VariableGenerator(dims, integer=True, nonneg=True, name=variable_name)
 
     return generated_variable
```

### Comparing `feloopy-0.2.5/feloopy/generators/variable/cylp_variable_generator.py` & `feloopy-0.2.6/feloopy/generators/variable/cylp_variable_generator.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,78 +23,89 @@
 
             Positive Variable Generator
 
 
             '''
 
             if variable_dim == 0:
-                GeneratedVariable = model_object.addVariable(
+                generated_variable = model_object.addVariable(
                     variable_name, 1, isInt=False)
             else:
                 if len(variable_dim) == 1:
-                    GeneratedVariable = {key: model_object.addVariable(
+                    generated_variable = {key: model_object.addVariable(
                         f"{variable_name}{key}", 1, isInt=False) for key in variable_dim[0]}
                 else:
-                    GeneratedVariable = {key: model_object.addVariable(
+                    generated_variable = {key: model_object.addVariable(
                         f"{variable_name}{key}", 1, isInt=False) for key in it.product(*variable_dim)}
 
         case 'bvar':
 
             '''
 
             Binary Variable Generator
 
 
             '''
 
             if variable_dim == 0:
-                GeneratedVariable = model_object.addVariable(
+                generated_variable = model_object.addVariable(
                     variable_name, 0, isInt=False)
             else:
                 if len(variable_dim) == 1:
-                    GeneratedVariable = {key: model_object.addVariable(
+                    generated_variable = {key: model_object.addVariable(
                         f"{variable_name}{key}", 1, isInt=True) for key in variable_dim[0]}
                 else:
-                    GeneratedVariable = {key: model_object.addVariable(
+                    generated_variable = {key: model_object.addVariable(
                         f"{variable_name}{key}", 1, isInt=True) for key in it.product(*variable_dim)}
 
         case 'ivar':
 
             '''
 
             Integer Variable Generator
 
 
             '''
 
             if variable_dim == 0:
-                GeneratedVariable = model_object.addVariable(
+                generated_variable = model_object.addVariable(
                     variable_name, 1, isInt=False)
             else:
                 if len(variable_dim) == 1:
-                    GeneratedVariable = {key: model_object.addVariable(
+                    generated_variable = {key: model_object.addVariable(
                         f"{variable_name}{key}", 1, isInt=True) for key in variable_dim[0]}
                 else:
-                    GeneratedVariable = {key: model_object.addVariable(
+                    generated_variable = {key: model_object.addVariable(
                         f"{variable_name}{key}", 1, isInt=True) for key in it.product(*variable_dim)}
 
         case 'fvar':
 
             '''
 
             Free Variable Generator
 
 
             '''
 
             if variable_dim == 0:
-                GeneratedVariable = model_object.addVariable(
+                generated_variable = model_object.addVariable(
                     variable_name, 1, isInt=False)
             else:
                 if len(variable_dim) == 1:
-                    GeneratedVariable = {key: model_object.addVariable(
+                    generated_variable = {key: model_object.addVariable(
                         f"{variable_name}{key}", 1, isInt=False) for key in variable_dim[0]}
                 else:
-                    GeneratedVariable = {key: model_object.addVariable(
+                    generated_variable = {key: model_object.addVariable(
                         f"{variable_name}{key}", 1, isInt=False) for key in it.product(*variable_dim)}
 
-    return GeneratedVariable
+    
+    if variable_bound[0] is not None and variable_bound[1] is not None and len(variable_bound) == 2:
+        lb, ub = variable_bound
+        if isinstance(generated_variable, dict):
+            for key in generated_variable:
+                model_object.setLowerBounds(generated_variable[key], lb)
+                model_object.setUpperBounds(generated_variable[key], ub)
+        else:
+            model_object.setLowerBounds(generated_variable, lb)
+            model_object.setUpperBounds(generated_variable, ub)
+    
+    return generated_variable
```

### Comparing `feloopy-0.2.5/feloopy/generators/variable/gekko_variable_generator.py` & `feloopy-0.2.6/feloopy/generators/variable/mip_variable_generator.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,18 +4,24 @@
  # @ Modified: 2023-05-12
  # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
+import mip as mip_interface
 import itertools as it
 
 sets = it.product
 
+BINARY = mip_interface.BINARY
+POSITIVE = mip_interface.CONTINUOUS
+INTEGER = mip_interface.INTEGER
+FREE = mip_interface.CONTINUOUS
+
 
 def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
 
     match variable_type:
 
         case 'pvar':
 
@@ -23,77 +29,73 @@
 
             Positive Variable Generator
 
 
             '''
 
             if variable_dim == 0:
-                GeneratedVariable = model_object.Var(
-                    lb=variable_bound[0], ub=variable_bound[1], integer=False)
+                GeneratedVariable = model_object.add_var(var_type=POSITIVE)
             else:
                 if len(variable_dim) == 1:
-                    GeneratedVariable = {key:  model_object.Var(
-                        lb=variable_bound[0], ub=variable_bound[1], integer=False) for key in variable_dim[0]}
+                    GeneratedVariable = {key: model_object.add_var(
+                        var_type=POSITIVE) for key in variable_dim[0]}
                 else:
-                    GeneratedVariable = {key: model_object.Var(
-                        lb=variable_bound[0], ub=variable_bound[1], integer=False) for key in sets(*variable_dim)}
+                    GeneratedVariable = {key: model_object.add_var(
+                        var_type=POSITIVE) for key in it.product(*variable_dim)}
 
         case 'bvar':
 
             '''
 
             Binary Variable Generator
 
 
             '''
 
             if variable_dim == 0:
-                GeneratedVariable = model_object.Var(
-                    lb=variable_bound[0], ub=variable_bound[1], integer=True)
+                GeneratedVariable = model_object.add_var(var_type=BINARY)
             else:
                 if len(variable_dim) == 1:
-                    GeneratedVariable = {key:  model_object.Var(
-                        lb=0, ub=1, integer=True) for key in variable_dim[0]}
+                    GeneratedVariable = {key: model_object.add_var(
+                        var_type=BINARY) for key in variable_dim[0]}
                 else:
-                    GeneratedVariable = {key: model_object.Var(
-                        lb=0, ub=1, integer=True) for key in sets(*variable_dim)}
+                    GeneratedVariable = {key: model_object.add_var(
+                        var_type=BINARY) for key in it.product(*variable_dim)}
 
         case 'ivar':
 
             '''
 
             Integer Variable Generator
 
 
             '''
 
             if variable_dim == 0:
-                GeneratedVariable = model_object.Var(
-                    lb=variable_bound[0], ub=variable_bound[1], integer=True)
+                GeneratedVariable = model_object.add_var(var_type=INTEGER)
             else:
                 if len(variable_dim) == 1:
-                    GeneratedVariable = {key:  model_object.Var(
-                        lb=variable_bound[0], ub=variable_bound[1], integer=True) for key in variable_dim[0]}
+                    GeneratedVariable = {key: model_object.add_var(
+                        var_type=INTEGER) for key in variable_dim[0]}
                 else:
-                    GeneratedVariable = {key: model_object.Var(
-                        lb=variable_bound[0], ub=variable_bound[1], integer=True) for key in sets(*variable_dim)}
+                    GeneratedVariable = {key: model_object.add_var(
+                        var_type=INTEGER) for key in it.product(*variable_dim)}
 
         case 'fvar':
 
             '''
 
             Free Variable Generator
 
 
             '''
-
             if variable_dim == 0:
-                GeneratedVariable = model_object.Var()
+                GeneratedVariable = model_object.add_var(var_type=POSITIVE)
             else:
                 if len(variable_dim) == 1:
-                    GeneratedVariable = {key:  model_object.Var()
-                                         for key in variable_dim[0]}
+                    GeneratedVariable = {key: model_object.add_var(
+                        var_type=POSITIVE) for key in variable_dim[0]}
                 else:
-                    GeneratedVariable = {key: model_object.Var()
-                                         for key in sets(*variable_dim)}
+                    GeneratedVariable = {key: model_object.add_var(
+                        var_type=POSITIVE) for key in it.product(*variable_dim)}
 
     return GeneratedVariable
```

### Comparing `feloopy-0.2.5/feloopy/generators/variable/gurobi_variable_generator.py` & `feloopy-0.2.6/feloopy/generators/variable/gurobi_variable_generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,21 +28,14 @@
     if variable_bound[1] == None:
         variable_bound[1] = +INFINITY
 
     match variable_type:
 
         case 'pvar':
 
-            '''
-
-            Positive Variable Generator
-
-
-            '''
-
             if variable_dim == 0:
 
                 generated_variable = model_object.addVar(
                     vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
 
             else:
 
@@ -54,21 +47,14 @@
                 else:
 
                     generated_variable = {key: model_object.addVar(
                         vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in sets(*variable_dim)}
 
         case 'bvar':
 
-            '''
-
-            Binary Variable Generator
-
-
-            '''
-
             if variable_dim == 0:
 
                 generated_variable = model_object.addVar(
                     vtype=BINARY, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
 
             else:
 
@@ -80,21 +66,14 @@
                 else:
 
                     generated_variable = {key: model_object.addVar(
                         vtype=BINARY, lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in sets(*variable_dim)}
 
         case 'ivar':
 
-            '''
-
-            Integer Variable Generator
-
-
-            '''
-
             if variable_dim == 0:
 
                 generated_variable = model_object.addVar(
                     vtype=INTEGER, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
 
             else:
 
@@ -106,21 +85,14 @@
                 else:
 
                     generated_variable = {key: model_object.addVar(
                         vtype=INTEGER, lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in sets(*variable_dim)}
 
         case 'fvar':
 
-            '''
-
-            Free Variable Generator
-
-
-            '''
-
             if variable_dim == 0:
 
                 generated_variable = model_object.addVar(
                     vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
 
             else:
 
@@ -132,19 +104,14 @@
                 else:
 
                     generated_variable = {key: model_object.addVar(
                         vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=f"{variable_name}{key}") for key in sets(*variable_dim)}
 
         case 'ptvar':
 
-            '''
-
-            Positive Tensor Variable Generator
-
-            '''
 
             if variable_dim == 0:
 
                 generated_variable = model_object.addVar(
                     vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
 
             else:
@@ -162,19 +129,14 @@
                 else:
 
                     generated_variable = model_object.addMVar(tuple(
                         [len(key) for key in variable_dim]), vtype=POSITIVE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
 
         case 'ftvar':
 
-            '''
-
-            Free Tensor Variable Generator
-
-            '''
 
             if variable_dim == 0:
                 generated_variable = model_object.addVar(
                     vtype=FREE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
 
             else:
 
@@ -186,21 +148,14 @@
                         variable_dim[1])), vtype=FREE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
                 else:
                     generated_variable = model_object.addMVar(tuple(
                         [len(key) for key in variable_dim]), vtype=FREE, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
 
         case 'btvar':
 
-            '''
-
-            Binary Tensor Variable Generator
-
-
-            '''
-
             if variable_dim == 0:
                 generated_variable = model_object.addVar(
                     vtype=BINARY, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
 
             else:
 
                 if len(variable_dim) == 1:
@@ -211,19 +166,14 @@
                         variable_dim[1])), vtype=BINARY, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
                 else:
                     generated_variable = model_object.addMVar(tuple(
                         [len(key) for key in variable_dim]), vtype=BINARY, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
 
         case 'itvar':
 
-            '''
-
-            Integer Tensor Variable Generator
-
-            '''
 
             if variable_dim == 0:
                 generated_variable = model_object.addVar(
                     vtype=INTEGER, lb=variable_bound[0], ub=variable_bound[1], name=variable_name)
 
             else:
```

### Comparing `feloopy-0.2.5/feloopy/generators/variable/linopy_variable_generator.py` & `feloopy-0.2.6/feloopy/generators/variable/localsolver_variable_generator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,56 @@
-'''
- # @ Author: Keivan Tafakkori
- # @ Created: 2023-05-11
- # @ Modified: 2023-05-12
- # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
- # @ Github: https://github.com/ktafakkori
- # @ Website: https://ktafakkori.github.io/
- # @ Copyright: 2023. MIT License. All Rights Reserved.
- '''
-
+import localsolver as ls
 import itertools as it
-import pandas as pd
 
 sets = it.product
 
-
 def generate_variable(model_object, variable_type, variable_name, variable_bound, variable_dim=0):
-
     match variable_type:
-
         case 'pvar':
-
             '''
-
             Positive Variable Generator
-
-
             '''
             if variable_dim == 0:
-                GeneratedVariable = model_object.add_variables(
-                    lower=variable_bound[0], upper=variable_bound[1], name=variable_name)
+                GeneratedVariable = model_object.Float(
+                    variable_bound[0], variable_bound[1], name=variable_name)
             else:
-                GeneratedVariable = model_object.add_variables(
-                    lower=variable_bound[0], upper=variable_bound[1], coords=pd.Index(variable_dim), name=variable_name)
-
+                GeneratedVariable = generate_multi_dimensional_var(model_object, variable_bound, variable_name, variable_dim, 'Float')
+                
         case 'bvar':
-
             '''
-
             Binary Variable Generator
-
-
             '''
-
             if variable_dim == 0:
-                GeneratedVariable = model_object.add_variables(
-                    name=variable_name, binary=True)
+                GeneratedVariable = model_object.Bool(name=variable_name)
             else:
-                GeneratedVariable = model_object.add_variables(
-                    coords=pd.Index(variable_dim), name=variable_name,  binary=True)
+                GeneratedVariable = generate_multi_dimensional_var(model_object, variable_bound, variable_name, variable_dim, 'Bool')
 
         case 'ivar':
-
             '''
-
             Integer Variable Generator
-
-
             '''
-
             if variable_dim == 0:
-                GeneratedVariable = model_object.add_variables(
-                    lower=variable_bound[0], upper=variable_bound[1], name=variable_name, binary=True)
+                GeneratedVariable = model_object.Int(
+                    variable_bound[0], variable_bound[1], name=variable_name)
             else:
-                GeneratedVariable = model_object.add_variables(
-                    lower=variable_bound[0], upper=variable_bound[1], coords=pd.Index(variable_dim), name=variable_name,  integer=True)
+                GeneratedVariable = generate_multi_dimensional_var(model_object, variable_bound, variable_name, variable_dim, 'Int')
 
         case 'fvar':
-
             '''
-
             Free Variable Generator
-
-
             '''
-
             if variable_dim == 0:
-                GeneratedVariable = model_object.add_variables(
-                    lower=variable_bound[0], upper=variable_bound[1], name=variable_name)
+                GeneratedVariable = model_object.Float(
+                    variable_bound[0], variable_bound[1], name=variable_name)
             else:
-                GeneratedVariable = model_object.add_variables(
-                    lower=variable_bound[0], upper=variable_bound[1], coords=pd.Index(variable_dim), name=variable_name)
+                GeneratedVariable = generate_multi_dimensional_var(model_object, variable_bound, variable_name, variable_dim, 'Float')
+
+    return GeneratedVariable
 
+def generate_multi_dimensional_var(model_object, variable_bound, variable_name, variable_dim, var_type):
+    if len(variable_dim) == 1:
+        GeneratedVariable = {key: getattr(model_object, var_type)(
+            variable_bound[0], variable_bound[1], name=f"{variable_name}{key}") for key in variable_dim[0]}
+    else:
+        GeneratedVariable = {key: getattr(model_object, var_type)(
+            variable_bound[0], variable_bound[1], name=f"{variable_name}{key}") for key in sets(*variable_dim)}
     return GeneratedVariable
```

### Comparing `feloopy-0.2.5/feloopy/generators/variable/ortools_cp_variable_generator.py` & `feloopy-0.2.6/feloopy/generators/variable/ortools_cp_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/generators/variable/ortools_variable_generator.py` & `feloopy-0.2.6/feloopy/generators/variable/ortools_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/generators/variable/picos_variable_generator.py` & `feloopy-0.2.6/feloopy/generators/variable/picos_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/generators/variable/pulp_variable_generator.py` & `feloopy-0.2.6/feloopy/generators/variable/pulp_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/generators/variable/pymprog_variable_generator.py` & `feloopy-0.2.6/feloopy/generators/variable/pymprog_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/generators/variable/pyomo_variable_generator.py` & `feloopy-0.2.6/feloopy/generators/variable/pyomo_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/generators/variable/xpress_variable_generator.py` & `feloopy-0.2.6/feloopy/generators/variable/xpress_variable_generator.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/generators/variable_generator.py` & `feloopy-0.2.6/feloopy/generators/variable_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,14 @@
  # @ Modified: 2023-05-12
  # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
-
 def generate_variable(interface_name, model_object, variable_type, variable_name, variable_bound, variable_dim):
 
     inputs = {'model_object': model_object,
               'variable_type': variable_type,
               'variable_name': variable_name,
               'variable_bound': variable_bound,
               'variable_dim': variable_dim}
@@ -65,14 +64,19 @@
             return pymprog_variable_generator.generate_variable(**inputs)
 
         case 'cplex':
 
             from .variable import cplex_variable_generator
             return cplex_variable_generator.generate_variable(**inputs)
 
+        case 'localsolver':
+
+            from .variable import localsolver_variable_generator
+            return localsolver_variable_generator.generate_variable(**inputs)
+        
         case 'cplex_cp':
 
             from .variable import cplex_cp_variable_generator
             return cplex_cp_variable_generator.generate_variable(**inputs)
 
         case 'gurobi':
 
@@ -89,7 +93,17 @@
             from .variable import mip_variable_generator
             return mip_variable_generator.generate_variable(**inputs)
 
         case 'linopy':
 
             from .variable import linopy_variable_generator
             return linopy_variable_generator.generate_variable(**inputs)
+
+        case 'rsome_ro':
+
+            from .variable import rsome_ro_variable_generator
+            return rsome_ro_variable_generator.generate_variable(**inputs)
+        
+        case 'rsome_dro':
+
+            from .variable import rsome_dro_variable_generator
+            return rsome_dro_variable_generator.generate_variable(**inputs)
```

### Comparing `feloopy-0.2.5/feloopy/helpers/empty.py` & `feloopy-0.2.6/feloopy/helpers/empty.py`

 * *Files identical despite different names*

### Comparing `feloopy-0.2.5/feloopy/operators/common.py` & `feloopy-0.2.6/feloopy/operators/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,19 +70,17 @@
 def log_of_base(input, base):
     return mt.log(input, base)
 
 
 def log(input):
     return np.log(input)
 
-
 def log10(input):
     return np.log10(input)
 
-
 def sqrt(input):
     return np.sqrt(input)
 
 
 def sin(input):
     return np.sin(input)
 
@@ -151,15 +149,14 @@
     sec %= 60
     if show:
         print("Elapsed time (microseconds):", (EndTime-StartTime)*10**6)
         print("Elapsed time (hour:min:sec):",
               "%02d:%02d:%02d" % (hour, min, sec))
     return EndTime
 
-
 def load_from_excel(data_file: str, data_dimension: list, shape: list, indices_list: None, sheet_name: str, path=None):
     '''
     Multi-Dimensional Excel Parameter Reader! 
     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     *data_file: Name of the dataset file (e.g., data.xlsx)
     *data_dimension: data_dimension of the dataset
```

### Comparing `feloopy-0.2.5/feloopy/operators/fix_operators.py` & `feloopy-0.2.6/feloopy/operators/set_operators.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,27 +4,23 @@
  # @ Modified: 2023-05-12
  # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
+import itertools as it
 
-def fix_dims(dim):
+def sets(*args):
+    """ 
+    Used to mimic 'for all' in mathamatical modeling, for multiple sets.
 
-    if dim == 0:
+    Arguments:
 
-        return dim
-    
-    if isinstance(dim, set):
+        * Multiple sets separated by commas.
+        * Required
 
-        return dim
+    Example: `for i,j in sets(I,J):`
 
-    elif dim != 0:
+    """
 
-        for i in range(len(dim)):
-
-            if type(dim[i]) != range:
-
-                dim[i] = range(dim[i])
-
-        return dim
+    return it.product(*args)
```

### Comparing `feloopy-0.2.5/feloopy/operators/update_operators.py` & `feloopy-0.2.6/feloopy/operators/update_operators.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,42 +4,43 @@
  # @ Modified: 2023-05-12
  # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
+import math as mt
 
-from .count_operators import *
+def product(iterable):
+    return mt.prod(iterable)
 
+def count_variable(variable_dim, total_count, special_count):
+    total_count[0] += 1
+    special_count[0] += 1
+    count = 1 if variable_dim == 0 else product(len(dims) for dims in variable_dim)
+    special_count[1] += count
+    total_count[1] += count
+    return total_count, special_count
 
 def update_variable_features(name, variable_dim, variable_bound, variable_counter_type, features):
-    """ For hierarchical updating the features of the problem.
-    """
-    match features['solution_method']:
-
-        case 'exact':
-
-            features['total_variable_counter'], features['variable_counter_type'] = count_variable(
-                variable_dim, features['total_variable_counter'], features[variable_counter_type])
-
-        case 'heuristic':
-
-            if features['agent_status'] == 'idle':
-
-                features['variable_spread'][name] = [
-                    features['total_variable_counter'][1], 0]
-                features['total_variable_counter'], features[variable_counter_type] = count_variable(
-                    variable_dim, features['total_variable_counter'], features[variable_counter_type])
-                features['variable_spread'][name][1] = features['total_variable_counter'][1]
-                if variable_counter_type == 'free_variable_counter':
-                    features['variable_type'][name] = 'fvar'
-                if variable_counter_type == 'binary_variable_counter':
-                    features['variable_type'][name] = 'bvar'
-                if variable_counter_type == 'integer_variable_counter':
-                    features['variable_type'][name] = 'ivar'
-                if variable_counter_type == 'positive_variable_counter':
-                    features['variable_type'][name] = 'pvar'
-                features['variable_bound'][name] = variable_bound
-                features['variable_dim'][name] = variable_dim
+    if features['solution_method'] == 'exact':
+        features['total_variable_counter'], features[variable_counter_type] = count_variable(variable_dim, features['total_variable_counter'], features[variable_counter_type])
 
-    return features
+    elif features['solution_method'] == 'heuristic' and features['agent_status'] == 'idle':
+
+        start_counter = features['total_variable_counter'][1]
+        
+        features['total_variable_counter'], features[variable_counter_type] = count_variable(variable_dim, features['total_variable_counter'], features[variable_counter_type])
+        end_counter = features['total_variable_counter'][1]
+
+        features['variable_spread'][name] = [start_counter, end_counter]
+        variable_type_mapping = {
+            'free_variable_counter': 'fvar',
+            'binary_variable_counter': 'bvar',
+            'integer_variable_counter': 'ivar',
+            'positive_variable_counter': 'pvar'
+        }
+        features['variable_type'][name] = variable_type_mapping[variable_counter_type]
+        features['variable_bound'][name] = variable_bound
+        features['variable_dim'][name] = variable_dim
+
+    return features
```

### Comparing `feloopy-0.2.5/feloopy.egg-info/PKG-INFO` & `feloopy-0.2.6/feloopy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feloopy
-Version: 0.2.5
+Version: 0.2.6
 Summary: FelooPy: An integrated optimization environment for automated operations research in Python.
 Home-page: https://github.com/ktafakkori/feloopy
 Download-URL: https://github.com/ktafakkori/feloopy/releases
 Author: Keivan Tafakkori
 Author-email: k.tafakkori@gmail.com
 Maintainer: Keivan Tafakkori
 Maintainer-email: k.tafakkori@gmail.com
@@ -17,18 +17,18 @@
 Provides-Extra: cplex
 Provides-Extra: xpress
 Provides-Extra: linux
 License-File: LICENSE
 
 ### **Introduction**
 
-| FelooPy                                            | [![version code](https://img.shields.io/badge/version-0.2.5-darkgreen.svg)](https://github.com/ktafakkori/feloopy/releases) [![number of users](https://static.pepy.tech/personalized-badge/feloopy?period=total&units=international_system&left_color=grey&right_color=darkgreen&left_text=users)](https://pepy.tech/project/feloopy) ![release date](https://img.shields.io/github/release-date/ktafakkori/feloopy?color=blue) [![monthly Downloads](https://static.pepy.tech/personalized-badge/feloopy?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20downloads%20)](https://pepy.tech/project/feloopy) [![license type](https://img.shields.io/badge/license-MIT-darkred.svg)](https://opensource.org/licenses/MIT) |
+| FelooPy                                            | [![version code](https://img.shields.io/badge/version-0.2.6-darkgreen.svg)](https://github.com/ktafakkori/feloopy/releases) [![number of users](https://static.pepy.tech/personalized-badge/feloopy?period=total&units=international_system&left_color=grey&right_color=darkgreen&left_text=users)](https://pepy.tech/project/feloopy) ![release date](https://img.shields.io/github/release-date/ktafakkori/feloopy?color=blue) [![monthly Downloads](https://static.pepy.tech/personalized-badge/feloopy?period=month&units=international_system&left_color=grey&right_color=blue&left_text=monthly%20downloads%20)](https://pepy.tech/project/feloopy) [![license type](https://img.shields.io/badge/license-MIT-darkred.svg)](https://opensource.org/licenses/MIT) |
 | :------------------------------------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | ![Image description](miscellaneous/logo/logo1.png) | FelooPy (pronounced /fɛlupaɪ/) is a free and open-source Python library for automated operations research that serves as both a hyper-optimization interface and an integrated optimization environment. The name comes from the idea of suggesting practical and applicable solutions for systems, industries, and supply chains, and it also references the importance of loops in programming and algorithm development, and draws similarities to the name "Floppy" to highlight memory efficiency. FelooPy helps operations research scientists achieve their goals using various target, representor, and learner models. In simple words, FelooPy is a unified framework for optimization algorithms, decision-making methods, and modeling and analytical tools. |
-| News                                               | 🎉 _Version 0.2.5 is out: Added new features!_ 🎉                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
+| News                                               | 🎉 _Version 0.2.6 is out: Robustness and stability!_ 🎉                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
 
 ### **Installation**
 
 FelooPy can be installed on Linux-based distributions, Windows, or macOS. It has a few dependencies that should work on all these platforms.
 
 <div align="center">
 
@@ -46,53 +46,53 @@
 <td> Python >= 3.10 </td>
 </tr>
 
 <tr>
 <td> PyPI </td>
 <td>
     
-`pip install feloopy==0.2.5`
+`pip install feloopy==0.2.6`
 </td>
 <td> Python >= 3.10 </td>
 </tr>
 
 <tr>
 <td> Command </td>
 <td>
     
-`!pip install feloopy==0.2.5`
+`!pip install feloopy==0.2.6`
 </td>
 <td> Python >= 3.10 </td>
 </tr>
 
 <tr>
 <td> Script </td>
 <td>
     
 ```python
 import pip
 
 def install(package):
-if hasattr(pip, 'main'):
-pip.main(['install','-U', package])
-else:
-pip._internal.main(['install','-U', package])
+  if hasattr(pip, 'main'):
+    pip.main(['install','-U', package])
+  else:
+    pip._internal.main(['install','-U', package])
 
-install('feloopy')
+install('feloopy==0.2.6')
 
 ````
 </td>
 <td> Python >= 3.10 </td>
 </tr>
 
 <tr>
 <td> Local </td>
 <td>
 
-1. Download the [feloopy-0.2.5.zip][c] file.
+1. Download the [feloopy-0.2.6.zip][c] file.
 2. Extract it into a specific directory.
 3. Open a terminal in that directory.
 4. Type: `pip install .`
 
 </td>
 
 <td> Python >= 3.10 </td>
@@ -110,15 +110,15 @@
 !bash ./py310.sh -b -f -p /usr/local
 !python -m ipykernel install --name "py310" --user
 ````
 
 2. Run this cell and reload (CTRL + R):
 
 ```python
-!pip install feloopy==0.2.5
+!pip install feloopy==0.2.6
 ```
 
 </td>
 
 <td> Python >= 3.10 </td>
 
 </tr>
@@ -143,42 +143,46 @@
 
 ```
 conda create --name feloopy python=3.10
 conda activate feloopy
 pip install feloopy
 ```
 
-FelooPy (v0.2.5) has a few optional dependencies that can be installed using the following commands:
+FelooPy (v0.2.6) has a few optional dependencies that can be installed using the following commands:
 
 * All solvers: `pip install feloopy[all_solvers]`
 * Gurobi: `pip install feloopy[gurobi]`
-* CPLEX: `pip install feloopy[cplex]`
-* XPRESS: `pip install feloopy[xpress]`
-* Linux: `pip install feloopy[linux]` (for multi-objective optimization)
+* Cplex: `pip install feloopy[cplex]`
+* Xpress: `pip install feloopy[xpress]`
+* Linux: `pip install feloopy[linux]` (better support for multi-objective optimization)
 
-For multi-objective optimization, you should use the linux command for installation. However, please note that the optional dependencies for Linux might not work on other operating systems. As a workaround, you can use a Conda-based Python 3.10 interpreter to ensure that optional dependencies for multi-objective optimization are installed correctly.
+For multi-objective optimization, you should use the linux command for installation. However, please note that the optional dependencies for Linux kernel might not work on some operating systems. As a workaround, you can use a Conda-based Python 3.10 interpreter to ensure that optional dependencies for multi-objective optimization are installed correctly.
 
 ### **Features**
 
 FelooPy offers the following key features:
 
 * **Simplest optimization programming language**: Designed to be easy to use, even for those with little or no programming experience.
 * **Modeling, solving and analyzing optimization problems**: Provides a complete suite of tools for modeling, solving and analyzing a wide range of optimization problems.
 * **Exact optimization algorithms**: Supports *107* exact optimization algorithms that guarantee the optimal solution to your problem.
 * **Heuristic optimization algorithms**: Supports *197* heuristic optimization algorithms that can find best possible solutions to complex problems.
 * **Convex optimization algorithms**: Supports *20* convex optimization algorithms that ease tensor- and matrix-form modeling, primarily for convex problems.
 * **Constraint optimization algorithms**: Supports *2* constraint optimization algorithms that can handle a wide range of complex constraints for operational and time-dependent decisions.
-* **Multi-objective optimization algorithms**: Supports *17* multi-objective optimization algorithms, in which objectives might be contradicting or with different numerical units.
+* **Multi-objective optimization algorithms**: Supports *17* multi-objective optimization algorithms, in which objectives might be conflicting or with different numerical units.
 * **Multi-critera decision-making methods**: Supports *41* MCDM algorithms to solve decision problems with expert-based inputs without mathematical modeling.
 * **Solver configurations**: Lets you configure the solver to meet specific requirements.
 * **Auto-encoders for general purpose programming**: Provides auto-encoders to simplify general-purpose programming tasks.
 * **Auto-linearizers for linear programming conversions**: Provides auto-linearizers that can handle mixed-integer non-linear programming problems.
 * **Auto-logic for modeling special constraints**: Provides auto-logic to help you model and solve problems with special constraints.
 * **Auto-sensitivity for analyzing the impact of key parameters**: Provides auto-sensitivity tools to help you analyze the impact of key parameters on your optimization problem.
 
+### **Documentation**
+
+Please refer to https://feloopy.readthedocs.io/en/latest/.
+
 ### **Contributions**
 
 We welcome your contributions to this project, such as reporting bugs, submitting pull requests, testing changes, providing examples, and so on.
 ### **Support FelooPy**
 
 We are committed to continuing the development of FelooPy and would greatly appreciate your support. You can help us by:
```

### Comparing `feloopy-0.2.5/feloopy.egg-info/SOURCES.txt` & `feloopy-0.2.6/feloopy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 feloopy.egg-info/SOURCES.txt
 feloopy.egg-info/dependency_links.txt
 feloopy.egg-info/requires.txt
 feloopy.egg-info/top_level.txt
 feloopy/algorithms/__init__.py
 feloopy/algorithms/constraint/__init__.py
 feloopy/algorithms/exact/__init__.py
+feloopy/algorithms/exact/benders.py
 feloopy/algorithms/heuristic/DE.py
 feloopy/algorithms/heuristic/GA.py
 feloopy/algorithms/heuristic/GWO.py
 feloopy/algorithms/heuristic/SA.py
 feloopy/algorithms/heuristic/TS.py
 feloopy/algorithms/heuristic/__init__.py
 feloopy/algorithms/mcdm/__init__.py
@@ -69,81 +70,93 @@
 feloopy/generators/model/cplex_model_generator.py
 feloopy/generators/model/cvxpy_model_generator.py
 feloopy/generators/model/cylp_model_generator.py
 feloopy/generators/model/feloopy_model_generator.py
 feloopy/generators/model/gekko_model_generator.py
 feloopy/generators/model/gurobi_model_generator.py
 feloopy/generators/model/linopy_model_generator.py
+feloopy/generators/model/localsolver_model_generator.py
 feloopy/generators/model/mealpy_model_generator.py
 feloopy/generators/model/mip_model_generator.py
 feloopy/generators/model/ortools_cp_model_generator.py
 feloopy/generators/model/ortools_model_generator.py
 feloopy/generators/model/picos_model_generator.py
 feloopy/generators/model/pulp_model_generator.py
 feloopy/generators/model/pymprog_model_generator.py
 feloopy/generators/model/pyomo_model_generator.py
+feloopy/generators/model/rsome_dro_model_generator.py
+feloopy/generators/model/rsome_ro_model_generator.py
 feloopy/generators/model/xpress_model_generator.py
 feloopy/generators/result/__init__.py
 feloopy/generators/result/cplex_cp_result_generator.py
 feloopy/generators/result/cplex_result_generator.py
 feloopy/generators/result/cvxpy_result_generator.py
 feloopy/generators/result/cylp_result_generator.py
 feloopy/generators/result/gekko_result_generator.py
 feloopy/generators/result/gurobi_result_generator.py
 feloopy/generators/result/linopy_result_generator.py
+feloopy/generators/result/localsolver_result_generator.py
 feloopy/generators/result/mip_result_generator.py
 feloopy/generators/result/ortools_cp_result_generator.py
 feloopy/generators/result/ortools_result_generator.py
 feloopy/generators/result/picos_result_generator.py
 feloopy/generators/result/pulp_result_generator.py
 feloopy/generators/result/pymprog_result_generator.py
 feloopy/generators/result/pyomo_result_generator.py
+feloopy/generators/result/rsome_dro_result_generator.py
+feloopy/generators/result/rsome_ro_result_generator.py
 feloopy/generators/result/xpress_result_generator.py
 feloopy/generators/solution/__init__.py
 feloopy/generators/solution/cplex_cp_solution_generator.py
 feloopy/generators/solution/cplex_solution_generator.py
 feloopy/generators/solution/cvxpy_solution_generator.py
 feloopy/generators/solution/cylp_solution_generator.py
 feloopy/generators/solution/feloopy_solution_generator.py
 feloopy/generators/solution/gekko_solution_generator.py
 feloopy/generators/solution/gurobi_solution_generator.py
 feloopy/generators/solution/linopy_solution_generator.py
+feloopy/generators/solution/localsolver_solution_generator.py
 feloopy/generators/solution/mealpy_solution_generator.py
 feloopy/generators/solution/mip_solution_generator.py
 feloopy/generators/solution/ortools_cp_solution_generator.py
 feloopy/generators/solution/ortools_solution_generator.py
 feloopy/generators/solution/picos_solution_generator.py
 feloopy/generators/solution/pulp_solution_generator.py
+feloopy/generators/solution/pymoo_solution_generator.py
 feloopy/generators/solution/pymprog_solution_generator.py
 feloopy/generators/solution/pymultiobjective_solution_generator.py
 feloopy/generators/solution/pyomo_solution_generator.py
+feloopy/generators/solution/rsome_dro_solution_generator.py
+feloopy/generators/solution/rsome_ro_solution_generator.py
 feloopy/generators/solution/xpress_solution_generator.py
 feloopy/generators/variable/__init__.py
 feloopy/generators/variable/cplex_cp_variable_generator.py
 feloopy/generators/variable/cplex_variable_generator.py
 feloopy/generators/variable/cvxpy_variable_generator.py
 feloopy/generators/variable/cylp_variable_generator.py
 feloopy/generators/variable/gekko_variable_generator.py
 feloopy/generators/variable/gurobi_variable_generator.py
 feloopy/generators/variable/linopy_variable_generator.py
+feloopy/generators/variable/localsolver_variable_generator.py
 feloopy/generators/variable/mip_variable_generator.py
 feloopy/generators/variable/ortools_cp_variable_generator.py
 feloopy/generators/variable/ortools_variable_generator.py
 feloopy/generators/variable/picos_variable_generator.py
 feloopy/generators/variable/pulp_variable_generator.py
 feloopy/generators/variable/pymprog_variable_generator.py
 feloopy/generators/variable/pyomo_variable_generator.py
+feloopy/generators/variable/rsome_dro_variable_generator.py
+feloopy/generators/variable/rsome_ro_variable_generator.py
 feloopy/generators/variable/xpress_variable_generator.py
 feloopy/helpers/__init__.py
 feloopy/helpers/empty.py
 feloopy/helpers/error.py
 feloopy/helpers/formatter.py
 feloopy/operators/__init__.py
 feloopy/operators/common.py
-feloopy/operators/count_operators.py
 feloopy/operators/epsilon.py
 feloopy/operators/exact.py
 feloopy/operators/fix_operators.py
 feloopy/operators/heuristic.py
 feloopy/operators/heuristic_operators.py
 feloopy/operators/math_operators.py
 feloopy/operators/metric_operators.py
```

### Comparing `feloopy-0.2.5/setup.py` & `feloopy-0.2.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,26 +4,23 @@
  # @ Modified: 2023-05-12
  # @ Contact: https://www.linkedin.com/in/keivan-tafakkori/
  # @ Github: https://github.com/ktafakkori
  # @ Website: https://ktafakkori.github.io/
  # @ Copyright: 2023. MIT License. All Rights Reserved.
  '''
 
-
 from setuptools import setup, find_packages
 
-common = ['tabulate', 'numpy', 'matplotlib',
-          'infix', 'pandas', 'openpyxl', 'numba', 'plotly']
-interfaces = ['gekko', 'ortools', 'pulp', 'pyomo', 'pymprog',
-              'picos', 'linopy', 'cvxpy', 'cylp', 'mip', 'mealpy', 'pyDecision']
+common = ['tabulate', 'numpy', 'matplotlib', 'infix', 'pandas', 'openpyxl', 'numba', 'plotly', 'psutil', 'py-cpuinfo', 'win-unicode-console']
+interfaces = ['gekko', 'ortools', 'pulp', 'pyomo', 'pymprog', 'picos', 'linopy', 'cvxpy', 'cylp<=0.91.5', 'mip', 'mealpy', 'pyDecision','rsome', 'pymoo']
 solvers = ['cplex', 'docplex', 'xpress', 'gurobipy']
 
 setup(
     name='feloopy',
-    version='0.2.5',
+    version='0.2.6',
     description='FelooPy: An integrated optimization environment for automated operations research in Python.',
     packages=find_packages(include=['feloopy', 'feloopy.*']),
     long_description=open('README.md', encoding="utf8").read(),
     long_description_content_type='text/markdown',
     keywords=['optimization', 'machine learning', 'simulation', 'operations research', 'computer science',
               'data science', 'management science', 'industrial engineering', 'supply chain', 'operations management'],
     author='Keivan Tafakkori',
```

