# Comparing `tmp/SELDOMpy-0.8.4.7.tar.gz` & `tmp/SELDOMpy-0.8.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SELDOMpy-0.8.4.7.tar", last modified: Thu Jul  6 09:25:07 2023, max compression
+gzip compressed data, was "dist\SELDOMpy-0.8.4.8.tar", last modified: Thu Jul  6 11:27:52 2023, max compression
```

## Comparing `SELDOMpy-0.8.4.7.tar` & `SELDOMpy-0.8.4.8.tar`

### file list

```diff
@@ -1,127 +1,132 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 09:25:07.952275 SELDOMpy-0.8.4.7/
--rw-rw-rw-   0        0        0    35149 2023-07-05 16:32:35.000000 SELDOMpy-0.8.4.7/LICENSE.txt
--rw-rw-rw-   0        0        0      284 2023-07-05 17:50:19.000000 SELDOMpy-0.8.4.7/MANIFEST.in
--rw-rw-rw-   0        0        0     4195 2023-07-06 09:25:07.952275 SELDOMpy-0.8.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     3446 2023-07-06 08:12:36.000000 SELDOMpy-0.8.4.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-06 09:25:07.812272 SELDOMpy-0.8.4.7/SELDOMpy/
--rw-rw-rw-   0        0        0    35149 2023-07-05 16:32:35.000000 SELDOMpy-0.8.4.7/SELDOMpy/LICENSE.txt
--rw-rw-rw-   0        0        0     3446 2023-07-06 08:12:36.000000 SELDOMpy-0.8.4.7/SELDOMpy/README.md
--rw-rw-rw-   0        0        0      390 2023-07-04 08:20:50.000000 SELDOMpy-0.8.4.7/SELDOMpy/__init__.py
--rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.8.4.7/SELDOMpy/buildmim.py
--rw-rw-rw-   0        0        0     1288 2023-07-04 08:20:50.000000 SELDOMpy-0.8.4.7/SELDOMpy/extras.py
--rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.8.4.7/SELDOMpy/gen_exps.py
--rw-rw-rw-   0        0        0     4838 2023-06-28 11:33:29.000000 SELDOMpy-0.8.4.7/SELDOMpy/getLBODEmodel.py
--rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.8.4.7/SELDOMpy/getRandomLBODEmodel.py
-drwxrwxrwx   0        0        0        0 2023-07-06 09:25:07.791292 SELDOMpy-0.8.4.7/SELDOMpy/include/
-drwxrwxrwx   0        0        0        0 2023-07-06 09:25:07.910276 SELDOMpy-0.8.4.7/SELDOMpy/include/include_amigo/
--rw-rw-rw-   0        0        0        4 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_amigo/AMIGO_hdf5.h
--rw-rw-rw-   0        0        0     3769 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_amigo/AMIGO_model.h
--rw-rw-rw-   0        0        0      442 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_amigo/AMIGO_model_stats.h
--rw-rw-rw-   0        0        0     1822 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_amigo/AMIGO_problem.h
--rw-rw-rw-   0        0        0      287 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_amigo/amigoJAC.h
--rw-rw-rw-   0        0        0       24 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_amigo/amigoRHS.h
--rw-rw-rw-   0        0        0      171 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_amigo/amigoSensRHS.h
--rw-rw-rw-   0        0        0      164 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_amigo/simulate_amigo_model.h
-drwxrwxrwx   0        0        0        0 2023-07-06 09:25:07.793322 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/
-drwxrwxrwx   0        0        0        0 2023-07-06 09:25:07.920274 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/
--rw-rw-rw-   0        0        0    84971 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes.h
--rw-rw-rw-   0        0        0     2442 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_band.h
--rw-rw-rw-   0        0        0     6547 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_bandpre.h
--rw-rw-rw-   0        0        0    13259 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_bbdpre.h
--rw-rw-rw-   0        0        0     2122 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_dense.h
--rw-rw-rw-   0        0        0     4845 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_diag.h
--rw-rw-rw-   0        0        0    14031 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_direct.h
--rw-rw-rw-   0        0        0     3732 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_lapack.h
--rw-rw-rw-   0        0        0     3061 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_spbcgs.h
--rw-rw-rw-   0        0        0     3021 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_spgmr.h
--rw-rw-rw-   0        0        0    18270 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_spils.h
--rw-rw-rw-   0        0        0     3085 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_sptfqmr.h
-drwxrwxrwx   0        0        0        0 2023-07-06 09:25:07.921275 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/nvector/
--rw-rw-rw-   0        0        0    10054 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/nvector/nvector_serial.h
-drwxrwxrwx   0        0        0        0 2023-07-06 09:25:07.934269 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/
--rw-rw-rw-   0        0        0     6539 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_band.h
--rw-rw-rw-   0        0        0     3157 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_config.h
--rw-rw-rw-   0        0        0     7865 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_dense.h
--rw-rw-rw-   0        0        0    13199 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_direct.h
--rw-rw-rw-   0        0        0     1129 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_fnvector.h
--rw-rw-rw-   0        0        0    13127 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_iterative.h
--rw-rw-rw-   0        0        0     4763 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_lapack.h
--rw-rw-rw-   0        0        0     4294 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_math.h
--rw-rw-rw-   0        0        0    15964 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_nvector.h
--rw-rw-rw-   0        0        0     7740 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_spbcgs.h
--rw-rw-rw-   0        0        0    12224 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_spgmr.h
--rw-rw-rw-   0        0        0    10246 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_sptfqmr.h
--rw-rw-rw-   0        0        0     3726 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_types.h
--rw-rw-rw-   0        0        0     2457 2023-07-06 09:18:42.000000 SELDOMpy-0.8.4.7/SELDOMpy/optimization.py
--rw-rw-rw-   0        0        0     1446 2023-07-06 08:30:16.000000 SELDOMpy-0.8.4.7/SELDOMpy/plot_results.py
--rw-rw-rw-   0        0        0     2524 2023-06-28 11:33:29.000000 SELDOMpy-0.8.4.7/SELDOMpy/reduce_fun.py
--rw-rw-rw-   0        0        0     4063 2023-06-28 11:33:29.000000 SELDOMpy-0.8.4.7/SELDOMpy/simulate_logic_based_ode.py
--rw-rw-rw-   0        0        0     3616 2023-06-28 11:33:29.000000 SELDOMpy-0.8.4.7/SELDOMpy/simulate_logic_based_ode_obs.py
-drwxrwxrwx   0        0        0        0 2023-07-06 09:25:07.946275 SELDOMpy-0.8.4.7/SELDOMpy/src/
--rw-rw-rw-   0        0        0    10952 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/AMIGO_model.c
--rw-rw-rw-   0        0        0      240 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/AMIGO_model_stats.c
--rw-rw-rw-   0        0        0     8027 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/AMIGO_problem.c
--rw-rw-rw-   0        0        0      811 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/CNOStructure.h
--rw-rw-rw-   0        0        0        0 2023-07-03 16:56:56.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/__init__.py
--rw-rw-rw-   0        0        0     3389 2023-04-10 15:09:09.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/anODEModel.c
--rw-rw-rw-   0        0        0    74908 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/cvodea.c
--rw-rw-rw-   0        0        0    18585 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/cvodea_io.c
--rw-rw-rw-   0        0        0   245647 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes.c
--rw-rw-rw-   0        0        0    13293 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_band.c
--rw-rw-rw-   0        0        0    16826 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_bandpre.c
--rw-rw-rw-   0        0        0     2272 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_bandpre_impl.h
--rw-rw-rw-   0        0        0    23592 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_bbdpre.c
--rw-rw-rw-   0        0        0     2929 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_bbdpre_impl.h
--rw-rw-rw-   0        0        0    12594 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_dense.c
--rw-rw-rw-   0        0        0    13921 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_diag.c
--rw-rw-rw-   0        0        0     2258 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_diag_impl.h
--rw-rw-rw-   0        0        0    20099 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_direct.c
--rw-rw-rw-   0        0        0     5473 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_direct_impl.h
--rw-rw-rw-   0        0        0    47504 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_impl.h
--rw-rw-rw-   0        0        0    41365 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_io.c
--rw-rw-rw-   0        0        0    16912 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_spbcgs.c
--rw-rw-rw-   0        0        0    17029 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_spgmr.c
--rw-rw-rw-   0        0        0    32809 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_spils.c
--rw-rw-rw-   0        0        0     6831 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_spils_impl.h
--rw-rw-rw-   0        0        0    17108 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_sptfqmr.c
--rw-rw-rw-   0        0        0      405 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/decimal2binary.c
--rw-rw-rw-   0        0        0     3792 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/dhc.c
--rw-rw-rw-   0        0        0      527 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/findStates.c
--rw-rw-rw-   0        0        0     3433 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/fnvector_serial.c
--rw-rw-rw-   0        0        0     2688 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/fnvector_serial.h
--rw-rw-rw-   0        0        0      693 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/getAdjacencyMatrix.c
--rw-rw-rw-   0        0        0      463 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/getNumBits.c
--rw-rw-rw-   0        0        0      475 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/getNumInputs.c
--rw-rw-rw-   0        0        0      695 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/getStateIndex.c
--rw-rw-rw-   0        0        0     3859 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/getTruthTables.c
--rw-rw-rw-   0        0        0      451 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/get_count_bits.c
--rw-rw-rw-   0        0        0      487 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/get_input_index.c
--rw-rw-rw-   0        0        0      594 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/get_support_truth_tables.c
--rw-rw-rw-   0        0        0      585 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/get_truth_tables_index.c
--rw-rw-rw-   0        0        0      224 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/hill_function.c
--rw-rw-rw-   0        0        0      219 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/linear_transfer_function.c
--rw-rw-rw-   0        0        0      227 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/normHill.c
--rw-rw-rw-   0        0        0    20778 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/nvector_serial.c
--rw-rw-rw-   0        0        0      305 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/printAdjMat.c
--rw-rw-rw-   0        0        0      315 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/printInterMat.c
--rw-rw-rw-   0        0        0      553 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/printNminiTerms.c
--rw-rw-rw-   0        0        0      410 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/printTruthTables.c
--rw-rw-rw-   0        0        0    15775 2023-04-28 16:16:22.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/sim_logic_ode.c
--rw-rw-rw-   0        0        0     9815 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/simulate_amigo_model.c
--rw-rw-rw-   0        0        0     6036 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/sundials_band.c
--rw-rw-rw-   0        0        0     8510 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/sundials_dense.c
--rw-rw-rw-   0        0        0     6225 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/sundials_direct.c
--rw-rw-rw-   0        0        0     7662 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/sundials_iterative.c
--rw-rw-rw-   0        0        0     2474 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/sundials_math.c
--rw-rw-rw-   0        0        0     4702 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/sundials_nvector.c
--rw-rw-rw-   0        0        0     9663 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/sundials_spbcgs.c
--rw-rw-rw-   0        0        0    12650 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/sundials_spgmr.c
--rw-rw-rw-   0        0        0    14744 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.7/SELDOMpy/src/sundials_sptfqmr.c
-drwxrwxrwx   0        0        0        0 2023-07-06 09:25:07.820260 SELDOMpy-0.8.4.7/SELDOMpy.egg-info/
--rw-rw-rw-   0        0        0     4195 2023-07-06 09:25:07.000000 SELDOMpy-0.8.4.7/SELDOMpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5606 2023-07-06 09:25:07.000000 SELDOMpy-0.8.4.7/SELDOMpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 09:25:07.000000 SELDOMpy-0.8.4.7/SELDOMpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-07-06 09:25:07.000000 SELDOMpy-0.8.4.7/SELDOMpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-06 09:25:07.000000 SELDOMpy-0.8.4.7/SELDOMpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-07-06 09:25:07.953275 SELDOMpy-0.8.4.7/setup.cfg
--rw-rw-rw-   0        0        0     3496 2023-07-06 09:25:05.000000 SELDOMpy-0.8.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 11:27:52.102156 SELDOMpy-0.8.4.8/
+-rw-rw-rw-   0        0        0    35149 2023-07-05 16:32:35.000000 SELDOMpy-0.8.4.8/LICENSE.txt
+-rw-rw-rw-   0        0        0      368 2023-07-06 11:26:53.000000 SELDOMpy-0.8.4.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     4195 2023-07-06 11:27:52.102156 SELDOMpy-0.8.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3446 2023-07-06 08:12:36.000000 SELDOMpy-0.8.4.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 11:27:51.957196 SELDOMpy-0.8.4.8/SELDOMpy/
+-rw-rw-rw-   0        0        0    35149 2023-07-05 16:32:35.000000 SELDOMpy-0.8.4.8/SELDOMpy/LICENSE.txt
+-rw-rw-rw-   0        0        0     3446 2023-07-06 08:12:36.000000 SELDOMpy-0.8.4.8/SELDOMpy/README.md
+-rw-rw-rw-   0        0        0      490 2023-07-06 11:23:03.000000 SELDOMpy-0.8.4.8/SELDOMpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 11:27:52.026155 SELDOMpy-0.8.4.8/SELDOMpy/functions/
+-rw-rw-rw-   0        0        0        0 2023-07-06 11:22:32.000000 SELDOMpy-0.8.4.8/SELDOMpy/functions/__init__.py
+-rw-rw-rw-   0        0        0     2309 2023-06-22 08:44:09.000000 SELDOMpy-0.8.4.8/SELDOMpy/functions/buildmim.py
+-rw-rw-rw-   0        0        0     1288 2023-07-04 08:20:50.000000 SELDOMpy-0.8.4.8/SELDOMpy/functions/extras.py
+-rw-rw-rw-   0        0        0     4159 2023-04-19 14:22:26.000000 SELDOMpy-0.8.4.8/SELDOMpy/functions/gen_exps.py
+-rw-rw-rw-   0        0        0     4848 2023-07-06 11:23:03.000000 SELDOMpy-0.8.4.8/SELDOMpy/functions/getLBODEmodel.py
+-rw-rw-rw-   0        0        0     3232 2023-04-24 18:45:26.000000 SELDOMpy-0.8.4.8/SELDOMpy/functions/getRandomLBODEmodel.py
+-rw-rw-rw-   0        0        0     2467 2023-07-06 11:23:03.000000 SELDOMpy-0.8.4.8/SELDOMpy/functions/optimization.py
+-rw-rw-rw-   0        0        0     1446 2023-07-06 08:30:16.000000 SELDOMpy-0.8.4.8/SELDOMpy/functions/plot_results.py
+-rw-rw-rw-   0        0        0     2534 2023-07-06 11:23:03.000000 SELDOMpy-0.8.4.8/SELDOMpy/functions/reduce_fun.py
+-rw-rw-rw-   0        0        0     4073 2023-07-06 11:23:03.000000 SELDOMpy-0.8.4.8/SELDOMpy/functions/simulate_logic_based_ode.py
+-rw-rw-rw-   0        0        0     3626 2023-07-06 11:23:03.000000 SELDOMpy-0.8.4.8/SELDOMpy/functions/simulate_logic_based_ode_obs.py
+drwxrwxrwx   0        0        0        0 2023-07-06 11:27:51.944163 SELDOMpy-0.8.4.8/SELDOMpy/include/
+drwxrwxrwx   0        0        0        0 2023-07-06 11:27:52.033161 SELDOMpy-0.8.4.8/SELDOMpy/include/include_amigo/
+-rw-rw-rw-   0        0        0        4 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_amigo/AMIGO_hdf5.h
+-rw-rw-rw-   0        0        0     3769 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_amigo/AMIGO_model.h
+-rw-rw-rw-   0        0        0      442 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_amigo/AMIGO_model_stats.h
+-rw-rw-rw-   0        0        0     1822 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_amigo/AMIGO_problem.h
+-rw-rw-rw-   0        0        0      287 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_amigo/amigoJAC.h
+-rw-rw-rw-   0        0        0       24 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_amigo/amigoRHS.h
+-rw-rw-rw-   0        0        0      171 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_amigo/amigoSensRHS.h
+-rw-rw-rw-   0        0        0      164 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_amigo/simulate_amigo_model.h
+drwxrwxrwx   0        0        0        0 2023-07-06 11:27:51.947163 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/
+drwxrwxrwx   0        0        0        0 2023-07-06 11:27:52.047163 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/
+-rw-rw-rw-   0        0        0    84971 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes.h
+-rw-rw-rw-   0        0        0     2442 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_band.h
+-rw-rw-rw-   0        0        0     6547 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_bandpre.h
+-rw-rw-rw-   0        0        0    13259 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_bbdpre.h
+-rw-rw-rw-   0        0        0     2122 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_dense.h
+-rw-rw-rw-   0        0        0     4845 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_diag.h
+-rw-rw-rw-   0        0        0    14031 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_direct.h
+-rw-rw-rw-   0        0        0     3732 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_lapack.h
+-rw-rw-rw-   0        0        0     3061 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_spbcgs.h
+-rw-rw-rw-   0        0        0     3021 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_spgmr.h
+-rw-rw-rw-   0        0        0    18270 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_spils.h
+-rw-rw-rw-   0        0        0     3085 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_sptfqmr.h
+drwxrwxrwx   0        0        0        0 2023-07-06 11:27:52.048162 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/nvector/
+-rw-rw-rw-   0        0        0    10054 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/nvector/nvector_serial.h
+drwxrwxrwx   0        0        0        0 2023-07-06 11:27:52.083161 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/
+-rw-rw-rw-   0        0        0     6539 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_band.h
+-rw-rw-rw-   0        0        0     3157 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_config.h
+-rw-rw-rw-   0        0        0     7865 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_dense.h
+-rw-rw-rw-   0        0        0    13199 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_direct.h
+-rw-rw-rw-   0        0        0     1129 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_fnvector.h
+-rw-rw-rw-   0        0        0    13127 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_iterative.h
+-rw-rw-rw-   0        0        0     4763 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_lapack.h
+-rw-rw-rw-   0        0        0     4294 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_math.h
+-rw-rw-rw-   0        0        0    15964 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_nvector.h
+-rw-rw-rw-   0        0        0     7740 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_spbcgs.h
+-rw-rw-rw-   0        0        0    12224 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_spgmr.h
+-rw-rw-rw-   0        0        0    10246 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_sptfqmr.h
+-rw-rw-rw-   0        0        0     3726 2022-12-07 11:24:13.000000 SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_types.h
+-rw-rw-rw-   0        0        0       90 2022-12-07 15:59:05.000000 SELDOMpy-0.8.4.8/SELDOMpy/makefile
+-rw-rw-rw-   0        0        0       71 2023-07-05 16:32:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/setup.cfg
+-rw-rw-rw-   0        0        0     3496 2023-07-06 11:27:24.000000 SELDOMpy-0.8.4.8/SELDOMpy/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 11:27:52.096163 SELDOMpy-0.8.4.8/SELDOMpy/src/
+-rw-rw-rw-   0        0        0    10952 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/AMIGO_model.c
+-rw-rw-rw-   0        0        0      240 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/AMIGO_model_stats.c
+-rw-rw-rw-   0        0        0     8027 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/AMIGO_problem.c
+-rw-rw-rw-   0        0        0      811 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/CNOStructure.h
+-rw-rw-rw-   0        0        0        0 2023-07-03 16:56:56.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/__init__.py
+-rw-rw-rw-   0        0        0     3389 2023-04-10 15:09:09.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/anODEModel.c
+-rw-rw-rw-   0        0        0    74908 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/cvodea.c
+-rw-rw-rw-   0        0        0    18585 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/cvodea_io.c
+-rw-rw-rw-   0        0        0   245647 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes.c
+-rw-rw-rw-   0        0        0    13293 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_band.c
+-rw-rw-rw-   0        0        0    16826 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_bandpre.c
+-rw-rw-rw-   0        0        0     2272 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_bandpre_impl.h
+-rw-rw-rw-   0        0        0    23592 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_bbdpre.c
+-rw-rw-rw-   0        0        0     2929 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_bbdpre_impl.h
+-rw-rw-rw-   0        0        0    12594 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_dense.c
+-rw-rw-rw-   0        0        0    13921 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_diag.c
+-rw-rw-rw-   0        0        0     2258 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_diag_impl.h
+-rw-rw-rw-   0        0        0    20099 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_direct.c
+-rw-rw-rw-   0        0        0     5473 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_direct_impl.h
+-rw-rw-rw-   0        0        0    47504 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_impl.h
+-rw-rw-rw-   0        0        0    41365 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_io.c
+-rw-rw-rw-   0        0        0    16912 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_spbcgs.c
+-rw-rw-rw-   0        0        0    17029 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_spgmr.c
+-rw-rw-rw-   0        0        0    32809 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_spils.c
+-rw-rw-rw-   0        0        0     6831 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_spils_impl.h
+-rw-rw-rw-   0        0        0    17108 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_sptfqmr.c
+-rw-rw-rw-   0        0        0      405 2022-12-07 11:24:11.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/decimal2binary.c
+-rw-rw-rw-   0        0        0     3792 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/dhc.c
+-rw-rw-rw-   0        0        0      527 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/findStates.c
+-rw-rw-rw-   0        0        0     3433 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/fnvector_serial.c
+-rw-rw-rw-   0        0        0     2688 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/fnvector_serial.h
+-rw-rw-rw-   0        0        0      693 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/getAdjacencyMatrix.c
+-rw-rw-rw-   0        0        0      463 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/getNumBits.c
+-rw-rw-rw-   0        0        0      475 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/getNumInputs.c
+-rw-rw-rw-   0        0        0      695 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/getStateIndex.c
+-rw-rw-rw-   0        0        0     3859 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/getTruthTables.c
+-rw-rw-rw-   0        0        0      451 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/get_count_bits.c
+-rw-rw-rw-   0        0        0      487 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/get_input_index.c
+-rw-rw-rw-   0        0        0      594 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/get_support_truth_tables.c
+-rw-rw-rw-   0        0        0      585 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/get_truth_tables_index.c
+-rw-rw-rw-   0        0        0      224 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/hill_function.c
+-rw-rw-rw-   0        0        0      219 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/linear_transfer_function.c
+-rw-rw-rw-   0        0        0      227 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/normHill.c
+-rw-rw-rw-   0        0        0    20778 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/nvector_serial.c
+-rw-rw-rw-   0        0        0      305 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/printAdjMat.c
+-rw-rw-rw-   0        0        0      315 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/printInterMat.c
+-rw-rw-rw-   0        0        0      553 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/printNminiTerms.c
+-rw-rw-rw-   0        0        0      410 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/printTruthTables.c
+-rw-rw-rw-   0        0        0    15775 2023-04-28 16:16:22.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/sim_logic_ode.c
+-rw-rw-rw-   0        0        0     9815 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/simulate_amigo_model.c
+-rw-rw-rw-   0        0        0     6036 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/sundials_band.c
+-rw-rw-rw-   0        0        0     8510 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/sundials_dense.c
+-rw-rw-rw-   0        0        0     6225 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/sundials_direct.c
+-rw-rw-rw-   0        0        0     7662 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/sundials_iterative.c
+-rw-rw-rw-   0        0        0     2474 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/sundials_math.c
+-rw-rw-rw-   0        0        0     4702 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/sundials_nvector.c
+-rw-rw-rw-   0        0        0     9663 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/sundials_spbcgs.c
+-rw-rw-rw-   0        0        0    12650 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/sundials_spgmr.c
+-rw-rw-rw-   0        0        0    14744 2022-12-07 11:24:12.000000 SELDOMpy-0.8.4.8/SELDOMpy/src/sundials_sptfqmr.c
+drwxrwxrwx   0        0        0        0 2023-07-06 11:27:51.964163 SELDOMpy-0.8.4.8/SELDOMpy.egg-info/
+-rw-rw-rw-   0        0        0     4195 2023-07-06 11:27:51.000000 SELDOMpy-0.8.4.8/SELDOMpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5792 2023-07-06 11:27:51.000000 SELDOMpy-0.8.4.8/SELDOMpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 11:27:51.000000 SELDOMpy-0.8.4.8/SELDOMpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2023-07-06 11:27:51.000000 SELDOMpy-0.8.4.8/SELDOMpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-06 11:27:51.000000 SELDOMpy-0.8.4.8/SELDOMpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-07-06 11:27:52.103162 SELDOMpy-0.8.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     3496 2023-07-06 11:27:24.000000 SELDOMpy-0.8.4.8/setup.py
```

### Comparing `SELDOMpy-0.8.4.7/LICENSE.txt` & `SELDOMpy-0.8.4.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/PKG-INFO` & `SELDOMpy-0.8.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SELDOMpy
-Version: 0.8.4.7
+Version: 0.8.4.8
 Summary: This package performs dynamic modelling of cellular signalling networks.
 Home-page: https://github.com/lupralo31/SELDOMpy
 Download-URL: https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz
 Author: Luis Prado
 Author-email: pradolopezluis@gmail.com
 License: GPLv3
 Keywords: SELDOMpy,SELDOM,dynamic modelling,cellular signalling networks,biomedical engineering
