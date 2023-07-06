# Comparing `tmp/cryspy-0.7.3.tar.gz` & `tmp/cryspy-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryspy-0.7.3.tar", last modified: Sun Mar 12 18:23:51 2023, max compression
+gzip compressed data, was "cryspy-0.7.4.tar", last modified: Thu Jul  6 15:14:34 2023, max compression
```

## Comparing `cryspy-0.7.3.tar` & `cryspy-0.7.4.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxrwxrwx   0        0        0        0 2023-03-12 18:23:51.841490 cryspy-0.7.3/
--rw-rw-rw-   0        0        0      188 2022-04-15 16:13:51.000000 cryspy-0.7.3/AUTHORS
--rw-rw-rw-   0        0        0     1136 2022-04-15 16:13:51.000000 cryspy-0.7.3/LICENSE
--rw-rw-rw-   0        0        0       91 2022-10-14 16:52:22.000000 cryspy-0.7.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3254 2023-03-12 18:23:51.830251 cryspy-0.7.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-12 18:23:49.871562 cryspy-0.7.3/cryspy/
-drwxrwxrwx   0        0        0        0 2023-03-12 18:23:50.957072 cryspy-0.7.3/cryspy/A_functions_base/
--rw-rw-rw-   0        0        0     7193 2022-08-05 13:41:36.000000 cryspy-0.7.3/cryspy/A_functions_base/charge_form_factor.py
--rw-rw-rw-   0        0        0   310024 2022-11-13 08:43:41.000000 cryspy-0.7.3/cryspy/A_functions_base/database.pickle
--rw-rw-rw-   0        0        0      163 2022-08-04 14:43:30.000000 cryspy-0.7.3/cryspy/A_functions_base/database.py
--rw-rw-rw-   0        0        0     8696 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/debye_waller_factor.py
--rw-rw-rw-   0        0        0    10281 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/extinction.py
--rw-rw-rw-   0        0        0    22814 2022-06-20 08:10:22.000000 cryspy-0.7.3/cryspy/A_functions_base/flip_ratio.py
--rw-rw-rw-   0        0        0     3519 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/function_1_algebra.py
--rw-rw-rw-   0        0        0    11651 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/function_1_atomic_vibrations.py
--rw-rw-rw-   0        0        0     3422 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/function_1_error_simplex.py
--rw-rw-rw-   0        0        0     3411 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/function_1_gamma_nu.py
--rw-rw-rw-   0        0        0     2634 2022-05-25 13:09:08.000000 cryspy-0.7.3/cryspy/A_functions_base/function_1_inversed_hessian.py
--rw-rw-rw-   0        0        0     1243 2022-08-05 10:34:06.000000 cryspy-0.7.3/cryspy/A_functions_base/function_1_magnetic.py
--rw-rw-rw-   0        0        0     3164 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/function_1_markdown.py
--rw-rw-rw-   0        0        0    22570 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/function_1_matrices.py
--rw-rw-rw-   0        0        0     3310 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/function_1_objects.py
--rw-rw-rw-   0        0        0     1852 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/function_1_roots.py
--rw-rw-rw-   0        0        0     4379 2022-08-05 13:19:13.000000 cryspy-0.7.3/cryspy/A_functions_base/function_1_scat_length_neutron.py
--rw-rw-rw-   0        0        0    10820 2023-03-09 15:46:40.000000 cryspy-0.7.3/cryspy/A_functions_base/function_1_strings.py
--rw-rw-rw-   0        0        0     4335 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/function_1_tof.py
--rw-rw-rw-   0        0        0    16837 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/function_2_crystallography_base.py
--rw-rw-rw-   0        0        0    13857 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/function_2_mem.py
--rw-rw-rw-   0        0        0    77767 2022-05-06 16:03:00.000000 cryspy-0.7.3/cryspy/A_functions_base/function_2_space_group.py
--rw-rw-rw-   0        0        0    14931 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/function_2_sym_elems.py
--rw-rw-rw-   0        0        0     7071 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/function_3_den_file.py
--rw-rw-rw-   0        0        0     4703 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/function_3_extinction.py
--rw-rw-rw-   0        0        0    32579 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/function_3_mcif.py
--rw-rw-rw-   0        0        0    12932 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/function_4_flip_ratio.py
--rw-rw-rw-   0        0        0    30783 2022-05-18 14:20:42.000000 cryspy-0.7.3/cryspy/A_functions_base/integrated_intensity_powder_diffraction.py
--rw-rw-rw-   0        0        0    67684 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/itables.txt
--rw-rw-rw-   0        0        0    12595 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/local_susceptibility.py
--rw-rw-rw-   0        0        0  9490894 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/magnetic_data.txt
--rw-rw-rw-   0        0        0     4869 2022-08-05 10:34:26.000000 cryspy-0.7.3/cryspy/A_functions_base/magnetic_form_factor.py
--rw-rw-rw-   0        0        0  3611707 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/magnetic_table_bns.txt
--rw-rw-rw-   0        0        0    60323 2022-05-29 10:03:27.000000 cryspy-0.7.3/cryspy/A_functions_base/matrix_operations.py
--rw-rw-rw-   0        0        0    24834 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/mempy.py
--rw-rw-rw-   0        0        0     3405 2022-07-25 15:20:14.000000 cryspy-0.7.3/cryspy/A_functions_base/orbital_functions.py
--rw-rw-rw-   0        0        0    12113 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/powder_diffraction_const_wavelength.py
--rw-rw-rw-   0        0        0     7969 2023-02-22 09:09:46.000000 cryspy-0.7.3/cryspy/A_functions_base/powder_diffraction_tof.py
--rw-rw-rw-   0        0        0     4767 2023-03-08 08:47:57.000000 cryspy-0.7.3/cryspy/A_functions_base/powder_diffraction_tof_zcode.py
--rw-rw-rw-   0        0        0     4458 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/preferred_orientation.py
--rw-rw-rw-   0        0        0    73575 2022-12-06 13:30:29.000000 cryspy-0.7.3/cryspy/A_functions_base/structure_factor.py
--rw-rw-rw-   0        0        0     4071 2023-03-12 16:33:33.000000 cryspy-0.7.3/cryspy/A_functions_base/symmetry_constraints.py
--rw-rw-rw-   0        0        0    17001 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/symmetry_elements.py
--rw-rw-rw-   0        0        0    51179 2022-07-12 15:17:43.000000 cryspy-0.7.3/cryspy/A_functions_base/unit_cell.py
--rw-rw-rw-   0        0        0   310358 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/A_functions_base/wyckoff.dat
-drwxrwxrwx   0        0        0        0 2023-03-12 18:23:51.016191 cryspy-0.7.3/cryspy/B_parent_classes/
--rw-rw-rw-   0        0        0    24843 2023-03-09 16:06:04.000000 cryspy-0.7.3/cryspy/B_parent_classes/cl_1_item.py
--rw-rw-rw-   0        0        0    25622 2023-03-09 13:01:33.000000 cryspy-0.7.3/cryspy/B_parent_classes/cl_2_loop.py
--rw-rw-rw-   0        0        0    19891 2023-03-09 13:30:52.000000 cryspy-0.7.3/cryspy/B_parent_classes/cl_3_data.py
--rw-rw-rw-   0        0        0    23487 2022-05-31 15:21:29.000000 cryspy-0.7.3/cryspy/B_parent_classes/cl_4_global.py
--rw-rw-rw-   0        0        0      363 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/B_parent_classes/preocedures.py
-drwxrwxrwx   0        0        0        0 2023-03-12 18:23:51.578560 cryspy-0.7.3/cryspy/C_item_loop_classes/
--rw-rw-rw-   0        0        0     4699 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_atom_electron_configuration.py
--rw-rw-rw-   0        0        0     6068 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_atom_local_axes.py
--rw-rw-rw-   0        0        0    13375 2023-03-12 16:45:30.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_atom_site.py
--rw-rw-rw-   0        0        0     8022 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_atom_site_aniso.py
--rw-rw-rw-   0        0        0     9201 2022-05-30 12:19:47.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_atom_site_exchange.py
--rw-rw-rw-   0        0        0     6330 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_atom_site_moment.py
--rw-rw-rw-   0        0        0    14073 2023-03-12 16:28:20.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_atom_site_susceptibility.py
--rw-rw-rw-   0        0        0     4753 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_atom_type.py
--rw-rw-rw-   0        0        0    11922 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_atom_type_scat.py
--rw-rw-rw-   0        0        0    26792 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_cell.py
--rw-rw-rw-   0        0        0     5172 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_channel_chi.py
--rw-rw-rw-   0        0        0     3598 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_channel_plus_minus.py
--rw-rw-rw-   0        0        0     3335 2023-03-09 16:46:50.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_chi2.py
--rw-rw-rw-   0        0        0     3448 2023-03-09 13:56:53.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_diffrn_radiation.py
--rw-rw-rw-   0        0        0    17644 2023-03-09 15:06:47.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_diffrn_refln.py
--rw-rw-rw-   0        0        0     3417 2023-03-12 16:13:57.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_exclude.py
--rw-rw-rw-   0        0        0     4627 2023-03-09 15:00:07.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_extinction.py
--rw-rw-rw-   0        0        0     9100 2022-05-25 13:16:34.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_inversed_hessian.py
--rw-rw-rw-   0        0        0     5815 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_mem_parameters.py
--rw-rw-rw-   0        0        0    11503 2023-03-09 15:28:56.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd2d_background.py
--rw-rw-rw-   0        0        0     5730 2023-03-09 15:20:20.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd2d_instr_reflex_asymmetry.py
--rw-rw-rw-   0        0        0     6487 2023-03-09 15:19:28.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd2d_instr_resolution.py
--rw-rw-rw-   0        0        0    25094 2022-04-25 14:37:50.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd2d_meas.py
--rw-rw-rw-   0        0        0     3923 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd2d_peak.py
--rw-rw-rw-   0        0        0    33547 2022-05-04 15:46:23.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd2d_proc.py
--rw-rw-rw-   0        0        0     6511 2023-03-09 14:12:36.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd_background.py
--rw-rw-rw-   0        0        0     5239 2023-03-09 16:46:49.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd_instr_reflex_asymmetry.py
--rw-rw-rw-   0        0        0     7101 2023-03-09 14:04:01.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd_instr_resolution.py
--rw-rw-rw-   0        0        0    12398 2022-04-25 12:45:48.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd_meas.py
--rw-rw-rw-   0        0        0     4735 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd_peak.py
--rw-rw-rw-   0        0        0    16037 2022-06-23 11:35:12.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd_proc.py
--rw-rw-rw-   0        0        0     7738 2023-03-09 15:05:18.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_phase.py
--rw-rw-rw-   0        0        0     3109 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_range.py
--rw-rw-rw-   0        0        0     4524 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_refine_ls.py
--rw-rw-rw-   0        0        0     5744 2022-05-03 13:20:25.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_refln.py
--rw-rw-rw-   0        0        0     5160 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_refln_susceptibility.py
--rw-rw-rw-   0        0        0     5925 2023-03-09 16:12:13.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_setup.py
--rw-rw-rw-   0        0        0    11063 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_space_group_symop.py
--rw-rw-rw-   0        0        0     7038 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_space_group_symop_magn_centering.py
--rw-rw-rw-   0        0        0    13393 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_space_group_wyckoff.py
--rw-rw-rw-   0        0        0     3454 2023-03-09 13:50:18.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_texture.py
--rw-rw-rw-   0        0        0     8641 2023-03-09 13:30:36.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_tof_background.py
--rw-rw-rw-   0        0        0     6651 2023-03-09 13:52:38.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_tof_intensity_incident.py
--rw-rw-rw-   0        0        0    11088 2023-03-09 13:32:15.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_tof_meas.py
--rw-rw-rw-   0        0        0     8693 2023-03-09 13:58:04.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_tof_parameters.py
--rw-rw-rw-   0        0        0     4504 2023-03-09 11:11:20.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_tof_peak.py
--rw-rw-rw-   0        0        0    12053 2023-03-09 10:51:17.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_tof_proc.py
--rw-rw-rw-   0        0        0    11129 2023-03-09 13:45:16.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_tof_profile.py
--rw-rw-rw-   0        0        0     9518 2022-08-05 13:18:50.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_2_atom_rho_orbital_radial_slater.py
--rw-rw-rw-   0        0        0     7415 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_2_atom_site_scat.py
--rw-rw-rw-   0        0        0    17113 2023-03-09 14:52:46.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_2_diffrn_orient_matrix.py
--rw-rw-rw-   0        0        0    11887 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_2_section.py
--rw-rw-rw-   0        0        0    38037 2022-05-06 16:02:37.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_2_space_group.py
--rw-rw-rw-   0        0        0     5759 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_2_space_group_symop_magn_operation.py
--rw-rw-rw-   0        0        0    46536 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/C_item_loop_classes/cl_3_density_point.py
-drwxrwxrwx   0        0        0        0 2023-03-12 18:23:51.647511 cryspy-0.7.3/cryspy/D_functions_item_loop/
--rw-rw-rw-   0        0        0     2319 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/D_functions_item_loop/debye_waller.py
--rw-rw-rw-   0        0        0    11316 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/D_functions_item_loop/function_1_calc_for_magcrystal.py
--rw-rw-rw-   0        0        0     2534 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/D_functions_item_loop/function_1_density_point_p1.py
--rw-rw-rw-   0        0        0     8278 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/D_functions_item_loop/function_1_flip_ratio.py
--rw-rw-rw-   0        0        0     3633 2022-08-09 16:41:52.000000 cryspy-0.7.3/cryspy/D_functions_item_loop/function_1_report_magnetization_ellipsoid.py
--rw-rw-rw-   0        0        0     6588 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/D_functions_item_loop/function_1_section_from_density_point.py
-drwxrwxrwx   0        0        0        0 2023-03-12 18:23:51.694231 cryspy-0.7.3/cryspy/E_data_classes/
--rw-rw-rw-   0        0        0    59599 2023-03-09 11:22:48.000000 cryspy-0.7.3/cryspy/E_data_classes/cl_1_crystal.py
--rw-rw-rw-   0        0        0    14237 2023-03-09 16:46:51.000000 cryspy-0.7.3/cryspy/E_data_classes/cl_2_diffrn.py
--rw-rw-rw-   0        0        0    18197 2023-03-09 14:43:18.000000 cryspy-0.7.3/cryspy/E_data_classes/cl_2_pd.py
--rw-rw-rw-   0        0        0    63118 2023-03-09 16:46:49.000000 cryspy-0.7.3/cryspy/E_data_classes/cl_2_pd2d.py
--rw-rw-rw-   0        0        0    14655 2023-03-09 13:58:13.000000 cryspy-0.7.3/cryspy/E_data_classes/cl_2_tof.py
-drwxrwxrwx   0        0        0        0 2023-03-12 18:23:51.703248 cryspy-0.7.3/cryspy/F_functions_data/
--rw-rw-rw-   0        0        0    33628 2023-03-09 11:22:48.000000 cryspy-0.7.3/cryspy/F_functions_data/script_1_mem.py
-drwxrwxrwx   0        0        0        0 2023-03-12 18:23:51.745495 cryspy-0.7.3/cryspy/H_functions_global/
--rw-rw-rw-   0        0        0     6442 2023-03-09 11:22:47.000000 cryspy-0.7.3/cryspy/H_functions_global/form_dictionary.py
--rw-rw-rw-   0        0        0    27191 2023-03-09 11:22:47.000000 cryspy-0.7.3/cryspy/H_functions_global/function_1_cryspy_objects.py
--rw-rw-rw-   0        0        0        2 2023-03-12 18:21:45.000000 cryspy-0.7.3/cryspy/H_functions_global/packages.dat
--rw-rw-rw-   0        0        0     7622 2023-03-09 11:22:47.000000 cryspy-0.7.3/cryspy/H_functions_global/powder_experiments.py
--rw-rw-rw-   0        0        0     3621 2023-03-09 11:22:46.000000 cryspy-0.7.3/cryspy/H_functions_global/simulations.py
--rw-rw-rw-   0        0        0    13384 2023-03-12 18:20:07.000000 cryspy-0.7.3/cryspy/__init__.py
--rw-rw-rw-   0        0        0     1100 2023-03-09 11:11:21.000000 cryspy-0.7.3/cryspy/__main__.py
-drwxrwxrwx   0        0        0        0 2023-03-12 18:23:51.769348 cryspy-0.7.3/cryspy/procedure_mempy/
--rw-rw-rw-   0        0        0    12654 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/procedure_mempy/mempy.py
--rw-rw-rw-   0        0        0    33539 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/procedure_mempy/mempy_by_dictionary.py
-drwxrwxrwx   0        0        0        0 2023-03-12 18:23:51.825537 cryspy-0.7.3/cryspy/procedure_rhochi/
--rw-rw-rw-   0        0        0     9225 2022-12-06 13:04:49.000000 cryspy-0.7.3/cryspy/procedure_rhochi/rhochi.py
--rw-rw-rw-   0        0        0    17194 2023-03-09 15:09:40.000000 cryspy-0.7.3/cryspy/procedure_rhochi/rhochi_by_dictionary.py
--rw-rw-rw-   0        0        0    19505 2023-03-09 16:46:52.000000 cryspy-0.7.3/cryspy/procedure_rhochi/rhochi_diffrn.py
--rw-rw-rw-   0        0        0    24395 2023-03-09 15:28:58.000000 cryspy-0.7.3/cryspy/procedure_rhochi/rhochi_pd.py
--rw-rw-rw-   0        0        0    28856 2022-04-15 16:13:51.000000 cryspy-0.7.3/cryspy/procedure_rhochi/rhochi_pd2d.py
--rw-rw-rw-   0        0        0    21651 2023-03-09 10:45:22.000000 cryspy-0.7.3/cryspy/procedure_rhochi/rhochi_tof.py
-drwxrwxrwx   0        0        0        0 2023-03-12 18:23:49.907451 cryspy-0.7.3/cryspy.egg-info/
--rw-rw-rw-   0        0        0     3254 2023-03-12 18:23:49.000000 cryspy-0.7.3/cryspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6396 2023-03-12 18:23:49.000000 cryspy-0.7.3/cryspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-12 18:23:49.000000 cryspy-0.7.3/cryspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-03-12 18:23:49.000000 cryspy-0.7.3/cryspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-12 18:23:49.000000 cryspy-0.7.3/cryspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2482 2023-03-09 11:11:23.000000 cryspy-0.7.3/readme.rst
--rw-rw-rw-   0        0        0       42 2023-03-12 18:23:51.842472 cryspy-0.7.3/setup.cfg
--rw-rw-rw-   0        0        0     2875 2023-03-12 18:20:22.000000 cryspy-0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:14:34.336575 cryspy-0.7.4/
+-rw-rw-rw-   0        0        0      188 2022-04-15 16:13:51.000000 cryspy-0.7.4/AUTHORS
+-rw-rw-rw-   0        0        0     1136 2022-04-15 16:13:51.000000 cryspy-0.7.4/LICENSE
+-rw-rw-rw-   0        0        0       91 2022-10-14 16:52:22.000000 cryspy-0.7.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3254 2023-07-06 15:14:34.336575 cryspy-0.7.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-06 15:14:34.082826 cryspy-0.7.4/cryspy/
+drwxrwxrwx   0        0        0        0 2023-07-06 15:14:34.222932 cryspy-0.7.4/cryspy/A_functions_base/
+-rw-rw-rw-   0        0        0     7193 2023-04-18 13:15:35.000000 cryspy-0.7.4/cryspy/A_functions_base/charge_form_factor.py
+-rw-rw-rw-   0        0        0   310024 2022-11-13 08:43:41.000000 cryspy-0.7.4/cryspy/A_functions_base/database.pickle
+-rw-rw-rw-   0        0        0      163 2022-08-04 14:43:30.000000 cryspy-0.7.4/cryspy/A_functions_base/database.py
+-rw-rw-rw-   0        0        0     8696 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/debye_waller_factor.py
+-rw-rw-rw-   0        0        0    10281 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/extinction.py
+-rw-rw-rw-   0        0        0    25416 2023-06-05 13:53:37.000000 cryspy-0.7.4/cryspy/A_functions_base/flip_ratio.py
+-rw-rw-rw-   0        0        0     3519 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/function_1_algebra.py
+-rw-rw-rw-   0        0        0    11651 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/function_1_atomic_vibrations.py
+-rw-rw-rw-   0        0        0     3422 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/function_1_error_simplex.py
+-rw-rw-rw-   0        0        0     3411 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/function_1_gamma_nu.py
+-rw-rw-rw-   0        0        0     2634 2022-05-25 13:09:08.000000 cryspy-0.7.4/cryspy/A_functions_base/function_1_inversed_hessian.py
+-rw-rw-rw-   0        0        0     1243 2022-08-05 10:34:06.000000 cryspy-0.7.4/cryspy/A_functions_base/function_1_magnetic.py
+-rw-rw-rw-   0        0        0     3164 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/function_1_markdown.py
+-rw-rw-rw-   0        0        0    22570 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/function_1_matrices.py
+-rw-rw-rw-   0        0        0     3310 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/function_1_objects.py
+-rw-rw-rw-   0        0        0     1852 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/function_1_roots.py
+-rw-rw-rw-   0        0        0     4379 2022-08-05 13:19:13.000000 cryspy-0.7.4/cryspy/A_functions_base/function_1_scat_length_neutron.py
+-rw-rw-rw-   0        0        0    10820 2023-03-09 15:46:40.000000 cryspy-0.7.4/cryspy/A_functions_base/function_1_strings.py
+-rw-rw-rw-   0        0        0     4335 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/function_1_tof.py
+-rw-rw-rw-   0        0        0    16837 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/function_2_crystallography_base.py
+-rw-rw-rw-   0        0        0    13857 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/function_2_mem.py
+-rw-rw-rw-   0        0        0    77767 2022-05-06 16:03:00.000000 cryspy-0.7.4/cryspy/A_functions_base/function_2_space_group.py
+-rw-rw-rw-   0        0        0    14931 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/function_2_sym_elems.py
+-rw-rw-rw-   0        0        0     7071 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/function_3_den_file.py
+-rw-rw-rw-   0        0        0     4703 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/function_3_extinction.py
+-rw-rw-rw-   0        0        0    32579 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/function_3_mcif.py
+-rw-rw-rw-   0        0        0    12932 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/function_4_flip_ratio.py
+-rw-rw-rw-   0        0        0    30783 2022-05-18 14:20:42.000000 cryspy-0.7.4/cryspy/A_functions_base/integrated_intensity_powder_diffraction.py
+-rw-rw-rw-   0        0        0    67684 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/itables.txt
+-rw-rw-rw-   0        0        0    12595 2023-03-23 12:42:45.000000 cryspy-0.7.4/cryspy/A_functions_base/local_susceptibility.py
+-rw-rw-rw-   0        0        0  9490894 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/magnetic_data.txt
+-rw-rw-rw-   0        0        0     4869 2022-08-05 10:34:26.000000 cryspy-0.7.4/cryspy/A_functions_base/magnetic_form_factor.py
+-rw-rw-rw-   0        0        0  3611707 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/magnetic_table_bns.txt
+-rw-rw-rw-   0        0        0    60323 2022-05-29 10:03:27.000000 cryspy-0.7.4/cryspy/A_functions_base/matrix_operations.py
+-rw-rw-rw-   0        0        0    24864 2023-06-05 13:50:42.000000 cryspy-0.7.4/cryspy/A_functions_base/mempy.py
+-rw-rw-rw-   0        0        0     3405 2022-07-25 15:20:14.000000 cryspy-0.7.4/cryspy/A_functions_base/orbital_functions.py
+-rw-rw-rw-   0        0        0    12113 2023-06-05 13:51:02.000000 cryspy-0.7.4/cryspy/A_functions_base/powder_diffraction_const_wavelength.py
+-rw-rw-rw-   0        0        0     7969 2023-02-22 09:09:46.000000 cryspy-0.7.4/cryspy/A_functions_base/powder_diffraction_tof.py
+-rw-rw-rw-   0        0        0     4767 2023-03-08 08:47:57.000000 cryspy-0.7.4/cryspy/A_functions_base/powder_diffraction_tof_zcode.py
+-rw-rw-rw-   0        0        0     4458 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/preferred_orientation.py
+-rw-rw-rw-   0        0        0    73575 2022-12-06 13:30:29.000000 cryspy-0.7.4/cryspy/A_functions_base/structure_factor.py
+-rw-rw-rw-   0        0        0     4071 2023-03-14 08:53:42.000000 cryspy-0.7.4/cryspy/A_functions_base/symmetry_constraints.py
+-rw-rw-rw-   0        0        0    17001 2023-05-19 08:23:39.000000 cryspy-0.7.4/cryspy/A_functions_base/symmetry_elements.py
+-rw-rw-rw-   0        0        0    51179 2022-07-12 15:17:43.000000 cryspy-0.7.4/cryspy/A_functions_base/unit_cell.py
+-rw-rw-rw-   0        0        0   310358 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/A_functions_base/wyckoff.dat
+drwxrwxrwx   0        0        0        0 2023-07-06 15:14:34.225467 cryspy-0.7.4/cryspy/B_parent_classes/
+-rw-rw-rw-   0        0        0    24843 2023-03-09 16:06:04.000000 cryspy-0.7.4/cryspy/B_parent_classes/cl_1_item.py
+-rw-rw-rw-   0        0        0    25938 2023-03-15 13:07:53.000000 cryspy-0.7.4/cryspy/B_parent_classes/cl_2_loop.py
+-rw-rw-rw-   0        0        0    19891 2023-03-09 13:30:52.000000 cryspy-0.7.4/cryspy/B_parent_classes/cl_3_data.py
+-rw-rw-rw-   0        0        0    23487 2023-07-05 13:45:24.000000 cryspy-0.7.4/cryspy/B_parent_classes/cl_4_global.py
+-rw-rw-rw-   0        0        0      363 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/B_parent_classes/preocedures.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:14:34.302699 cryspy-0.7.4/cryspy/C_item_loop_classes/
+-rw-rw-rw-   0        0        0     4699 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_atom_electron_configuration.py
+-rw-rw-rw-   0        0        0     6068 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_atom_local_axes.py
+-rw-rw-rw-   0        0        0    13375 2023-03-12 16:45:30.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_atom_site.py
+-rw-rw-rw-   0        0        0     8022 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_atom_site_aniso.py
+-rw-rw-rw-   0        0        0     9201 2022-05-30 12:19:47.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_atom_site_exchange.py
+-rw-rw-rw-   0        0        0     6330 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_atom_site_moment.py
+-rw-rw-rw-   0        0        0    14073 2023-03-12 16:28:20.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_atom_site_susceptibility.py
+-rw-rw-rw-   0        0        0     4749 2023-03-17 08:32:09.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_atom_type.py
+-rw-rw-rw-   0        0        0    11922 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_atom_type_scat.py
+-rw-rw-rw-   0        0        0    26792 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_cell.py
+-rw-rw-rw-   0        0        0     5172 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_channel_chi.py
+-rw-rw-rw-   0        0        0     3598 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_channel_plus_minus.py
+-rw-rw-rw-   0        0        0     3335 2023-03-09 16:46:50.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_chi2.py
+-rw-rw-rw-   0        0        0     3492 2023-05-15 14:52:23.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_diffrn_radiation.py
+-rw-rw-rw-   0        0        0    17644 2023-03-09 15:06:47.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_diffrn_refln.py
+-rw-rw-rw-   0        0        0     3417 2023-03-12 16:13:57.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_exclude.py
+-rw-rw-rw-   0        0        0     4627 2023-03-09 15:00:07.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_extinction.py
+-rw-rw-rw-   0        0        0     9100 2022-05-25 13:16:34.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_inversed_hessian.py
+-rw-rw-rw-   0        0        0     5815 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_mem_parameters.py
+-rw-rw-rw-   0        0        0    11503 2023-03-09 15:28:56.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd2d_background.py
+-rw-rw-rw-   0        0        0     5730 2023-03-09 15:20:20.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd2d_instr_reflex_asymmetry.py
+-rw-rw-rw-   0        0        0     6487 2023-03-09 15:19:28.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd2d_instr_resolution.py
+-rw-rw-rw-   0        0        0    25094 2022-04-25 14:37:50.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd2d_meas.py
+-rw-rw-rw-   0        0        0     3923 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd2d_peak.py
+-rw-rw-rw-   0        0        0    33547 2022-05-04 15:46:23.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd2d_proc.py
+-rw-rw-rw-   0        0        0     6511 2023-03-09 14:12:36.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd_background.py
+-rw-rw-rw-   0        0        0     5239 2023-03-09 16:46:49.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd_instr_reflex_asymmetry.py
+-rw-rw-rw-   0        0        0     7101 2023-03-09 14:04:01.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd_instr_resolution.py
+-rw-rw-rw-   0        0        0    12398 2022-04-25 12:45:48.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd_meas.py
+-rw-rw-rw-   0        0        0     4735 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd_peak.py
+-rw-rw-rw-   0        0        0    16037 2022-06-23 11:35:12.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd_proc.py
+-rw-rw-rw-   0        0        0     7738 2023-03-09 15:05:18.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_phase.py
+-rw-rw-rw-   0        0        0     3109 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_range.py
+-rw-rw-rw-   0        0        0     4524 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_refine_ls.py
+-rw-rw-rw-   0        0        0     5744 2022-05-03 13:20:25.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_refln.py
+-rw-rw-rw-   0        0        0     5160 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_refln_susceptibility.py
+-rw-rw-rw-   0        0        0     5925 2023-03-09 16:12:13.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_setup.py
+-rw-rw-rw-   0        0        0    11063 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_space_group_symop.py
+-rw-rw-rw-   0        0        0     7038 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_space_group_symop_magn_centering.py
+-rw-rw-rw-   0        0        0    13393 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_space_group_wyckoff.py
+-rw-rw-rw-   0        0        0     3454 2023-03-09 13:50:18.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_texture.py
+-rw-rw-rw-   0        0        0     8641 2023-03-09 13:30:36.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_tof_background.py
+-rw-rw-rw-   0        0        0     6651 2023-03-09 13:52:38.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_tof_intensity_incident.py
+-rw-rw-rw-   0        0        0    11088 2023-03-09 13:32:15.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_tof_meas.py
+-rw-rw-rw-   0        0        0     8693 2023-03-09 13:58:04.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_tof_parameters.py
+-rw-rw-rw-   0        0        0     4504 2023-03-09 11:11:20.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_tof_peak.py
+-rw-rw-rw-   0        0        0    12053 2023-03-09 10:51:17.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_tof_proc.py
+-rw-rw-rw-   0        0        0    11129 2023-03-09 13:45:16.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_tof_profile.py
+-rw-rw-rw-   0        0        0     9518 2022-08-05 13:18:50.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_2_atom_rho_orbital_radial_slater.py
+-rw-rw-rw-   0        0        0     7415 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_2_atom_site_scat.py
+-rw-rw-rw-   0        0        0    17113 2023-03-09 14:52:46.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_2_diffrn_orient_matrix.py
+-rw-rw-rw-   0        0        0    11887 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_2_section.py
+-rw-rw-rw-   0        0        0    38037 2022-05-06 16:02:37.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_2_space_group.py
+-rw-rw-rw-   0        0        0     5759 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_2_space_group_symop_magn_operation.py
+-rw-rw-rw-   0        0        0    46536 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/C_item_loop_classes/cl_3_density_point.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:14:34.304713 cryspy-0.7.4/cryspy/D_functions_item_loop/
+-rw-rw-rw-   0        0        0     2319 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/D_functions_item_loop/debye_waller.py
+-rw-rw-rw-   0        0        0    11316 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/D_functions_item_loop/function_1_calc_for_magcrystal.py
+-rw-rw-rw-   0        0        0     2534 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/D_functions_item_loop/function_1_density_point_p1.py
+-rw-rw-rw-   0        0        0     8278 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/D_functions_item_loop/function_1_flip_ratio.py
+-rw-rw-rw-   0        0        0     3633 2022-08-09 16:41:52.000000 cryspy-0.7.4/cryspy/D_functions_item_loop/function_1_report_magnetization_ellipsoid.py
+-rw-rw-rw-   0        0        0     6588 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/D_functions_item_loop/function_1_section_from_density_point.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:14:34.312721 cryspy-0.7.4/cryspy/E_data_classes/
+-rw-rw-rw-   0        0        0    59624 2023-07-06 13:01:16.000000 cryspy-0.7.4/cryspy/E_data_classes/cl_1_crystal.py
+-rw-rw-rw-   0        0        0    14270 2023-06-05 13:50:42.000000 cryspy-0.7.4/cryspy/E_data_classes/cl_2_diffrn.py
+-rw-rw-rw-   0        0        0    18197 2023-03-09 14:43:18.000000 cryspy-0.7.4/cryspy/E_data_classes/cl_2_pd.py
+-rw-rw-rw-   0        0        0    63118 2023-03-09 16:46:49.000000 cryspy-0.7.4/cryspy/E_data_classes/cl_2_pd2d.py
+-rw-rw-rw-   0        0        0    16242 2023-05-15 12:08:55.000000 cryspy-0.7.4/cryspy/E_data_classes/cl_2_tof.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:14:34.312721 cryspy-0.7.4/cryspy/F_functions_data/
+-rw-rw-rw-   0        0        0    33628 2023-03-09 11:22:48.000000 cryspy-0.7.4/cryspy/F_functions_data/script_1_mem.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:14:34.322661 cryspy-0.7.4/cryspy/H_functions_global/
+-rw-rw-rw-   0        0        0     6442 2023-03-09 11:22:47.000000 cryspy-0.7.4/cryspy/H_functions_global/form_dictionary.py
+-rw-rw-rw-   0        0        0    27191 2023-03-09 11:22:47.000000 cryspy-0.7.4/cryspy/H_functions_global/function_1_cryspy_objects.py
+-rw-rw-rw-   0        0        0        2 2023-07-06 14:34:24.000000 cryspy-0.7.4/cryspy/H_functions_global/packages.dat
+-rw-rw-rw-   0        0        0     9765 2023-04-13 10:20:19.000000 cryspy-0.7.4/cryspy/H_functions_global/powder_experiments.py
+-rw-rw-rw-   0        0        0     3621 2023-03-09 11:22:46.000000 cryspy-0.7.4/cryspy/H_functions_global/simulations.py
+-rw-rw-rw-   0        0        0    13429 2023-07-06 15:13:48.000000 cryspy-0.7.4/cryspy/__init__.py
+-rw-rw-rw-   0        0        0     1100 2023-03-09 11:11:21.000000 cryspy-0.7.4/cryspy/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:14:34.322661 cryspy-0.7.4/cryspy/procedure_mempy/
+-rw-rw-rw-   0        0        0    12654 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/procedure_mempy/mempy.py
+-rw-rw-rw-   0        0        0    33515 2023-06-05 13:50:41.000000 cryspy-0.7.4/cryspy/procedure_mempy/mempy_by_dictionary.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:14:34.336575 cryspy-0.7.4/cryspy/procedure_rhochi/
+-rw-rw-rw-   0        0        0     9225 2022-12-06 13:04:49.000000 cryspy-0.7.4/cryspy/procedure_rhochi/rhochi.py
+-rw-rw-rw-   0        0        0    17194 2023-03-09 15:09:40.000000 cryspy-0.7.4/cryspy/procedure_rhochi/rhochi_by_dictionary.py
+-rw-rw-rw-   0        0        0    19478 2023-06-05 13:50:39.000000 cryspy-0.7.4/cryspy/procedure_rhochi/rhochi_diffrn.py
+-rw-rw-rw-   0        0        0    24453 2023-07-05 12:12:26.000000 cryspy-0.7.4/cryspy/procedure_rhochi/rhochi_pd.py
+-rw-rw-rw-   0        0        0    28856 2022-04-15 16:13:51.000000 cryspy-0.7.4/cryspy/procedure_rhochi/rhochi_pd2d.py
+-rw-rw-rw-   0        0        0    23575 2023-03-17 09:02:53.000000 cryspy-0.7.4/cryspy/procedure_rhochi/rhochi_tof.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:14:34.092937 cryspy-0.7.4/cryspy.egg-info/
+-rw-rw-rw-   0        0        0     3254 2023-07-06 15:14:33.000000 cryspy-0.7.4/cryspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6396 2023-07-06 15:14:33.000000 cryspy-0.7.4/cryspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 15:14:33.000000 cryspy-0.7.4/cryspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-07-06 15:14:33.000000 cryspy-0.7.4/cryspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 15:14:33.000000 cryspy-0.7.4/cryspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2482 2023-03-09 11:11:23.000000 cryspy-0.7.4/readme.rst
+-rw-rw-rw-   0        0        0       42 2023-07-06 15:14:34.336575 cryspy-0.7.4/setup.cfg
+-rw-rw-rw-   0        0        0     2875 2023-07-06 15:12:21.000000 cryspy-0.7.4/setup.py
```

### Comparing `cryspy-0.7.3/LICENSE` & `cryspy-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/PKG-INFO` & `cryspy-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryspy
-Version: 0.7.3
+Version: 0.7.4
 Summary: PNPD data analysis
 Home-page: https://github.com/ikibalin/cryspy
 Author: Iurii Kibalin
 Author-email: yurikibalin@outlook.com
 License: MIT License
 Keywords: Polarized Neutron Diffraction Data Analysis
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/charge_form_factor.py` & `cryspy-0.7.4/cryspy/A_functions_base/charge_form_factor.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/database.pickle` & `cryspy-0.7.4/cryspy/A_functions_base/database.pickle`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/debye_waller_factor.py` & `cryspy-0.7.4/cryspy/A_functions_base/debye_waller_factor.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/extinction.py` & `cryspy-0.7.4/cryspy/A_functions_base/extinction.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/flip_ratio.py` & `cryspy-0.7.4/cryspy/A_functions_base/flip_ratio.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,269 +1,325 @@
 from typing import Callable
 import numpy
 
 
 def calc_iint(
-        beam_polarization: float, flipper_efficiency: float, f_nucl, f_m_perp, matrix_u, func_extinction: Callable = None,
-        flag_beam_polarization: bool = False, flag_flipper_efficiency: bool = False,
-        flag_f_nucl: bool = False, flag_f_m_perp: bool = False,
-        dict_in_out: dict = None, flag_use_precalculated_data: bool = False):
+        beam_polarization: float, 
+        flipper_efficiency: float, 
+        f_nucl, f_m_perp,
+        axis_z, 
+        func_extinction: Callable = None,
+        flag_beam_polarization: bool = False, 
+        flag_flipper_efficiency: bool = False,
+        flag_f_nucl: bool = False, 
+        flag_f_m_perp: bool = False,
+        dict_in_out: dict = None):
     """Calculate integrated intensities.
+    Sizes:
+        beam_polarization = float or [n_hkl] / the last option is for TOF
+        flipper_efficiency = float or [n_hkl] / the last option is for TOF
+        f_nucl = [n_hkl]
+        f_m_perp = [3, n_hkl]
+        axis_Zlab_XYZ = [3] or [3, n_hkl] / the last option is for powder
+        func_extinction is function take as input F_square
 
-    It is supposed that crystal is not rotate during the calculations 
-    (orientation matrix is the same for all reflections)
+    for single crystal measurements:
+    axis_Zlab_XYZ = [U_31, U_32, U_33]
     """
     if dict_in_out is None:
         flag_dict = False
-        dict_in_out_keys = []
     else:
         flag_dict = True
-        dict_in_out_keys = dict_in_out.keys()
 
-    p_u = beam_polarization
-    p_d = beam_polarization*(2*flipper_efficiency-1)
+    p_u = numpy.atleast_1d(beam_polarization)
+    p_d = numpy.atleast_1d(beam_polarization * (2 * flipper_efficiency - 1))
     flag_f_plus_sq = flag_f_nucl or flag_f_m_perp
     flag_f_minus_sq = flag_f_nucl or flag_f_m_perp
     flag_f_m_perp_xy_sq = flag_f_m_perp
 
     f_n = numpy.atleast_1d(f_nucl)
-    f_m_perp = numpy.atleast_1d(f_m_perp)
-    f_n_sq = numpy.square(numpy.abs(f_n))
-
-    f_m_perp_x = f_m_perp[0]*matrix_u[0] + f_m_perp[1]*matrix_u[1] + f_m_perp[2]*matrix_u[2]
-    f_m_perp_y = f_m_perp[0]*matrix_u[3] + f_m_perp[1]*matrix_u[4] + f_m_perp[2]*matrix_u[5]
-    f_m_perp_z = f_m_perp[0]*matrix_u[6] + f_m_perp[1]*matrix_u[7] + f_m_perp[2]*matrix_u[8]
+    if len(f_m_perp .shape) == 1:
+        f_m_perp = numpy.expand_dims(f_m_perp , -1)
+    if len(axis_z.shape) == 1:
+        axis_z = numpy.expand_dims(axis_z, -1)
+    
+    f_m_perp_sq = numpy.sum(numpy.square(f_m_perp.real), axis=0) + \
+        numpy.sum(numpy.square(f_m_perp.imag), axis=0)
     
-    f_m_perp_x_sq = numpy.square(numpy.abs(f_m_perp_x))
-    f_m_perp_y_sq = numpy.square(numpy.abs(f_m_perp_y))
-    f_m_perp_z_sq = numpy.square(numpy.abs(f_m_perp_z))
-
-    f_n_f_m_perp_z = 2.*(f_n.real * f_m_perp_z.real + f_n.imag * f_m_perp_z.imag)
-
-    f_plus_sq = f_n_sq + f_m_perp_z_sq + f_n_f_m_perp_z
-    f_minus_sq = f_n_sq + f_m_perp_z_sq - f_n_f_m_perp_z
-    f_m_perp_xy_sq = f_m_perp_x_sq + f_m_perp_y_sq
+    f_m_perp_zlab = numpy.sum(f_m_perp * axis_z, axis=0) 
+
+    f_m_perp_zlab_sq =  numpy.square(f_m_perp_zlab.real) + \
+        numpy.square(f_m_perp_zlab.imag)
+
+
+    f_plus = f_n + f_m_perp_zlab
+    f_minus = f_n - f_m_perp_zlab
+    f_plus_sq = numpy.square(f_plus.real) + numpy.square(f_plus.imag)
+    f_minus_sq = numpy.square(f_minus.real) + numpy.square(f_minus.imag)
+
+    f_m_perp_xy_sq = f_m_perp_sq - f_m_perp_zlab_sq
+
 
     if func_extinction is None:
         dder_y_plus, dder_y_minus, dder_y_m_perp_xy = {}, {}, {}
         y_plus = numpy.ones_like(f_plus_sq)
         y_minus = numpy.ones_like(f_minus_sq)
         y_m_perp_xy = numpy.ones_like(f_m_perp_xy_sq)
     else:
         y_plus, dder_y_plus = func_extinction(f_plus_sq, flag_f_sq=flag_f_plus_sq)
         y_minus, dder_y_minus = func_extinction(f_minus_sq, flag_f_sq=flag_f_minus_sq)
         y_m_perp_xy, dder_y_m_perp_xy = func_extinction(f_m_perp_xy_sq, flag_f_sq=flag_f_m_perp_xy_sq)
 
-    chiral_term = 2.*(f_m_perp_x.imag * f_m_perp_y.real - f_m_perp_x.real * f_m_perp_y.imag)
+    fmpx_r, fmpx_i = f_m_perp[0].real, f_m_perp[0].imag
+    fmpy_r, fmpy_i = f_m_perp[1].real, f_m_perp[1].imag
+    fmpz_r, fmpz_i = f_m_perp[2].real, f_m_perp[2].imag
+
+    chiral_term = 2.*(
+        axis_z[0] * (fmpy_i * fmpz_r - fmpy_r * fmpz_i) +
+        axis_z[1] * (fmpz_i * fmpx_r - fmpz_r * fmpx_i) +
+        axis_z[2] * (fmpx_i * fmpy_r - fmpx_r * fmpy_i))
+    
     if flag_dict:
         dict_in_out["chiral_term"] = chiral_term
 
-    iint_plus = 0.5*((1.+p_u)*y_plus*f_plus_sq +
-                     (1.-p_u)*y_minus*f_minus_sq) + \
-                    y_m_perp_xy * f_m_perp_xy_sq + \
-                    p_u * chiral_term
-
-    iint_minus = 0.5*((1.-p_d)*y_plus*f_plus_sq +
-                     (1.+p_d)*y_minus*f_minus_sq) + \
-                    y_m_perp_xy * f_m_perp_xy_sq - \
-                    p_d * chiral_term
+    iint_plus = 0.5 * ((1. + p_u) * y_plus * f_plus_sq +
+                       (1. - p_u) * y_minus * f_minus_sq) + \
+                y_m_perp_xy * f_m_perp_xy_sq + \
+                p_u * chiral_term
+
+    iint_minus = 0.5 * ((1. - p_d) * y_plus * f_plus_sq +
+                        (1. + p_d) * y_minus * f_minus_sq) + \
+                 y_m_perp_xy * f_m_perp_xy_sq - \
+                 p_d * chiral_term
 
     if flag_dict:
         dict_in_out["iint_plus"] = iint_plus
         dict_in_out["iint_minus"] = iint_minus
         dict_in_out["y_plus"] = y_plus
         dict_in_out["f_plus_sq"] = f_plus_sq
         dict_in_out["y_minus"] = y_minus
         dict_in_out["f_minus_sq"] = f_minus_sq
         dict_in_out["y_m_perp_xy"] = y_m_perp_xy
         dict_in_out["f_m_perp_xy_sq"] = f_m_perp_xy_sq
 
     dder_plus = {}
     dder_minus = {}
     if flag_beam_polarization:
-        dder_plus["beam_polarization"] = 0.5*(y_plus*f_plus_sq - y_minus*f_minus_sq + 2.*chiral_term) * \
+        dder_plus["beam_polarization"] = 0.5 * (
+            y_plus * f_plus_sq - 
+            y_minus * f_minus_sq + 
+            2. * chiral_term) * \
             numpy.ones_like(beam_polarization)
-        dder_minus["beam_polarization"] = 0.5*(-y_plus*f_plus_sq + y_minus*f_minus_sq - 2.*chiral_term) * \
+        dder_minus["beam_polarization"] = 0.5 * (
+            -y_plus * f_plus_sq + 
+            y_minus * f_minus_sq - 
+            2. * chiral_term) * \
             numpy.ones_like(beam_polarization)*(2.*flipper_efficiency-1.)
 
     if flag_flipper_efficiency:
-        dder_minus["flipper_efficiency"] = beam_polarization*(-y_plus*f_plus_sq + y_minus*f_minus_sq - 2.*chiral_term) * \
+        dder_minus["flipper_efficiency"] = beam_polarization*(
+            -y_plus * f_plus_sq + 
+            y_minus * f_minus_sq - 
+            2. * chiral_term) * \
             numpy.ones_like(flipper_efficiency)
     
     if flag_f_nucl:
-        f_plus_sq_f_n_real = 2. * (f_n.real + f_m_perp_z.real) * numpy.ones_like(f_n.real)
-        f_plus_sq_f_n_imag = 2. * (f_n.imag + f_m_perp_z.imag) * numpy.ones_like(f_n.imag)
-        f_minus_sq_f_n_real = 2. * (f_n.real - f_m_perp_z.real)* numpy.ones_like(f_n.real)
-        f_minus_sq_f_n_imag = 2. * (f_n.imag - f_m_perp_z.imag) * numpy.ones_like(f_n.imag)
+        f_plus_sq_f_n_real = 2. * f_plus.real 
+        f_plus_sq_f_n_imag = 2. * f_plus.imag 
+        f_minus_sq_f_n_real = 2. * f_minus.real 
+        f_minus_sq_f_n_imag = 2. * f_minus.imag 
 
         y_plus_f_n_real, y_minus_f_n_real = 0, 0 
         y_plus_f_n_imag, y_minus_f_n_imag = 0, 0 
         if "f_sq" in dder_y_plus.keys(): 
-            y_plus_f_n_real = dder_y_plus["f_sq"]*f_plus_sq_f_n_real
-            y_plus_f_n_imag = dder_y_plus["f_sq"]*f_plus_sq_f_n_imag
+            y_plus_f_n_real = dder_y_plus["f_sq"] * f_plus_sq_f_n_real
+            y_plus_f_n_imag = dder_y_plus["f_sq"] * f_plus_sq_f_n_imag
         if "f_sq" in dder_y_minus.keys(): 
-            y_minus_f_n_real = dder_y_minus["f_sq"]*f_minus_sq_f_n_real
-            y_minus_f_n_imag = dder_y_minus["f_sq"]*f_minus_sq_f_n_imag
+            y_minus_f_n_real = dder_y_minus["f_sq"] * f_minus_sq_f_n_real
+            y_minus_f_n_imag = dder_y_minus["f_sq"] * f_minus_sq_f_n_imag
 
-        dder_plus["f_nucl_real"] =  0.5*(
+        dder_plus["f_nucl_real"] =  0.5 * (
             (1.+p_u)*(y_plus*f_plus_sq_f_n_real+y_plus_f_n_real*f_plus_sq) +
             (1.-p_u)*(y_minus*f_minus_sq_f_n_real+y_minus_f_n_real*f_minus_sq))
         
-        dder_plus["f_nucl_imag"] =  0.5*(
+        dder_plus["f_nucl_imag"] =  0.5 * (
             (1.+p_u)*(y_plus*f_plus_sq_f_n_imag+y_plus_f_n_imag*f_plus_sq) +
             (1.-p_u)*(y_minus*f_minus_sq_f_n_imag+y_minus_f_n_imag*f_minus_sq))
 
-        dder_minus["f_nucl_real"] =  0.5*(
+        dder_minus["f_nucl_real"] =  0.5 * (
             (1.-p_d)*(y_plus*f_plus_sq_f_n_real+y_plus_f_n_real*f_plus_sq) +
             (1.+p_d)*(y_minus*f_minus_sq_f_n_real+y_minus_f_n_real*f_minus_sq))
         
-        dder_minus["f_nucl_imag"] =  0.5*(
+        dder_minus["f_nucl_imag"] =  0.5 * (
             (1.-p_d)*(y_plus*f_plus_sq_f_n_imag+y_plus_f_n_imag*f_plus_sq) +
             (1.+p_d)*(y_minus*f_minus_sq_f_n_imag+y_minus_f_n_imag*f_minus_sq))
 
 
     if flag_f_m_perp:
-        f_plus_sq_f_m_perp_z_real = 2. * (f_n.real + f_m_perp_z.real) * numpy.ones_like(f_m_perp_z.real)
-        f_plus_sq_f_m_perp_z_imag = 2. * (f_n.imag + f_m_perp_z.imag) * numpy.ones_like(f_m_perp_z.imag)
-        f_minus_sq_f_m_perp_z_real = -2. * (f_n.real - f_m_perp_z.real) * numpy.ones_like(f_m_perp_z.real)
-        f_minus_sq_f_m_perp_z_imag = -2. * (f_n.imag - f_m_perp_z.imag) * numpy.ones_like(f_m_perp_z.imag)
-        f_m_perp_xy_sq_f_m_perp_x_real = 2 * f_m_perp_x.real * numpy.ones_like(f_m_perp_x.real)
-        f_m_perp_xy_sq_f_m_perp_x_imag = 2 * f_m_perp_x.imag * numpy.ones_like(f_m_perp_x.imag)
-        f_m_perp_xy_sq_f_m_perp_y_real = 2 * f_m_perp_y.real * numpy.ones_like(f_m_perp_y.real)
-        f_m_perp_xy_sq_f_m_perp_y_imag = 2 * f_m_perp_y.imag * numpy.ones_like(f_m_perp_y.imag)
-        chiral_term_f_m_perp_x_real = -2 * f_m_perp_y.imag * numpy.ones_like(f_m_perp_x.real)
-        chiral_term_f_m_perp_x_imag = 2 * f_m_perp_y.real * numpy.ones_like(f_m_perp_x.imag)
-        chiral_term_f_m_perp_y_real = 2 * f_m_perp_x.imag * numpy.ones_like(f_m_perp_y.real)
-        chiral_term_f_m_perp_y_imag = -2 * f_m_perp_x.real * numpy.ones_like(f_m_perp_y.imag)
-
-        y_plus_f_m_perp_z_real, y_plus_f_m_perp_z_imag = 0, 0 
-        y_minus_f_m_perp_z_real, y_minus_f_m_perp_z_imag = 0, 0 
-        y_m_perp_xy_f_m_perp_x_real, y_m_perp_xy_f_m_perp_x_imag = 0, 0 
-        y_m_perp_xy_f_m_perp_y_real, y_m_perp_xy_f_m_perp_y_imag = 0, 0 
+        f_plus_sq_f_m_perp_x_real = 2. * f_plus.real * axis_z[0] 
+        f_plus_sq_f_m_perp_x_imag = 2. * f_plus.imag * axis_z[0] 
+        f_plus_sq_f_m_perp_y_real = 2. * f_plus.real * axis_z[1] 
+        f_plus_sq_f_m_perp_y_imag = 2. * f_plus.imag * axis_z[1] 
+        f_plus_sq_f_m_perp_z_real = 2. * f_plus.real * axis_z[2] 
+        f_plus_sq_f_m_perp_z_imag = 2. * f_plus.imag * axis_z[2]
+        
+        f_minus_sq_f_m_perp_x_real = -2. * f_minus.real * axis_z[0] 
+        f_minus_sq_f_m_perp_x_imag = -2. * f_minus.imag * axis_z[0] 
+        f_minus_sq_f_m_perp_y_real = -2. * f_minus.real * axis_z[1] 
+        f_minus_sq_f_m_perp_y_imag = -2. * f_minus.imag * axis_z[1] 
+        f_minus_sq_f_m_perp_z_real = -2. * f_minus.real * axis_z[2] 
+        f_minus_sq_f_m_perp_z_imag = -2. * f_minus.imag * axis_z[2] 
+        
+        zx, zy, zz = axis_z[0], axis_z[1], axis_z[2]
+        z_sq = numpy.square(axis_z)
+        zx_sq, zy_sq, zz_sq = z_sq[0], z_sq[1], z_sq[2]
+
+        f_m_perp_xy_sq_f_m_perp_x_real = 2. * (
+            (1. - zx_sq) * fmpx_r - zx * (zy * fmpy_r + zz * fmpz_r))
+        f_m_perp_xy_sq_f_m_perp_x_imag = 2. * (
+            (1. - zx_sq) * fmpx_i - zx * (zy * fmpy_i + zz * fmpz_i))
+        f_m_perp_xy_sq_f_m_perp_y_real = 2. * (
+            (1. - zy_sq) * fmpy_r - zy * (zz * fmpz_r + zx * fmpx_r))
+        f_m_perp_xy_sq_f_m_perp_y_imag = 2. * (
+            (1. - zy_sq) * fmpy_i - zy * (zz * fmpz_i + zx * fmpx_i))
+        f_m_perp_xy_sq_f_m_perp_z_real = 2. * (
+            (1. - zz_sq) * fmpz_r - zz * (zx * fmpx_r + zy * fmpy_r))
+        f_m_perp_xy_sq_f_m_perp_z_imag = 2. * (
+            (1. - zz_sq) * fmpz_i - zz * (zx * fmpx_i + zy * fmpy_i))
+
+        chiral_term_f_m_perp_x_real = 2. * (zy * fmpz_i - zz * fmpy_i)
+        chiral_term_f_m_perp_x_imag = -2. * (zy * fmpz_r - zz * fmpy_r)
+        chiral_term_f_m_perp_y_real = -2. * (zx * fmpz_i - zz * fmpx_i)
+        chiral_term_f_m_perp_y_imag = 2. * (zx * fmpz_r - zz * fmpx_r) 
+        chiral_term_f_m_perp_z_real = 2. * (zx * fmpy_i - zy * fmpx_i) 
+        chiral_term_f_m_perp_z_imag = -2. * (zx * fmpy_r - zy * fmpx_r)
+
+
+        y_plus_f_m_perp_x_real, y_plus_f_m_perp_x_imag = 0., 0. 
+        y_plus_f_m_perp_y_real, y_plus_f_m_perp_y_imag = 0., 0. 
+        y_plus_f_m_perp_z_real, y_plus_f_m_perp_z_imag = 0., 0. 
+        y_minus_f_m_perp_x_real, y_minus_f_m_perp_x_imag = 0., 0. 
+        y_minus_f_m_perp_y_real, y_minus_f_m_perp_y_imag = 0., 0. 
+        y_minus_f_m_perp_z_real, y_minus_f_m_perp_z_imag = 0., 0. 
+        y_m_perp_xy_f_m_perp_x_real, y_m_perp_xy_f_m_perp_x_imag = 0., 0. 
+        y_m_perp_xy_f_m_perp_y_real, y_m_perp_xy_f_m_perp_y_imag = 0., 0. 
+        y_m_perp_xy_f_m_perp_z_real, y_m_perp_xy_f_m_perp_z_imag = 0., 0. 
         if "f_sq" in dder_y_plus.keys(): 
+            y_plus_f_m_perp_x_real = dder_y_plus["f_sq"]*f_plus_sq_f_m_perp_x_real
+            y_plus_f_m_perp_x_imag = dder_y_plus["f_sq"]*f_plus_sq_f_m_perp_x_imag
+            y_plus_f_m_perp_y_real = dder_y_plus["f_sq"]*f_plus_sq_f_m_perp_y_real
+            y_plus_f_m_perp_y_imag = dder_y_plus["f_sq"]*f_plus_sq_f_m_perp_y_imag
             y_plus_f_m_perp_z_real = dder_y_plus["f_sq"]*f_plus_sq_f_m_perp_z_real
             y_plus_f_m_perp_z_imag = dder_y_plus["f_sq"]*f_plus_sq_f_m_perp_z_imag
         if "f_sq" in dder_y_minus.keys(): 
+            y_minus_f_m_perp_x_real = dder_y_minus["f_sq"]*f_minus_sq_f_m_perp_x_real
+            y_minus_f_m_perp_x_imag = dder_y_minus["f_sq"]*f_minus_sq_f_m_perp_x_imag
+            y_minus_f_m_perp_y_real = dder_y_minus["f_sq"]*f_minus_sq_f_m_perp_y_real
+            y_minus_f_m_perp_y_imag = dder_y_minus["f_sq"]*f_minus_sq_f_m_perp_y_imag
             y_minus_f_m_perp_z_real = dder_y_minus["f_sq"]*f_minus_sq_f_m_perp_z_real
             y_minus_f_m_perp_z_imag = dder_y_minus["f_sq"]*f_minus_sq_f_m_perp_z_imag
         if "f_sq" in dder_y_m_perp_xy.keys(): 
             y_m_perp_xy_f_m_perp_x_real = dder_y_m_perp_xy["f_sq"]*f_m_perp_xy_sq_f_m_perp_x_real
             y_m_perp_xy_f_m_perp_x_imag = dder_y_m_perp_xy["f_sq"]*f_m_perp_xy_sq_f_m_perp_x_imag
             y_m_perp_xy_f_m_perp_y_real = dder_y_m_perp_xy["f_sq"]*f_m_perp_xy_sq_f_m_perp_y_real
             y_m_perp_xy_f_m_perp_y_imag = dder_y_m_perp_xy["f_sq"]*f_m_perp_xy_sq_f_m_perp_y_imag
+            y_m_perp_xy_f_m_perp_z_real = dder_y_m_perp_xy["f_sq"]*f_m_perp_xy_sq_f_m_perp_z_real
+            y_m_perp_xy_f_m_perp_z_imag = dder_y_m_perp_xy["f_sq"]*f_m_perp_xy_sq_f_m_perp_z_imag
+
 
-        dder_plus_f_m_perp_x_real = \
-            y_m_perp_xy_f_m_perp_x_real * f_m_perp_xy_sq + \
-            y_m_perp_xy * f_m_perp_xy_sq_f_m_perp_x_real +\
+        dder_plus_f_m_perp_x_real =  0.5*(
+            (1. + p_u) * (y_plus * f_plus_sq_f_m_perp_x_real + y_plus_f_m_perp_x_real * f_plus_sq) +
+            (1. - p_u) * (y_minus * f_minus_sq_f_m_perp_x_real + y_minus_f_m_perp_x_real * f_minus_sq)) + \
+            y_m_perp_xy_f_m_perp_x_real * f_m_perp_xy_sq + y_m_perp_xy * f_m_perp_xy_sq_f_m_perp_x_real + \
             p_u * chiral_term_f_m_perp_x_real
-        dder_plus_f_m_perp_x_imag = \
-            y_m_perp_xy_f_m_perp_x_imag * f_m_perp_xy_sq + \
-            y_m_perp_xy * f_m_perp_xy_sq_f_m_perp_x_imag +\
+        dder_plus_f_m_perp_x_imag =  0.5*(
+            (1. + p_u) * (y_plus * f_plus_sq_f_m_perp_x_imag + y_plus_f_m_perp_x_imag * f_plus_sq) +
+            (1. - p_u) * (y_minus * f_minus_sq_f_m_perp_x_imag + y_minus_f_m_perp_x_imag * f_minus_sq)) + \
+            y_m_perp_xy_f_m_perp_x_imag * f_m_perp_xy_sq + y_m_perp_xy * f_m_perp_xy_sq_f_m_perp_x_imag + \
             p_u * chiral_term_f_m_perp_x_imag
-        dder_plus_f_m_perp_y_real = \
-            y_m_perp_xy_f_m_perp_y_real * f_m_perp_xy_sq + \
-            y_m_perp_xy * f_m_perp_xy_sq_f_m_perp_y_real +\
+
+        dder_plus_f_m_perp_y_real =  0.5*(
+            (1. + p_u) * (y_plus * f_plus_sq_f_m_perp_y_real + y_plus_f_m_perp_y_real * f_plus_sq) +
+            (1. - p_u) * (y_minus * f_minus_sq_f_m_perp_y_real + y_minus_f_m_perp_y_real * f_minus_sq)) + \
+            y_m_perp_xy_f_m_perp_y_real * f_m_perp_xy_sq + y_m_perp_xy * f_m_perp_xy_sq_f_m_perp_y_real + \
             p_u * chiral_term_f_m_perp_y_real
-        dder_plus_f_m_perp_y_imag = \
-            y_m_perp_xy_f_m_perp_y_imag * f_m_perp_xy_sq + \
-            y_m_perp_xy * f_m_perp_xy_sq_f_m_perp_y_imag +\
+        dder_plus_f_m_perp_y_imag =  0.5*(
+            (1. + p_u) * (y_plus * f_plus_sq_f_m_perp_y_imag + y_plus_f_m_perp_y_imag * f_plus_sq) +
+            (1. - p_u) * (y_minus * f_minus_sq_f_m_perp_y_imag + y_minus_f_m_perp_y_imag * f_minus_sq)) + \
+            y_m_perp_xy_f_m_perp_y_imag * f_m_perp_xy_sq + y_m_perp_xy * f_m_perp_xy_sq_f_m_perp_y_imag + \
             p_u * chiral_term_f_m_perp_y_imag
+
         dder_plus_f_m_perp_z_real =  0.5*(
-            (1.+p_u)*(y_plus*f_plus_sq_f_m_perp_z_real+y_plus_f_m_perp_z_real*f_plus_sq) +
-            (1.-p_u)*(y_minus*f_minus_sq_f_m_perp_z_real+y_minus_f_m_perp_z_real*f_minus_sq))
+            (1. + p_u) * (y_plus * f_plus_sq_f_m_perp_z_real + y_plus_f_m_perp_z_real * f_plus_sq) +
+            (1. - p_u) * (y_minus * f_minus_sq_f_m_perp_z_real + y_minus_f_m_perp_z_real * f_minus_sq)) + \
+            y_m_perp_xy_f_m_perp_z_real * f_m_perp_xy_sq + y_m_perp_xy * f_m_perp_xy_sq_f_m_perp_z_real + \
+            p_u * chiral_term_f_m_perp_z_real
         dder_plus_f_m_perp_z_imag =  0.5*(
-            (1.+p_u)*(y_plus*f_plus_sq_f_m_perp_z_imag+y_plus_f_m_perp_z_imag*f_plus_sq) +
-            (1.-p_u)*(y_minus*f_minus_sq_f_m_perp_z_imag+y_minus_f_m_perp_z_imag*f_minus_sq))
+            (1. + p_u) * (y_plus * f_plus_sq_f_m_perp_z_imag + y_plus_f_m_perp_z_imag * f_plus_sq) +
+            (1. - p_u) * (y_minus * f_minus_sq_f_m_perp_z_imag + y_minus_f_m_perp_z_imag * f_minus_sq)) + \
+            y_m_perp_xy_f_m_perp_z_imag * f_m_perp_xy_sq + y_m_perp_xy * f_m_perp_xy_sq_f_m_perp_z_imag + \
+            p_u * chiral_term_f_m_perp_z_imag
 
-        dder_plus_f_m_perp_1_real = \
-            dder_plus_f_m_perp_x_real*matrix_u[0] + \
-            dder_plus_f_m_perp_y_real*matrix_u[3] + \
-            dder_plus_f_m_perp_z_real*matrix_u[6]
-        dder_plus_f_m_perp_1_imag = \
-            dder_plus_f_m_perp_x_imag*matrix_u[0] + \
-            dder_plus_f_m_perp_y_imag*matrix_u[3] + \
-            dder_plus_f_m_perp_z_imag*matrix_u[6]
-        dder_plus_f_m_perp_2_real = \
-            dder_plus_f_m_perp_x_real*matrix_u[1] + \
-            dder_plus_f_m_perp_y_real*matrix_u[4] + \
-            dder_plus_f_m_perp_z_real*matrix_u[7]
-        dder_plus_f_m_perp_2_imag = \
-            dder_plus_f_m_perp_x_imag*matrix_u[1] + \
-            dder_plus_f_m_perp_y_imag*matrix_u[4] + \
-            dder_plus_f_m_perp_z_imag*matrix_u[7]
-        dder_plus_f_m_perp_3_real = \
-            dder_plus_f_m_perp_x_real*matrix_u[2] + \
-            dder_plus_f_m_perp_y_real*matrix_u[5] + \
-            dder_plus_f_m_perp_z_real*matrix_u[8]
-        dder_plus_f_m_perp_3_imag = \
-            dder_plus_f_m_perp_x_imag*matrix_u[2] + \
-            dder_plus_f_m_perp_y_imag*matrix_u[5] + \
-            dder_plus_f_m_perp_z_imag*matrix_u[8]
 
         dder_plus["f_m_perp_real"] = numpy.stack([
-            dder_plus_f_m_perp_1_real, dder_plus_f_m_perp_2_real, dder_plus_f_m_perp_3_real],
+            dder_plus_f_m_perp_x_real, 
+            dder_plus_f_m_perp_y_real, 
+            dder_plus_f_m_perp_z_real],
             axis=0) 
+
         dder_plus["f_m_perp_imag"] = numpy.stack([
-            dder_plus_f_m_perp_1_imag, dder_plus_f_m_perp_2_imag, dder_plus_f_m_perp_3_imag],
+            dder_plus_f_m_perp_x_imag,
+            dder_plus_f_m_perp_y_imag, 
+            dder_plus_f_m_perp_z_imag],
             axis=0)
 
 
-        dder_minus_f_m_perp_x_real = \
-            y_m_perp_xy_f_m_perp_x_real * f_m_perp_xy_sq + \
-            y_m_perp_xy * f_m_perp_xy_sq_f_m_perp_x_real -\
+        dder_minus_f_m_perp_x_real =  0.5*(
+            (1. - p_d) * (y_plus * f_plus_sq_f_m_perp_x_real + y_plus_f_m_perp_x_real * f_plus_sq) +
+            (1. + p_d) * (y_minus * f_minus_sq_f_m_perp_x_real + y_minus_f_m_perp_x_real * f_minus_sq)) + \
+            y_m_perp_xy_f_m_perp_x_real * f_m_perp_xy_sq + y_m_perp_xy * f_m_perp_xy_sq_f_m_perp_x_real - \
             p_d * chiral_term_f_m_perp_x_real
-        dder_minus_f_m_perp_x_imag = \
-            y_m_perp_xy_f_m_perp_x_imag * f_m_perp_xy_sq + \
-            y_m_perp_xy * f_m_perp_xy_sq_f_m_perp_x_imag -\
+        dder_minus_f_m_perp_x_imag =  0.5*(
+            (1. - p_d) * (y_plus * f_plus_sq_f_m_perp_x_imag + y_plus_f_m_perp_x_imag * f_plus_sq) +
+            (1. + p_d) * (y_minus * f_minus_sq_f_m_perp_x_imag + y_minus_f_m_perp_x_imag * f_minus_sq)) + \
+            y_m_perp_xy_f_m_perp_x_imag * f_m_perp_xy_sq + y_m_perp_xy * f_m_perp_xy_sq_f_m_perp_x_imag - \
             p_d * chiral_term_f_m_perp_x_imag
-        dder_minus_f_m_perp_y_real = \
-            y_m_perp_xy_f_m_perp_y_real * f_m_perp_xy_sq + \
-            y_m_perp_xy * f_m_perp_xy_sq_f_m_perp_y_real -\
+
+        dder_minus_f_m_perp_y_real =  0.5*(
+            (1. - p_d) * (y_plus * f_plus_sq_f_m_perp_y_real + y_plus_f_m_perp_y_real * f_plus_sq) +
+            (1. + p_d) * (y_minus * f_minus_sq_f_m_perp_y_real + y_minus_f_m_perp_y_real * f_minus_sq)) + \
+            y_m_perp_xy_f_m_perp_y_real * f_m_perp_xy_sq + y_m_perp_xy * f_m_perp_xy_sq_f_m_perp_y_real - \
             p_d * chiral_term_f_m_perp_y_real
-        dder_minus_f_m_perp_y_imag = \
-            y_m_perp_xy_f_m_perp_y_imag * f_m_perp_xy_sq + \
-            y_m_perp_xy * f_m_perp_xy_sq_f_m_perp_y_imag -\
+        dder_minus_f_m_perp_y_imag =  0.5*(
+            (1. - p_d) * (y_plus * f_plus_sq_f_m_perp_y_imag + y_plus_f_m_perp_y_imag * f_plus_sq) +
+            (1. + p_d) * (y_minus * f_minus_sq_f_m_perp_y_imag + y_minus_f_m_perp_y_imag * f_minus_sq)) + \
+            y_m_perp_xy_f_m_perp_y_imag * f_m_perp_xy_sq + y_m_perp_xy * f_m_perp_xy_sq_f_m_perp_y_imag - \
             p_d * chiral_term_f_m_perp_y_imag
+
         dder_minus_f_m_perp_z_real =  0.5*(
-            (1.-p_d)*(y_plus*f_plus_sq_f_m_perp_z_real+y_plus_f_m_perp_z_real*f_plus_sq) +
-            (1.+p_d)*(y_minus*f_minus_sq_f_m_perp_z_real+y_minus_f_m_perp_z_real*f_minus_sq))
+            (1. - p_d) * (y_plus * f_plus_sq_f_m_perp_z_real + y_plus_f_m_perp_z_real * f_plus_sq) +
+            (1. + p_d) * (y_minus * f_minus_sq_f_m_perp_z_real + y_minus_f_m_perp_z_real * f_minus_sq)) + \
+            y_m_perp_xy_f_m_perp_z_real * f_m_perp_xy_sq + y_m_perp_xy * f_m_perp_xy_sq_f_m_perp_z_real - \
+            p_d * chiral_term_f_m_perp_z_real
         dder_minus_f_m_perp_z_imag =  0.5*(
-            (1.-p_d)*(y_plus*f_plus_sq_f_m_perp_z_imag+y_plus_f_m_perp_z_imag*f_plus_sq) +
-            (1.+p_d)*(y_minus*f_minus_sq_f_m_perp_z_imag+y_minus_f_m_perp_z_imag*f_minus_sq))
+            (1. - p_d) * (y_plus * f_plus_sq_f_m_perp_z_imag + y_plus_f_m_perp_z_imag * f_plus_sq) +
+            (1. + p_d) * (y_minus * f_minus_sq_f_m_perp_z_imag + y_minus_f_m_perp_z_imag * f_minus_sq)) + \
+            y_m_perp_xy_f_m_perp_z_imag * f_m_perp_xy_sq + y_m_perp_xy * f_m_perp_xy_sq_f_m_perp_z_imag - \
+            p_d * chiral_term_f_m_perp_z_imag
 
-        dder_minus_f_m_perp_1_real = \
-            dder_minus_f_m_perp_x_real*matrix_u[0] + \
-            dder_minus_f_m_perp_y_real*matrix_u[3] + \
-            dder_minus_f_m_perp_z_real*matrix_u[6]
-        dder_minus_f_m_perp_1_imag = \
-            dder_minus_f_m_perp_x_imag*matrix_u[0] + \
-            dder_minus_f_m_perp_y_imag*matrix_u[3] + \
-            dder_minus_f_m_perp_z_imag*matrix_u[6]
-        dder_minus_f_m_perp_2_real = \
-            dder_minus_f_m_perp_x_real*matrix_u[1] + \
-            dder_minus_f_m_perp_y_real*matrix_u[4] + \
-            dder_minus_f_m_perp_z_real*matrix_u[7]
-        dder_minus_f_m_perp_2_imag = \
-            dder_minus_f_m_perp_x_imag*matrix_u[1] + \
-            dder_minus_f_m_perp_y_imag*matrix_u[4] + \
-            dder_minus_f_m_perp_z_imag*matrix_u[7]
-        dder_minus_f_m_perp_3_real = \
-            dder_minus_f_m_perp_x_real*matrix_u[2] + \
-            dder_minus_f_m_perp_y_real*matrix_u[5] + \
-            dder_minus_f_m_perp_z_real*matrix_u[8]
-        dder_minus_f_m_perp_3_imag = \
-            dder_minus_f_m_perp_x_imag*matrix_u[2] + \
-            dder_minus_f_m_perp_y_imag*matrix_u[5] + \
-            dder_minus_f_m_perp_z_imag*matrix_u[8]
 
         dder_minus["f_m_perp_real"] = numpy.stack([
-            dder_minus_f_m_perp_1_real, dder_minus_f_m_perp_2_real, dder_minus_f_m_perp_3_real], 
+            dder_minus_f_m_perp_x_real, 
+            dder_minus_f_m_perp_y_real, 
+            dder_minus_f_m_perp_z_real],
             axis=0) 
         dder_minus["f_m_perp_imag"] = numpy.stack([
-            dder_minus_f_m_perp_1_imag, dder_minus_f_m_perp_2_imag, dder_minus_f_m_perp_3_imag], 
+            dder_minus_f_m_perp_x_imag, 
+            dder_minus_f_m_perp_y_imag, 
+            dder_minus_f_m_perp_z_imag],
             axis=0)
 
     extinction_keys = dder_y_plus.keys()
     if len(extinction_keys) != 0:
         for key in extinction_keys:
             if key == "f_sq":
                 pass
@@ -275,14 +331,15 @@
                 dder_minus[key] = \
                     0.5*((1.-p_d)*f_plus_sq*dder_y_plus[key] +
                          (1.+p_d)*f_minus_sq*dder_y_minus[key]) + \
                     f_m_perp_xy_sq * dder_y_m_perp_xy[key]
     return iint_plus, iint_minus, dder_plus, dder_minus
 
 
+
 def calc_flip_ratio_by_iint(
         iint_plus, iint_minus, c_lambda2: float = None, iint_2hkl = None,
         flag_iint_plus: bool = False, flag_iint_minus: bool = False, 
         flag_c_lambda2: bool = False, flag_iint_2hkl: bool = False):
     """Calculate flip ratio by given integrated intensities.
     """
     dder = {}
@@ -337,54 +394,57 @@
     if flag_iint_2hkl:
         dder["iint_2hkl"] = 2.*c_lambda2*( - (iint_plus - iint_minus) / numpy.square(denom)) * \
             numpy.ones_like(iint_2hkl)
     return asymmetry, dder
 
 
 def calc_intensities_by_structure_factors(
-        beam_polarization: float, flipper_efficiency: float, f_nucl, f_m_perp, matrix_u, func_extinction: Callable = None,
+        beam_polarization: float, flipper_efficiency: float, f_nucl, f_m_perp,
+        axis_z, func_extinction: Callable = None,
         c_lambda2: float=None, f_nucl_2hkl=None, f_m_perp_2hkl=None,
         flag_beam_polarization: bool = False, flag_flipper_efficiency: bool = False,
         flag_f_nucl: bool = False, flag_f_m_perp: bool = False,
         flag_c_lambda2: bool = False,
         flag_f_nucl_2hkl: bool = False, flag_f_m_perp_2hkl: bool = False,
-        dict_in_out: dict = None, flag_use_precalculated_data: bool = False):
+        dict_in_out: dict = None):
     """Calculate flip ratio by given structure factors
     """
     if dict_in_out is None:
         flag_dict = False
         dict_in_out_keys = []
     else:
         flag_dict = True
         dict_in_out_keys = dict_in_out.keys()
     
     iint_plus, iint_minus, dder_plus_hkl, dder_minus_hkl = calc_iint(
-        beam_polarization, flipper_efficiency, f_nucl, f_m_perp, matrix_u, func_extinction=func_extinction,
+        beam_polarization, flipper_efficiency, f_nucl, f_m_perp, axis_z,
+        func_extinction=func_extinction,
         flag_beam_polarization=flag_beam_polarization, flag_flipper_efficiency=flag_flipper_efficiency,
         flag_f_nucl=flag_f_nucl, flag_f_m_perp=flag_f_m_perp,
-        dict_in_out=dict_in_out, flag_use_precalculated_data=flag_use_precalculated_data)
+        dict_in_out=dict_in_out)
 
     cond = (c_lambda2 is None) or (f_nucl_2hkl is None) or (f_m_perp_2hkl is None)
     if isinstance(c_lambda2, numpy.ndarray) and not(cond):
         cond = numpy.any(numpy.isnan(c_lambda2))
     if cond:
         c_lambda2 = None
         iint_2hkl = None
         flag_iint_2hkl = False
         dder_2hkl = {}
     else:
         iint_plus_2hkl, iint_minus_2hkl, dder_plus_2hkl, dder_minus_2hkl = calc_iint(
-            0, 0, f_nucl_2hkl, f_m_perp_2hkl, matrix_u, func_extinction=func_extinction,
+            0, 0, f_nucl_2hkl, f_m_perp_2hkl, axis_z,
+            func_extinction=func_extinction,
             flag_beam_polarization=False, flag_flipper_efficiency=False,
             flag_f_nucl=flag_f_nucl_2hkl, flag_f_m_perp=flag_f_m_perp_2hkl,
-            dict_in_out=None, flag_use_precalculated_data=False)
+            dict_in_out=None)
         iint_2hkl = iint_plus_2hkl
         dder_2hkl = dder_plus_2hkl
         flag_iint_2hkl = len(dder_2hkl.keys()) > 0
-        print("here")
+        
         iint_plus += c_lambda2*iint_2hkl
         iint_minus += c_lambda2*iint_2hkl
 
         if flag_f_nucl_2hkl:
             dder_2hkl["f_nucl_2hkl_real"] = dder_2hkl.pop("f_nucl_real")
             dder_2hkl["f_nucl_2hkl_imag"] = dder_2hkl.pop("f_nucl_imag")
         if flag_f_m_perp_2hkl:
@@ -425,38 +485,42 @@
     if flag_c_lambda2:
         dder_plus["c_lambda2"] = iint_2hkl
         dder_minus["c_lambda2"] = iint_2hkl
     return iint_plus, iint_minus, dder_plus, dder_minus
 
 
 def calc_flip_ratio_by_structure_factors(
-        beam_polarization: float, flipper_efficiency: float, f_nucl, f_m_perp, matrix_u, func_extinction: Callable = None,
+        beam_polarization: float, flipper_efficiency: float, f_nucl, f_m_perp,
+        axis_z, func_extinction: Callable = None,
         c_lambda2: float=None, f_nucl_2hkl=None, f_m_perp_2hkl=None,
-        flag_beam_polarization: bool = False, flag_flipper_efficiency: bool = False,
+        flag_beam_polarization: bool = False,
+        flag_flipper_efficiency: bool = False,
         flag_f_nucl: bool = False, flag_f_m_perp: bool = False,
         flag_c_lambda2: bool = False,
         flag_f_nucl_2hkl: bool = False, flag_f_m_perp_2hkl: bool = False,
         dict_in_out: dict = None, flag_use_precalculated_data: bool = False):
     """Calculate flip ratio by given structure factors
     """
     if dict_in_out is None:
         flag_dict = False
         dict_in_out_keys = []
     else:
         flag_dict = True
         dict_in_out_keys = dict_in_out.keys()
 
-    iint_plus, iint_minus, dder_plus, dder_minus = calc_intensities_by_structure_factors(
-        beam_polarization, flipper_efficiency, f_nucl, f_m_perp, matrix_u, func_extinction=func_extinction,
+    iint_plus, iint_minus, dder_plus, dder_minus = \
+        calc_intensities_by_structure_factors(
+        beam_polarization, flipper_efficiency, f_nucl, f_m_perp, axis_z,
+        func_extinction=func_extinction,
         c_lambda2=c_lambda2, f_nucl_2hkl=f_nucl_2hkl, f_m_perp_2hkl=f_m_perp_2hkl,
         flag_beam_polarization=flag_beam_polarization, flag_flipper_efficiency=flag_flipper_efficiency,
         flag_f_nucl=flag_f_nucl, flag_f_m_perp=flag_f_m_perp,
         flag_c_lambda2=flag_c_lambda2,
         flag_f_nucl_2hkl=flag_f_nucl_2hkl, flag_f_m_perp_2hkl=flag_f_m_perp_2hkl,
-        dict_in_out=dict_in_out, flag_use_precalculated_data=flag_use_precalculated_data)
+        dict_in_out=dict_in_out)
 
     flip_ration = iint_plus/iint_minus
 
     dder = {}
     keys_plus = dder_plus.keys()
     keys_minus = dder_minus.keys()
     set_key = set(keys_plus) | set(keys_minus)
```

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_1_algebra.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_1_algebra.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_1_atomic_vibrations.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_1_atomic_vibrations.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_1_error_simplex.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_1_error_simplex.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_1_gamma_nu.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_1_gamma_nu.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_1_inversed_hessian.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_1_inversed_hessian.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_1_magnetic.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_1_magnetic.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_1_markdown.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_1_markdown.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_1_matrices.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_1_matrices.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_1_objects.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_1_objects.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_1_roots.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_1_roots.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_1_scat_length_neutron.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_1_scat_length_neutron.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_1_strings.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_1_strings.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_1_tof.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_1_tof.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_2_crystallography_base.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_2_crystallography_base.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_2_mem.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_2_mem.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_2_space_group.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_2_space_group.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_2_sym_elems.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_2_sym_elems.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_3_den_file.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_3_den_file.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_3_extinction.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_3_extinction.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_3_mcif.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_3_mcif.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/function_4_flip_ratio.py` & `cryspy-0.7.4/cryspy/A_functions_base/function_4_flip_ratio.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/integrated_intensity_powder_diffraction.py` & `cryspy-0.7.4/cryspy/A_functions_base/integrated_intensity_powder_diffraction.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/itables.txt` & `cryspy-0.7.4/cryspy/A_functions_base/itables.txt`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/local_susceptibility.py` & `cryspy-0.7.4/cryspy/A_functions_base/local_susceptibility.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/magnetic_data.txt` & `cryspy-0.7.4/cryspy/A_functions_base/magnetic_data.txt`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/magnetic_form_factor.py` & `cryspy-0.7.4/cryspy/A_functions_base/magnetic_form_factor.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/magnetic_table_bns.txt` & `cryspy-0.7.4/cryspy/A_functions_base/magnetic_table_bns.txt`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/matrix_operations.py` & `cryspy-0.7.4/cryspy/A_functions_base/matrix_operations.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/mempy.py` & `cryspy-0.7.4/cryspy/A_functions_base/mempy.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,16 +442,17 @@
             f_sq, extinction_radius, extinction_mosaicity, volume_unit_cell, cos_2theta, wavelength,
             extinction_model, flag_f_sq=False, flag_radius=False,
             flag_mosaicity=False,
             flag_volume_unit_cell=False,
             flag_cos_2theta=False,
             flag_wavelength=False)
 
+        axis_z = matrix_u[6:9]
         iint_plus, iint_minus, dder_plus, dder_minus = calc_iint(
-            beam_polarization, flipper_efficiency, f_nucl, f_m_perp, matrix_u, func_extinction = func_extinction,
+            beam_polarization, flipper_efficiency, f_nucl, f_m_perp, axis_z, func_extinction = func_extinction,
             flag_beam_polarization = False, flag_flipper_efficiency = False,
             flag_f_nucl = False, flag_f_m_perp = True,
             dict_in_out = dict_in_out, flag_use_precalculated_data = flag_use_precalculated_data)
 
     
         if flag_asymmetry:
             model_exp, dder_model_exp = calc_asymmetry_by_iint(
```

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/orbital_functions.py` & `cryspy-0.7.4/cryspy/A_functions_base/orbital_functions.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/powder_diffraction_const_wavelength.py` & `cryspy-0.7.4/cryspy/A_functions_base/powder_diffraction_const_wavelength.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/powder_diffraction_tof.py` & `cryspy-0.7.4/cryspy/A_functions_base/powder_diffraction_tof.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/powder_diffraction_tof_zcode.py` & `cryspy-0.7.4/cryspy/A_functions_base/powder_diffraction_tof_zcode.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/preferred_orientation.py` & `cryspy-0.7.4/cryspy/A_functions_base/preferred_orientation.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/structure_factor.py` & `cryspy-0.7.4/cryspy/A_functions_base/structure_factor.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/symmetry_constraints.py` & `cryspy-0.7.4/cryspy/A_functions_base/symmetry_constraints.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/symmetry_elements.py` & `cryspy-0.7.4/cryspy/A_functions_base/symmetry_elements.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/unit_cell.py` & `cryspy-0.7.4/cryspy/A_functions_base/unit_cell.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/A_functions_base/wyckoff.dat` & `cryspy-0.7.4/cryspy/A_functions_base/wyckoff.dat`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/B_parent_classes/cl_1_item.py` & `cryspy-0.7.4/cryspy/B_parent_classes/cl_1_item.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/B_parent_classes/cl_2_loop.py` & `cryspy-0.7.4/cryspy/B_parent_classes/cl_2_loop.py`

 * *Files 1% similar despite different names*