```

### Comparing `SELDOMpy-0.8.4.7/README.md` & `SELDOMpy-0.8.4.8/README.md`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/LICENSE.txt` & `SELDOMpy-0.8.4.8/SELDOMpy/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/README.md` & `SELDOMpy-0.8.4.8/SELDOMpy/README.md`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/buildmim.py` & `SELDOMpy-0.8.4.8/SELDOMpy/functions/buildmim.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/extras.py` & `SELDOMpy-0.8.4.8/SELDOMpy/functions/extras.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/gen_exps.py` & `SELDOMpy-0.8.4.8/SELDOMpy/functions/gen_exps.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/getLBODEmodel.py` & `SELDOMpy-0.8.4.8/SELDOMpy/functions/getLBODEmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from SELDOMpy.getRandomLBODEmodel import *
+from SELDOMpy.functions.getRandomLBODEmodel import *
 # Importo el archivo getRandomLBODEmodel en el que se realiza la ruleta para la creación de modelos
 
 
 class Model:
     def __init__(self, n_states, n_stimuli, x, adjMat, index_opt, LB, UB, k_pars, n_pars, w_pars,
                  tau_pars, nthreads, estimated_pars=None, active_pars=None, count_inputs=None, count_active_inputs=None,
                  namesSpecies=None):