```diff
@@ -740,8 +740,20 @@
         res = {}
         return res
     
     def take_parameters_from_dictionary(self, ddict_diffrn, l_parameter_name: list=None, l_sigma: list=None):
         """
         """
         pass
-        return None
+        return None
+
+def get_prefix_of_loop(item: LoopN):
+    if not(isinstance(item, LoopN)):
+        return ""
+    if item.ITEM_CLASS is ItemN:
+        if len(item.items) > 0:
+            prefix = item.items[0].PREFIX
+        else:
+            return ""
+    else:
+        prefix = item.ITEM_CLASS.PREFIX
+    return prefix
```

### Comparing `cryspy-0.7.3/cryspy/B_parent_classes/cl_3_data.py` & `cryspy-0.7.4/cryspy/B_parent_classes/cl_3_data.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/B_parent_classes/cl_4_global.py` & `cryspy-0.7.4/cryspy/B_parent_classes/cl_4_global.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_atom_electron_configuration.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_atom_electron_configuration.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_atom_local_axes.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_atom_local_axes.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_atom_site.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_atom_site.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_atom_site_aniso.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_atom_site_aniso.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_atom_site_exchange.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_atom_site_exchange.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_atom_site_moment.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_atom_site_moment.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_atom_site_susceptibility.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_atom_site_susceptibility.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_atom_type.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_atom_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     form_items_by_dictionary
 
 from cryspy.B_parent_classes.cl_1_item import ItemN
 from cryspy.B_parent_classes.cl_2_loop import LoopN
 
 class AtomType(ItemN):
     """Details about properties of the atom.
-    
+
     Data items in the ATOM_TYPE category record details about
     properties of the atoms that occupy the atom sites, such as the
     atomic scattering factors.
 
     Mandatory attributes:
         - label
         - type_symbol
```

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_atom_type_scat.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_atom_type_scat.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_cell.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_cell.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_channel_chi.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_channel_chi.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_channel_plus_minus.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_channel_plus_minus.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_chi2.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_chi2.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_diffrn_radiation.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_diffrn_radiation.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,18 +53,20 @@
 
     PREFIX = "diffrn_radiation"
 
     def __init__(self, **kwargs) -> NoReturn:
         super(DiffrnRadiation, self).__init__()
 
         # defined for any integer and float parameters
-        D_MIN = {"polarization": -1., "efficiency": -1.}
+        # D_MIN = {"polarization": -1., "efficiency": -1.}
+        D_MIN = {}
 
         # defined for ani integer and float parameters
-        D_MAX = {"polarization": 1., "efficiency": 1.}
+        # D_MAX = {"polarization": 1., "efficiency": 1.}
+        D_MAX = {}
 
         self.__dict__["D_MIN"] = D_MIN
         self.__dict__["D_MAX"] = D_MAX
         for key, attr in self.D_DEFAULT.items():
             setattr(self, key, attr)
         for key, attr in kwargs.items():
             setattr(self, key, attr)
```

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_diffrn_refln.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_diffrn_refln.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_exclude.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_exclude.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_extinction.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_extinction.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_inversed_hessian.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_inversed_hessian.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_mem_parameters.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_mem_parameters.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd2d_background.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd2d_background.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd2d_instr_reflex_asymmetry.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd2d_instr_reflex_asymmetry.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd2d_instr_resolution.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd2d_instr_resolution.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd2d_meas.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd2d_meas.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd2d_peak.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd2d_peak.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd2d_proc.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd2d_proc.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd_background.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd_background.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd_instr_reflex_asymmetry.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd_instr_reflex_asymmetry.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd_instr_resolution.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd_instr_resolution.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd_meas.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd_meas.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd_peak.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd_peak.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_pd_proc.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_pd_proc.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_phase.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_phase.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_range.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_range.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_refine_ls.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_refine_ls.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_refln.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_refln.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_refln_susceptibility.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_refln_susceptibility.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_setup.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_setup.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_space_group_symop.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_space_group_symop.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_space_group_symop_magn_centering.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_space_group_symop_magn_centering.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_space_group_wyckoff.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_space_group_wyckoff.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_texture.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_texture.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_tof_background.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_tof_background.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_tof_intensity_incident.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_tof_intensity_incident.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_tof_meas.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_tof_meas.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_tof_parameters.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_tof_parameters.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_tof_peak.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_tof_peak.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_tof_proc.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_tof_proc.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_1_tof_profile.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_1_tof_profile.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_2_atom_rho_orbital_radial_slater.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_2_atom_rho_orbital_radial_slater.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_2_atom_site_scat.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_2_atom_site_scat.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_2_diffrn_orient_matrix.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_2_diffrn_orient_matrix.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_2_section.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_2_section.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_2_space_group.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_2_space_group.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_2_space_group_symop_magn_operation.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_2_space_group_symop_magn_operation.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/C_item_loop_classes/cl_3_density_point.py` & `cryspy-0.7.4/cryspy/C_item_loop_classes/cl_3_density_point.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/D_functions_item_loop/debye_waller.py` & `cryspy-0.7.4/cryspy/D_functions_item_loop/debye_waller.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/D_functions_item_loop/function_1_calc_for_magcrystal.py` & `cryspy-0.7.4/cryspy/D_functions_item_loop/function_1_calc_for_magcrystal.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/D_functions_item_loop/function_1_density_point_p1.py` & `cryspy-0.7.4/cryspy/D_functions_item_loop/function_1_density_point_p1.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/D_functions_item_loop/function_1_flip_ratio.py` & `cryspy-0.7.4/cryspy/D_functions_item_loop/function_1_flip_ratio.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/D_functions_item_loop/function_1_report_magnetization_ellipsoid.py` & `cryspy-0.7.4/cryspy/D_functions_item_loop/function_1_report_magnetization_ellipsoid.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/D_functions_item_loop/function_1_section_from_density_point.py` & `cryspy-0.7.4/cryspy/D_functions_item_loop/function_1_section_from_density_point.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/E_data_classes/cl_1_crystal.py` & `cryspy-0.7.4/cryspy/E_data_classes/cl_1_crystal.py`

 * *Files 0% similar despite different names*

```diff
@@ -698,16 +698,16 @@
                     jl = calc_jl_for_ion(table_sthovl, type_symbol)
                     scattering_amplitude = jl[:,0]
                 except UserWarning:
                     try:
                         scattering_amplitude = calc_scattering_amplitude_tabulated(type_symbol, table_sthovl)[0]
                     except KeyError:
                         flag_atom_scattering_amplitude = False
-                        break
-                l_table_atom_scattering_amplitude.append(scattering_amplitude)
+                if flag_atom_scattering_amplitude:
+                    l_table_atom_scattering_amplitude.append(scattering_amplitude)
 
                 type_atom = get_atom_name_ion_charge_shell(type_symbol)[0]
                 try:
                     l_table_atom_dispersion.append(d_dispersion[type_atom.capitalize()])
                 except KeyError:
                     l_table_atom_dispersion.append(numpy.zeros_like(table_wavelength))
             if flag_atom_scattering_amplitude:
```

### Comparing `cryspy-0.7.3/cryspy/E_data_classes/cl_2_diffrn.py` & `cryspy-0.7.4/cryspy/E_data_classes/cl_2_diffrn.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,17 +205,17 @@
             """
             mag_loc_1 = u_matrix[2, 0]*f_mag*0.2695
             mag_loc_2 = u_matrix[2, 1]*f_mag*0.2695
             mag_loc_3 = u_matrix[2, 2]*f_mag*0.2695
             mag_loc = numpy.stack([mag_loc_1, mag_loc_2, mag_loc_3], axis=0)
             f_m_perp, dder_fm_perp_loc = calc_vector_product_v1_v2_v1(eq_ccs, mag_loc, flag_v1=False, flag_v2=False)
 
-
+            axis_z = u_matrix[2, :]
             f_r, dder_f_r = calc_flip_ratio_by_structure_factors(
-                       polarization, flipper_efficiency, f_nucl, f_m_perp, u_matrix, func_extinction=func_extinction,
+                       polarization, flipper_efficiency, f_nucl, f_m_perp, axis_z, func_extinction=func_extinction,
                        c_lambda2=ratio_lambdaover2, f_n_2h=f_nucl_2hkl, f_m_perp_2h=fm_perp_loc_2hkl,
                        flag_polarization=False, flag_flipper=False,
                        flag_f_n=False, flag_f_m_perp=False,
                        flag_c_lambda2=False,
                        flag_f_n_2h=False, flag_f_m_perp_2h=False)
 
             return f_r
```

### Comparing `cryspy-0.7.3/cryspy/E_data_classes/cl_2_pd.py` & `cryspy-0.7.4/cryspy/E_data_classes/cl_2_pd.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/E_data_classes/cl_2_pd2d.py` & `cryspy-0.7.4/cryspy/E_data_classes/cl_2_pd2d.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/E_data_classes/cl_2_tof.py` & `cryspy-0.7.4/cryspy/E_data_classes/cl_2_tof.py`

 * *Files 8% similar despite different names*

```diff
@@ -220,14 +220,42 @@
 
         if "background_coefficients" in keys:
             tof_background = self.tof_background
             hh = ddict_diffrn["background_coefficients"]
             for i_hh in range(hh.size):
                 setattr(tof_background, f"coeff{i_hh+1:}", float(hh[i_hh]))
 