```

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/getRandomLBODEmodel.py` & `SELDOMpy-0.8.4.8/SELDOMpy/functions/getRandomLBODEmodel.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_amigo/AMIGO_model.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_amigo/AMIGO_model.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_amigo/AMIGO_problem.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_amigo/AMIGO_problem.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_band.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_band.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_bandpre.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_bandpre.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_bbdpre.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_bbdpre.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_dense.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_dense.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_diag.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_diag.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_direct.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_direct.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_lapack.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_lapack.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_spbcgs.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_spbcgs.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_spgmr.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_spgmr.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_spils.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_spils.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/cvodes/cvodes_sptfqmr.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/cvodes/cvodes_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/nvector/nvector_serial.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/nvector/nvector_serial.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_band.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_band.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_config.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_config.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_dense.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_dense.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_direct.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_direct.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_fnvector.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_fnvector.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_iterative.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_iterative.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_lapack.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_lapack.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_math.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_math.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_nvector.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_nvector.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_spbcgs.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_spbcgs.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_spgmr.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_spgmr.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_sptfqmr.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_sptfqmr.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/include/include_cvodes/sundials/sundials_types.h` & `SELDOMpy-0.8.4.8/SELDOMpy/include/include_cvodes/sundials/sundials_types.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/optimization.py` & `SELDOMpy-0.8.4.8/SELDOMpy/functions/optimization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from mealpy.evolutionary_based import DE
-from SELDOMpy.simulate_logic_based_ode import *
+from SELDOMpy.functions.simulate_logic_based_ode import *
 # Se importa para hacer las simulaciones en la función objetivo tratando de minimizar el valor que obtenga aquí
 import datetime
 # Se importa para guardar la fecha en time dentro del objeto de la clase Res_opt que se devuelve
 import copy
 
 
 class Res_opt:
```

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/plot_results.py` & `SELDOMpy-0.8.4.8/SELDOMpy/functions/plot_results.py`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/reduce_fun.py` & `SELDOMpy-0.8.4.8/SELDOMpy/functions/reduce_fun.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from SELDOMpy.simulate_logic_based_ode import *
+from SELDOMpy.functions.simulate_logic_based_ode import *
 from math import log
 import copy
 
 
 def get_reduced_model(model, is_stimuli=None, delete_edge=-1):
     adjMat = copy.deepcopy(model.adjMat)
     model_copy = copy.deepcopy(model)
```

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/simulate_logic_based_ode.py` & `SELDOMpy-0.8.4.8/SELDOMpy/functions/simulate_logic_based_ode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import hello
 # Así importo la librería hello con el archivo sim_logic_ode.c y los includes compilados para poder ejecutarse