+        if "profile_peak_shape" in keys:
+            profile_peak_shape = ddict_diffrn["profile_peak_shape"]
+            if profile_peak_shape == "pseudo-Voigt":
+                pass
+            elif profile_peak_shape == "Gauss":
+                pass
+            elif profile_peak_shape == "type0m":
+                profile_alphas = ddict_diffrn["profile_alphas"]
+                profile_betas = ddict_diffrn["profile_betas"]
+                profile_sigmas = ddict_diffrn["profile_sigmas"]
+                profile_gammas = ddict_diffrn["profile_gammas"]
+                profile_rs = ddict_diffrn["profile_rs"]
+                tof_profile = self.tof_profile
+                setattr(tof_profile, "alpha1", profile_alphas[0])
+                setattr(tof_profile, "alpha2", profile_alphas[1])
+                setattr(tof_profile, "beta00", profile_betas[0])
+                setattr(tof_profile, "beta01", profile_betas[1])
+                setattr(tof_profile, "beta10", profile_betas[2])
+                setattr(tof_profile, "sigma0", profile_sigmas[0])
+                setattr(tof_profile, "sigma1", profile_sigmas[1])
+                setattr(tof_profile, "sigma2", profile_sigmas[2])
+                setattr(tof_profile, "gamma0", profile_gammas[0])
+                setattr(tof_profile, "gamma1", profile_gammas[1])
+                setattr(tof_profile, "gamma2", profile_gammas[2])
+                setattr(tof_profile, "r01", profile_rs[0])
+                setattr(tof_profile, "r02", profile_rs[1])
+                setattr(tof_profile, "r03", profile_rs[2])
+
 
         if len(parameter_label) > 0:
             for name, sigma in zip(l_parameter_name, l_sigma):
                 if name[0] == "phase_scale":
                     self.phase.items[name[1][0]].scale_sigma = float(sigma)
                 if name[0] == "phase_ig":
                     self.phase.items[name[1][0]].igsize_sigma = float(sigma)