-from SELDOMpy.extras import *
+from SELDOMpy.functions.extras import *
 # Necesario para usar la función fill_array
 #import tracemalloc
 import decimal
 
 
 def simulate_logic_based_ode(model, exps, ivpsol):
     #tracemalloc.start()
```

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/simulate_logic_based_ode_obs.py` & `SELDOMpy-0.8.4.8/SELDOMpy/functions/simulate_logic_based_ode_obs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import hello
 # Así importo la librería hello con el archivo sim_logic_ode.c y los includes compilados para poder ejecutarse
-from SELDOMpy.extras import *
+from SELDOMpy.functions.extras import *
 # Necesario para usar la función fill_array
 
 
 def simulate_logic_based_ode_obs(model, exps, ivpsol):
 
     task = "OBS_CVODES_ODE"
```

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/AMIGO_model.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/AMIGO_model.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/AMIGO_problem.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/AMIGO_problem.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/CNOStructure.h` & `SELDOMpy-0.8.4.8/SELDOMpy/src/CNOStructure.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/anODEModel.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/anODEModel.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/cvodea.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/cvodea.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/cvodea_io.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/cvodea_io.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_band.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_band.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_bandpre.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_bandpre.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_bandpre_impl.h` & `SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_bandpre_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_bbdpre.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_bbdpre.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_bbdpre_impl.h` & `SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_bbdpre_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_dense.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_dense.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_diag.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_diag.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_diag_impl.h` & `SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_diag_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_direct.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_direct.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_direct_impl.h` & `SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_direct_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_impl.h` & `SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_io.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_io.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_spbcgs.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_spbcgs.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_spgmr.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_spgmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_spils.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_spils.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_spils_impl.h` & `SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_spils_impl.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/cvodes_sptfqmr.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/cvodes_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/dhc.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/dhc.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/findStates.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/findStates.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/fnvector_serial.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/fnvector_serial.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/fnvector_serial.h` & `SELDOMpy-0.8.4.8/SELDOMpy/src/fnvector_serial.h`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/getAdjacencyMatrix.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/getAdjacencyMatrix.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/getStateIndex.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/getStateIndex.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/getTruthTables.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/getTruthTables.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/get_support_truth_tables.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/get_support_truth_tables.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/get_truth_tables_index.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/get_truth_tables_index.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/nvector_serial.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/nvector_serial.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/printNminiTerms.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/printNminiTerms.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/sim_logic_ode.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/sim_logic_ode.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/simulate_amigo_model.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/simulate_amigo_model.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/sundials_band.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/sundials_band.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/sundials_dense.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/sundials_dense.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/sundials_direct.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/sundials_direct.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/sundials_iterative.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/sundials_iterative.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/sundials_math.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/sundials_math.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/sundials_nvector.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/sundials_nvector.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/sundials_spbcgs.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/sundials_spbcgs.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/sundials_spgmr.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/sundials_spgmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy/src/sundials_sptfqmr.c` & `SELDOMpy-0.8.4.8/SELDOMpy/src/sundials_sptfqmr.c`

 * *Files identical despite different names*

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy.egg-info/PKG-INFO` & `SELDOMpy-0.8.4.8/SELDOMpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SELDOMpy
-Version: 0.8.4.7
+Version: 0.8.4.8
 Summary: This package performs dynamic modelling of cellular signalling networks.
 Home-page: https://github.com/lupralo31/SELDOMpy
 Download-URL: https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz
 Author: Luis Prado
 Author-email: pradolopezluis@gmail.com
 License: GPLv3
 Keywords: SELDOMpy,SELDOM,dynamic modelling,cellular signalling networks,biomedical engineering