```

### Comparing `cryspy-0.7.3/cryspy/F_functions_data/script_1_mem.py` & `cryspy-0.7.4/cryspy/F_functions_data/script_1_mem.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/H_functions_global/form_dictionary.py` & `cryspy-0.7.4/cryspy/H_functions_global/form_dictionary.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/H_functions_global/function_1_cryspy_objects.py` & `cryspy-0.7.4/cryspy/H_functions_global/function_1_cryspy_objects.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/H_functions_global/powder_experiments.py` & `cryspy-0.7.4/cryspy/H_functions_global/powder_experiments.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,90 @@
 import numpy
 from cryspy.A_functions_base.database import DATABASE
-from cryspy.A_functions_base.charge_form_factor import  get_atom_name_ion_charge_shell
+from cryspy.A_functions_base.charge_form_factor import get_atom_name_ion_charge_shell
 from cryspy.B_parent_classes.cl_4_global import GlobalN
 
 from cryspy.A_functions_base.structure_factor import calc_bulk_susceptibility_by_dictionary
 from cryspy.A_functions_base.unit_cell import calc_volume_uc_by_unit_cell_parameters
 from cryspy.E_data_classes.cl_1_crystal import Crystal
 from cryspy.E_data_classes.cl_2_pd import Pd
 from cryspy.E_data_classes.cl_2_pd2d import Pd2d
 from cryspy.E_data_classes.cl_2_diffrn import Diffrn
 from cryspy.E_data_classes.cl_2_tof import TOF
 