```

### Comparing `SELDOMpy-0.8.4.7/SELDOMpy.egg-info/SOURCES.txt` & `SELDOMpy-0.8.4.8/SELDOMpy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,24 +2,17 @@
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 SELDOMpy/LICENSE.txt
 SELDOMpy/README.md
 SELDOMpy/__init__.py
-SELDOMpy/buildmim.py
-SELDOMpy/extras.py
-SELDOMpy/gen_exps.py
-SELDOMpy/getLBODEmodel.py
-SELDOMpy/getRandomLBODEmodel.py
-SELDOMpy/optimization.py
-SELDOMpy/plot_results.py
-SELDOMpy/reduce_fun.py
-SELDOMpy/simulate_logic_based_ode.py
-SELDOMpy/simulate_logic_based_ode_obs.py
+SELDOMpy/makefile
+SELDOMpy/setup.cfg
+SELDOMpy/setup.py
 SELDOMpy.egg-info/PKG-INFO
 SELDOMpy.egg-info/SOURCES.txt
 SELDOMpy.egg-info/dependency_links.txt
 SELDOMpy.egg-info/requires.txt
 SELDOMpy.egg-info/top_level.txt
 SELDOMpy/src/AMIGO_model.c
 SELDOMpy/src/AMIGO_model_stats.c