+
+COEFF_N_A_MU_B = 6.022*0.927*1000.
+
+
+def calc_unit_cell_weight(crystal: Crystal) -> float:
+    """
+    Calculate the weight of unit cell for crystal.
+
+    Parameters
+    ----------
+    crystal : Crystal
+        description of the crystals.
+
+    Returns
+    -------
+    float
+        unit cell in atomic weight.
+    """
+    d_elements = DATABASE["Elements"]
+    crystal.apply_constraints()
+    atom_site = crystal.atom_site
+    atom_multiplicity = numpy.array(atom_site.multiplicity, dtype=int)
+    atom_occupancy = numpy.array(atom_site.occupancy, dtype=float)
+    l_atom_type_symbol = [get_atom_name_ion_charge_shell(
+        ion_name)[0].capitalize() for ion_name in atom_site.type_symbol]
+    atomic_weight = numpy.array([float(d_elements[(
+        "Atomic weight", atom_type)]) for atom_type in l_atom_type_symbol],
+        dtype=float)
+
+    unit_cell_weight = numpy.sum(
+        atom_multiplicity*atom_occupancy*atomic_weight)
+    return unit_cell_weight
+
+
+def calc_density_of_crystal(crystal: Crystal) -> float:
+    """
+    Calculate the density of crystal.
+
+    Parameters
+    ----------
+    crystal : Crystal
+        description of the crystals.
+
+    Returns
+    -------
+    float
+        density in g/cm^3.
+    """
+    unit_cell_weight = calc_unit_cell_weight(crystal)
+    unit_cell_parameters = crystal.cell.get_unit_cell_parameters()
+    unit_cell_volume = calc_volume_uc_by_unit_cell_parameters(
+        unit_cell_parameters, flag_unit_cell_parameters=False)[0]
+    density = unit_cell_weight/(unit_cell_volume*0.6022)  # g/cm^3
+    return density
+
+
 def report_powder_experiments(rcif_object: GlobalN):
     d_elements = DATABASE["Elements"]
     ls_out = []
     rcif_dict = rcif_object.get_dictionary()
     rcif_dict_keys = rcif_dict.keys()
-    l_crystal_dict_keys = [hh for hh in rcif_dict_keys if hh.startswith("crystal_")]
+    l_crystal_dict_keys = [
+        hh for hh in rcif_dict_keys if hh.startswith("crystal_")]
     l_pd_dict_keys = [hh for hh in rcif_dict_keys if hh.startswith("pd_")]
     l_pd2d_dict_keys = [hh for hh in rcif_dict_keys if hh.startswith("pd2d_")]
-    
-    l_crystal = [item for item in rcif_object.items if isinstance(item, Crystal)]
+
+    l_crystal = [
+        item for item in rcif_object.items if isinstance(item, Crystal)]
     l_crystal_name = [item.data_name.lower() for item in l_crystal]
-    
+
     for item in rcif_object.items:
         f_powder = isinstance(item, (Pd, Pd2d, TOF))
         f_single = isinstance(item, (Diffrn, ))
         if f_powder or f_single:
             phase = item.phase
 
         if f_single:
@@ -34,101 +92,127 @@
         elif f_powder:
             l_phase_items = phase.items
 
         if f_powder or f_single:
             field = item.setup.field
             ls_out.append(f"In experiment '{item.data_name:}' \n")
 
-            
-            m_chi_total = numpy.zeros((3,3), dtype=float)
+            m_chi_total = numpy.zeros((3, 3), dtype=float)
             l_s_v_sq, l_v_uc, l_m_uc = [], [], []
             l_m_chi, l_s_v_m = [], []
             l_m_chi_ion = []
 
-
             for phase_item in l_phase_items:
                 phase_label = phase_item.label.lower()
                 if f_single:
                     phase_scale = 1.
                 else:
                     phase_scale = phase_item.scale
                 ind_phase = l_crystal_name.index(phase_label)
                 crystal = l_crystal[ind_phase]
 
+                # FIXME: replace by functions defined above
                 crystal.apply_constraints()
                 atom_site = crystal.atom_site
-                atom_multiplicity = numpy.array(atom_site.multiplicity, dtype=int)
+                atom_multiplicity = numpy.array(
+                    atom_site.multiplicity, dtype=int)
                 atom_occupancy = numpy.array(atom_site.occupancy, dtype=float)
-                l_atom_type_symbol = [get_atom_name_ion_charge_shell(ion_name)[0].capitalize() for ion_name in atom_site.type_symbol]
-                atomic_weight = numpy.array([ float(d_elements[("Atomic weight", atom_type)]) for atom_type in l_atom_type_symbol], dtype=float)
+                l_atom_type_symbol = [get_atom_name_ion_charge_shell(
+                    ion_name)[0].capitalize() for ion_name in atom_site.type_symbol]
+                atomic_weight = numpy.array([float(d_elements[(
+                    "Atomic weight", atom_type)]) for atom_type in l_atom_type_symbol], dtype=float)
+
+                unit_cell_weight = numpy.sum(
+                    atom_multiplicity*atom_occupancy*atomic_weight)
+                coeff = COEFF_N_A_MU_B/unit_cell_weight
                 
-                unit_cell_weight = numpy.sum(atom_multiplicity*atom_occupancy*atomic_weight)
-                coeff = 6.022*0.927*1000/unit_cell_weight
-
                 crystal_dict = crystal.get_dictionary()
                 crystal_dict_keys = crystal_dict.keys()
                 if "atom_para_sc_chi" in crystal_dict_keys:
                     dict_in_out = {}
                     flag_use_precalculated_data = False
                     bulk_susceptibility, dder = calc_bulk_susceptibility_by_dictionary(
-                        crystal_dict, dict_in_out, flag_use_precalculated_data = flag_use_precalculated_data)
+                        crystal_dict, dict_in_out, flag_use_precalculated_data=flag_use_precalculated_data)
                     m_chi = numpy.array([
-                        [bulk_susceptibility[0], bulk_susceptibility[1], bulk_susceptibility[2]],
-                        [bulk_susceptibility[3], bulk_susceptibility[4], bulk_susceptibility[5]],
+                        [bulk_susceptibility[0], bulk_susceptibility[1],
+                            bulk_susceptibility[2]],
+                        [bulk_susceptibility[3], bulk_susceptibility[4],
+                            bulk_susceptibility[5]],
                         [bulk_susceptibility[6], bulk_susceptibility[7], bulk_susceptibility[8]]], dtype=float)
                     atom_para_index = atom_para_index = crystal_dict["atom_para_index"]
-                    n_ions = numpy.sum((atom_multiplicity*atom_occupancy)[atom_para_index])
+                    n_ions = numpy.sum(
+                        (atom_multiplicity*atom_occupancy)[atom_para_index])
                 else:
-                    m_chi = numpy.zeros((3,3), dtype=float)
+                    m_chi = numpy.zeros((3, 3), dtype=float)
                     n_ions = 1
-                
+
                 v_uc, dder = calc_volume_uc_by_unit_cell_parameters(
                     crystal_dict["unit_cell_parameters"], flag_unit_cell_parameters=False)
 
                 s_v_sq = phase_scale * v_uc * v_uc
                 s_v_m = phase_scale * v_uc * unit_cell_weight
                 l_m_uc.append(unit_cell_weight)
                 l_v_uc.append(v_uc)
                 l_s_v_sq.append(s_v_sq)
                 l_s_v_m.append(s_v_m)
-                
+
                 l_m_chi.append(m_chi*coeff)
                 l_m_chi_ion.append(m_chi/n_ions)
             sum_s_v_m = numpy.sum(l_s_v_m)
             sum_s_v_sq = numpy.sum(l_s_v_sq)
             ls_out.append(f"For polycrystalline sample at field {field:.2f}T:")
-            ls_out.append("-----------------------------------------------------------")
-            ls_out.append("Phase      Density      wF  mass M      vF       M   Moment")
-            ls_out.append("            g/cm^3           emu/g        emu/cm^3 mu_B/ion")
-            ls_out.append("-----------------------------------------------------------")
-            
+            ls_out.append(
+                "-----------------------------------------------------------")
+            ls_out.append(
+                "Phase      Density      wF  mass M      vF       M   Moment")
+            ls_out.append(
+                "            g/cm^3           emu/g        emu/cm^3 mu_B/ion")
+            ls_out.append(
+                "-----------------------------------------------------------")
+
             m_chi_mixture = 0.
             m_volume_mixture = 0.
-            for phase_item, v_uc, m_uc, s_v_sq, m_chi, s_v_m, m_chi_ion in zip(l_phase_items, l_v_uc, l_m_uc, l_s_v_sq, l_m_chi, l_s_v_m, l_m_chi_ion):
+            for phase_item, v_uc, m_uc, s_v_sq, m_chi, s_v_m, m_chi_ion in zip(
+                    l_phase_items, l_v_uc, l_m_uc, l_s_v_sq, l_m_chi, l_s_v_m,
+                    l_m_chi_ion):
                 volume_fraction = s_v_sq/sum_s_v_sq
                 weight_fraction = s_v_m/sum_s_v_m
                 m_chi_aver = field*(m_chi[0, 0]+m_chi[1, 1]+m_chi[2, 2])/3
-                density = m_uc/(v_uc*0.6022) # g/cm^3
+                density = m_uc/(v_uc*0.6022)  # g/cm^3
                 m_volume_aver = m_chi_aver*density
-                m_chi_ion_aver = field*(m_chi_ion[0, 0]+m_chi_ion[1, 1]+m_chi_ion[2, 2])/3
-                
-                ls_out.append(f"{phase_item.label:10} {density:7.3f}  {weight_fraction*100:5.1f}% {m_chi_aver:7.0f}  {volume_fraction*100:5.1f}% {m_volume_aver:7.0f} {m_chi_ion_aver:8.3f}")
+                m_chi_ion_aver = field * \
+                    (m_chi_ion[0, 0]+m_chi_ion[1, 1]+m_chi_ion[2, 2])/3
+
+                ls_out.append(
+                    f"{phase_item.label:10} {density:7.3f}  {weight_fraction*100:5.1f}% {m_chi_aver:7.0f}  {volume_fraction*100:5.1f}% {m_volume_aver:7.0f} {m_chi_ion_aver:8.3f}")
                 m_chi_mixture += weight_fraction*m_chi_aver
                 m_volume_mixture += volume_fraction*m_volume_aver
-            ls_out.append("-----------------------------------------------------------")
-            ls_out.append("  wF is weight-fraction of given phase in a mixture;")
+            ls_out.append(
+                "-----------------------------------------------------------")
+            ls_out.append(
+                "  wF is weight-fraction of given phase in a mixture;")
             ls_out.append("  mass M is mass magnetization of powder sample;")
-            ls_out.append("  vF is volume-fraction of given phase in a mixture;")
+            ls_out.append(
+                "  vF is volume-fraction of given phase in a mixture;")
             ls_out.append("   M is volume magnetization of powder sample.\n")
-            ls_out.append(f"Mass magnetization of a mixture is {m_chi_mixture:.2f} [emu/g];")
-            ls_out.append(f"Volume magnetization of a mixture is {m_volume_mixture:.2f} [emu/cm^3].\n")
-            
-            ls_out.append("----------------------------------------------------")      
-            ls_out.append("Phase           Mass susceptibility tensor x 10 000")
-            ls_out.append("----------------------------------------------------")      
+            ls_out.append(
+                f"Mass magnetization of a mixture is {m_chi_mixture:.2f} [emu/g];")
+            ls_out.append(
+                f"Volume magnetization of a mixture is {m_volume_mixture:.2f} [emu/cm^3].\n")
+
+            ls_out.append(
+                "----------------------------------------------------")
+            ls_out.append(
+                "Phase           Mass susceptibility tensor x 10 000")
+            ls_out.append(
+                "----------------------------------------------------")
             for phase_item, m_chi in zip(l_phase_items, l_m_chi):
-                ls_out.append(f"{phase_item.label:10} {m_chi[0, 0]:6.2f} {m_chi[1, 1]:6.2f} {m_chi[2, 2]:6.2f} {m_chi[0, 1]:6.2f} {m_chi[0, 2]:6.2f} {m_chi[1, 2]:6.2f}")
-            ls_out.append("----------------------------------------------------")
-            ls_out.append("The tensor is defined in Cartezian coordinate system")
-            ls_out.append("such as axis Z || c, axis X || a* for each phase in ")
+                ls_out.append(
+                    f"{phase_item.label:10} {m_chi[0, 0]:6.2f} {m_chi[1, 1]:6.2f} {m_chi[2, 2]:6.2f} {m_chi[0, 1]:6.2f} {m_chi[0, 2]:6.2f} {m_chi[1, 2]:6.2f}")
+            ls_out.append(
+                "----------------------------------------------------")
+            ls_out.append(
+                "The tensor is defined in Cartezian coordinate system")
+            ls_out.append(
+                "such as axis Z || c, axis X || a* for each phase in ")
             ls_out.append("[emu/(Oe g)].")
     return "\n".join(ls_out)