@@ -67,14 +60,25 @@
 SELDOMpy/src/sundials_direct.c
 SELDOMpy/src/sundials_iterative.c
 SELDOMpy/src/sundials_math.c
 SELDOMpy/src/sundials_nvector.c
 SELDOMpy/src/sundials_spbcgs.c
 SELDOMpy/src/sundials_spgmr.c
 SELDOMpy/src/sundials_sptfqmr.c
+SELDOMpy/functions/__init__.py
+SELDOMpy/functions/buildmim.py
+SELDOMpy/functions/extras.py
+SELDOMpy/functions/gen_exps.py
+SELDOMpy/functions/getLBODEmodel.py
+SELDOMpy/functions/getRandomLBODEmodel.py
+SELDOMpy/functions/optimization.py
+SELDOMpy/functions/plot_results.py
+SELDOMpy/functions/reduce_fun.py
+SELDOMpy/functions/simulate_logic_based_ode.py
+SELDOMpy/functions/simulate_logic_based_ode_obs.py
 SELDOMpy/include/include_amigo/AMIGO_hdf5.h
 SELDOMpy/include/include_amigo/AMIGO_model.h
 SELDOMpy/include/include_amigo/AMIGO_model_stats.h
 SELDOMpy/include/include_amigo/AMIGO_problem.h
 SELDOMpy/include/include_amigo/amigoJAC.h
 SELDOMpy/include/include_amigo/amigoRHS.h
 SELDOMpy/include/include_amigo/amigoSensRHS.h
```

### Comparing `SELDOMpy-0.8.4.7/setup.py` & `SELDOMpy-0.8.4.8/SELDOMpy/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 numpy_include = np.get_include()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='SELDOMpy',
-    version='0.8.4.7',
+    version='0.8.4.8',
     description='This package performs dynamic modelling of cellular signalling networks.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Luis Prado',
     author_email='pradolopezluis@gmail.com',
     url='https://github.com/lupralo31/SELDOMpy',
     download_url='https://github.com/lupralo31/SELDOMpy/archive/refs/tags/V_0.2.1.tar.gz',
```