```

### Comparing `cryspy-0.7.3/cryspy/H_functions_global/simulations.py` & `cryspy-0.7.4/cryspy/H_functions_global/simulations.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/__init__.py` & `cryspy-0.7.4/cryspy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,24 +33,24 @@
 
 For more information please see the site: https://ikibalin.github.io/cryspy/
 """
 __author__ = 'Iurii KIBALIN'
 __copyright__   = "Copyright 2023, "
 __credits__ = ["Iurii KIBALIN", "Andrew SAZONOV", "Arsen GOUKASSOV"]
 __license__ = "GPL"
-__version__ = "0.7.3"
+__version__ = "0.7.4"
 __maintainer__ = "Iurii KIBALIN"
 __email__ = "yurikibalin@outlook.com"
 __status__ = "Development"
-__date__ = "08.03.2023"
+__date__ = "06.07.2023"
 name = "cryspy"
 
 
 from cryspy.B_parent_classes.cl_1_item import ItemN
-from cryspy.B_parent_classes.cl_2_loop import LoopN
+from cryspy.B_parent_classes.cl_2_loop import LoopN, get_prefix_of_loop
 from cryspy.B_parent_classes.cl_3_data import DataN
 from cryspy.B_parent_classes.cl_4_global import GlobalN
 
 
 from cryspy.A_functions_base.function_1_algebra import \
     calc_scalar_product_by_vectors,\
     calc_scalar_product_by_complex_vectors,\
@@ -201,14 +201,15 @@
         else:
             
             ls_out.append("    "+doc.strip().split("\n")[0])
     return "\n".join(ls_out)
 
 
 L_FUNCTION = [
+    get_prefix_of_loop,
     calc_scalar_product_by_vectors,
     calc_scalar_product_by_complex_vectors,
     calc_modulus_sq_by_complex_vector,
     calc_beta_by_u, vibration_constraints, apply_constraint_on_cell_by_type_cell,
     error_estimation_simplex,
     gammanu_to_tthphi, tthphi_to_gammanu, recal_int_to_tthphi_grid, recal_int_to_gammanu_grid,
     estimate_inversed_hessian_matrix,
```

### Comparing `cryspy-0.7.3/cryspy/__main__.py` & `cryspy-0.7.4/cryspy/__main__.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/procedure_mempy/mempy.py` & `cryspy-0.7.4/cryspy/procedure_mempy/mempy.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/procedure_mempy/mempy_by_dictionary.py` & `cryspy-0.7.4/cryspy/procedure_mempy/mempy_by_dictionary.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,19 +337,20 @@
                     f_sq, extinction_radius, extinction_mosaicity, volume_unit_cell, cos_2theta, wavelength,
                     extinction_model, flag_f_sq=False, flag_radius=False,
                     flag_mosaicity=False,
                     flag_volume_unit_cell=False,
                     flag_cos_2theta=False,
                     flag_wavelength=False)
 
+            axis_z = matrix_u[6:9] 
             iint_plus, iint_minus, dder_plus, dder_minus = calc_iint(
-                beam_polarization, flipper_efficiency, f_nucl, f_m_perp, matrix_u, func_extinction = func_extinction,
+                beam_polarization, flipper_efficiency, f_nucl, f_m_perp, axis_z, func_extinction = func_extinction,
                 flag_beam_polarization = False, flag_flipper_efficiency = False,
                 flag_f_nucl = False, flag_f_m_perp = True,
-                dict_in_out = dict_in_out, flag_use_precalculated_data = flag_use_precalculated_data)
+                dict_in_out = dict_in_out)
 
             diffrn_dict_in_out["flip_ratio"] = iint_plus/iint_minus
 
             der_int_plus_fm_perp_real = dder_plus["f_m_perp_real"]
             der_int_plus_fm_perp_imag = dder_plus["f_m_perp_imag"]
             der_int_minus_fm_perp_real = dder_minus["f_m_perp_real"]
             der_int_minus_fm_perp_imag = dder_minus["f_m_perp_imag"]
```

### Comparing `cryspy-0.7.3/cryspy/procedure_rhochi/rhochi.py` & `cryspy-0.7.4/cryspy/procedure_rhochi/rhochi.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/procedure_rhochi/rhochi_by_dictionary.py` & `cryspy-0.7.4/cryspy/procedure_rhochi/rhochi_by_dictionary.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/procedure_rhochi/rhochi_diffrn.py` & `cryspy-0.7.4/cryspy/procedure_rhochi/rhochi_diffrn.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,23 +205,24 @@
     flag_flip_ratio = flag_extincton or flags_beam_polarization or flags_flipper_efficiency or \
         flag_f_nucl or flag_f_m_perp or flags_c_lambda2 or flag_f_nucl_2hkl or flag_f_m_perp_2hkl
     if (flag_use_precalculated_data and not(flag_flip_ratio) 
             and "iint_plus" in dict_in_out_keys and "iint_minus" in dict_in_out_keys):
         iint_plus = dict_in_out["iint_plus"]
         iint_minus = dict_in_out["iint_minus"]
     else:
+        axis_z = matrix_u[6:9]
         iint_plus, iint_minus, dder_plus, dder_minus = calc_intensities_by_structure_factors(
-            beam_polarization, flipper_efficiency, f_nucl, f_m_perp, matrix_u,
+            beam_polarization, flipper_efficiency, f_nucl, f_m_perp, axis_z,
             func_extinction=func_extinction,
             c_lambda2=c_lambda2, f_nucl_2hkl=f_nucl_2hkl, f_m_perp_2hkl=f_m_perp_2hkl,
             flag_beam_polarization=flags_beam_polarization, flag_flipper_efficiency=flags_flipper_efficiency,
             flag_f_nucl=flag_f_nucl, flag_f_m_perp=flag_f_m_perp,
             flag_c_lambda2=flags_c_lambda2,
             flag_f_nucl_2hkl=flag_f_nucl_2hkl, flag_f_m_perp_2hkl=flag_f_m_perp_2hkl,
-            dict_in_out=dict_in_out, flag_use_precalculated_data=flag_use_precalculated_data)
+            dict_in_out=dict_in_out)
         if flag_dict:
             dict_in_out["iint_plus"] = iint_plus
             dict_in_out["iint_minus"] = iint_minus
 
     if flag_asymmetry:
         asymmetry_e = (flip_ratio_es[0] -1.)/(flip_ratio_es[0] + 1.)
         asymmetry_s = numpy.sqrt(2.)*flip_ratio_es[1] * numpy.sqrt(numpy.square(flip_ratio_es[0]) + 1.)/numpy.square(flip_ratio_es[0] + 1.)
```

### Comparing `cryspy-0.7.3/cryspy/procedure_rhochi/rhochi_pd.py` & `cryspy-0.7.4/cryspy/procedure_rhochi/rhochi_pd.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,15 +250,15 @@
         dict_in_out_phase["ttheta_hkl"] = ttheta_hkl + offset_ttheta
         if radiation[0].startswith("neutrons"):
             f_nucl, dder_f_nucl = calc_f_nucl_by_dictionary(
                 dict_crystal, dict_in_out_phase, flag_use_precalculated_data=flag_use_precalculated_data)
             flag_f_nucl = len(dder_f_nucl.keys()) > 0
 
             flag_para = False
-            if "atom_para_index" in dict_crystal_keys:
+            if (("atom_para_index" in dict_crystal_keys) and ("atom_para_susceptibility" in dict_crystal_keys)):
                 sft_ccs, dder_sft_ccs = calc_sft_ccs_by_dictionary(
                     dict_crystal, dict_in_out_phase, flag_use_precalculated_data=flag_use_precalculated_data)
                 flag_sft_ccs  = len(dder_sft_ccs.keys()) > 0
 
                 flag_matrix_t = flag_unit_cell_parameters
                 matrix_t, dder_matrix_t = calc_matrix_t(
                     index_hkl, unit_cell_parameters, flag_unit_cell_parameters=flag_unit_cell_parameters)
```

### Comparing `cryspy-0.7.3/cryspy/procedure_rhochi/rhochi_pd2d.py` & `cryspy-0.7.4/cryspy/procedure_rhochi/rhochi_pd2d.py`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/cryspy/procedure_rhochi/rhochi_tof.py` & `cryspy-0.7.4/cryspy/procedure_rhochi/rhochi_tof.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,20 +93,30 @@
     neutron_type = dict_tof["neutron_type"]
     if neutron_type == "thermal":
         zero = dict_tof["zero"]
         dtt1 = dict_tof["dtt1"]
         dtt2 = dict_tof["dtt2"]
         d = calc_d_by_time_for_thermal_neutrons(time, zero, dtt1, dtt2)
         d_min_max = calc_d_min_max_by_time_thermal_neutrons(time, zero, dtt1, dtt2)
+        flag_time = (
+            numpy.any(dict_tof["flags_zero"]) or
+            numpy.any(dict_tof["flags_dtt1"]) or
+            numpy.any(dict_tof["flags_dtt2"]))
     else: # epithermal
         zero = dict_tof["zero"]
         dtt1 = dict_tof["dtt1"]
         zerot = dict_tof["zerot"]
         dtt1t = dict_tof["dtt1t"]
         dtt2t = dict_tof["dtt2t"]
+        flag_time = (
+            numpy.any(dict_tof["flags_zero"]) or
+            numpy.any(dict_tof["flags_dtt1"]) or
+            numpy.any(dict_tof["flags_zerot"]) or
+            numpy.any(dict_tof["flags_dtt1t"]) or
+            numpy.any(dict_tof["flags_dtt2t"]))
         d_min_max = calc_d_min_max_by_time_epithermal_neutrons(time, zero, dtt1, zerot, dtt1t, dtt2t)
         raise AttributeError("Epithermal neutrons are not introudiced")
 
     sthovl_min = 0.5/d_min_max[1]
     sthovl_max = 0.5/d_min_max[0]
 
     if flag_dict:
@@ -165,27 +175,39 @@
 
     profile_peak_shape = dict_tof["profile_peak_shape"]
     if profile_peak_shape == "pseudo-Voigt":
         profile_alphas = dict_tof["profile_alphas"]
         profile_betas = dict_tof["profile_betas"]
         profile_sigmas = dict_tof["profile_sigmas"]
         profile_gammas = dict_tof["profile_gammas"]
+        flag_profile_shape = (
+            numpy.any(dict_tof["flags_profile_alphas"]) or
+            numpy.any(dict_tof["flags_profile_betas"]) or
+            numpy.any(dict_tof["flags_profile_sigmas"]) or
+            numpy.any(dict_tof["flags_profile_gammas"]))
     elif profile_peak_shape == "Gauss":
         profile_alphas = dict_tof["profile_alphas"]
         profile_betas = dict_tof["profile_betas"]
         profile_sigmas = dict_tof["profile_sigmas"]
+        flag_profile_shape = (
+            numpy.any(dict_tof["flags_profile_alphas"]) or
+            numpy.any(dict_tof["flags_profile_betas"]) or
+            numpy.any(dict_tof["flags_profile_sigmas"]))
     elif profile_peak_shape == "type0m":
-        profile_sigmas = dict_tof["profile_sigmas"]
-        profile_gammas = dict_tof["profile_gammas"]
         profile_alphas = dict_tof["profile_alphas"]
-        flags_profile_alphas = dict_tof["flags_profile_alphas"]
         profile_betas = dict_tof["profile_betas"]
-        flags_profile_betas = dict_tof["flags_profile_betas"]
+        profile_sigmas = dict_tof["profile_sigmas"]
+        profile_gammas = dict_tof["profile_gammas"]
         profile_rs = dict_tof["profile_rs"]
-        flags_profile_rs = dict_tof["flags_profile_rs"]
+        flag_profile_shape = (
+            numpy.any(dict_tof["flags_profile_alphas"]) or
+            numpy.any(dict_tof["flags_profile_betas"]) or
+            numpy.any(dict_tof["flags_profile_sigmas"]) or
+            numpy.any(dict_tof["flags_profile_gammas"]) or
+            numpy.any(dict_tof["flags_profile_rs"]))
         
     
     if "texture_name" in dict_tof_keys:
         flag_texture = True
         texture_name = dict_tof["texture_name"]
         texture_g1 = dict_tof["texture_g1"]
         texture_g2 = dict_tof["texture_g2"]
@@ -291,22 +313,27 @@
 
         flag_matrix_t = flag_unit_cell_parameters
         matrix_t, dder_matrix_t = calc_matrix_t(
             index_hkl, unit_cell_parameters, flag_unit_cell_parameters=flag_unit_cell_parameters)
 
         flag_tensor_sigma = flag_sft_ccs or flag_unit_cell_parameters
         tensor_sigma, dder_tensor_sigma = calc_m1_m2_m1t(matrix_t, sft_ccs, flag_m1=flag_sft_ccs, flag_m2=flag_unit_cell_parameters)
-
-        iint_plus, iint_minus, dder_plus, dder_minus = calc_powder_iint_1d_para(
-            f_nucl, tensor_sigma, beam_polarization, flipper_efficiency, magnetic_field,
-            flag_f_nucl=flag_f_nucl, flag_tensor_sigma=flag_tensor_sigma,
-            flag_polarization=flags_beam_polarization, flag_flipper=flags_flipper_efficiency)
         
-        dict_in_out_phase["iint_plus"] = iint_plus
-        dict_in_out_phase["iint_minus"] = iint_minus
+        flag_iint_plus_minus = flag_f_nucl or flag_tensor_sigma or flags_beam_polarization or flags_flipper_efficiency
+
+        if (("iint_plus" in dict_in_out_phase_keys) and ("iint_minu" in dict_in_out_phase_keys) and
+                        flag_use_precalculated_data and not(flag_iint_plus_minus)):
+            iint_plus, iint_minus = dict_in_out_phase["iint_plus"], dict_in_out_phase["iint_minus"]
+        else:
+            iint_plus, iint_minus, dder_plus, dder_minus = calc_powder_iint_1d_para(
+                f_nucl, tensor_sigma, beam_polarization, flipper_efficiency, magnetic_field,
+                flag_f_nucl=flag_f_nucl, flag_tensor_sigma=flag_tensor_sigma,
+                flag_polarization=flags_beam_polarization, flag_flipper=flags_flipper_efficiency)
+            dict_in_out_phase["iint_plus"] = iint_plus
+            dict_in_out_phase["iint_minus"] = iint_minus
 
         if flag_phase_texture:
             flag_texture_g1 = numpy.any(flags_texture_g1)
             flag_texture_g2 = numpy.any(flags_texture_g2)
             flag_texture_axis = numpy.any(flags_texture_axis)
             flag_hh = numpy.any([flag_texture_g1, flag_texture_g2, flag_texture_axis])
             if (flag_use_precalculated_data and 
@@ -317,41 +344,46 @@
                 preferred_orientation, dder_po = calc_preferred_orientation_tof(
                     index_hkl, texture_g1, texture_g2, texture_axis, unit_cell_parameters, 
                     flag_texture_g1=flag_texture_g1 and flag_calc_analytical_derivatives,
                     flag_texture_g2=flag_texture_g2 and flag_calc_analytical_derivatives,
                     flag_texture_axis=flag_texture_axis and flag_calc_analytical_derivatives)
                 dict_in_out_phase["preferred_orientation"] = preferred_orientation
         
-        if profile_peak_shape == "pseudo-Voigt":
-            profile_tof = calc_peak_shape_function(
-                profile_alphas, profile_betas, profile_sigmas,
-                d, time, time_hkl,
-                gammas=profile_gammas, size_g=0., size_l=0.,
-                strain_g=0.,strain_l=0., peak_shape=profile_peak_shape)
-        elif profile_peak_shape == "Gauss":
-            profile_tof = calc_peak_shape_function(
-                profile_alphas, profile_betas, profile_sigmas,
-                d, time, time_hkl,
-                gammas=None, size_g=0., size_l=0.,
-                strain_g=0.,strain_l=0., peak_shape=profile_peak_shape)
-        elif profile_peak_shape == "type0m":
-            time_2d = numpy.expand_dims(time, axis=1)
-            time_hkl_2d = numpy.expand_dims(time_hkl, axis=0)
-            d_hkl_2d = numpy.expand_dims(d_hkl, axis=0)
-            delta_t_2d = time_2d - time_hkl_2d
-            profile_sigmas_sq = numpy.square(profile_sigmas)
-            profile_tof = calc_profile_by_zcode_parameters(
-                delta_t_2d, d_hkl_2d,
-                profile_sigmas_sq[0], profile_sigmas_sq[1], profile_sigmas_sq[2],
-                profile_gammas[0], profile_gammas[1], profile_gammas[2],
-                profile_rs[0], profile_rs[1], profile_rs[2],
-                profile_alphas[0], profile_alphas[1],
-                profile_betas[0], profile_betas[1], profile_betas[2])
-                
-        dict_in_out_phase["profile_tof"] = profile_tof
+        flag_profile_tof = (flag_unit_cell_parameters or flag_time or flag_profile_shape)
+        if (("profile_tof" in dict_in_out_phase_keys) and
+                        flag_use_precalculated_data and not(flag_profile_tof)):
+            profile_tof = dict_in_out_phase["profile_tof"] 
+        else:
+            if profile_peak_shape == "pseudo-Voigt":
+                profile_tof = calc_peak_shape_function(
+                    profile_alphas, profile_betas, profile_sigmas,
+                    d, time, time_hkl,
+                    gammas=profile_gammas, size_g=0., size_l=0.,
+                    strain_g=0.,strain_l=0., peak_shape=profile_peak_shape)
+            elif profile_peak_shape == "Gauss":
+                profile_tof = calc_peak_shape_function(
+                    profile_alphas, profile_betas, profile_sigmas,
+                    d, time, time_hkl,
+                    gammas=None, size_g=0., size_l=0.,
+                    strain_g=0.,strain_l=0., peak_shape=profile_peak_shape)
+            elif profile_peak_shape == "type0m":
+                time_2d = numpy.expand_dims(time, axis=1)
+                time_hkl_2d = numpy.expand_dims(time_hkl, axis=0)
+                d_hkl_2d = numpy.expand_dims(d_hkl, axis=0)
+                delta_t_2d = time_2d - time_hkl_2d
+                profile_sigmas_sq = numpy.square(profile_sigmas)
+                profile_tof = calc_profile_by_zcode_parameters(
+                    delta_t_2d, d_hkl_2d,
+                    profile_sigmas_sq[0], profile_sigmas_sq[1], profile_sigmas_sq[2],
+                    profile_gammas[0], profile_gammas[1], profile_gammas[2],
+                    profile_rs[0], profile_rs[1], profile_rs[2],
+                    profile_alphas[0], profile_alphas[1],
+                    profile_betas[0], profile_betas[1], profile_betas[2])
+                    
+            dict_in_out_phase["profile_tof"] = profile_tof
 
 
         # flags_p_scale
         iint_m_plus = iint_plus * multiplicity_hkl
         iint_m_minus = iint_minus * multiplicity_hkl
 
         dict_in_out_phase["iint_plus_with_factors"] = 0.5 * p_scale * iint_m_plus*lorentz_factor*wavelength_4_hkl
```

### Comparing `cryspy-0.7.3/cryspy.egg-info/PKG-INFO` & `cryspy-0.7.4/cryspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryspy
-Version: 0.7.3
+Version: 0.7.4
 Summary: PNPD data analysis
 Home-page: https://github.com/ikibalin/cryspy
 Author: Iurii Kibalin
 Author-email: yurikibalin@outlook.com
 License: MIT License
 Keywords: Polarized Neutron Diffraction Data Analysis
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cryspy-0.7.3/cryspy.egg-info/SOURCES.txt` & `cryspy-0.7.4/cryspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/readme.rst` & `cryspy-0.7.4/readme.rst`

 * *Files identical despite different names*

### Comparing `cryspy-0.7.3/setup.py` & `cryspy-0.7.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-# Copyright (c) 2018-2019 Iurii Kibalin   
+# Copyright (c) 2018-2023 Iurii Kibalin   
 # https://github.com/ikibalin/cryspy  
 # All rights reserved.
 # 
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are
 # met:
 # 
@@ -37,15 +37,15 @@
 
 f_name = os.path.join(os.path.dirname(__file__), "readme.rst")
 with open(f_name, 'r') as f:
     long_description = f.read()
 
 setup(
     name='cryspy',
-    version='0.7.3',
+    version='0.7.4',
     description='PNPD data analysis',
     long_description = long_description,
     author='Iurii Kibalin',
     author_email='yurikibalin@outlook.com',
     url = 'https://github.com/ikibalin/cryspy',
     license          = 'MIT License',
     keywords         = 'Polarized Neutron Diffraction Data Analysis',
```

