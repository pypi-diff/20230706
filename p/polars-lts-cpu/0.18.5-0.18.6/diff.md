# Comparing `tmp/polars_lts_cpu-0.18.5.tar.gz` & `tmp/polars_lts_cpu-0.18.6.tar.gz`

## Comparing `polars_lts_cpu-0.18.5.tar` & `polars_lts_cpu-0.18.6.tar`

### file list

```diff
@@ -1,1264 +1,1270 @@
--rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/LICENSE
--rw-r--r--   0     1001      123      144 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/README.md
--rw-r--r--   0     1001      123     1975 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/array/default_arrays.rs
--rw-r--r--   0     1001      123     1791 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/array/fixed_size_list.rs
--rw-r--r--   0     1001      123     3773 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/array/get.rs
--rw-r--r--   0     1001      123     6664 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/array/list.rs
--rw-r--r--   0     1001      123     8165 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/array/mod.rs
--rw-r--r--   0     1001      123      878 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/array/null.rs
--rw-r--r--   0     1001      123     1125 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/array/slice.rs
--rw-r--r--   0     1001      123     2253 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/array/utf8.rs
--rw-r--r--   0     1001      123     2294 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/bit_util.rs
--rw-r--r--   0     1001      123       17 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/bitmap/mod.rs
--rw-r--r--   0     1001      123      819 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/bitmap/mutable.rs
--rw-r--r--   0     1001      123      370 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/add.rs
--rw-r--r--   0     1001      123     2181 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/commutative.rs
--rw-r--r--   0     1001      123     1482 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/div.rs
--rw-r--r--   0     1001      123     1028 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mod.rs
--rw-r--r--   0     1001      123     1177 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mul.rs
--rw-r--r--   0     1001      123      508 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/sub.rs
--rw-r--r--   0     1001      123       51 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/arithmetics/mod.rs
--rw-r--r--   0     1001      123        1 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/arity.rs
--rw-r--r--   0     1001      123      727 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/bitwise.rs
--rw-r--r--   0     1001      123     1206 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/cast.rs
--rw-r--r--   0     1001      123     3964 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/decimal.rs
--rw-r--r--   0     1001      123     1250 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/mod.rs
--rw-r--r--   0     1001      123      391 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/take/bitmap.rs
--rw-r--r--   0     1001      123     2767 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/take/boolean.rs
--rw-r--r--   0     1001      123     3489 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/take/fixed_size_list.rs
--rw-r--r--   0     1001      123    25290 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/take/mod.rs
--rw-r--r--   0     1001      123      797 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/tile.rs
--rw-r--r--   0     1001      123     1102 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/conversion.rs
--rw-r--r--   0     1001      123     1609 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/data_types.rs
--rw-r--r--   0     1001      123       25 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/error.rs
--rw-r--r--   0     1001      123       28 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/export.rs
--rw-r--r--   0     1001      123       26 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/floats/mod.rs
--rw-r--r--   0     1001      123     2066 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/floats/ord.rs
--rw-r--r--   0     1001      123     1273 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/index.rs
--rw-r--r--   0     1001      123      984 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/is_valid.rs
--rw-r--r--   0     1001      123     4783 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
--rw-r--r--   0     1001      123     1074 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/comparison.rs
--rw-r--r--   0     1001      123     1068 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/concatenate.rs
--rw-r--r--   0     1001      123     5161 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
--rw-r--r--   0     1001      123     1808 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
--rw-r--r--   0     1001      123    25065 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
--rw-r--r--   0     1001      123     1406 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/float.rs
--rw-r--r--   0     1001      123     4908 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/list.rs
--rw-r--r--   0     1001      123     1885 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
--rw-r--r--   0     1001      123     9783 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/mod.rs
--rw-r--r--   0     1001      123     3923 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
--rw-r--r--   0     1001      123     2019 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
--rw-r--r--   0     1001      123    16187 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
--rw-r--r--   0     1001      123     3848 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
--rw-r--r--   0     1001      123    13521 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
--rw-r--r--   0     1001      123     5684 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
--rw-r--r--   0     1001      123     7807 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
--rw-r--r--   0     1001      123     1879 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
--rw-r--r--   0     1001      123    14722 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
--rw-r--r--   0     1001      123    10055 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
--rw-r--r--   0     1001      123    11643 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
--rw-r--r--   0     1001      123     4821 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
--rw-r--r--   0     1001      123     6856 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
--rw-r--r--   0     1001      123     8109 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
--rw-r--r--   0     1001      123     4753 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/set.rs
--rw-r--r--   0     1001      123     4529 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
--rw-r--r--   0     1001      123     2948 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
--rw-r--r--   0     1001      123     5974 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
--rw-r--r--   0     1001      123      231 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
--rw-r--r--   0     1001      123      842 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/string.rs
--rw-r--r--   0     1001      123     2310 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs
--rw-r--r--   0     1001      123     4315 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs
--rw-r--r--   0     1001      123     2606 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs
--rw-r--r--   0     1001      123     3672 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/time.rs
--rw-r--r--   0     1001      123      341 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/lib.rs
--rw-r--r--   0     1001      123      496 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/prelude.rs
--rw-r--r--   0     1001      123      534 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/slice.rs
--rw-r--r--   0     1001      123      183 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/time_zone.rs
--rw-r--r--   0     1001      123      998 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
--rw-r--r--   0     1001      123     2821 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/trusted_len/mod.rs
--rw-r--r--   0     1001      123     2054 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
--rw-r--r--   0     1001      123      158 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/trusted_len/rev.rs
--rw-r--r--   0     1001      123     5233 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/utils.rs
--rw-r--r--   0        0        0     6264 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/LICENSE
--rw-r--r--   0     1001      123      358 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/README.md
--rw-r--r--   0     1001      123     1796 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/dot.rs
--rw-r--r--   0     1001      123     4479 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/dsl/eval.rs
--rw-r--r--   0     1001      123     7115 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/dsl/functions.rs
--rw-r--r--   0     1001      123      164 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/dsl/into.rs
--rw-r--r--   0     1001      123     6754 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/dsl/list.rs
--rw-r--r--   0     1001      123     2899 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/dsl/mod.rs
--rw-r--r--   0     1001      123     1182 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
--rw-r--r--   0     1001      123     9285 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/frame/csv.rs
--rw-r--r--   0     1001      123     4368 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
--rw-r--r--   0     1001      123     2261 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/frame/ipc.rs
--rw-r--r--   0     1001      123    49541 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/frame/mod.rs
--rw-r--r--   0     1001      123     3382 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/frame/ndjson.rs
--rw-r--r--   0     1001      123     2734 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/frame/parquet.rs
--rw-r--r--   0     1001      123     2892 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/frame/pivot.rs
--rw-r--r--   0     1001      123      459 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/frame/python.rs
--rw-r--r--   0     1001      123     6374 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/lib.rs
--rw-r--r--   0     1001      123     1049 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
--rw-r--r--   0     1001      123      776 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
--rw-r--r--   0     1001      123      670 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
--rw-r--r--   0     1001      123     1555 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
--rw-r--r--   0     1001      123     3986 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
--rw-r--r--   0     1001      123     4125 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
--rw-r--r--   0     1001      123    13599 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
--rw-r--r--   0     1001      123     4883 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
--rw-r--r--   0     1001      123     5859 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
--rw-r--r--   0     1001      123     6753 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
--rw-r--r--   0     1001      123     2045 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
--rw-r--r--   0     1001      123     1761 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
--rw-r--r--   0     1001      123     2854 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
--rw-r--r--   0     1001      123     1963 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
--rw-r--r--   0     1001      123     4303 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
--rw-r--r--   0     1001      123     1209 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
--rw-r--r--   0     1001      123     2421 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
--rw-r--r--   0     1001      123      548 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
--rw-r--r--   0     1001      123     2197 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
--rw-r--r--   0     1001      123     2015 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
--rw-r--r--   0     1001      123      663 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
--rw-r--r--   0     1001      123     4041 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
--rw-r--r--   0     1001      123      838 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
--rw-r--r--   0     1001      123     1335 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
--rw-r--r--   0     1001      123    21959 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
--rw-r--r--   0     1001      123     2689 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
--rw-r--r--   0     1001      123    18581 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
--rw-r--r--   0     1001      123    17674 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
--rw-r--r--   0     1001      123     2583 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/cache.rs
--rw-r--r--   0     1001      123     3153 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
--rw-r--r--   0     1001      123     6326 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
--rw-r--r--   0     1001      123     1996 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
--rw-r--r--   0     1001      123     5809 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
--rw-r--r--   0     1001      123     4131 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
--rw-r--r--   0     1001      123     5304 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
--rw-r--r--   0     1001      123    23566 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
--rw-r--r--   0     1001      123    10091 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
--rw-r--r--   0     1001      123     4332 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
--rw-r--r--   0     1001      123    13549 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
--rw-r--r--   0     1001      123     8331 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
--rw-r--r--   0     1001      123    14360 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
--rw-r--r--   0     1001      123    31970 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
--rw-r--r--   0     1001      123     2039 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
--rw-r--r--   0     1001      123      414 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/mod.rs
--rw-r--r--   0     1001      123     2005 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
--rw-r--r--   0     1001      123    24174 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
--rw-r--r--   0     1001      123    20552 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
--rw-r--r--   0     1001      123       87 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
--rw-r--r--   0     1001      123    10203 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/state.rs
--rw-r--r--   0     1001      123     2583 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/streaming/checks.rs
--rw-r--r--   0     1001      123     9280 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/streaming/construct_pipeline.rs
--rw-r--r--   0     1001      123    16847 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/streaming/convert_alp.rs
--rw-r--r--   0     1001      123      116 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
--rw-r--r--   0     1001      123     5827 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
--rw-r--r--   0     1001      123      722 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/prelude.rs
--rw-r--r--   0     1001      123    15000 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/aggregations.rs
--rw-r--r--   0     1001      123     2339 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/arity.rs
--rw-r--r--   0     1001      123     7276 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/cse.rs
--rw-r--r--   0     1001      123    12752 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/io.rs
--rw-r--r--   0     1001      123     4166 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/logical.rs
--rw-r--r--   0     1001      123     4273 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/mod.rs
--rw-r--r--   0     1001      123    15770 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
--rw-r--r--   0     1001      123     6772 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
--rw-r--r--   0     1001      123     3165 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/projection_queries.rs
--rw-r--r--   0     1001      123    47685 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/queries.rs
--rw-r--r--   0     1001      123     9519 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/streaming.rs
--rw-r--r--   0     1001      123     2893 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/tpch.rs
--rw-r--r--   0     1001      123     1028 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/utils.rs
--rw-r--r--   0        0        0     3552 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/LICENSE
--rw-r--r--   0     1001      123      132 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/README.md
--rw-r--r--   0     1001      123     2382 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/array/min_max.rs
--rw-r--r--   0     1001      123      267 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/array/mod.rs
--rw-r--r--   0     1001      123     1512 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/array/namespace.rs
--rw-r--r--   0     1001      123     4108 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/array/sum_mean.rs
--rw-r--r--   0     1001      123      234 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
--rw-r--r--   0     1001      123     3549 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
--rw-r--r--   0     1001      123    11023 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
--rw-r--r--   0     1001      123     1930 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/list/any_all.rs
--rw-r--r--   0     1001      123     1687 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/list/count.rs
--rw-r--r--   0     1001      123     2419 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
--rw-r--r--   0     1001      123     7861 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
--rw-r--r--   0     1001      123      644 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    19897 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
--rw-r--r--   0     1001      123    10391 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/list/sets.rs
--rw-r--r--   0     1001      123     7633 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
--rw-r--r--   0     1001      123     2435 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
--rw-r--r--   0     1001      123      545 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     9452 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
--rw-r--r--   0     1001      123     6795 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/set.rs
--rw-r--r--   0     1001      123     8781 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
--rw-r--r--   0     1001      123     8593 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
--rw-r--r--   0     1001      123     2345 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
--rw-r--r--   0     1001      123      514 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
--rw-r--r--   0     1001      123    14951 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
--rw-r--r--   0     1001      123     4053 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
--rw-r--r--   0     1001      123      439 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/sum.rs
--rw-r--r--   0     1001      123     2486 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/top_k.rs
--rw-r--r--   0     1001      123     7727 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
--rw-r--r--   0     1001      123    18232 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/frame/join/mod.rs
--rw-r--r--   0     1001      123     4291 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/frame/mod.rs
--rw-r--r--   0     1001      123    10257 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/frame/pivot/mod.rs
--rw-r--r--   0     1001      123    13486 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
--rw-r--r--   0     1001      123      237 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/lib.rs
--rw-r--r--   0     1001      123      290 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/prelude.rs
--rw-r--r--   0     1001      123       25 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/mod.rs
--rw-r--r--   0     1001      123     9623 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs
--rw-r--r--   0     1001      123      118 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/approx_algo/mod.rs
--rw-r--r--   0     1001      123     2016 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/approx_unique.rs
--rw-r--r--   0     1001      123    11866 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
--rw-r--r--   0     1001      123     3669 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/cut.rs
--rw-r--r--   0     1001      123     3688 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
--rw-r--r--   0     1001      123     5245 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/fused.rs
--rw-r--r--   0     1001      123     3423 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/is_first.rs
--rw-r--r--   0     1001      123     2975 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/is_unique.rs
--rw-r--r--   0     1001      123     3626 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/log.rs
--rw-r--r--   0     1001      123     1268 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     1769 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/rolling.rs
--rw-r--r--   0     1001      123     7642 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
--rw-r--r--   0     1001      123     2603 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
--rw-r--r--   0     1001      123     2067 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/various.rs
--rw-r--r--   0        0        0     5424 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/LICENSE
--rw-r--r--   0     1001      123       45 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/constants.rs
--rw-r--r--   0     1001      123    17253 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dot.rs
--rw-r--r--   0     1001      123     4789 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/arithmetic.rs
--rw-r--r--   0     1001      123     3992 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/arity.rs
--rw-r--r--   0     1001      123     1278 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/array.rs
--rw-r--r--   0     1001      123      935 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/binary.rs
--rw-r--r--   0     1001      123      650 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/cat.rs
--rw-r--r--   0     1001      123    10729 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/dt.rs
--rw-r--r--   0     1001      123     9542 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/expr.rs
--rw-r--r--   0     1001      123     8359 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/expr_dyn_fn.rs
--rw-r--r--   0     1001      123      753 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/from.rs
--rw-r--r--   0     1001      123       85 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/abs.rs
--rw-r--r--   0     1001      123     1431 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
--rw-r--r--   0     1001      123     1074 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/array.rs
--rw-r--r--   0     1001      123     1327 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
--rw-r--r--   0     1001      123     4221 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs
--rw-r--r--   0     1001      123     1910 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs
--rw-r--r--   0     1001      123     1216 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs
--rw-r--r--   0     1001      123      344 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
--rw-r--r--   0     1001      123      257 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/concat.rs
--rw-r--r--   0     1001      123     6125 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/correlation.rs
--rw-r--r--   0     1001      123     1593 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs
--rw-r--r--   0     1001      123    11615 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
--rw-r--r--   0     1001      123      782 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
--rw-r--r--   0     1001      123     2567 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
--rw-r--r--   0     1001      123      992 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/fused.rs
--rw-r--r--   0     1001      123     8997 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
--rw-r--r--   0     1001      123      581 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/log.rs
--rw-r--r--   0     1001      123    24898 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
--rw-r--r--   0     1001      123      462 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
--rw-r--r--   0     1001      123     3132 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
--rw-r--r--   0     1001      123     1410 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/random.rs
--rw-r--r--   0     1001      123     5146 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/range.rs
--rw-r--r--   0     1001      123      152 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
--rw-r--r--   0     1001      123      260 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/round.rs
--rw-r--r--   0     1001      123      200 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
--rw-r--r--   0     1001      123    19251 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
--rw-r--r--   0     1001      123      306 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
--rw-r--r--   0     1001      123     3812 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
--rw-r--r--   0     1001      123     1238 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
--rw-r--r--   0     1001      123      972 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
--rw-r--r--   0     1001      123    22249 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
--rw-r--r--   0     1001      123     1017 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
--rw-r--r--   0     1001      123     8438 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
--rw-r--r--   0     1001      123     6112 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
--rw-r--r--   0     1001      123      170 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/unique.rs
--rw-r--r--   0     1001      123     1155 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/arity.rs
--rw-r--r--   0     1001      123      611 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/coerce.rs
--rw-r--r--   0     1001      123     2717 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/concat.rs
--rw-r--r--   0     1001      123     4525 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/correlation.rs
--rw-r--r--   0     1001      123     8736 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/horizontal.rs
--rw-r--r--   0     1001      123     1042 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/index.rs
--rw-r--r--   0     1001      123      968 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/mod.rs
--rw-r--r--   0     1001      123     4129 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/range.rs
--rw-r--r--   0     1001      123     1308 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/selectors.rs
--rw-r--r--   0     1001      123     1973 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/syntactic_sugar.rs
--rw-r--r--   0     1001      123    11328 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/temporal.rs
--rw-r--r--   0     1001      123    12282 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/list.rs
--rw-r--r--   0     1001      123     4501 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/meta.rs
--rw-r--r--   0     1001      123    61388 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/mod.rs
--rw-r--r--   0     1001      123       40 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/names.rs
--rw-r--r--   0     1001      123     2658 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/options.rs
--rw-r--r--   0     1001      123     7017 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/python_udf.rs
--rw-r--r--   0     1001      123     1432 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/random.rs
--rw-r--r--   0     1001      123     1068 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/selector.rs
--rw-r--r--   0     1001      123    17626 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/string.rs
--rw-r--r--   0     1001      123     2715 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/struct_.rs
--rw-r--r--   0     1001      123       38 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/frame/mod.rs
--rw-r--r--   0     1001      123      933 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/frame/opt_state.rs
--rw-r--r--   0     1001      123      466 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/global.rs
--rw-r--r--   0     1001      123      175 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/lib.rs
--rw-r--r--   0     1001      123    10651 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
--rw-r--r--   0     1001      123    11920 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
--rw-r--r--   0     1001      123    25683 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/alp.rs
--rw-r--r--   0     1001      123     1622 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
--rw-r--r--   0     1001      123     1428 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/apply.rs
--rw-r--r--   0     1001      123    25639 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/builder.rs
--rw-r--r--   0     1001      123    29993 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/conversion.rs
--rw-r--r--   0     1001      123      301 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/debug.rs
--rw-r--r--   0     1001      123    15713 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/format.rs
--rw-r--r--   0     1001      123      895 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
--rw-r--r--   0     1001      123      137 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
--rw-r--r--   0     1001      123     1169 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
--rw-r--r--   0     1001      123    13288 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
--rw-r--r--   0     1001      123     1031 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/functions/python_udf.rs
--rw-r--r--   0     1001      123     1330 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
--rw-r--r--   0     1001      123    10157 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/iterator.rs
--rw-r--r--   0     1001      123    10559 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/lit.rs
--rw-r--r--   0     1001      123     8142 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/mod.rs
--rw-r--r--   0     1001      123     7416 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
--rw-r--r--   0     1001      123    15277 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
--rw-r--r--   0     1001      123     2889 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
--rw-r--r--   0     1001      123     3236 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
--rw-r--r--   0     1001      123     4663 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
--rw-r--r--   0     1001      123    14479 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
--rw-r--r--   0     1001      123     1556 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
--rw-r--r--   0     1001      123     6017 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/fused.rs
--rw-r--r--   0     1001      123     6778 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
--rw-r--r--   0     1001      123     1222 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
--rw-r--r--   0     1001      123    28901 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
--rw-r--r--   0     1001      123     2571 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
--rw-r--r--   0     1001      123    16171 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
--rw-r--r--   0     1001      123     1755 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
--rw-r--r--   0     1001      123     3930 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
--rw-r--r--   0     1001      123     1799 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
--rw-r--r--   0     1001      123     3269 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
--rw-r--r--   0     1001      123     2638 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
--rw-r--r--   0     1001      123    15874 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
--rw-r--r--   0     1001      123    26739 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
--rw-r--r--   0     1001      123     3707 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
--rw-r--r--   0     1001      123     2639 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
--rw-r--r--   0     1001      123     3509 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
--rw-r--r--   0     1001      123    27269 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
--rw-r--r--   0     1001      123     3496 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
--rw-r--r--   0     1001      123    13232 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
--rw-r--r--   0     1001      123     4181 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
--rw-r--r--   0     1001      123     9796 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
--rw-r--r--   0     1001      123    20215 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
--rw-r--r--   0     1001      123    10653 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/options.rs
--rw-r--r--   0     1001      123    19151 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/projection.rs
--rw-r--r--   0     1001      123     6144 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
--rw-r--r--   0     1001      123    13026 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/schema.rs
--rw-r--r--   0     1001      123     6699 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/tree_format.rs
--rw-r--r--   0     1001      123     3544 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/visitor/expr.rs
--rw-r--r--   0     1001      123      930 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/visitor/mod.rs
--rw-r--r--   0     1001      123     4408 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/visitor/visitors.rs
--rw-r--r--   0     1001      123      832 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/prelude.rs
--rw-r--r--   0     1001      123    12428 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/utils.rs
--rw-r--r--   0        0        0     2037 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/LICENSE
--rw-r--r--   0     1001      123      143 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/README.md
--rw-r--r--   0     1001      123     1018 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/base_utc_offset.rs
--rw-r--r--   0     1001      123     3569 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/date.rs
--rw-r--r--   0     1001      123     6465 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/datetime.rs
--rw-r--r--   0     1001      123     3305 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/duration.rs
--rw-r--r--   0     1001      123     5607 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/kernels.rs
--rw-r--r--   0     1001      123     1062 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/mod.rs
--rw-r--r--   0     1001      123     6759 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
--rw-r--r--   0     1001      123     2582 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
--rw-r--r--   0     1001      123    11122 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
--rw-r--r--   0     1001      123      413 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
--rw-r--r--   0     1001      123     4810 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
--rw-r--r--   0     1001      123     2372 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/time.rs
--rw-r--r--   0     1001      123    21334 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
--rw-r--r--   0     1001      123    18997 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
--rw-r--r--   0     1001      123     3975 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
--rw-r--r--   0     1001      123    11229 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
--rw-r--r--   0     1001      123     3340 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/date_range.rs
--rw-r--r--   0     1001      123      994 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/dst_offset.rs
--rw-r--r--   0     1001      123    34703 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/groupby/dynamic.rs
--rw-r--r--   0     1001      123       88 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/groupby/mod.rs
--rw-r--r--   0     1001      123      769 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/lib.rs
--rw-r--r--   0     1001      123     2976 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/month_end.rs
--rw-r--r--   0     1001      123     3365 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/month_start.rs
--rw-r--r--   0     1001      123      274 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/prelude.rs
--rw-r--r--   0     1001      123     1381 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/round.rs
--rw-r--r--   0     1001      123     3992 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/series/_trait.rs
--rw-r--r--   0     1001      123      136 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123      140 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/series/implementations/categoricals.rs
--rw-r--r--   0     1001      123      133 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/series/implementations/date.rs
--rw-r--r--   0     1001      123      137 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123      137 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123     1863 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     1792 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/series/implementations/integers.rs
--rw-r--r--   0     1001      123      133 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/series/implementations/list.rs
--rw-r--r--   0     1001      123      486 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123      155 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/series/implementations/object.rs
--rw-r--r--   0     1001      123      135 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123      133 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/series/implementations/time.rs
--rw-r--r--   0     1001      123      133 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123    12791 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/series/mod.rs
--rw-r--r--   0     1001      123     1443 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/truncate.rs
--rw-r--r--   0     1001      123     7619 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/upsample.rs
--rw-r--r--   0     1001      123     2511 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/utils.rs
--rw-r--r--   0     1001      123     1524 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/windows/bounds.rs
--rw-r--r--   0     1001      123     2672 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/windows/calendar.rs
--rw-r--r--   0     1001      123    25303 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/windows/duration.rs
--rw-r--r--   0     1001      123    20201 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/windows/groupby.rs
--rw-r--r--   0     1001      123      503 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/windows/mod.rs
--rw-r--r--   0     1001      123    23627 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/windows/test.rs
--rw-r--r--   0     1001      123    10657 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/windows/window.rs
--rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-row/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-row/LICENSE
--rw-r--r--   0     1001      123      137 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-row/README.md
--rw-r--r--   0     1001      123     2377 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-row/src/decode.rs
--rw-r--r--   0     1001      123    13364 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-row/src/encode.rs
--rw-r--r--   0     1001      123     7767 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-row/src/fixed.rs
--rw-r--r--   0     1001      123    13846 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-row/src/lib.rs
--rw-r--r--   0     1001      123     3019 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-row/src/row.rs
--rw-r--r--   0     1001      123      682 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-row/src/utils.rs
--rw-r--r--   0     1001      123     8679 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-row/src/variable.rs
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/LICENSE
--rw-r--r--   0     1001      123      165 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/README.md
--rw-r--r--   0     1001      123       98 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/mod.rs
--rw-r--r--   0     1001      123     1219 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/operators/filter.rs
--rw-r--r--   0     1001      123     4103 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/operators/function.rs
--rw-r--r--   0     1001      123      266 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/operators/mod.rs
--rw-r--r--   0     1001      123      682 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/operators/pass.rs
--rw-r--r--   0     1001      123      548 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
--rw-r--r--   0     1001      123     3553 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/operators/projection.rs
--rw-r--r--   0     1001      123     3559 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
--rw-r--r--   0     1001      123     6479 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
--rw-r--r--   0     1001      123    11288 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
--rw-r--r--   0     1001      123     1207 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
--rw-r--r--   0     1001      123     1888 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
--rw-r--r--   0     1001      123     4554 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
--rw-r--r--   0     1001      123     1746 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
--rw-r--r--   0     1001      123     5413 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
--rw-r--r--   0     1001      123     4951 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
--rw-r--r--   0     1001      123      211 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
--rw-r--r--   0     1001      123      856 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
--rw-r--r--   0     1001      123     4294 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
--rw-r--r--   0     1001      123     4109 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs
--rw-r--r--   0     1001      123     7404 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs
--rw-r--r--   0     1001      123    10554 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs
--rw-r--r--   0     1001      123     3589 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs
--rw-r--r--   0     1001      123     2767 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs
--rw-r--r--   0     1001      123     6326 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs
--rw-r--r--   0     1001      123     3116 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/source.rs
--rw-r--r--   0     1001      123    10194 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs
--rw-r--r--   0     1001      123     2119 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
--rw-r--r--   0     1001      123     4695 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
--rw-r--r--   0     1001      123     1887 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
--rw-r--r--   0     1001      123    20783 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
--rw-r--r--   0     1001      123    23825 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
--rw-r--r--   0     1001      123     2457 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
--rw-r--r--   0     1001      123     9239 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/io.rs
--rw-r--r--   0     1001      123     5451 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
--rw-r--r--   0     1001      123    12056 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
--rw-r--r--   0     1001      123    11658 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
--rw-r--r--   0     1001      123      178 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
--rw-r--r--   0     1001      123     2241 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
--rw-r--r--   0     1001      123      589 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
--rw-r--r--   0     1001      123     1492 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
--rw-r--r--   0     1001      123     1824 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
--rw-r--r--   0     1001      123     3108 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
--rw-r--r--   0     1001      123      130 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
--rw-r--r--   0     1001      123     6774 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
--rw-r--r--   0     1001      123     7279 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
--rw-r--r--   0     1001      123    11679 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
--rw-r--r--   0     1001      123     3908 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
--rw-r--r--   0     1001      123      526 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
--rw-r--r--   0     1001      123     5984 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sources/csv.rs
--rw-r--r--   0     1001      123     1231 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sources/frame.rs
--rw-r--r--   0     1001      123      987 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
--rw-r--r--   0     1001      123      366 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sources/mod.rs
--rw-r--r--   0     1001      123     4335 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
--rw-r--r--   0     1001      123     1146 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
--rw-r--r--   0     1001      123     1022 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sources/union.rs
--rw-r--r--   0     1001      123      448 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/expressions.rs
--rw-r--r--   0     1001      123      272 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/lib.rs
--rw-r--r--   0     1001      123      719 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/operators/chunks.rs
--rw-r--r--   0     1001      123      474 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/operators/context.rs
--rw-r--r--   0     1001      123      223 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/operators/mod.rs
--rw-r--r--   0     1001      123      514 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/operators/operator.rs
--rw-r--r--   0     1001      123      626 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/operators/sink.rs
--rw-r--r--   0     1001      123      241 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/operators/source.rs
--rw-r--r--   0     1001      123        1 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/pipeline/config.rs
--rw-r--r--   0     1001      123    21320 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/pipeline/convert.rs
--rw-r--r--   0     1001      123    20362 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
--rw-r--r--   0     1001      123     1155 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/pipeline/mod.rs
--rw-r--r--   0        0        0     4397 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/LICENSE
--rw-r--r--   0     1001      123      138 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/README.md
--rw-r--r--   0     1001      123     2383 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/avro/mod.rs
--rw-r--r--   0     1001      123     3608 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/avro/read.rs
--rw-r--r--   0     1001      123     2622 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/avro/write.rs
--rw-r--r--   0     1001      123     4505 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/cloud/adaptors.rs
--rw-r--r--   0     1001      123     9506 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/cloud/glob.rs
--rw-r--r--   0     1001      123     3089 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/cloud/mod.rs
--rw-r--r--   0     1001      123    28829 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/buffer.rs
--rw-r--r--   0     1001      123     1815 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/mod.rs
--rw-r--r--   0     1001      123    19446 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/parser.rs
--rw-r--r--   0     1001      123    22228 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/read.rs
--rw-r--r--   0     1001      123    10847 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
--rw-r--r--   0     1001      123    13939 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
--rw-r--r--   0     1001      123    30724 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/read_impl/mod.rs
--rw-r--r--   0     1001      123    11466 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/splitfields.rs
--rw-r--r--   0     1001      123    24531 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/utils.rs
--rw-r--r--   0     1001      123     2796 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/write.rs
--rw-r--r--   0     1001      123    14759 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/write_impl.rs
--rw-r--r--   0     1001      123      184 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/export.rs
--rw-r--r--   0     1001      123     7586 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/ipc/ipc_file.rs
--rw-r--r--   0     1001      123     9227 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/ipc/ipc_stream.rs
--rw-r--r--   0     1001      123     3253 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/ipc/mmap.rs
--rw-r--r--   0     1001      123      401 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/ipc/mod.rs
--rw-r--r--   0     1001      123     8287 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/ipc/write.rs
--rw-r--r--   0     1001      123     1471 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/ipc/write_async.rs
--rw-r--r--   0     1001      123    11044 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/json/mod.rs
--rw-r--r--   0     1001      123     4771 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/lib.rs
--rw-r--r--   0     1001      123     1969 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/mmap.rs
--rw-r--r--   0     1001      123     7228 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/ndjson/buffer.rs
--rw-r--r--   0     1001      123    11979 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/ndjson/core.rs
--rw-r--r--   0     1001      123       37 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/ndjson/mod.rs
--rw-r--r--   0     1001      123      273 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/options.rs
--rw-r--r--   0     1001      123     7360 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/parquet/async_impl.rs
--rw-r--r--   0     1001      123     3093 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/parquet/mmap.rs
--rw-r--r--   0     1001      123     3132 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/parquet/mod.rs
--rw-r--r--   0     1001      123     4784 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/parquet/predicates.rs
--rw-r--r--   0     1001      123     9623 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/parquet/read.rs
--rw-r--r--   0     1001      123    17321 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/parquet/read_impl.rs
--rw-r--r--   0     1001      123    10129 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/parquet/write.rs
--rw-r--r--   0     1001      123     5334 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/partition.rs
--rw-r--r--   0     1001      123     1455 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/predicates.rs
--rw-r--r--   0     1001      123      621 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/prelude.rs
--rw-r--r--   0     1001      123      417 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/tests.rs
--rw-r--r--   0     1001      123     4374 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/utils.rs
--rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/LICENSE
--rw-r--r--   0     1001      123      144 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/README.md
--rw-r--r--   0     1001      123     5158 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/arithmetic/decimal.rs
--rw-r--r--   0     1001      123     8275 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/arithmetic/mod.rs
--rw-r--r--   0     1001      123     9417 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/arithmetic/numeric.rs
--rw-r--r--   0     1001      123     3588 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/array/iterator.rs
--rw-r--r--   0     1001      123     2551 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/array/mod.rs
--rw-r--r--   0     1001      123     6448 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/bitwise.rs
--rw-r--r--   0     1001      123     2298 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
--rw-r--r--   0     1001      123     1207 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
--rw-r--r--   0     1001      123     4311 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/builder/fixed_size_list.rs
--rw-r--r--   0     1001      123     1556 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/builder/from.rs
--rw-r--r--   0     1001      123    20366 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/builder/list.rs
--rw-r--r--   0     1001      123     8969 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
--rw-r--r--   0     1001      123     1410 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
--rw-r--r--   0     1001      123     2291 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
--rw-r--r--   0     1001      123    17014 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/cast.rs
--rw-r--r--   0     1001      123    50501 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
--rw-r--r--   0     1001      123    10060 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
--rw-r--r--   0     1001      123      551 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/drop.rs
--rw-r--r--   0     1001      123      963 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/float.rs
--rw-r--r--   0     1001      123     7945 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/from.rs
--rw-r--r--   0     1001      123    42339 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
--rw-r--r--   0     1001      123     1453 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
--rw-r--r--   0     1001      123       28 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
--rw-r--r--   0     1001      123     1129 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
--rw-r--r--   0     1001      123       21 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
--rw-r--r--   0     1001      123     2347 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
--rw-r--r--   0     1001      123     7963 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
--rw-r--r--   0     1001      123     3242 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    19831 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
--rw-r--r--   0     1001      123     3688 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
--rw-r--r--   0     1001      123     4270 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
--rw-r--r--   0     1001      123    10219 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
--rw-r--r--   0     1001      123     1263 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
--rw-r--r--   0     1001      123      358 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
--rw-r--r--   0     1001      123      192 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
--rw-r--r--   0     1001      123     2731 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
--rw-r--r--   0     1001      123     2172 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
--rw-r--r--   0     1001      123      925 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
--rw-r--r--   0     1001      123     6805 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
--rw-r--r--   0     1001      123     1604 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/date.rs
--rw-r--r--   0     1001      123     4105 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
--rw-r--r--   0     1001      123     4443 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
--rw-r--r--   0     1001      123     2434 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
--rw-r--r--   0     1001      123     2556 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
--rw-r--r--   0     1001      123      476 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
--rw-r--r--   0     1001      123    15983 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
--rw-r--r--   0     1001      123     1182 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/time.rs
--rw-r--r--   0     1001      123    23273 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     9064 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ndarray.rs
--rw-r--r--   0     1001      123     4484 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/object/builder.rs
--rw-r--r--   0     1001      123     1547 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
--rw-r--r--   0     1001      123     3124 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
--rw-r--r--   0     1001      123     7054 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
--rw-r--r--   0     1001      123     3410 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
--rw-r--r--   0     1001      123      137 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
--rw-r--r--   0     1001      123     4419 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
--rw-r--r--   0     1001      123     4806 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/object/mod.rs
--rw-r--r--   0     1001      123     2956 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/object/registry.rs
--rw-r--r--   0     1001      123      272 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
--rw-r--r--   0     1001      123    32662 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
--rw-r--r--   0     1001      123    10025 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
--rw-r--r--   0     1001      123     2880 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
--rw-r--r--   0     1001      123    10551 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
--rw-r--r--   0     1001      123     4526 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/append.rs
--rw-r--r--   0     1001      123    28257 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
--rw-r--r--   0     1001      123    12799 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
--rw-r--r--   0     1001      123     6236 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
--rw-r--r--   0     1001      123    11537 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
--rw-r--r--   0     1001      123     1737 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
--rw-r--r--   0     1001      123     4801 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
--rw-r--r--   0     1001      123      908 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/decimal.rs
--rw-r--r--   0     1001      123     7056 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
--rw-r--r--   0     1001      123    19462 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
--rw-r--r--   0     1001      123     8691 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/explode_and_offsets.rs
--rw-r--r--   0     1001      123     9103 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
--rw-r--r--   0     1001      123    13777 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
--rw-r--r--   0     1001      123     6356 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
--rw-r--r--   0     1001      123     5876 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/full.rs
--rw-r--r--   0     1001      123        1 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
--rw-r--r--   0     1001      123    16797 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
--rw-r--r--   0     1001      123        1 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/len.rs
--rw-r--r--   0     1001      123     2658 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs
--rw-r--r--   0     1001      123    23299 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
--rw-r--r--   0     1001      123     2414 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
--rw-r--r--   0     1001      123      593 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
--rw-r--r--   0     1001      123     4375 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
--rw-r--r--   0     1001      123     2771 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
--rw-r--r--   0     1001      123    10267 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
--rw-r--r--   0     1001      123    12518 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/set.rs
--rw-r--r--   0     1001      123     7391 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
--rw-r--r--   0     1001      123     2299 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
--rw-r--r--   0     1001      123     5522 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
--rw-r--r--   0     1001      123     7543 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
--rw-r--r--   0     1001      123    28138 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
--rw-r--r--   0     1001      123      380 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
--rw-r--r--   0     1001      123    22089 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
--rw-r--r--   0     1001      123     7848 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
--rw-r--r--   0     1001      123      301 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
--rw-r--r--   0     1001      123    16256 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
--rw-r--r--   0     1001      123     6275 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
--rw-r--r--   0     1001      123     6072 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
--rw-r--r--   0     1001      123      459 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/tile.rs
--rw-r--r--   0     1001      123    12251 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
--rw-r--r--   0     1001      123    14620 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
--rw-r--r--   0     1001      123     5846 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
--rw-r--r--   0     1001      123     9093 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/random.rs
--rw-r--r--   0     1001      123     1875 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
--rw-r--r--   0     1001      123     2826 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
--rw-r--r--   0     1001      123    10336 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
--rw-r--r--   0     1001      123     3201 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
--rw-r--r--   0     1001      123     1061 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
--rw-r--r--   0     1001      123     3042 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
--rw-r--r--   0     1001      123      872 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/to_vec.rs
--rw-r--r--   0     1001      123     8114 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
--rw-r--r--   0     1001      123    25939 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
--rw-r--r--   0     1001      123     7944 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/cloud.rs
--rw-r--r--   0     1001      123     1549 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/config.rs
--rw-r--r--   0     1001      123     4469 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/datatypes/_serde.rs
--rw-r--r--   0     1001      123     2509 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/datatypes/aliases.rs
--rw-r--r--   0     1001      123    42659 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/datatypes/any_value.rs
--rw-r--r--   0     1001      123    13349 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/datatypes/dtype.rs
--rw-r--r--   0     1001      123     5609 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/datatypes/field.rs
--rw-r--r--   0     1001      123     8059 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/datatypes/mod.rs
--rw-r--r--   0     1001      123     2016 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/datatypes/time_unit.rs
--rw-r--r--   0     1001      123      118 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/doc/changelog/mod.rs
--rw-r--r--   0     1001      123      898 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
--rw-r--r--   0     1001      123      481 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
--rw-r--r--   0     1001      123      293 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
--rw-r--r--   0     1001      123      499 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
--rw-r--r--   0     1001      123      288 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
--rw-r--r--   0     1001      123     1071 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
--rw-r--r--   0     1001      123      819 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
--rw-r--r--   0     1001      123      596 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
--rw-r--r--   0     1001      123       43 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/doc/mod.rs
--rw-r--r--   0     1001      123       25 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/error.rs
--rw-r--r--   0     1001      123      263 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/export.rs
--rw-r--r--   0     1001      123    36573 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/fmt.rs
--rw-r--r--   0     1001      123     5177 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/arithmetic.rs
--rw-r--r--   0     1001      123     9916 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/asof_join/asof.rs
--rw-r--r--   0     1001      123    35743 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/asof_join/groups.rs
--rw-r--r--   0     1001      123     7168 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/asof_join/mod.rs
--rw-r--r--   0     1001      123      559 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/chunks.rs
--rw-r--r--   0     1001      123     5181 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/cross_join.rs
--rw-r--r--   0     1001      123    16760 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/explode.rs
--rw-r--r--   0     1001      123     1019 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/from.rs
--rw-r--r--   0     1001      123    19219 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
--rw-r--r--   0     1001      123     4113 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs
--rw-r--r--   0     1001      123     7749 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
--rw-r--r--   0     1001      123    40479 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
--rw-r--r--   0     1001      123     5634 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs
--rw-r--r--   0     1001      123      218 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/groupby/expr.rs
--rw-r--r--   0     1001      123    22901 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/groupby/hashing.rs
--rw-r--r--   0     1001      123    14380 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
--rw-r--r--   0     1001      123    39623 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/groupby/mod.rs
--rw-r--r--   0     1001      123    10637 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/groupby/perfect.rs
--rw-r--r--   0     1001      123    19780 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/groupby/proxy.rs
--rw-r--r--   0     1001      123     5416 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/args.rs
--rw-r--r--   0     1001      123    13172 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/mod.rs
--rw-r--r--   0     1001      123    22364 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
--rw-r--r--   0     1001      123     2400 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
--rw-r--r--   0     1001      123    17372 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
--rw-r--r--   0     1001      123     4677 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
--rw-r--r--   0     1001      123     6502 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
--rw-r--r--   0     1001      123     4665 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
--rw-r--r--   0     1001      123     3913 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
--rw-r--r--   0     1001      123    12313 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
--rw-r--r--   0     1001      123     3865 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/zip_outer.rs
--rw-r--r--   0     1001      123   126294 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/mod.rs
--rw-r--r--   0     1001      123    27652 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/row/av_buffer.rs
--rw-r--r--   0     1001      123     5183 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/row/dataframe.rs
--rw-r--r--   0     1001      123     5976 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/row/mod.rs
--rw-r--r--   0     1001      123     9875 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/row/transpose.rs
--rw-r--r--   0     1001      123     2811 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/top_k.rs
--rw-r--r--   0     1001      123     1388 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/upstream_traits.rs
--rw-r--r--   0     1001      123    10198 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/functions.rs
--rw-r--r--   0     1001      123     2149 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/hashing/fx.rs
--rw-r--r--   0     1001      123     1503 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/hashing/identity.rs
--rw-r--r--   0     1001      123      457 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/hashing/mod.rs
--rw-r--r--   0     1001      123     2684 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/hashing/partition.rs
--rw-r--r--   0     1001      123    17704 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/hashing/vector_hasher.rs
--rw-r--r--   0     1001      123     1896 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/lib.rs
--rw-r--r--   0     1001      123    15733 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/named_from.rs
--rw-r--r--   0     1001      123     2502 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/prelude.rs
--rw-r--r--   0     1001      123    18242 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/schema.rs
--rw-r--r--   0     1001      123     3995 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/serde/chunked_array.rs
--rw-r--r--   0     1001      123     1094 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/serde/df.rs
--rw-r--r--   0     1001      123     4734 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/serde/mod.rs
--rw-r--r--   0     1001      123     9938 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/serde/series.rs
--rw-r--r--   0     1001      123    18543 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/any_value.rs
--rw-r--r--   0     1001      123    28755 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
--rw-r--r--   0     1001      123      222 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/arithmetic/mod.rs
--rw-r--r--   0     1001      123     3546 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/arithmetic/owned.rs
--rw-r--r--   0     1001      123    19293 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/comparison.rs
--rw-r--r--   0     1001      123    29766 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/from.rs
--rw-r--r--   0     1001      123     6080 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/array.rs
--rw-r--r--   0     1001      123     9089 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/binary.rs
--rw-r--r--   0     1001      123    10835 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123    12800 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/categorical.rs
--rw-r--r--   0     1001      123    18214 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/dates_time.rs
--rw-r--r--   0     1001      123    15034 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123     7981 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/decimal.rs
--rw-r--r--   0     1001      123    14734 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123    14063 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     6078 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/list.rs
--rw-r--r--   0     1001      123    18396 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123     5522 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/null.rs
--rw-r--r--   0     1001      123     7939 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/object.rs
--rw-r--r--   0     1001      123    11788 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123     9607 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123     4471 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/into.rs
--rw-r--r--   0     1001      123     6241 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/iterator.rs
--rw-r--r--   0     1001      123    39074 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/mod.rs
--rw-r--r--   0     1001      123      853 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/diff.rs
--rw-r--r--   0     1001      123     5814 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/downcast.rs
--rw-r--r--   0     1001      123     3601 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/ewm.rs
--rw-r--r--   0     1001      123      413 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/extend.rs
--rw-r--r--   0     1001      123      562 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     5974 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/moment.rs
--rw-r--r--   0     1001      123     3181 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/null.rs
--rw-r--r--   0     1001      123     1347 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/pct_change.rs
--rw-r--r--   0     1001      123     4620 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/round.rs
--rw-r--r--   0     1001      123     5073 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/to_list.rs
--rw-r--r--   0     1001      123     1476 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/unique.rs
--rw-r--r--   0     1001      123    18408 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/series_trait.rs
--rw-r--r--   0     1001      123     2912 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/unstable.rs
--rw-r--r--   0     1001      123     7077 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/testing.rs
--rw-r--r--   0     1001      123      508 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/tests.rs
--rw-r--r--   0     1001      123     2492 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/utils/flatten.rs
--rw-r--r--   0     1001      123    31194 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/utils/mod.rs
--rw-r--r--   0     1001      123     1600 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/utils/series.rs
--rw-r--r--   0     1001      123    13201 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/utils/supertype.rs
--rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-json/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-json/LICENSE
--rw-r--r--   0     1001      123    16461 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-json/src/json/deserialize.rs
--rw-r--r--   0     1001      123     6564 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-json/src/json/infer_schema.rs
--rw-r--r--   0     1001      123      189 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-json/src/json/mod.rs
--rw-r--r--   0     1001      123       30 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-json/src/lib.rs
--rw-r--r--   0     1001      123     1198 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-json/src/ndjson/deserialize.rs
--rw-r--r--   0     1001      123     4808 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-json/src/ndjson/file.rs
--rw-r--r--   0     1001      123      143 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-json/src/ndjson/mod.rs
--rw-r--r--   0        0        0    10755 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/LICENSE
--rw-r--r--   0     1001      123     3472 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/Makefile
--rw-r--r--   0     1001      123      215 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/build.rs
--rw-r--r--   0     1001      123       78 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/clippy.toml
--rw-r--r--   0     1001      123    17614 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/src/docs/eager.rs
--rw-r--r--   0     1001      123     8815 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/src/docs/lazy.rs
--rw-r--r--   0     1001      123       50 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/src/docs/mod.rs
--rw-r--r--   0     1001      123     3806 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/src/docs/performance.rs
--rw-r--r--   0     1001      123       59 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/src/export.rs
--rw-r--r--   0     1001      123    19848 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/src/lib.rs
--rw-r--r--   0     1001      123      387 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/src/prelude.rs
--rw-r--r--   0     1001      123       54 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/src/sql.rs
--rw-r--r--   0     1001      123     4272 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/core/date_like.rs
--rw-r--r--   0     1001      123     2401 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/core/groupby.rs
--rw-r--r--   0     1001      123    17838 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/core/joins.rs
--rw-r--r--   0     1001      123      545 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/core/list.rs
--rw-r--r--   0     1001      123      198 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/core/mod.rs
--rw-r--r--   0     1001      123       24 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/core/ops/mod.rs
--rw-r--r--   0     1001      123      457 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/core/ops/take.rs
--rw-r--r--   0     1001      123     6259 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/core/pivot.rs
--rw-r--r--   0     1001      123     1102 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/core/random.rs
--rw-r--r--   0     1001      123    11096 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/core/rolling_window.rs
--rw-r--r--   0     1001      123     1093 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/core/series.rs
--rw-r--r--   0     1001      123      370 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/core/utils.rs
--rw-r--r--   0     1001      123    30423 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/io/csv.rs
--rw-r--r--   0     1001      123     4490 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/io/ipc_stream.rs
--rw-r--r--   0     1001      123     7043 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/io/json.rs
--rw-r--r--   0     1001      123      378 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/io/mod.rs
--rw-r--r--   0     1001      123      531 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/io/parquet.rs
--rw-r--r--   0     1001      123     1530 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/joins.rs
--rw-r--r--   0     1001      123     2452 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/aggregation.rs
--rw-r--r--   0     1001      123      821 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/cse.rs
--rw-r--r--   0     1001      123      500 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/explodes.rs
--rw-r--r--   0     1001      123     2278 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
--rw-r--r--   0     1001      123    10285 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
--rw-r--r--   0     1001      123     1065 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
--rw-r--r--   0     1001      123     1008 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
--rw-r--r--   0     1001      123      428 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
--rw-r--r--   0     1001      123      121 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
--rw-r--r--   0     1001      123      659 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
--rw-r--r--   0     1001      123    10657 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/expressions/window.rs
--rw-r--r--   0     1001      123      579 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/folds.rs
--rw-r--r--   0     1001      123      557 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/functions.rs
--rw-r--r--   0     1001      123     4482 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/groupby.rs
--rw-r--r--   0     1001      123     1681 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
--rw-r--r--   0     1001      123      691 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/mod.rs
--rw-r--r--   0     1001      123     5747 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
--rw-r--r--   0     1001      123     4483 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/projection_queries.rs
--rw-r--r--   0     1001      123     6584 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/queries.rs
--rw-r--r--   0     1001      123      151 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/main.rs
--rw-r--r--   0     1001      123    12591 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/schema.rs
--rw-r--r--   0     1001      123     1899 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/time/date_range.rs
--rw-r--r--   0     1001      123       16 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/time/mod.rs
--rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-error/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-error/LICENSE
--rw-r--r--   0     1001      123      145 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-error/README.md
--rw-r--r--   0     1001      123     7567 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-error/src/lib.rs
--rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-algo/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-algo/LICENSE
--rw-r--r--   0     1001      123      142 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-algo/README.md
--rw-r--r--   0     1001      123     7548 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-algo/src/algo.rs
--rw-r--r--   0     1001      123       88 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-algo/src/lib.rs
--rw-r--r--   0     1001      123       28 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-algo/src/prelude.rs
--rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/LICENSE
--rw-r--r--   0     1001      123      141 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/README.md
--rw-r--r--   0     1001      123      151 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/aliases.rs
--rw-r--r--   0     1001      123     2879 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/arena.rs
--rw-r--r--   0     1001      123     1379 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/atomic.rs
--rw-r--r--   0     1001      123     2659 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/cell.rs
--rw-r--r--   0     1001      123     1015 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/contention_pool.rs
--rw-r--r--   0     1001      123      509 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/error.rs
--rw-r--r--   0     1001      123      271 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/fmt.rs
--rw-r--r--   0     1001      123      763 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/functions.rs
--rw-r--r--   0     1001      123     2709 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
--rw-r--r--   0     1001      123       61 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/iter/mod.rs
--rw-r--r--   0     1001      123      503 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/lib.rs
--rw-r--r--   0     1001      123      573 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/macros.rs
--rw-r--r--   0     1001      123      282 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/mem.rs
--rw-r--r--   0     1001      123     2642 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/slice.rs
--rw-r--r--   0     1001      123     2467 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/sort.rs
--rw-r--r--   0     1001      123     1115 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/sync.rs
--rw-r--r--   0     1001      123      504 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/sys.rs
--rw-r--r--   0     1001      123      697 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/unwrap.rs
--rw-r--r--   0     1001      123     2024 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/vec.rs
--rw-r--r--   0     1001      123      616 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/wasm.rs
--rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/LICENSE
--rw-r--r--   0     1001      123      466 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/README.md
--rw-r--r--   0     1001      123    23373 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/src/context.rs
--rw-r--r--   0     1001      123    23921 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/src/functions.rs
--rw-r--r--   0     1001      123     2122 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/src/keywords.rs
--rw-r--r--   0     1001      123      239 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/src/lib.rs
--rw-r--r--   0     1001      123    20933 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/src/sql_expr.rs
--rw-r--r--   0     1001      123     4572 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/src/table_functions.rs
--rw-r--r--   0     1001      123     1682 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/functions_cumulative.rs
--rw-r--r--   0     1001      123     3063 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/functions_io.rs
--rw-r--r--   0     1001      123     1539 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/functions_math.rs
--rw-r--r--   0     1001      123      860 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/functions_meta.rs
--rw-r--r--   0     1001      123     2982 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/functions_string.rs
--rw-r--r--   0     1001      123     1056 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/iss_7436.rs
--rw-r--r--   0     1001      123      888 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/iss_7437.rs
--rw-r--r--   0     1001      123      652 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/iss_7440.rs
--rw-r--r--   0     1001      123      700 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/iss_8395.rs
--rw-r--r--   0     1001      123     1062 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/iss_8419.rs
--rw-r--r--   0     1001      123      982 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/ops_distinct_on.rs
--rw-r--r--   0     1001      123    15811 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/simple_exprs.rs
--rw-r--r--   0     1001      123     3976 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/statements.rs
--rw-r--r--   0        0        0     4544 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.5/Cargo.toml
--rw-r--r--   0     1001      123       76 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/.gitignore
--rw-r--r--   0     1001      123     1055 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/LICENSE
--rw-r--r--   0     1001      123     2414 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/Makefile
--rw-r--r--   0     1001      123    11696 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/README.md
--rw-r--r--   0     1001      123      651 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/build.rs
--rw-r--r--   0     1001      123       32 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/.gitignore
--rw-r--r--   0     1001      123      682 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/Makefile
--rw-r--r--   0     1001      123      318 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/_templates/api_redirect.html
--rw-r--r--   0     1001      123      151 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/_templates/autosummary/accessor.rst
--rw-r--r--   0     1001      123      160 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/_templates/autosummary/accessor_attribute.rst
--rw-r--r--   0     1001      123      168 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/_templates/autosummary/accessor_callable.rst
--rw-r--r--   0     1001      123      157 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/_templates/autosummary/accessor_method.rst
--rw-r--r--   0     1001      123      836 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      123       94 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/_templates/autosummary/class_without_autosummary.rst
--rw-r--r--   0     1001      123      406 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/_templates/sidebar-nav-bs.html
--rw-r--r--   0     1001      123      559 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/requirements-docs.txt
--rw-r--r--   0     1001      123     1164 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/run_live_docs_server.py
--rw-r--r--   0     1001      123     1567 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/_static/css/custom.css
--rw-r--r--   0     1001      123     7297 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/conf.py
--rw-r--r--   0     1001      123       51 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/index.rst
--rw-r--r--   0     1001      123     6767 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/api.rst
--rw-r--r--   0     1001      123     2069 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/config.rst
--rw-r--r--   0     1001      123      274 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/dataframe/aggregation.rst
--rw-r--r--   0     1001      123      221 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/dataframe/attributes.rst
--rw-r--r--   0     1001      123      142 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/dataframe/computation.rst
--rw-r--r--   0     1001      123      319 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/dataframe/descriptive.rst
--rw-r--r--   0     1001      123      319 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/dataframe/export.rst
--rw-r--r--   0     1001      123      464 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/dataframe/groupby.rst
--rw-r--r--   0     1001      123      379 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/dataframe/index.rst
--rw-r--r--   0     1001      123      189 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/dataframe/miscellaneous.rst
--rw-r--r--   0     1001      123     1538 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/dataframe/modify_select.rst
--rw-r--r--   0     1001      123      673 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/datatypes.rst
--rw-r--r--   0     1001      123      421 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/exceptions.rst
--rw-r--r--   0     1001      123      391 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/expressions/aggregation.rst
--rw-r--r--   0     1001      123      267 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/expressions/array.rst
--rw-r--r--   0     1001      123      309 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/expressions/binary.rst
--rw-r--r--   0     1001      123      338 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/expressions/boolean.rst
--rw-r--r--   0     1001      123      237 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/expressions/categories.rst
--rw-r--r--   0     1001      123      221 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/expressions/columns.rst
--rw-r--r--   0     1001      123     1095 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/expressions/computation.rst
--rw-r--r--   0     1001      123     1215 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/expressions/functions.rst
--rw-r--r--   0     1001      123      470 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/expressions/index.rst
--rw-r--r--   0     1001      123      830 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/expressions/list.rst
--rw-r--r--   0     1001      123      458 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/expressions/meta.rst
--rw-r--r--   0     1001      123      159 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/expressions/miscellaneous.rst
--rw-r--r--   0     1001      123      977 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/expressions/modify_select.rst
--rw-r--r--   0     1001      123      679 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/expressions/operators.rst
--rw-r--r--   0     1001      123      977 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/expressions/string.rst
--rw-r--r--   0     1001      123      254 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/expressions/struct.rst
--rw-r--r--   0     1001      123     1087 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/expressions/temporal.rst
--rw-r--r--   0     1001      123       98 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/expressions/window.rst
--rw-r--r--   0     1001      123      694 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/functions.rst
--rw-r--r--   0     1001      123      405 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/index.rst
--rw-r--r--   0     1001      123     1294 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/io.rst
--rw-r--r--   0     1001      123      277 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/lazyframe/aggregation.rst
--rw-r--r--   0     1001      123      179 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/lazyframe/attributes.rst
--rw-r--r--   0     1001      123      146 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/lazyframe/descriptive.rst
--rw-r--r--   0     1001      123      497 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/lazyframe/groupby.rst
--rw-r--r--   0     1001      123      354 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/lazyframe/index.rst
--rw-r--r--   0     1001      123      455 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/lazyframe/miscellaneous.rst
--rw-r--r--   0     1001      123     1013 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/lazyframe/modify_select.rst
--rw-r--r--   0     1001      123     3279 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/selectors.rst
--rw-r--r--   0     1001      123      358 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/series/aggregation.rst
--rw-r--r--   0     1001      123      277 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/series/array.rst
--rw-r--r--   0     1001      123      257 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/series/attributes.rst
--rw-r--r--   0     1001      123      321 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/series/binary.rst
--rw-r--r--   0     1001      123      117 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/series/boolean.rst
--rw-r--r--   0     1001      123      241 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/series/categories.rst
--rw-r--r--   0     1001      123     1103 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/series/computation.rst
--rw-r--r--   0     1001      123      744 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/series/descriptive.rst
--rw-r--r--   0     1001      123      240 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/series/export.rst
--rw-r--r--   0     1001      123      437 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/series/index.rst
--rw-r--r--   0     1001      123      894 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/series/list.rst
--rw-r--r--   0     1001      123      236 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/series/miscellaneous.rst
--rw-r--r--   0     1001      123     1077 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/series/modify_select.rst
--rw-r--r--   0     1001      123     1049 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/series/string.rst
--rw-r--r--   0     1001      123      421 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/series/struct.rst
--rw-r--r--   0     1001      123     1247 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/series/temporal.rst
--rw-r--r--   0     1001      123      503 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/sql.rst
--rw-r--r--   0     1001      123     8067 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/testing.rst
--rw-r--r--   0     1001      123      168 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/docs/source/reference/utils.rst
--rw-r--r--   0     1001      123     6370 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/__init__.py
--rw-r--r--   0     1001      123      280 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/_reexport.py
--rw-r--r--   0     1001      123    13229 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/api.py
--rw-r--r--   0     1001      123    29652 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/config.py
--rw-r--r--   0     1001      123    28090 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/convert.py
--rw-r--r--   0     1001      123       77 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/dataframe/__init__.py
--rw-r--r--   0     1001      123     5227 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/dataframe/_html.py
--rw-r--r--   0     1001      123   323980 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/dataframe/frame.py
--rw-r--r--   0     1001      123    41618 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/dataframe/groupby.py
--rw-r--r--   0     1001      123     2692 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/datatypes/__init__.py
--rw-r--r--   0     1001      123    17874 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/datatypes/classes.py
--rw-r--r--   0     1001      123     1690 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/datatypes/constants.py
--rw-r--r--   0     1001      123     4701 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/datatypes/constructor.py
--rw-r--r--   0     1001      123    15446 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/datatypes/convert.py
--rw-r--r--   0     1001      123     7358 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/dependencies.py
--rw-r--r--   0     1001      123     3792 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/exceptions.py
--rw-r--r--   0     1001      123       61 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/expr/__init__.py
--rw-r--r--   0     1001      123     3020 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/expr/array.py
--rw-r--r--   0     1001      123    10330 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/expr/binary.py
--rw-r--r--   0     1001      123     1698 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/expr/categorical.py
--rw-r--r--   0     1001      123    80633 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/expr/datetime.py
--rw-r--r--   0     1001      123   314741 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/expr/expr.py
--rw-r--r--   0     1001      123    30816 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/expr/list.py
--rw-r--r--   0     1001      123     4683 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/expr/meta.py
--rw-r--r--   0     1001      123    60086 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/expr/string.py
--rw-r--r--   0     1001      123     5426 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/expr/struct.py
--rw-r--r--   0     1001      123     2126 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/functions/__init__.py
--rw-r--r--   0     1001      123    16430 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/functions/as_datatype.py
--rw-r--r--   0     1001      123    18732 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/functions/eager.py
--rw-r--r--   0     1001      123    72418 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/functions/lazy.py
--rw-r--r--   0     1001      123    20012 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/functions/range.py
--rw-r--r--   0     1001      123     6043 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/functions/repeat.py
--rw-r--r--   0     1001      123     6051 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/functions/whenthen.py
--rw-r--r--   0     1001      123      952 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/__init__.py
--rw-r--r--   0     1001      123     6364 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/_utils.py
--rw-r--r--   0     1001      123      861 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/avro.py
--rw-r--r--   0     1001      123      144 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/csv/__init__.py
--rw-r--r--   0     1001      123     1072 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/csv/_utils.py
--rw-r--r--   0     1001      123     4681 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/csv/batched_reader.py
--rw-r--r--   0     1001      123    35482 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/csv/functions.py
--rw-r--r--   0     1001      123     6428 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/database.py
--rw-r--r--   0     1001      123    11047 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/delta.py
--rw-r--r--   0     1001      123       75 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/excel/__init__.py
--rw-r--r--   0     1001      123    18338 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/excel/_write_utils.py
--rw-r--r--   0     1001      123     6355 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/excel/functions.py
--rw-r--r--   0     1001      123      142 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/ipc/__init__.py
--rw-r--r--   0     1001      123     1227 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/ipc/anonymous_scan.py
--rw-r--r--   0     1001      123     5804 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/ipc/functions.py
--rw-r--r--   0     1001      123      510 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/json.py
--rw-r--r--   0     1001      123     2215 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/ndjson.py
--rw-r--r--   0     1001      123      170 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/parquet/__init__.py
--rw-r--r--   0     1001      123     1259 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/parquet/anonymous_scan.py
--rw-r--r--   0     1001      123     7177 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/parquet/functions.py
--rw-r--r--   0     1001      123      136 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/pyarrow_dataset/__init__.py
--rw-r--r--   0     1001      123     2186 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/pyarrow_dataset/anonymous_scan.py
--rw-r--r--   0     1001      123     3601 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/io/pyarrow_dataset/functions.py
--rw-r--r--   0     1001      123       77 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/lazyframe/__init__.py
--rw-r--r--   0     1001      123   172003 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/lazyframe/frame.py
--rw-r--r--   0     1001      123    25094 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/lazyframe/groupby.py
--rw-r--r--   0     1001      123        0 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/py.typed
--rw-r--r--   0     1001      123    38494 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/selectors.py
--rw-r--r--   0     1001      123       69 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/series/__init__.py
--rw-r--r--   0     1001      123     1572 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/series/_numpy.py
--rw-r--r--   0     1001      123     2515 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/series/array.py
--rw-r--r--   0     1001      123     1913 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/series/binary.py
--rw-r--r--   0     1001      123     1692 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/series/categorical.py
--rw-r--r--   0     1001      123    54653 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/series/datetime.py
--rw-r--r--   0     1001      123    16940 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/series/list.py
--rw-r--r--   0     1001      123   169195 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/series/series.py
--rw-r--r--   0     1001      123    38879 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/series/string.py
--rw-r--r--   0     1001      123     2542 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/series/struct.py
--rw-r--r--   0     1001      123     5361 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/series/utils.py
--rw-r--r--   0     1001      123     7559 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/slice.py
--rw-r--r--   0     1001      123       75 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/sql/__init__.py
--rw-r--r--   0     1001      123    17286 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/sql/context.py
--rw-r--r--   0     1001      123     4793 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/string_cache.py
--rw-r--r--   0     1001      123      362 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/testing/__init__.py
--rw-r--r--   0     1001      123     1060 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/testing/_private.py
--rw-r--r--   0     1001      123    16964 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/testing/asserts.py
--rw-r--r--   0     1001      123      898 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/testing/parametric/__init__.py
--rw-r--r--   0     1001      123    28187 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/testing/parametric/primitives.py
--rw-r--r--   0     1001      123     3371 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/testing/parametric/profiles.py
--rw-r--r--   0     1001      123    13165 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/testing/parametric/strategies.py
--rw-r--r--   0     1001      123     6460 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/type_aliases.py
--rw-r--r--   0     1001      123     1157 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/utils/__init__.py
--rw-r--r--   0     1001      123    56946 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/utils/_construction.py
--rw-r--r--   0     1001      123     4937 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/utils/_parse_expr_input.py
--rw-r--r--   0     1001      123      647 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/utils/_scan.py
--rw-r--r--   0     1001      123      579 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/utils/_wrap.py
--rw-r--r--   0     1001      123      683 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/utils/build_info.py
--rw-r--r--   0     1001      123     8702 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/utils/convert.py
--rw-r--r--   0     1001      123     7199 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/utils/decorators.py
--rw-r--r--   0     1001      123     1660 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/utils/meta.py
--rw-r--r--   0     1001      123      514 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/utils/polars_version.py
--rw-r--r--   0     1001      123     2509 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/utils/show_versions.py
--rw-r--r--   0     1001      123    13340 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/polars/utils/various.py
--rw-r--r--   0     1001      123     5370 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/pyproject.toml
--rw-r--r--   0     1001      123      756 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/requirements-dev.txt
--rw-r--r--   0     1001      123       70 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/requirements-lint.txt
--rw-r--r--   0     1001      123     1610 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/scripts/check_stacklevels.py
--rw-r--r--   0     1001      123    10980 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/apply/dataframe.rs
--rw-r--r--   0     1001      123     6428 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/apply/lazy.rs
--rw-r--r--   0     1001      123     8402 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/apply/mod.rs
--rw-r--r--   0     1001      123    90347 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/apply/series.rs
--rw-r--r--   0     1001      123       32 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/arrow_interop/mod.rs
--rw-r--r--   0     1001      123     1306 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/arrow_interop/to_py.rs
--rw-r--r--   0     1001      123     3902 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/arrow_interop/to_rust.rs
--rw-r--r--   0     1001      123     5250 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/batched_csv.rs
--rw-r--r--   0     1001      123    49804 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/conversion.rs
--rw-r--r--   0     1001      123    46152 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/dataframe.rs
--rw-r--r--   0     1001      123     3950 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/datatypes.rs
--rw-r--r--   0     1001      123     3506 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/error.rs
--rw-r--r--   0     1001      123      570 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/expr/array.rs
--rw-r--r--   0     1001      123     2080 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/expr/binary.rs
--rw-r--r--   0     1001      123      274 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/expr/categorical.rs
--rw-r--r--   0     1001      123     6206 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/expr/datetime.rs
--rw-r--r--   0     1001      123    35096 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/expr/general.rs
--rw-r--r--   0     1001      123     4693 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/expr/list.rs
--rw-r--r--   0     1001      123     3152 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/expr/meta.rs
--rw-r--r--   0     1001      123      870 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/expr/mod.rs
--rw-r--r--   0     1001      123     8366 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/expr/string.rs
--rw-r--r--   0     1001      123      467 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/expr/struct.rs
--rw-r--r--   0     1001      123     9482 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/file.rs
--rw-r--r--   0     1001      123     2777 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/functions/eager.rs
--rw-r--r--   0     1001      123     1657 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/functions/io.rs
--rw-r--r--   0     1001      123    11595 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/functions/lazy.rs
--rw-r--r--   0     1001      123     1312 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/functions/meta.rs
--rw-r--r--   0     1001      123      217 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/functions/misc.rs
--rw-r--r--   0     1001      123      102 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/functions/mod.rs
--rw-r--r--   0     1001      123      689 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/functions/range.rs
--rw-r--r--   0     1001      123     1474 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/functions/whenthen.rs
--rw-r--r--   0     1001      123    28073 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/lazyframe.rs
--rw-r--r--   0     1001      123     2670 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/lazygroupby.rs
--rw-r--r--   0     1001      123     8553 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/lib.rs
--rw-r--r--   0     1001      123       47 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/object.rs
--rw-r--r--   0     1001      123     2989 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/on_startup.rs
--rw-r--r--   0     1001      123      122 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/prelude.rs
--rw-r--r--   0     1001      123      435 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/py_modules.rs
--rw-r--r--   0     1001      123     1964 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/series/aggregation.rs
--rw-r--r--   0     1001      123     5406 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/series/arithmetic.rs
--rw-r--r--   0     1001      123     5138 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/series/comparison.rs
--rw-r--r--   0     1001      123     9077 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/series/construction.rs
--rw-r--r--   0     1001      123     8971 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/series/export.rs
--rw-r--r--   0     1001      123    26606 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/series/mod.rs
--rw-r--r--   0     1001      123     4569 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/series/numpy_ufunc.rs
--rw-r--r--   0     1001      123     4046 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/series/set_at_idx.rs
--rw-r--r--   0     1001      123     1036 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/sql.rs
--rw-r--r--   0     1001      123     2335 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/src/utils.rs
--rw-r--r--   0     1001      123     6165 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/README.md
--rw-r--r--   0     1001      123     2189 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/benchmark/groupby-datagen.R
--rw-r--r--   0     1001      123     7963 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/benchmark/run_h2oai_benchmark.py
--rw-r--r--   0     1001      123     6530 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/benchmark/test_release.py
--rw-r--r--   0     1001      123     4589 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/docs/run_doctest.py
--rw-r--r--   0     1001      123        0 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/parametric/__init__.py
--rw-r--r--   0     1001      123      179 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/parametric/conftest.py
--rw-r--r--   0     1001      123     3856 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/parametric/test_dataframe.py
--rw-r--r--   0     1001      123     2398 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/parametric/test_groupby_rolling.py
--rw-r--r--   0     1001      123     1692 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/parametric/test_lazyframe.py
--rw-r--r--   0     1001      123      976 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/parametric/test_lit.py
--rw-r--r--   0     1001      123     6853 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/parametric/test_series.py
--rw-r--r--   0     1001      123     8467 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/parametric/test_testing.py
--rw-r--r--   0     1001      123     1554 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/parametric/time_series/test_to_datetime.py
--rw-r--r--   0     1001      123        0 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/__init__.py
--rw-r--r--   0     1001      123     3382 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/conftest.py
--rw-r--r--   0     1001      123       86 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/datatypes/__init__.py
--rw-r--r--   0     1001      123     1285 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/datatypes/test_array.py
--rw-r--r--   0     1001      123      847 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/datatypes/test_binary.py
--rw-r--r--   0     1001      123     1420 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/datatypes/test_bool.py
--rw-r--r--   0     1001      123    13609 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/datatypes/test_categorical.py
--rw-r--r--   0     1001      123     5222 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/datatypes/test_decimal.py
--rw-r--r--   0     1001      123      549 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/datatypes/test_duration.py
--rw-r--r--   0     1001      123      423 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/datatypes/test_integer.py
--rw-r--r--   0     1001      123    14052 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/datatypes/test_list.py
--rw-r--r--   0     1001      123      284 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/datatypes/test_null.py
--rw-r--r--   0     1001      123     3028 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/datatypes/test_object.py
--rw-r--r--   0     1001      123    27697 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/datatypes/test_struct.py
--rw-r--r--   0     1001      123    87698 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/datatypes/test_temporal.py
--rw-r--r--   0     1001      123      418 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/datatypes/test_time.py
--rw-r--r--   0     1001      123        0 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/functions/__init__.py
--rw-r--r--   0     1001      123    13970 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/functions/test_as_datatype.py
--rw-r--r--   0     1001      123      480 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/functions/test_concat.py
--rw-r--r--   0     1001      123    15574 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/functions/test_functions.py
--rw-r--r--   0     1001      123    30418 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/functions/test_range.py
--rw-r--r--   0     1001      123     3847 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/functions/test_repeat.py
--rw-r--r--   0     1001      123      218 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/conftest.py
--rw-r--r--   0     1001      123       16 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
--rw-r--r--   0     1001      123       16 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
--rw-r--r--   0     1001      123      905 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123      936 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
--rw-r--r--   0     1001      123      972 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
--rw-r--r--   0     1001      123      690 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
--rw-r--r--   0     1001      123        0 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/empty.csv
--rw-r--r--   0     1001      123     5959 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/example.xlsx
--rw-r--r--   0     1001      123      457 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/foods1.csv
--rw-r--r--   0     1001      123     2351 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/foods1.ipc
--rw-r--r--   0     1001      123     1713 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/foods1.ndjson
--rw-r--r--   0     1001      123     1427 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/foods1.parquet
--rw-r--r--   0     1001      123      455 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/foods2.csv
--rw-r--r--   0     1001      123     2351 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/foods2.ipc
--rw-r--r--   0     1001      123     1711 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/foods2.ndjson
--rw-r--r--   0     1001      123     1916 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/foods2.parquet
--rw-r--r--   0     1001      123      455 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/foods3.csv
--rw-r--r--   0     1001      123      457 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/foods4.csv
--rw-r--r--   0     1001      123      452 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/foods5.csv
--rw-r--r--   0     1001      123       49 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/gzipped.csv
--rw-r--r--   0     1001      123       57 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/small.csv
--rw-r--r--   0     1001      123      756 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/files/small.parquet
--rw-r--r--   0     1001      123     1884 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/test_avro.py
--rw-r--r--   0     1001      123    41164 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/test_csv.py
--rw-r--r--   0     1001      123     6271 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/test_database.py
--rw-r--r--   0     1001      123     6172 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/test_delta.py
--rw-r--r--   0     1001      123    11169 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/test_excel.py
--rw-r--r--   0     1001      123     5483 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/test_ipc.py
--rw-r--r--   0     1001      123     4389 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/test_json.py
--rw-r--r--   0     1001      123     7379 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/test_lazy_csv.py
--rw-r--r--   0     1001      123     2060 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/test_lazy_ipc.py
--rw-r--r--   0     1001      123     2867 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/test_lazy_json.py
--rw-r--r--   0     1001      123    11145 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/test_lazy_parquet.py
--rw-r--r--   0     1001      123     2012 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/test_other.py
--rw-r--r--   0     1001      123    14157 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/test_parquet.py
--rw-r--r--   0     1001      123      612 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/test_pickle.py
--rw-r--r--   0     1001      123     3706 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/io/test_pyarrow_dataset.py
--rw-r--r--   0     1001      123      509 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/namespaces/__init__.py
--rw-r--r--   0     1001      123      589 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/namespaces/test_array.py
--rw-r--r--   0     1001      123     3218 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/namespaces/test_binary.py
--rw-r--r--   0     1001      123     2489 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/namespaces/test_categorical.py
--rw-r--r--   0     1001      123    23231 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/namespaces/test_datetime.py
--rw-r--r--   0     1001      123    15154 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/namespaces/test_list.py
--rw-r--r--   0     1001      123     2472 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/namespaces/test_meta.py
--rw-r--r--   0     1001      123    24050 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/namespaces/test_string.py
--rw-r--r--   0     1001      123    20819 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/namespaces/test_strptime.py
--rw-r--r--   0     1001      123      982 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/namespaces/test_struct.py
--rw-r--r--   0     1001      123       85 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/__init__.py
--rw-r--r--   0     1001      123     8008 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_aggregations.py
--rw-r--r--   0     1001      123    10613 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_apply.py
--rw-r--r--   0     1001      123     6896 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_arithmetic.py
--rw-r--r--   0     1001      123     4940 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_comparison.py
--rw-r--r--   0     1001      123     3275 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_drop.py
--rw-r--r--   0     1001      123     8813 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_explode.py
--rw-r--r--   0     1001      123     3664 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_filter.py
--rw-r--r--   0     1001      123     1801 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_folds.py
--rw-r--r--   0     1001      123    25037 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_groupby.py
--rw-r--r--   0     1001      123     7649 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_groupby_rolling.py
--rw-r--r--   0     1001      123     2983 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_is_in.py
--rw-r--r--   0     1001      123    18993 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_join.py
--rw-r--r--   0     1001      123    14952 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_join_asof.py
--rw-r--r--   0     1001      123      643 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_melt.py
--rw-r--r--   0     1001      123    10253 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_pivot.py
--rw-r--r--   0     1001      123     3187 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_random.py
--rw-r--r--   0     1001      123    24274 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_rolling.py
--rw-r--r--   0     1001      123     2389 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_select.py
--rw-r--r--   0     1001      123    20770 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_sort.py
--rw-r--r--   0     1001      123     6121 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_statistics.py
--rw-r--r--   0     1001      123     4130 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_transpose.py
--rw-r--r--   0     1001      123      771 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_unique.py
--rw-r--r--   0     1001      123    11644 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_window.py
--rw-r--r--   0     1001      123     5480 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/operations/test_with_columns.py
--rw-r--r--   0     1001      123        0 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/streaming/__init__.py
--rw-r--r--   0     1001      123      196 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/streaming/conftest.py
--rw-r--r--   0     1001      123      908 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/streaming/test_ooc.py
--rw-r--r--   0     1001      123    19789 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/streaming/test_streaming.py
--rw-r--r--   0     1001      123     4831 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_api.py
--rw-r--r--   0     1001      123     1969 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_arity.py
--rw-r--r--   0     1001      123    20397 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_cfg.py
--rw-r--r--   0     1001      123    43560 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_constructors.py
--rw-r--r--   0     1001      123      454 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_context.py
--rw-r--r--   0     1001      123     2626 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_cse.py
--rw-r--r--   0     1001      123     5191 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_datatypes.py
--rw-r--r--   0     1001      123   120452 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_df.py
--rw-r--r--   0     1001      123     2741 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_empty.py
--rw-r--r--   0     1001      123    19664 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_errors.py
--rw-r--r--   0     1001      123     2741 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_expr_multi_cols.py
--rw-r--r--   0     1001      123    33619 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_exprs.py
--rw-r--r--   0     1001      123     3516 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_fmt.py
--rw-r--r--   0     1001      123     3512 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_interchange.py
--rw-r--r--   0     1001      123    38530 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_interop.py
--rw-r--r--   0     1001      123    49654 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_lazy.py
--rw-r--r--   0     1001      123     2463 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_polars_import.py
--rw-r--r--   0     1001      123     4883 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_predicates.py
--rw-r--r--   0     1001      123     7572 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_projections.py
--rw-r--r--   0     1001      123    11551 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_queries.py
--rw-r--r--   0     1001      123     8100 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_rows.py
--rw-r--r--   0     1001      123    13961 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_schema.py
--rw-r--r--   0     1001      123    12341 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_selectors.py
--rw-r--r--   0     1001      123     4107 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_serde.py
--rw-r--r--   0     1001      123    82889 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_series.py
--rw-r--r--   0     1001      123      657 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_single.py
--rw-r--r--   0     1001      123    16616 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_sql.py
--rw-r--r--   0     1001      123    35314 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/test_testing.py
--rw-r--r--   0     1001      123       41 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/utils/__init__.py
--rw-r--r--   0     1001      123      306 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/utils/test_build_info.py
--rw-r--r--   0     1001      123     2855 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/utils/test_parse_expr_input.py
--rw-r--r--   0     1001      123      247 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/utils/test_show_versions.py
--rw-r--r--   0     1001      123     5026 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/tests/unit/utils/test_utils.py
--rw-r--r--   0     1001      123    65129 2023-07-05 14:01:02.000000 polars_lts_cpu-0.18.5/Cargo.lock
--rw-r--r--   0        0        0    14286 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.5/PKG-INFO
+-rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-algo/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-algo/LICENSE
+-rw-r--r--   0     1001      123      142 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-algo/README.md
+-rw-r--r--   0     1001      123     7548 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-algo/src/algo.rs
+-rw-r--r--   0     1001      123       88 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-algo/src/lib.rs
+-rw-r--r--   0     1001      123       28 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-algo/src/prelude.rs
+-rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-json/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-json/LICENSE
+-rw-r--r--   0     1001      123    16461 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-json/src/json/deserialize.rs
+-rw-r--r--   0     1001      123     6564 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-json/src/json/infer_schema.rs
+-rw-r--r--   0     1001      123      189 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-json/src/json/mod.rs
+-rw-r--r--   0     1001      123       30 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-json/src/lib.rs
+-rw-r--r--   0     1001      123     1198 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-json/src/ndjson/deserialize.rs
+-rw-r--r--   0     1001      123     4808 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-json/src/ndjson/file.rs
+-rw-r--r--   0     1001      123      143 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-json/src/ndjson/mod.rs
+-rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/LICENSE
+-rw-r--r--   0     1001      123      466 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/README.md
+-rw-r--r--   0     1001      123    23373 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/src/context.rs
+-rw-r--r--   0     1001      123    23921 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/src/functions.rs
+-rw-r--r--   0     1001      123     2122 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/src/keywords.rs
+-rw-r--r--   0     1001      123      239 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/src/lib.rs
+-rw-r--r--   0     1001      123    20933 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/src/sql_expr.rs
+-rw-r--r--   0     1001      123     4572 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/src/table_functions.rs
+-rw-r--r--   0     1001      123     1682 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/functions_cumulative.rs
+-rw-r--r--   0     1001      123     3063 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/functions_io.rs
+-rw-r--r--   0     1001      123     1539 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/functions_math.rs
+-rw-r--r--   0     1001      123      860 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/functions_meta.rs
+-rw-r--r--   0     1001      123     2982 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/functions_string.rs
+-rw-r--r--   0     1001      123     1056 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/iss_7436.rs
+-rw-r--r--   0     1001      123      888 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/iss_7437.rs
+-rw-r--r--   0     1001      123      652 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/iss_7440.rs
+-rw-r--r--   0     1001      123      700 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/iss_8395.rs
+-rw-r--r--   0     1001      123     1062 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/iss_8419.rs
+-rw-r--r--   0     1001      123      982 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/ops_distinct_on.rs
+-rw-r--r--   0     1001      123    15811 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/simple_exprs.rs
+-rw-r--r--   0     1001      123     3976 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/statements.rs
+-rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/LICENSE
+-rw-r--r--   0     1001      123      144 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/README.md
+-rw-r--r--   0     1001      123     5158 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/arithmetic/decimal.rs
+-rw-r--r--   0     1001      123     8275 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/arithmetic/mod.rs
+-rw-r--r--   0     1001      123     9417 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/arithmetic/numeric.rs
+-rw-r--r--   0     1001      123     3588 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/array/iterator.rs
+-rw-r--r--   0     1001      123     2551 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/array/mod.rs
+-rw-r--r--   0     1001      123     6448 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/bitwise.rs
+-rw-r--r--   0     1001      123     2298 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
+-rw-r--r--   0     1001      123     1207 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
+-rw-r--r--   0     1001      123     4311 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/fixed_size_list.rs
+-rw-r--r--   0     1001      123     1556 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/from.rs
+-rw-r--r--   0     1001      123     5762 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/list/anonymous.rs
+-rw-r--r--   0     1001      123     4418 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/list/binary.rs
+-rw-r--r--   0     1001      123     2374 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/list/boolean.rs
+-rw-r--r--   0     1001      123     1392 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/list/categorical.rs
+-rw-r--r--   0     1001      123     1575 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/list/dtypes.rs
+-rw-r--r--   0     1001      123     4953 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/list/mod.rs
+-rw-r--r--   0     1001      123     3506 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/list/primitive.rs
+-rw-r--r--   0     1001      123     8969 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
+-rw-r--r--   0     1001      123     1410 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
+-rw-r--r--   0     1001      123     2291 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
+-rw-r--r--   0     1001      123    17014 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/cast.rs
+-rw-r--r--   0     1001      123    50501 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
+-rw-r--r--   0     1001      123    10060 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
+-rw-r--r--   0     1001      123      551 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/drop.rs
+-rw-r--r--   0     1001      123      963 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/float.rs
+-rw-r--r--   0     1001      123     7945 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/from.rs
+-rw-r--r--   0     1001      123    42339 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
+-rw-r--r--   0     1001      123     1453 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
+-rw-r--r--   0     1001      123       28 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
+-rw-r--r--   0     1001      123     1129 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
+-rw-r--r--   0     1001      123       21 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
+-rw-r--r--   0     1001      123     2347 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
+-rw-r--r--   0     1001      123     7963 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
+-rw-r--r--   0     1001      123     3242 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    19831 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
+-rw-r--r--   0     1001      123     3688 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
+-rw-r--r--   0     1001      123     5693 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
+-rw-r--r--   0     1001      123    10219 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
+-rw-r--r--   0     1001      123     1263 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
+-rw-r--r--   0     1001      123      358 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
+-rw-r--r--   0     1001      123      192 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
+-rw-r--r--   0     1001      123     2731 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
+-rw-r--r--   0     1001      123     2172 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
+-rw-r--r--   0     1001      123      925 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
+-rw-r--r--   0     1001      123     6805 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
+-rw-r--r--   0     1001      123     1604 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/date.rs
+-rw-r--r--   0     1001      123     4105 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
+-rw-r--r--   0     1001      123     4443 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
+-rw-r--r--   0     1001      123     2434 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
+-rw-r--r--   0     1001      123     2556 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
+-rw-r--r--   0     1001      123      476 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
+-rw-r--r--   0     1001      123    15983 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/time.rs
+-rw-r--r--   0     1001      123    23309 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     9064 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ndarray.rs
+-rw-r--r--   0     1001      123     4484 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/object/builder.rs
+-rw-r--r--   0     1001      123     1547 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
+-rw-r--r--   0     1001      123     3097 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
+-rw-r--r--   0     1001      123     7054 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
+-rw-r--r--   0     1001      123     3410 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
+-rw-r--r--   0     1001      123      137 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
+-rw-r--r--   0     1001      123     4419 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
+-rw-r--r--   0     1001      123     4806 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/object/mod.rs
+-rw-r--r--   0     1001      123     2956 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/object/registry.rs
+-rw-r--r--   0     1001      123      272 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
+-rw-r--r--   0     1001      123    32662 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
+-rw-r--r--   0     1001      123    10025 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
+-rw-r--r--   0     1001      123     2880 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
+-rw-r--r--   0     1001      123    10551 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
+-rw-r--r--   0     1001      123     4526 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/append.rs
+-rw-r--r--   0     1001      123    28257 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
+-rw-r--r--   0     1001      123    12799 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
+-rw-r--r--   0     1001      123     6236 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
+-rw-r--r--   0     1001      123    11537 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
+-rw-r--r--   0     1001      123     1737 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
+-rw-r--r--   0     1001      123     4801 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
+-rw-r--r--   0     1001      123      908 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/decimal.rs
+-rw-r--r--   0     1001      123     7056 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
+-rw-r--r--   0     1001      123    19462 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
+-rw-r--r--   0     1001      123     8691 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/explode_and_offsets.rs
+-rw-r--r--   0     1001      123     9103 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
+-rw-r--r--   0     1001      123    13777 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
+-rw-r--r--   0     1001      123     6356 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
+-rw-r--r--   0     1001      123     5886 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/full.rs
+-rw-r--r--   0     1001      123        1 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
+-rw-r--r--   0     1001      123    16797 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
+-rw-r--r--   0     1001      123        1 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/len.rs
+-rw-r--r--   0     1001      123     2658 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs
+-rw-r--r--   0     1001      123    23299 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
+-rw-r--r--   0     1001      123     2414 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
+-rw-r--r--   0     1001      123      593 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
+-rw-r--r--   0     1001      123     4375 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
+-rw-r--r--   0     1001      123     2771 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
+-rw-r--r--   0     1001      123    10267 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
+-rw-r--r--   0     1001      123    12518 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/set.rs
+-rw-r--r--   0     1001      123     7391 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
+-rw-r--r--   0     1001      123     2299 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
+-rw-r--r--   0     1001      123     5522 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
+-rw-r--r--   0     1001      123     7543 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
+-rw-r--r--   0     1001      123    28138 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
+-rw-r--r--   0     1001      123      380 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
+-rw-r--r--   0     1001      123    22089 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
+-rw-r--r--   0     1001      123     7848 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
+-rw-r--r--   0     1001      123      301 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
+-rw-r--r--   0     1001      123    16256 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
+-rw-r--r--   0     1001      123     6275 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
+-rw-r--r--   0     1001      123     6072 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
+-rw-r--r--   0     1001      123      459 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/tile.rs
+-rw-r--r--   0     1001      123    12251 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
+-rw-r--r--   0     1001      123    14620 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
+-rw-r--r--   0     1001      123     5846 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
+-rw-r--r--   0     1001      123     9093 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/random.rs
+-rw-r--r--   0     1001      123     1875 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
+-rw-r--r--   0     1001      123     2826 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
+-rw-r--r--   0     1001      123    10336 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
+-rw-r--r--   0     1001      123     3201 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
+-rw-r--r--   0     1001      123     1061 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
+-rw-r--r--   0     1001      123     3042 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
+-rw-r--r--   0     1001      123      872 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/to_vec.rs
+-rw-r--r--   0     1001      123     8114 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
+-rw-r--r--   0     1001      123    26020 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
+-rw-r--r--   0     1001      123     7944 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/cloud.rs
+-rw-r--r--   0     1001      123     1549 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/config.rs
+-rw-r--r--   0     1001      123     4469 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/datatypes/_serde.rs
+-rw-r--r--   0     1001      123     2509 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/datatypes/aliases.rs
+-rw-r--r--   0     1001      123    42659 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/datatypes/any_value.rs
+-rw-r--r--   0     1001      123    13381 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/datatypes/dtype.rs
+-rw-r--r--   0     1001      123     5609 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/datatypes/field.rs
+-rw-r--r--   0     1001      123     8059 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/datatypes/mod.rs
+-rw-r--r--   0     1001      123     2016 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/datatypes/time_unit.rs
+-rw-r--r--   0     1001      123      118 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/doc/changelog/mod.rs
+-rw-r--r--   0     1001      123      898 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
+-rw-r--r--   0     1001      123      481 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
+-rw-r--r--   0     1001      123      293 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
+-rw-r--r--   0     1001      123      499 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
+-rw-r--r--   0     1001      123      288 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
+-rw-r--r--   0     1001      123     1071 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
+-rw-r--r--   0     1001      123      819 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
+-rw-r--r--   0     1001      123      596 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
+-rw-r--r--   0     1001      123       43 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/doc/mod.rs
+-rw-r--r--   0     1001      123       25 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/error.rs
+-rw-r--r--   0     1001      123      263 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/export.rs
+-rw-r--r--   0     1001      123    36573 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/fmt.rs
+-rw-r--r--   0     1001      123     5177 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/arithmetic.rs
+-rw-r--r--   0     1001      123     9916 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/asof_join/asof.rs
+-rw-r--r--   0     1001      123    35743 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/asof_join/groups.rs
+-rw-r--r--   0     1001      123     7168 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/asof_join/mod.rs
+-rw-r--r--   0     1001      123      559 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/chunks.rs
+-rw-r--r--   0     1001      123     5181 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/cross_join.rs
+-rw-r--r--   0     1001      123    16760 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/explode.rs
+-rw-r--r--   0     1001      123     1019 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/from.rs
+-rw-r--r--   0     1001      123    19239 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
+-rw-r--r--   0     1001      123     4113 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs
+-rw-r--r--   0     1001      123     7749 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
+-rw-r--r--   0     1001      123    40479 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
+-rw-r--r--   0     1001      123     5634 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs
+-rw-r--r--   0     1001      123      218 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/expr.rs
+-rw-r--r--   0     1001      123    22901 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/hashing.rs
+-rw-r--r--   0     1001      123    14380 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
+-rw-r--r--   0     1001      123    39623 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/mod.rs
+-rw-r--r--   0     1001      123    10637 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/perfect.rs
+-rw-r--r--   0     1001      123    19780 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/proxy.rs
+-rw-r--r--   0     1001      123     5416 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/args.rs
+-rw-r--r--   0     1001      123    13172 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/mod.rs
+-rw-r--r--   0     1001      123    22364 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
+-rw-r--r--   0     1001      123     2400 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
+-rw-r--r--   0     1001      123    17372 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
+-rw-r--r--   0     1001      123     4677 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
+-rw-r--r--   0     1001      123     6502 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
+-rw-r--r--   0     1001      123     4665 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
+-rw-r--r--   0     1001      123     3913 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
+-rw-r--r--   0     1001      123    12313 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
+-rw-r--r--   0     1001      123     3865 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/zip_outer.rs
+-rw-r--r--   0     1001      123   126294 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/mod.rs
+-rw-r--r--   0     1001      123    27652 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/row/av_buffer.rs
+-rw-r--r--   0     1001      123     5183 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/row/dataframe.rs
+-rw-r--r--   0     1001      123     5976 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/row/mod.rs
+-rw-r--r--   0     1001      123     9875 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/row/transpose.rs
+-rw-r--r--   0     1001      123     2811 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/top_k.rs
+-rw-r--r--   0     1001      123     1388 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/upstream_traits.rs
+-rw-r--r--   0     1001      123    10198 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/functions.rs
+-rw-r--r--   0     1001      123     2149 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/hashing/fx.rs
+-rw-r--r--   0     1001      123     1503 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/hashing/identity.rs
+-rw-r--r--   0     1001      123      457 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/hashing/mod.rs
+-rw-r--r--   0     1001      123     2684 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/hashing/partition.rs
+-rw-r--r--   0     1001      123    17704 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/hashing/vector_hasher.rs
+-rw-r--r--   0     1001      123     1896 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/lib.rs
+-rw-r--r--   0     1001      123    15763 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/named_from.rs
+-rw-r--r--   0     1001      123     2502 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/prelude.rs
+-rw-r--r--   0     1001      123    18242 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/schema.rs
+-rw-r--r--   0     1001      123     3995 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/serde/chunked_array.rs
+-rw-r--r--   0     1001      123     1094 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/serde/df.rs
+-rw-r--r--   0     1001      123     4734 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/serde/mod.rs
+-rw-r--r--   0     1001      123     9938 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/serde/series.rs
+-rw-r--r--   0     1001      123    18543 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/any_value.rs
+-rw-r--r--   0     1001      123    28755 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
+-rw-r--r--   0     1001      123      222 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/arithmetic/mod.rs
+-rw-r--r--   0     1001      123     3546 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/arithmetic/owned.rs
+-rw-r--r--   0     1001      123    19293 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/comparison.rs
+-rw-r--r--   0     1001      123    29766 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/from.rs
+-rw-r--r--   0     1001      123     6080 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/array.rs
+-rw-r--r--   0     1001      123     9089 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/binary.rs
+-rw-r--r--   0     1001      123    10835 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123    12800 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/categorical.rs
+-rw-r--r--   0     1001      123    18214 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/dates_time.rs
+-rw-r--r--   0     1001      123    15034 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123     7981 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/decimal.rs
+-rw-r--r--   0     1001      123    14734 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123    14063 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     6078 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123    18396 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123     5522 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/null.rs
+-rw-r--r--   0     1001      123     7939 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123    11788 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123     9607 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123     4471 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/into.rs
+-rw-r--r--   0     1001      123     6241 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/iterator.rs
+-rw-r--r--   0     1001      123    39074 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/mod.rs
+-rw-r--r--   0     1001      123      853 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/diff.rs
+-rw-r--r--   0     1001      123     5814 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/downcast.rs
+-rw-r--r--   0     1001      123     3601 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/ewm.rs
+-rw-r--r--   0     1001      123      413 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/extend.rs
+-rw-r--r--   0     1001      123      562 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     5974 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/moment.rs
+-rw-r--r--   0     1001      123     3181 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/null.rs
+-rw-r--r--   0     1001      123     1347 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/pct_change.rs
+-rw-r--r--   0     1001      123     4620 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/round.rs
+-rw-r--r--   0     1001      123     5082 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/to_list.rs
+-rw-r--r--   0     1001      123     1476 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/unique.rs
+-rw-r--r--   0     1001      123    18408 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/series_trait.rs
+-rw-r--r--   0     1001      123     2912 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/unstable.rs
+-rw-r--r--   0     1001      123     7077 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/testing.rs
+-rw-r--r--   0     1001      123      508 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/tests.rs
+-rw-r--r--   0     1001      123     2492 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/utils/flatten.rs
+-rw-r--r--   0     1001      123    31194 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/utils/mod.rs
+-rw-r--r--   0     1001      123     1600 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/utils/series.rs
+-rw-r--r--   0     1001      123    13201 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/utils/supertype.rs
+-rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/LICENSE
+-rw-r--r--   0     1001      123      144 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/README.md
+-rw-r--r--   0     1001      123     1975 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/array/default_arrays.rs
+-rw-r--r--   0     1001      123     1791 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/array/fixed_size_list.rs
+-rw-r--r--   0     1001      123     3773 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/array/get.rs
+-rw-r--r--   0     1001      123     6664 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/array/list.rs
+-rw-r--r--   0     1001      123     8165 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/array/mod.rs
+-rw-r--r--   0     1001      123      878 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/array/null.rs
+-rw-r--r--   0     1001      123     1125 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/array/slice.rs
+-rw-r--r--   0     1001      123     2253 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/array/utf8.rs
+-rw-r--r--   0     1001      123     2294 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/bit_util.rs
+-rw-r--r--   0     1001      123       17 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/bitmap/mod.rs
+-rw-r--r--   0     1001      123      819 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/bitmap/mutable.rs
+-rw-r--r--   0     1001      123      370 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/add.rs
+-rw-r--r--   0     1001      123     2181 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/commutative.rs
+-rw-r--r--   0     1001      123     1482 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/div.rs
+-rw-r--r--   0     1001      123     1028 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mod.rs
+-rw-r--r--   0     1001      123     1177 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mul.rs
+-rw-r--r--   0     1001      123      508 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/sub.rs
+-rw-r--r--   0     1001      123       51 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/arithmetics/mod.rs
+-rw-r--r--   0     1001      123        1 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/arity.rs
+-rw-r--r--   0     1001      123      727 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/bitwise.rs
+-rw-r--r--   0     1001      123     1206 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/cast.rs
+-rw-r--r--   0     1001      123     3964 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/decimal.rs
+-rw-r--r--   0     1001      123     1250 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/mod.rs
+-rw-r--r--   0     1001      123      391 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/take/bitmap.rs
+-rw-r--r--   0     1001      123     2767 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/take/boolean.rs
+-rw-r--r--   0     1001      123     3489 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/take/fixed_size_list.rs
+-rw-r--r--   0     1001      123    25290 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/take/mod.rs
+-rw-r--r--   0     1001      123      797 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/tile.rs
+-rw-r--r--   0     1001      123     1102 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/conversion.rs
+-rw-r--r--   0     1001      123     1609 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/data_types.rs
+-rw-r--r--   0     1001      123       25 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/error.rs
+-rw-r--r--   0     1001      123       28 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/export.rs
+-rw-r--r--   0     1001      123       26 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/floats/mod.rs
+-rw-r--r--   0     1001      123     2066 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/floats/ord.rs
+-rw-r--r--   0     1001      123     1273 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/index.rs
+-rw-r--r--   0     1001      123      984 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/is_valid.rs
+-rw-r--r--   0     1001      123     4783 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
+-rw-r--r--   0     1001      123     1074 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/comparison.rs
+-rw-r--r--   0     1001      123     1068 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/concatenate.rs
+-rw-r--r--   0     1001      123     5161 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
+-rw-r--r--   0     1001      123     1808 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
+-rw-r--r--   0     1001      123    25065 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
+-rw-r--r--   0     1001      123     1406 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/float.rs
+-rw-r--r--   0     1001      123     4908 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/list.rs
+-rw-r--r--   0     1001      123     1885 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
+-rw-r--r--   0     1001      123     9783 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/mod.rs
+-rw-r--r--   0     1001      123     3923 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
+-rw-r--r--   0     1001      123     2019 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
+-rw-r--r--   0     1001      123    16187 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
+-rw-r--r--   0     1001      123     3848 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
+-rw-r--r--   0     1001      123    13521 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
+-rw-r--r--   0     1001      123     5684 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
+-rw-r--r--   0     1001      123     7807 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
+-rw-r--r--   0     1001      123     1879 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
+-rw-r--r--   0     1001      123    14722 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
+-rw-r--r--   0     1001      123    10055 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
+-rw-r--r--   0     1001      123    11643 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
+-rw-r--r--   0     1001      123     4821 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
+-rw-r--r--   0     1001      123     6856 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
+-rw-r--r--   0     1001      123     8109 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
+-rw-r--r--   0     1001      123     4753 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/set.rs
+-rw-r--r--   0     1001      123     4529 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
+-rw-r--r--   0     1001      123     2948 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
+-rw-r--r--   0     1001      123     5974 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
+-rw-r--r--   0     1001      123      231 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
+-rw-r--r--   0     1001      123      842 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/string.rs
+-rw-r--r--   0     1001      123     2310 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs
+-rw-r--r--   0     1001      123     4315 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs
+-rw-r--r--   0     1001      123     2606 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs
+-rw-r--r--   0     1001      123     3672 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/time.rs
+-rw-r--r--   0     1001      123      341 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/lib.rs
+-rw-r--r--   0     1001      123      496 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/prelude.rs
+-rw-r--r--   0     1001      123      534 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/slice.rs
+-rw-r--r--   0     1001      123      183 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/time_zone.rs
+-rw-r--r--   0     1001      123      998 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
+-rw-r--r--   0     1001      123     2821 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/trusted_len/mod.rs
+-rw-r--r--   0     1001      123     2054 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
+-rw-r--r--   0     1001      123      158 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/trusted_len/rev.rs
+-rw-r--r--   0     1001      123     5233 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/utils.rs
+-rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/LICENSE
+-rw-r--r--   0     1001      123      165 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/README.md
+-rw-r--r--   0     1001      123       98 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/mod.rs
+-rw-r--r--   0     1001      123     1219 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/operators/filter.rs
+-rw-r--r--   0     1001      123     4103 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/operators/function.rs
+-rw-r--r--   0     1001      123      266 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/operators/mod.rs
+-rw-r--r--   0     1001      123      682 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/operators/pass.rs
+-rw-r--r--   0     1001      123      548 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
+-rw-r--r--   0     1001      123     3553 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/operators/projection.rs
+-rw-r--r--   0     1001      123     3559 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
+-rw-r--r--   0     1001      123     6479 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
+-rw-r--r--   0     1001      123    11288 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
+-rw-r--r--   0     1001      123     1207 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
+-rw-r--r--   0     1001      123     1888 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
+-rw-r--r--   0     1001      123     4554 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
+-rw-r--r--   0     1001      123     1746 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
+-rw-r--r--   0     1001      123     5413 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
+-rw-r--r--   0     1001      123     4951 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
+-rw-r--r--   0     1001      123      211 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
+-rw-r--r--   0     1001      123      856 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
+-rw-r--r--   0     1001      123     4294 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
+-rw-r--r--   0     1001      123     4109 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs
+-rw-r--r--   0     1001      123     7404 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs
+-rw-r--r--   0     1001      123    10554 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs
+-rw-r--r--   0     1001      123     3589 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs
+-rw-r--r--   0     1001      123     2767 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs
+-rw-r--r--   0     1001      123     6326 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs
+-rw-r--r--   0     1001      123     3116 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/source.rs
+-rw-r--r--   0     1001      123    10194 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs
+-rw-r--r--   0     1001      123     2119 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
+-rw-r--r--   0     1001      123     4695 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
+-rw-r--r--   0     1001      123     1887 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
+-rw-r--r--   0     1001      123    20783 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
+-rw-r--r--   0     1001      123    23825 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
+-rw-r--r--   0     1001      123     2457 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
+-rw-r--r--   0     1001      123     9239 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/io.rs
+-rw-r--r--   0     1001      123     5451 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
+-rw-r--r--   0     1001      123    12056 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
+-rw-r--r--   0     1001      123    11658 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
+-rw-r--r--   0     1001      123      178 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
+-rw-r--r--   0     1001      123     2241 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
+-rw-r--r--   0     1001      123      589 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
+-rw-r--r--   0     1001      123     1492 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
+-rw-r--r--   0     1001      123     1824 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
+-rw-r--r--   0     1001      123     3108 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
+-rw-r--r--   0     1001      123      130 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
+-rw-r--r--   0     1001      123     6774 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
+-rw-r--r--   0     1001      123     7279 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
+-rw-r--r--   0     1001      123    11679 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
+-rw-r--r--   0     1001      123     3908 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
+-rw-r--r--   0     1001      123      526 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
+-rw-r--r--   0     1001      123     5984 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sources/csv.rs
+-rw-r--r--   0     1001      123     1231 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sources/frame.rs
+-rw-r--r--   0     1001      123      987 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
+-rw-r--r--   0     1001      123      366 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sources/mod.rs
+-rw-r--r--   0     1001      123     4335 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
+-rw-r--r--   0     1001      123     1146 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
+-rw-r--r--   0     1001      123     1022 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sources/union.rs
+-rw-r--r--   0     1001      123      448 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/expressions.rs
+-rw-r--r--   0     1001      123      272 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/lib.rs
+-rw-r--r--   0     1001      123      719 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/operators/chunks.rs
+-rw-r--r--   0     1001      123      474 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/operators/context.rs
+-rw-r--r--   0     1001      123      223 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/operators/mod.rs
+-rw-r--r--   0     1001      123      514 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/operators/operator.rs
+-rw-r--r--   0     1001      123      626 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/operators/sink.rs
+-rw-r--r--   0     1001      123      241 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/operators/source.rs
+-rw-r--r--   0     1001      123        1 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/pipeline/config.rs
+-rw-r--r--   0     1001      123    21320 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/pipeline/convert.rs
+-rw-r--r--   0     1001      123    20362 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
+-rw-r--r--   0     1001      123     1155 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/pipeline/mod.rs
+-rw-r--r--   0        0        0     5424 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/LICENSE
+-rw-r--r--   0     1001      123       45 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/constants.rs
+-rw-r--r--   0     1001      123    17253 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dot.rs
+-rw-r--r--   0     1001      123     4789 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/arithmetic.rs
+-rw-r--r--   0     1001      123     3992 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/arity.rs
+-rw-r--r--   0     1001      123     1278 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/array.rs
+-rw-r--r--   0     1001      123      935 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/binary.rs
+-rw-r--r--   0     1001      123      650 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/cat.rs
+-rw-r--r--   0     1001      123    10729 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/dt.rs
+-rw-r--r--   0     1001      123     9542 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/expr.rs
+-rw-r--r--   0     1001      123     8359 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/expr_dyn_fn.rs
+-rw-r--r--   0     1001      123      753 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/from.rs
+-rw-r--r--   0     1001      123       85 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/abs.rs
+-rw-r--r--   0     1001      123     1431 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
+-rw-r--r--   0     1001      123     1074 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/array.rs
+-rw-r--r--   0     1001      123     1327 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
+-rw-r--r--   0     1001      123     4221 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs
+-rw-r--r--   0     1001      123     1910 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs
+-rw-r--r--   0     1001      123     1216 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs
+-rw-r--r--   0     1001      123      344 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
+-rw-r--r--   0     1001      123      257 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/concat.rs
+-rw-r--r--   0     1001      123     6125 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/correlation.rs
+-rw-r--r--   0     1001      123     1593 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs
+-rw-r--r--   0     1001      123    11615 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
+-rw-r--r--   0     1001      123      782 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
+-rw-r--r--   0     1001      123     2567 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
+-rw-r--r--   0     1001      123      992 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/fused.rs
+-rw-r--r--   0     1001      123     8997 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
+-rw-r--r--   0     1001      123      581 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/log.rs
+-rw-r--r--   0     1001      123    24898 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
+-rw-r--r--   0     1001      123      462 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
+-rw-r--r--   0     1001      123     3132 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
+-rw-r--r--   0     1001      123     1410 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/random.rs
+-rw-r--r--   0     1001      123     5146 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/range.rs
+-rw-r--r--   0     1001      123      152 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
+-rw-r--r--   0     1001      123      260 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/round.rs
+-rw-r--r--   0     1001      123      200 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
+-rw-r--r--   0     1001      123    19251 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
+-rw-r--r--   0     1001      123      306 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
+-rw-r--r--   0     1001      123     3812 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
+-rw-r--r--   0     1001      123     1238 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
+-rw-r--r--   0     1001      123      972 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
+-rw-r--r--   0     1001      123    22249 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
+-rw-r--r--   0     1001      123     1017 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
+-rw-r--r--   0     1001      123     8438 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
+-rw-r--r--   0     1001      123     6112 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
+-rw-r--r--   0     1001      123      170 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/unique.rs
+-rw-r--r--   0     1001      123     1155 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/arity.rs
+-rw-r--r--   0     1001      123      611 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/coerce.rs
+-rw-r--r--   0     1001      123     2717 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/concat.rs
+-rw-r--r--   0     1001      123     4525 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/correlation.rs
+-rw-r--r--   0     1001      123     8736 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/horizontal.rs
+-rw-r--r--   0     1001      123     1042 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/index.rs
+-rw-r--r--   0     1001      123      968 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/mod.rs
+-rw-r--r--   0     1001      123     4129 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/range.rs
+-rw-r--r--   0     1001      123     1308 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/selectors.rs
+-rw-r--r--   0     1001      123     1973 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/syntactic_sugar.rs
+-rw-r--r--   0     1001      123    11328 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/temporal.rs
+-rw-r--r--   0     1001      123    12282 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/list.rs
+-rw-r--r--   0     1001      123     4501 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/meta.rs
+-rw-r--r--   0     1001      123    61162 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/mod.rs
+-rw-r--r--   0     1001      123       40 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/names.rs
+-rw-r--r--   0     1001      123     2658 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/options.rs
+-rw-r--r--   0     1001      123     7017 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/python_udf.rs
+-rw-r--r--   0     1001      123     1432 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/random.rs
+-rw-r--r--   0     1001      123     1068 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/selector.rs
+-rw-r--r--   0     1001      123    17626 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/string.rs
+-rw-r--r--   0     1001      123     2715 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/struct_.rs
+-rw-r--r--   0     1001      123       38 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/frame/mod.rs
+-rw-r--r--   0     1001      123      933 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/frame/opt_state.rs
+-rw-r--r--   0     1001      123      466 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/global.rs
+-rw-r--r--   0     1001      123      175 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/lib.rs
+-rw-r--r--   0     1001      123    10651 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
+-rw-r--r--   0     1001      123    11920 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
+-rw-r--r--   0     1001      123    25683 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/alp.rs
+-rw-r--r--   0     1001      123     1622 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
+-rw-r--r--   0     1001      123     1428 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/apply.rs
+-rw-r--r--   0     1001      123    25639 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/builder.rs
+-rw-r--r--   0     1001      123    29993 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/conversion.rs
+-rw-r--r--   0     1001      123      301 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/debug.rs
+-rw-r--r--   0     1001      123    15713 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/format.rs
+-rw-r--r--   0     1001      123      895 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
+-rw-r--r--   0     1001      123      137 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
+-rw-r--r--   0     1001      123     1169 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
+-rw-r--r--   0     1001      123    13288 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
+-rw-r--r--   0     1001      123     1031 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/functions/python_udf.rs
+-rw-r--r--   0     1001      123     1330 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
+-rw-r--r--   0     1001      123    10157 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/iterator.rs
+-rw-r--r--   0     1001      123    10559 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/lit.rs
+-rw-r--r--   0     1001      123     8142 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/mod.rs
+-rw-r--r--   0     1001      123     7416 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
+-rw-r--r--   0     1001      123    15277 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
+-rw-r--r--   0     1001      123     2889 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
+-rw-r--r--   0     1001      123     3236 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
+-rw-r--r--   0     1001      123     4663 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
+-rw-r--r--   0     1001      123    14479 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
+-rw-r--r--   0     1001      123     1556 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
+-rw-r--r--   0     1001      123     6017 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/fused.rs
+-rw-r--r--   0     1001      123     6778 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
+-rw-r--r--   0     1001      123     1222 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
+-rw-r--r--   0     1001      123    28901 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
+-rw-r--r--   0     1001      123     2571 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
+-rw-r--r--   0     1001      123    16171 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
+-rw-r--r--   0     1001      123     1755 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
+-rw-r--r--   0     1001      123     3930 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
+-rw-r--r--   0     1001      123     1799 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
+-rw-r--r--   0     1001      123     3269 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
+-rw-r--r--   0     1001      123     2638 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
+-rw-r--r--   0     1001      123    15874 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
+-rw-r--r--   0     1001      123    26739 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
+-rw-r--r--   0     1001      123     3707 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
+-rw-r--r--   0     1001      123     2639 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
+-rw-r--r--   0     1001      123     3509 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
+-rw-r--r--   0     1001      123    27269 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
+-rw-r--r--   0     1001      123     3496 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
+-rw-r--r--   0     1001      123    13232 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
+-rw-r--r--   0     1001      123     4181 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
+-rw-r--r--   0     1001      123     9796 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
+-rw-r--r--   0     1001      123    20215 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
+-rw-r--r--   0     1001      123    10653 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/options.rs
+-rw-r--r--   0     1001      123    19151 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/projection.rs
+-rw-r--r--   0     1001      123     6144 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
+-rw-r--r--   0     1001      123    13026 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/schema.rs
+-rw-r--r--   0     1001      123     6699 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/tree_format.rs
+-rw-r--r--   0     1001      123     3544 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/visitor/expr.rs
+-rw-r--r--   0     1001      123      930 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/visitor/mod.rs
+-rw-r--r--   0     1001      123     4408 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/visitor/visitors.rs
+-rw-r--r--   0     1001      123      832 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/prelude.rs
+-rw-r--r--   0     1001      123    12428 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/utils.rs
+-rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-error/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-error/LICENSE
+-rw-r--r--   0     1001      123      145 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-error/README.md
+-rw-r--r--   0     1001      123     7567 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-error/src/lib.rs
+-rw-r--r--   0        0        0     2037 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/LICENSE
+-rw-r--r--   0     1001      123      143 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/README.md
+-rw-r--r--   0     1001      123     1018 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/base_utc_offset.rs
+-rw-r--r--   0     1001      123     3569 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/date.rs
+-rw-r--r--   0     1001      123     6465 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/datetime.rs
+-rw-r--r--   0     1001      123     3305 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/duration.rs
+-rw-r--r--   0     1001      123     5607 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/kernels.rs
+-rw-r--r--   0     1001      123     1062 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/mod.rs
+-rw-r--r--   0     1001      123     6759 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
+-rw-r--r--   0     1001      123     2582 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
+-rw-r--r--   0     1001      123    11122 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
+-rw-r--r--   0     1001      123      413 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
+-rw-r--r--   0     1001      123     4810 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
+-rw-r--r--   0     1001      123     2372 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/time.rs
+-rw-r--r--   0     1001      123    21334 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
+-rw-r--r--   0     1001      123    18997 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
+-rw-r--r--   0     1001      123     3975 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
+-rw-r--r--   0     1001      123    11229 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
+-rw-r--r--   0     1001      123     3340 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/date_range.rs
+-rw-r--r--   0     1001      123      994 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/dst_offset.rs
+-rw-r--r--   0     1001      123    34703 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/groupby/dynamic.rs
+-rw-r--r--   0     1001      123       88 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/groupby/mod.rs
+-rw-r--r--   0     1001      123      769 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/lib.rs
+-rw-r--r--   0     1001      123     2976 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/month_end.rs
+-rw-r--r--   0     1001      123     3365 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/month_start.rs
+-rw-r--r--   0     1001      123      274 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/prelude.rs
+-rw-r--r--   0     1001      123     1381 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/round.rs
+-rw-r--r--   0     1001      123     3992 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/series/_trait.rs
+-rw-r--r--   0     1001      123      136 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123      140 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/series/implementations/categoricals.rs
+-rw-r--r--   0     1001      123      133 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/series/implementations/date.rs
+-rw-r--r--   0     1001      123      137 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123      137 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123     1863 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     1792 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/series/implementations/integers.rs
+-rw-r--r--   0     1001      123      133 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123      486 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123      155 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123      135 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123      133 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/series/implementations/time.rs
+-rw-r--r--   0     1001      123      133 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123    12791 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/series/mod.rs
+-rw-r--r--   0     1001      123     1443 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/truncate.rs
+-rw-r--r--   0     1001      123     7619 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/upsample.rs
+-rw-r--r--   0     1001      123     2511 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/utils.rs
+-rw-r--r--   0     1001      123     1524 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/windows/bounds.rs
+-rw-r--r--   0     1001      123     2672 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/windows/calendar.rs
+-rw-r--r--   0     1001      123    25303 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/windows/duration.rs
+-rw-r--r--   0     1001      123    20201 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/windows/groupby.rs
+-rw-r--r--   0     1001      123      503 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/windows/mod.rs
+-rw-r--r--   0     1001      123    23627 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/windows/test.rs
+-rw-r--r--   0     1001      123    10657 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/windows/window.rs
+-rw-r--r--   0        0        0    10755 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/LICENSE
+-rw-r--r--   0     1001      123     3472 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/Makefile
+-rw-r--r--   0     1001      123      215 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/build.rs
+-rw-r--r--   0     1001      123       78 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/clippy.toml
+-rw-r--r--   0     1001      123    17614 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/src/docs/eager.rs
+-rw-r--r--   0     1001      123     8815 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/src/docs/lazy.rs
+-rw-r--r--   0     1001      123       50 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3806 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/src/docs/performance.rs
+-rw-r--r--   0     1001      123       59 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/src/export.rs
+-rw-r--r--   0     1001      123    19848 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/src/lib.rs
+-rw-r--r--   0     1001      123      387 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/src/prelude.rs
+-rw-r--r--   0     1001      123       54 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/src/sql.rs
+-rw-r--r--   0     1001      123     4272 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/core/date_like.rs
+-rw-r--r--   0     1001      123     2401 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/core/groupby.rs
+-rw-r--r--   0     1001      123    17838 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/core/joins.rs
+-rw-r--r--   0     1001      123      545 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/core/list.rs
+-rw-r--r--   0     1001      123      198 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/core/mod.rs
+-rw-r--r--   0     1001      123       24 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/core/ops/mod.rs
+-rw-r--r--   0     1001      123      457 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/core/ops/take.rs
+-rw-r--r--   0     1001      123     6259 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/core/pivot.rs
+-rw-r--r--   0     1001      123     1102 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/core/random.rs
+-rw-r--r--   0     1001      123    11096 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/core/rolling_window.rs
+-rw-r--r--   0     1001      123     1093 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/core/series.rs
+-rw-r--r--   0     1001      123      370 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/core/utils.rs
+-rw-r--r--   0     1001      123    30423 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/io/csv.rs
+-rw-r--r--   0     1001      123     4490 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/io/ipc_stream.rs
+-rw-r--r--   0     1001      123     7043 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/io/json.rs
+-rw-r--r--   0     1001      123      378 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/io/mod.rs
+-rw-r--r--   0     1001      123      531 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/io/parquet.rs
+-rw-r--r--   0     1001      123     1530 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/joins.rs
+-rw-r--r--   0     1001      123     2452 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/aggregation.rs
+-rw-r--r--   0     1001      123      821 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/cse.rs
+-rw-r--r--   0     1001      123      500 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/explodes.rs
+-rw-r--r--   0     1001      123     2278 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
+-rw-r--r--   0     1001      123    10285 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
+-rw-r--r--   0     1001      123     1065 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
+-rw-r--r--   0     1001      123     1008 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
+-rw-r--r--   0     1001      123      428 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
+-rw-r--r--   0     1001      123      121 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
+-rw-r--r--   0     1001      123      659 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
+-rw-r--r--   0     1001      123    10657 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/expressions/window.rs
+-rw-r--r--   0     1001      123      579 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/folds.rs
+-rw-r--r--   0     1001      123      557 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/functions.rs
+-rw-r--r--   0     1001      123     4482 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/groupby.rs
+-rw-r--r--   0     1001      123     1681 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
+-rw-r--r--   0     1001      123      691 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/mod.rs
+-rw-r--r--   0     1001      123     5747 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
+-rw-r--r--   0     1001      123     4483 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/projection_queries.rs
+-rw-r--r--   0     1001      123     6584 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/queries.rs
+-rw-r--r--   0     1001      123      151 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/main.rs
+-rw-r--r--   0     1001      123    12591 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/schema.rs
+-rw-r--r--   0     1001      123     1899 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/time/date_range.rs
+-rw-r--r--   0     1001      123       16 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/time/mod.rs
+-rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/LICENSE
+-rw-r--r--   0     1001      123      141 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/README.md
+-rw-r--r--   0     1001      123      151 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/aliases.rs
+-rw-r--r--   0     1001      123     2879 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/arena.rs
+-rw-r--r--   0     1001      123     1379 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/atomic.rs
+-rw-r--r--   0     1001      123     2659 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/cell.rs
+-rw-r--r--   0     1001      123     1015 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/contention_pool.rs
+-rw-r--r--   0     1001      123      509 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/error.rs
+-rw-r--r--   0     1001      123      271 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/fmt.rs
+-rw-r--r--   0     1001      123      763 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/functions.rs
+-rw-r--r--   0     1001      123     2709 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
+-rw-r--r--   0     1001      123       61 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/iter/mod.rs
+-rw-r--r--   0     1001      123      503 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/lib.rs
+-rw-r--r--   0     1001      123      573 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/macros.rs
+-rw-r--r--   0     1001      123      282 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/mem.rs
+-rw-r--r--   0     1001      123     2642 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/slice.rs
+-rw-r--r--   0     1001      123     2467 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/sort.rs
+-rw-r--r--   0     1001      123     1115 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/sync.rs
+-rw-r--r--   0     1001      123      504 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/sys.rs
+-rw-r--r--   0     1001      123      697 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/unwrap.rs
+-rw-r--r--   0     1001      123     2024 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/vec.rs
+-rw-r--r--   0     1001      123      616 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/wasm.rs
+-rw-r--r--   0        0        0     6286 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/LICENSE
+-rw-r--r--   0     1001      123      358 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/README.md
+-rw-r--r--   0     1001      123     1796 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/dot.rs
+-rw-r--r--   0     1001      123     4479 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/dsl/eval.rs
+-rw-r--r--   0     1001      123     7115 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/dsl/functions.rs
+-rw-r--r--   0     1001      123      164 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/dsl/into.rs
+-rw-r--r--   0     1001      123     6754 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/dsl/list.rs
+-rw-r--r--   0     1001      123     2899 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/dsl/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
+-rw-r--r--   0     1001      123     9285 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/frame/csv.rs
+-rw-r--r--   0     1001      123     4368 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
+-rw-r--r--   0     1001      123     2261 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/frame/ipc.rs
+-rw-r--r--   0     1001      123    49541 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/frame/mod.rs
+-rw-r--r--   0     1001      123     3382 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/frame/ndjson.rs
+-rw-r--r--   0     1001      123     2734 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/frame/parquet.rs
+-rw-r--r--   0     1001      123     2892 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/frame/pivot.rs
+-rw-r--r--   0     1001      123      459 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/frame/python.rs
+-rw-r--r--   0     1001      123     6374 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/lib.rs
+-rw-r--r--   0     1001      123     1049 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
+-rw-r--r--   0     1001      123      776 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
+-rw-r--r--   0     1001      123      670 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
+-rw-r--r--   0     1001      123     1555 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
+-rw-r--r--   0     1001      123     3986 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
+-rw-r--r--   0     1001      123     4125 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
+-rw-r--r--   0     1001      123    13599 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
+-rw-r--r--   0     1001      123     4883 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
+-rw-r--r--   0     1001      123     5859 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
+-rw-r--r--   0     1001      123     6753 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
+-rw-r--r--   0     1001      123     2045 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
+-rw-r--r--   0     1001      123     1761 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
+-rw-r--r--   0     1001      123     2854 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
+-rw-r--r--   0     1001      123     1963 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
+-rw-r--r--   0     1001      123     4303 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
+-rw-r--r--   0     1001      123     1209 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
+-rw-r--r--   0     1001      123     2421 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
+-rw-r--r--   0     1001      123      548 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
+-rw-r--r--   0     1001      123     2197 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
+-rw-r--r--   0     1001      123     2015 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
+-rw-r--r--   0     1001      123      663 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
+-rw-r--r--   0     1001      123     4041 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
+-rw-r--r--   0     1001      123      838 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
+-rw-r--r--   0     1001      123     1335 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
+-rw-r--r--   0     1001      123    21959 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
+-rw-r--r--   0     1001      123     2689 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
+-rw-r--r--   0     1001      123    18581 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
+-rw-r--r--   0     1001      123    17674 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
+-rw-r--r--   0     1001      123     2583 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/cache.rs
+-rw-r--r--   0     1001      123     3153 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
+-rw-r--r--   0     1001      123     6326 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
+-rw-r--r--   0     1001      123     1996 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
+-rw-r--r--   0     1001      123     5809 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
+-rw-r--r--   0     1001      123     4131 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
+-rw-r--r--   0     1001      123     5304 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
+-rw-r--r--   0     1001      123    23566 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
+-rw-r--r--   0     1001      123    10091 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
+-rw-r--r--   0     1001      123     4332 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
+-rw-r--r--   0     1001      123    13549 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
+-rw-r--r--   0     1001      123     8331 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
+-rw-r--r--   0     1001      123    14360 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
+-rw-r--r--   0     1001      123    31970 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
+-rw-r--r--   0     1001      123     2039 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
+-rw-r--r--   0     1001      123      414 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/mod.rs
+-rw-r--r--   0     1001      123     2005 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
+-rw-r--r--   0     1001      123    24174 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
+-rw-r--r--   0     1001      123    20552 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
+-rw-r--r--   0     1001      123       87 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
+-rw-r--r--   0     1001      123    10203 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/state.rs
+-rw-r--r--   0     1001      123     2583 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/streaming/checks.rs
+-rw-r--r--   0     1001      123     9280 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/streaming/construct_pipeline.rs
+-rw-r--r--   0     1001      123    16847 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/streaming/convert_alp.rs
+-rw-r--r--   0     1001      123      116 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
+-rw-r--r--   0     1001      123     5827 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
+-rw-r--r--   0     1001      123      722 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/prelude.rs
+-rw-r--r--   0     1001      123    15000 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/aggregations.rs
+-rw-r--r--   0     1001      123     2339 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/arity.rs
+-rw-r--r--   0     1001      123     7276 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/cse.rs
+-rw-r--r--   0     1001      123    12752 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/io.rs
+-rw-r--r--   0     1001      123     4166 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/logical.rs
+-rw-r--r--   0     1001      123     4273 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/mod.rs
+-rw-r--r--   0     1001      123    15770 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
+-rw-r--r--   0     1001      123     6772 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
+-rw-r--r--   0     1001      123     3165 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/projection_queries.rs
+-rw-r--r--   0     1001      123    47685 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/queries.rs
+-rw-r--r--   0     1001      123     9519 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/streaming.rs
+-rw-r--r--   0     1001      123     2893 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/tpch.rs
+-rw-r--r--   0     1001      123     1028 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/utils.rs
+-rw-r--r--   0        0        0     3552 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/LICENSE
+-rw-r--r--   0     1001      123      132 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/README.md
+-rw-r--r--   0     1001      123     2382 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/array/min_max.rs
+-rw-r--r--   0     1001      123      267 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/array/mod.rs
+-rw-r--r--   0     1001      123     1512 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/array/namespace.rs
+-rw-r--r--   0     1001      123     4108 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/array/sum_mean.rs
+-rw-r--r--   0     1001      123      234 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
+-rw-r--r--   0     1001      123     3549 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
+-rw-r--r--   0     1001      123    11023 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
+-rw-r--r--   0     1001      123     1930 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/list/any_all.rs
+-rw-r--r--   0     1001      123     1687 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/list/count.rs
+-rw-r--r--   0     1001      123     2419 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
+-rw-r--r--   0     1001      123     7861 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
+-rw-r--r--   0     1001      123      644 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    19916 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
+-rw-r--r--   0     1001      123     9376 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/list/sets.rs
+-rw-r--r--   0     1001      123     7633 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
+-rw-r--r--   0     1001      123     2435 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
+-rw-r--r--   0     1001      123      545 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     9452 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
+-rw-r--r--   0     1001      123     6795 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/set.rs
+-rw-r--r--   0     1001      123     8781 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
+-rw-r--r--   0     1001      123     8593 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
+-rw-r--r--   0     1001      123     2345 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
+-rw-r--r--   0     1001      123      514 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
+-rw-r--r--   0     1001      123    14951 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
+-rw-r--r--   0     1001      123     4053 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
+-rw-r--r--   0     1001      123      439 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/sum.rs
+-rw-r--r--   0     1001      123     2486 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/top_k.rs
+-rw-r--r--   0     1001      123     7727 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
+-rw-r--r--   0     1001      123    18232 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/frame/join/mod.rs
+-rw-r--r--   0     1001      123     4291 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/frame/mod.rs
+-rw-r--r--   0     1001      123    10257 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/frame/pivot/mod.rs
+-rw-r--r--   0     1001      123    13486 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
+-rw-r--r--   0     1001      123      237 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/lib.rs
+-rw-r--r--   0     1001      123      290 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/prelude.rs
+-rw-r--r--   0     1001      123       25 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/mod.rs
+-rw-r--r--   0     1001      123     9623 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs
+-rw-r--r--   0     1001      123      118 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/approx_algo/mod.rs
+-rw-r--r--   0     1001      123     2016 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/approx_unique.rs
+-rw-r--r--   0     1001      123    11866 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
+-rw-r--r--   0     1001      123     3669 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/cut.rs
+-rw-r--r--   0     1001      123     3688 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
+-rw-r--r--   0     1001      123     5245 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/fused.rs
+-rw-r--r--   0     1001      123     3423 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/is_first.rs
+-rw-r--r--   0     1001      123     2975 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/is_unique.rs
+-rw-r--r--   0     1001      123     3626 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/log.rs
+-rw-r--r--   0     1001      123     1268 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     1769 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/rolling.rs
+-rw-r--r--   0     1001      123     7642 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
+-rw-r--r--   0     1001      123     2603 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
+-rw-r--r--   0     1001      123     2067 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/various.rs
+-rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-row/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-row/LICENSE
+-rw-r--r--   0     1001      123      137 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-row/README.md
+-rw-r--r--   0     1001      123     2377 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-row/src/decode.rs
+-rw-r--r--   0     1001      123    13364 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-row/src/encode.rs
+-rw-r--r--   0     1001      123     7767 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-row/src/fixed.rs
+-rw-r--r--   0     1001      123    13846 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-row/src/lib.rs
+-rw-r--r--   0     1001      123     3019 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-row/src/row.rs
+-rw-r--r--   0     1001      123      682 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-row/src/utils.rs
+-rw-r--r--   0     1001      123     8679 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-row/src/variable.rs
+-rw-r--r--   0        0        0     4397 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/LICENSE
+-rw-r--r--   0     1001      123      138 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/README.md
+-rw-r--r--   0     1001      123     2383 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/avro/mod.rs
+-rw-r--r--   0     1001      123     3608 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/avro/read.rs
+-rw-r--r--   0     1001      123     2622 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/avro/write.rs
+-rw-r--r--   0     1001      123     4505 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/cloud/adaptors.rs
+-rw-r--r--   0     1001      123     9506 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/cloud/glob.rs
+-rw-r--r--   0     1001      123     3089 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/cloud/mod.rs
+-rw-r--r--   0     1001      123    28829 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/buffer.rs
+-rw-r--r--   0     1001      123     1815 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/mod.rs
+-rw-r--r--   0     1001      123    19446 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/parser.rs
+-rw-r--r--   0     1001      123    22228 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/read.rs
+-rw-r--r--   0     1001      123    10847 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
+-rw-r--r--   0     1001      123    13939 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
+-rw-r--r--   0     1001      123    30724 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/read_impl/mod.rs
+-rw-r--r--   0     1001      123    11466 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/splitfields.rs
+-rw-r--r--   0     1001      123    24531 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/utils.rs
+-rw-r--r--   0     1001      123     2796 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/write.rs
+-rw-r--r--   0     1001      123    14759 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/write_impl.rs
+-rw-r--r--   0     1001      123      184 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/export.rs
+-rw-r--r--   0     1001      123     7586 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/ipc/ipc_file.rs
+-rw-r--r--   0     1001      123     9227 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/ipc/ipc_stream.rs
+-rw-r--r--   0     1001      123     3253 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/ipc/mmap.rs
+-rw-r--r--   0     1001      123      401 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/ipc/mod.rs
+-rw-r--r--   0     1001      123     8287 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/ipc/write.rs
+-rw-r--r--   0     1001      123     1471 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/ipc/write_async.rs
+-rw-r--r--   0     1001      123    11044 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/json/mod.rs
+-rw-r--r--   0     1001      123     4771 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/lib.rs
+-rw-r--r--   0     1001      123     1969 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/mmap.rs
+-rw-r--r--   0     1001      123     7228 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/ndjson/buffer.rs
+-rw-r--r--   0     1001      123    11979 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/ndjson/core.rs
+-rw-r--r--   0     1001      123       37 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/ndjson/mod.rs
+-rw-r--r--   0     1001      123      273 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/options.rs
+-rw-r--r--   0     1001      123     7360 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/parquet/async_impl.rs
+-rw-r--r--   0     1001      123     3093 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/parquet/mmap.rs
+-rw-r--r--   0     1001      123     3132 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/parquet/mod.rs
+-rw-r--r--   0     1001      123     4784 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/parquet/predicates.rs
+-rw-r--r--   0     1001      123     9623 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/parquet/read.rs
+-rw-r--r--   0     1001      123    17321 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/parquet/read_impl.rs
+-rw-r--r--   0     1001      123    10129 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/parquet/write.rs
+-rw-r--r--   0     1001      123     5334 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/partition.rs
+-rw-r--r--   0     1001      123     1455 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/predicates.rs
+-rw-r--r--   0     1001      123      621 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/prelude.rs
+-rw-r--r--   0     1001      123      417 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/tests.rs
+-rw-r--r--   0     1001      123     4374 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/utils.rs
+-rw-r--r--   0        0        0     4544 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.6/Cargo.toml
+-rw-r--r--   0     1001      123       76 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/.gitignore
+-rw-r--r--   0     1001      123     1055 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/LICENSE
+-rw-r--r--   0     1001      123     2414 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/Makefile
+-rw-r--r--   0     1001      123    11696 2023-07-06 16:19:18.000000 polars_lts_cpu-0.18.6/README.md
+-rw-r--r--   0     1001      123      651 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/build.rs
+-rw-r--r--   0     1001      123       32 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/.gitignore
+-rw-r--r--   0     1001      123      682 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/Makefile
+-rw-r--r--   0     1001      123      318 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/_templates/api_redirect.html
+-rw-r--r--   0     1001      123      151 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/_templates/autosummary/accessor.rst
+-rw-r--r--   0     1001      123      160 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/_templates/autosummary/accessor_attribute.rst
+-rw-r--r--   0     1001      123      168 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/_templates/autosummary/accessor_callable.rst
+-rw-r--r--   0     1001      123      157 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/_templates/autosummary/accessor_method.rst
+-rw-r--r--   0     1001      123      836 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      123       94 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/_templates/autosummary/class_without_autosummary.rst
+-rw-r--r--   0     1001      123      406 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/_templates/sidebar-nav-bs.html
+-rw-r--r--   0     1001      123      559 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/requirements-docs.txt
+-rw-r--r--   0     1001      123     1164 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/run_live_docs_server.py
+-rw-r--r--   0     1001      123     1567 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/_static/css/custom.css
+-rw-r--r--   0     1001      123     7297 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/conf.py
+-rw-r--r--   0     1001      123       51 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/index.rst
+-rw-r--r--   0     1001      123     6767 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/api.rst
+-rw-r--r--   0     1001      123     2069 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/config.rst
+-rw-r--r--   0     1001      123      274 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/dataframe/aggregation.rst
+-rw-r--r--   0     1001      123      221 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/dataframe/attributes.rst
+-rw-r--r--   0     1001      123      142 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/dataframe/computation.rst
+-rw-r--r--   0     1001      123      319 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/dataframe/descriptive.rst
+-rw-r--r--   0     1001      123      319 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/dataframe/export.rst
+-rw-r--r--   0     1001      123      464 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/dataframe/groupby.rst
+-rw-r--r--   0     1001      123      379 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/dataframe/index.rst
+-rw-r--r--   0     1001      123      189 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/dataframe/miscellaneous.rst
+-rw-r--r--   0     1001      123     1538 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/dataframe/modify_select.rst
+-rw-r--r--   0     1001      123      673 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/datatypes.rst
+-rw-r--r--   0     1001      123      421 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/exceptions.rst
+-rw-r--r--   0     1001      123      391 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/expressions/aggregation.rst
+-rw-r--r--   0     1001      123      267 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/expressions/array.rst
+-rw-r--r--   0     1001      123      309 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/expressions/binary.rst
+-rw-r--r--   0     1001      123      338 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/expressions/boolean.rst
+-rw-r--r--   0     1001      123      237 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/expressions/categories.rst
+-rw-r--r--   0     1001      123      221 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/expressions/columns.rst
+-rw-r--r--   0     1001      123     1095 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/expressions/computation.rst
+-rw-r--r--   0     1001      123     1215 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/expressions/functions.rst
+-rw-r--r--   0     1001      123      470 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/expressions/index.rst
+-rw-r--r--   0     1001      123      830 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/expressions/list.rst
+-rw-r--r--   0     1001      123      458 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/expressions/meta.rst
+-rw-r--r--   0     1001      123      159 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/expressions/miscellaneous.rst
+-rw-r--r--   0     1001      123      977 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/expressions/modify_select.rst
+-rw-r--r--   0     1001      123      679 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/expressions/operators.rst
+-rw-r--r--   0     1001      123      977 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/expressions/string.rst
+-rw-r--r--   0     1001      123      254 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/expressions/struct.rst
+-rw-r--r--   0     1001      123     1087 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/expressions/temporal.rst
+-rw-r--r--   0     1001      123       98 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/expressions/window.rst
+-rw-r--r--   0     1001      123      694 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/functions.rst
+-rw-r--r--   0     1001      123      405 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/index.rst
+-rw-r--r--   0     1001      123     1294 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/io.rst
+-rw-r--r--   0     1001      123      277 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/lazyframe/aggregation.rst
+-rw-r--r--   0     1001      123      179 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/lazyframe/attributes.rst
+-rw-r--r--   0     1001      123      146 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/lazyframe/descriptive.rst
+-rw-r--r--   0     1001      123      497 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/lazyframe/groupby.rst
+-rw-r--r--   0     1001      123      354 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/lazyframe/index.rst
+-rw-r--r--   0     1001      123      455 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/lazyframe/miscellaneous.rst
+-rw-r--r--   0     1001      123     1013 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/lazyframe/modify_select.rst
+-rw-r--r--   0     1001      123     3279 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/selectors.rst
+-rw-r--r--   0     1001      123      358 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/series/aggregation.rst
+-rw-r--r--   0     1001      123      277 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/series/array.rst
+-rw-r--r--   0     1001      123      257 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/series/attributes.rst
+-rw-r--r--   0     1001      123      321 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/series/binary.rst
+-rw-r--r--   0     1001      123      117 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/series/boolean.rst
+-rw-r--r--   0     1001      123      241 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/series/categories.rst
+-rw-r--r--   0     1001      123     1103 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/series/computation.rst
+-rw-r--r--   0     1001      123      744 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/series/descriptive.rst
+-rw-r--r--   0     1001      123      240 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/series/export.rst
+-rw-r--r--   0     1001      123      437 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/series/index.rst
+-rw-r--r--   0     1001      123      894 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/series/list.rst
+-rw-r--r--   0     1001      123      236 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/series/miscellaneous.rst
+-rw-r--r--   0     1001      123     1077 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/series/modify_select.rst
+-rw-r--r--   0     1001      123     1049 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/series/string.rst
+-rw-r--r--   0     1001      123      421 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/series/struct.rst
+-rw-r--r--   0     1001      123     1247 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/series/temporal.rst
+-rw-r--r--   0     1001      123      503 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/sql.rst
+-rw-r--r--   0     1001      123     8067 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/testing.rst
+-rw-r--r--   0     1001      123      168 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/docs/source/reference/utils.rst
+-rw-r--r--   0     1001      123     6370 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/__init__.py
+-rw-r--r--   0     1001      123      280 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/_reexport.py
+-rw-r--r--   0     1001      123    13229 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/api.py
+-rw-r--r--   0     1001      123    29652 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/config.py
+-rw-r--r--   0     1001      123    28090 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/convert.py
+-rw-r--r--   0     1001      123       77 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/dataframe/__init__.py
+-rw-r--r--   0     1001      123     5227 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/dataframe/_html.py
+-rw-r--r--   0     1001      123   323980 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/dataframe/frame.py
+-rw-r--r--   0     1001      123    41618 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/dataframe/groupby.py
+-rw-r--r--   0     1001      123     2692 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/datatypes/__init__.py
+-rw-r--r--   0     1001      123    17874 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/datatypes/classes.py
+-rw-r--r--   0     1001      123     1690 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/datatypes/constants.py
+-rw-r--r--   0     1001      123     4701 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/datatypes/constructor.py
+-rw-r--r--   0     1001      123    15446 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/datatypes/convert.py
+-rw-r--r--   0     1001      123     7358 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/dependencies.py
+-rw-r--r--   0     1001      123     3792 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/exceptions.py
+-rw-r--r--   0     1001      123       61 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/expr/__init__.py
+-rw-r--r--   0     1001      123     3020 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/expr/array.py
+-rw-r--r--   0     1001      123    10330 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/expr/binary.py
+-rw-r--r--   0     1001      123     1698 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/expr/categorical.py
+-rw-r--r--   0     1001      123    80633 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/expr/datetime.py
+-rw-r--r--   0     1001      123   319136 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/expr/expr.py
+-rw-r--r--   0     1001      123    31956 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/expr/list.py
+-rw-r--r--   0     1001      123     4683 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/expr/meta.py
+-rw-r--r--   0     1001      123    60086 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/expr/string.py
+-rw-r--r--   0     1001      123     5426 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/expr/struct.py
+-rw-r--r--   0     1001      123     2126 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/functions/__init__.py
+-rw-r--r--   0     1001      123    16430 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/functions/as_datatype.py
+-rw-r--r--   0     1001      123    18732 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/functions/eager.py
+-rw-r--r--   0     1001      123    72418 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/functions/lazy.py
+-rw-r--r--   0     1001      123    20012 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/functions/range.py
+-rw-r--r--   0     1001      123     6043 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/functions/repeat.py
+-rw-r--r--   0     1001      123     6051 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/functions/whenthen.py
+-rw-r--r--   0     1001      123      952 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/__init__.py
+-rw-r--r--   0     1001      123     6364 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/_utils.py
+-rw-r--r--   0     1001      123      861 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/avro.py
+-rw-r--r--   0     1001      123      144 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/csv/__init__.py
+-rw-r--r--   0     1001      123     1072 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/csv/_utils.py
+-rw-r--r--   0     1001      123     4681 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/csv/batched_reader.py
+-rw-r--r--   0     1001      123    35482 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/csv/functions.py
+-rw-r--r--   0     1001      123     6428 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/database.py
+-rw-r--r--   0     1001      123    11047 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/delta.py
+-rw-r--r--   0     1001      123       75 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/excel/__init__.py
+-rw-r--r--   0     1001      123    18338 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/excel/_write_utils.py
+-rw-r--r--   0     1001      123     6355 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/excel/functions.py
+-rw-r--r--   0     1001      123      142 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/ipc/__init__.py
+-rw-r--r--   0     1001      123     1227 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/ipc/anonymous_scan.py
+-rw-r--r--   0     1001      123     5804 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/ipc/functions.py
+-rw-r--r--   0     1001      123      510 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/json.py
+-rw-r--r--   0     1001      123     2215 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/ndjson.py
+-rw-r--r--   0     1001      123      170 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/parquet/__init__.py
+-rw-r--r--   0     1001      123     1259 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/parquet/anonymous_scan.py
+-rw-r--r--   0     1001      123     7177 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/parquet/functions.py
+-rw-r--r--   0     1001      123      136 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/pyarrow_dataset/__init__.py
+-rw-r--r--   0     1001      123     2186 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/pyarrow_dataset/anonymous_scan.py
+-rw-r--r--   0     1001      123     3601 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/io/pyarrow_dataset/functions.py
+-rw-r--r--   0     1001      123       77 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/lazyframe/__init__.py
+-rw-r--r--   0     1001      123   172003 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/lazyframe/frame.py
+-rw-r--r--   0     1001      123    25094 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/lazyframe/groupby.py
+-rw-r--r--   0     1001      123        0 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/py.typed
+-rw-r--r--   0     1001      123    38494 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/selectors.py
+-rw-r--r--   0     1001      123       69 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/series/__init__.py
+-rw-r--r--   0     1001      123     1572 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/series/_numpy.py
+-rw-r--r--   0     1001      123     2515 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/series/array.py
+-rw-r--r--   0     1001      123     1913 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/series/binary.py
+-rw-r--r--   0     1001      123     1692 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/series/categorical.py
+-rw-r--r--   0     1001      123    54653 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/series/datetime.py
+-rw-r--r--   0     1001      123    16940 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/series/list.py
+-rw-r--r--   0     1001      123   170756 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/series/series.py
+-rw-r--r--   0     1001      123    38879 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/series/string.py
+-rw-r--r--   0     1001      123     2542 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/series/struct.py
+-rw-r--r--   0     1001      123     5361 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/series/utils.py
+-rw-r--r--   0     1001      123     7559 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/slice.py
+-rw-r--r--   0     1001      123       75 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/sql/__init__.py
+-rw-r--r--   0     1001      123    17286 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/sql/context.py
+-rw-r--r--   0     1001      123     4793 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/string_cache.py
+-rw-r--r--   0     1001      123      362 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/testing/__init__.py
+-rw-r--r--   0     1001      123     1060 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/testing/_private.py
+-rw-r--r--   0     1001      123    16964 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/testing/asserts.py
+-rw-r--r--   0     1001      123      898 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/testing/parametric/__init__.py
+-rw-r--r--   0     1001      123    28187 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/testing/parametric/primitives.py
+-rw-r--r--   0     1001      123     3371 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/testing/parametric/profiles.py
+-rw-r--r--   0     1001      123    13165 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/testing/parametric/strategies.py
+-rw-r--r--   0     1001      123     6460 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/type_aliases.py
+-rw-r--r--   0     1001      123     1157 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/utils/__init__.py
+-rw-r--r--   0     1001      123    56946 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/utils/_construction.py
+-rw-r--r--   0     1001      123     4937 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/utils/_parse_expr_input.py
+-rw-r--r--   0     1001      123      647 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/utils/_scan.py
+-rw-r--r--   0     1001      123      579 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/utils/_wrap.py
+-rw-r--r--   0     1001      123      683 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/utils/build_info.py
+-rw-r--r--   0     1001      123     8702 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/utils/convert.py
+-rw-r--r--   0     1001      123     7199 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/utils/decorators.py
+-rw-r--r--   0     1001      123     1660 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/utils/meta.py
+-rw-r--r--   0     1001      123      514 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/utils/polars_version.py
+-rw-r--r--   0     1001      123     2509 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/utils/show_versions.py
+-rw-r--r--   0     1001      123    13340 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/polars/utils/various.py
+-rw-r--r--   0     1001      123     5370 2023-07-06 16:19:18.000000 polars_lts_cpu-0.18.6/pyproject.toml
+-rw-r--r--   0     1001      123      756 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/requirements-dev.txt
+-rw-r--r--   0     1001      123       70 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/requirements-lint.txt
+-rw-r--r--   0     1001      123     1610 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/scripts/check_stacklevels.py
+-rw-r--r--   0     1001      123    10980 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/apply/dataframe.rs
+-rw-r--r--   0     1001      123     6428 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/apply/lazy.rs
+-rw-r--r--   0     1001      123     8535 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/apply/mod.rs
+-rw-r--r--   0     1001      123    90654 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/apply/series.rs
+-rw-r--r--   0     1001      123       32 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/arrow_interop/mod.rs
+-rw-r--r--   0     1001      123     1306 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/arrow_interop/to_py.rs
+-rw-r--r--   0     1001      123     3902 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/arrow_interop/to_rust.rs
+-rw-r--r--   0     1001      123     5250 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/batched_csv.rs
+-rw-r--r--   0     1001      123    49813 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/conversion.rs
+-rw-r--r--   0     1001      123    46152 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/dataframe.rs
+-rw-r--r--   0     1001      123     3950 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/datatypes.rs
+-rw-r--r--   0     1001      123     3506 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/error.rs
+-rw-r--r--   0     1001      123      570 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/expr/array.rs
+-rw-r--r--   0     1001      123     2080 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/expr/binary.rs
+-rw-r--r--   0     1001      123      274 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/expr/categorical.rs
+-rw-r--r--   0     1001      123     6206 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/expr/datetime.rs
+-rw-r--r--   0     1001      123    35096 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/expr/general.rs
+-rw-r--r--   0     1001      123     4693 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/expr/list.rs
+-rw-r--r--   0     1001      123     3152 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/expr/meta.rs
+-rw-r--r--   0     1001      123      870 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/expr/mod.rs
+-rw-r--r--   0     1001      123     8366 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/expr/string.rs
+-rw-r--r--   0     1001      123      467 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/expr/struct.rs
+-rw-r--r--   0     1001      123     9482 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/file.rs
+-rw-r--r--   0     1001      123     2777 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/functions/eager.rs
+-rw-r--r--   0     1001      123     1657 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/functions/io.rs
+-rw-r--r--   0     1001      123    11595 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/functions/lazy.rs
+-rw-r--r--   0     1001      123     1312 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/functions/meta.rs
+-rw-r--r--   0     1001      123      217 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/functions/misc.rs
+-rw-r--r--   0     1001      123      102 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/functions/mod.rs
+-rw-r--r--   0     1001      123      689 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/functions/range.rs
+-rw-r--r--   0     1001      123     1474 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/functions/whenthen.rs
+-rw-r--r--   0     1001      123    28073 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/lazyframe.rs
+-rw-r--r--   0     1001      123     2670 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/lazygroupby.rs
+-rw-r--r--   0     1001      123     8553 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/lib.rs
+-rw-r--r--   0     1001      123       47 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/object.rs
+-rw-r--r--   0     1001      123     2989 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/on_startup.rs
+-rw-r--r--   0     1001      123      122 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/prelude.rs
+-rw-r--r--   0     1001      123      435 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/py_modules.rs
+-rw-r--r--   0     1001      123     1964 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/series/aggregation.rs
+-rw-r--r--   0     1001      123     5406 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/series/arithmetic.rs
+-rw-r--r--   0     1001      123     5138 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/series/comparison.rs
+-rw-r--r--   0     1001      123     9077 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/series/construction.rs
+-rw-r--r--   0     1001      123     8971 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/series/export.rs
+-rw-r--r--   0     1001      123    26606 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/series/mod.rs
+-rw-r--r--   0     1001      123     4569 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/series/numpy_ufunc.rs
+-rw-r--r--   0     1001      123     4046 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/series/set_at_idx.rs
+-rw-r--r--   0     1001      123     1036 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/sql.rs
+-rw-r--r--   0     1001      123     2335 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/src/utils.rs
+-rw-r--r--   0     1001      123     6165 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/README.md
+-rw-r--r--   0     1001      123     2189 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/benchmark/groupby-datagen.R
+-rw-r--r--   0     1001      123     7963 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/benchmark/run_h2oai_benchmark.py
+-rw-r--r--   0     1001      123     6530 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/benchmark/test_release.py
+-rw-r--r--   0     1001      123     4589 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/docs/run_doctest.py
+-rw-r--r--   0     1001      123        0 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/parametric/__init__.py
+-rw-r--r--   0     1001      123      179 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/parametric/conftest.py
+-rw-r--r--   0     1001      123     3856 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/parametric/test_dataframe.py
+-rw-r--r--   0     1001      123     2398 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/parametric/test_groupby_rolling.py
+-rw-r--r--   0     1001      123     1692 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/parametric/test_lazyframe.py
+-rw-r--r--   0     1001      123      976 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/parametric/test_lit.py
+-rw-r--r--   0     1001      123     6853 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/parametric/test_series.py
+-rw-r--r--   0     1001      123     8467 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/parametric/test_testing.py
+-rw-r--r--   0     1001      123     1554 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/parametric/time_series/test_to_datetime.py
+-rw-r--r--   0     1001      123        0 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/__init__.py
+-rw-r--r--   0     1001      123     3382 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/conftest.py
+-rw-r--r--   0     1001      123       86 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/datatypes/__init__.py
+-rw-r--r--   0     1001      123     1285 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/datatypes/test_array.py
+-rw-r--r--   0     1001      123      847 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/datatypes/test_binary.py
+-rw-r--r--   0     1001      123     1420 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/datatypes/test_bool.py
+-rw-r--r--   0     1001      123    13982 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/datatypes/test_categorical.py
+-rw-r--r--   0     1001      123     5222 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/datatypes/test_decimal.py
+-rw-r--r--   0     1001      123      549 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/datatypes/test_duration.py
+-rw-r--r--   0     1001      123      423 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/datatypes/test_integer.py
+-rw-r--r--   0     1001      123    14052 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/datatypes/test_list.py
+-rw-r--r--   0     1001      123      284 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/datatypes/test_null.py
+-rw-r--r--   0     1001      123     3028 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/datatypes/test_object.py
+-rw-r--r--   0     1001      123    27697 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/datatypes/test_struct.py
+-rw-r--r--   0     1001      123    87698 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/datatypes/test_temporal.py
+-rw-r--r--   0     1001      123      418 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/datatypes/test_time.py
+-rw-r--r--   0     1001      123        0 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/functions/__init__.py
+-rw-r--r--   0     1001      123    13970 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/functions/test_as_datatype.py
+-rw-r--r--   0     1001      123      480 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/functions/test_concat.py
+-rw-r--r--   0     1001      123    15574 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/functions/test_functions.py
+-rw-r--r--   0     1001      123    30418 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/functions/test_range.py
+-rw-r--r--   0     1001      123     3847 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/functions/test_repeat.py
+-rw-r--r--   0     1001      123      218 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/conftest.py
+-rw-r--r--   0     1001      123       16 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
+-rw-r--r--   0     1001      123       16 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
+-rw-r--r--   0     1001      123      905 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123      936 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123      972 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
+-rw-r--r--   0     1001      123      690 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
+-rw-r--r--   0     1001      123        0 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/empty.csv
+-rw-r--r--   0     1001      123     5959 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/example.xlsx
+-rw-r--r--   0     1001      123      457 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/foods1.csv
+-rw-r--r--   0     1001      123     2351 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/foods1.ipc
+-rw-r--r--   0     1001      123     1713 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/foods1.ndjson
+-rw-r--r--   0     1001      123     1427 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/foods1.parquet
+-rw-r--r--   0     1001      123      455 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/foods2.csv
+-rw-r--r--   0     1001      123     2351 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/foods2.ipc
+-rw-r--r--   0     1001      123     1711 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/foods2.ndjson
+-rw-r--r--   0     1001      123     1916 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/foods2.parquet
+-rw-r--r--   0     1001      123      455 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/foods3.csv
+-rw-r--r--   0     1001      123      457 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/foods4.csv
+-rw-r--r--   0     1001      123      452 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/foods5.csv
+-rw-r--r--   0     1001      123       49 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/gzipped.csv
+-rw-r--r--   0     1001      123       57 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/small.csv
+-rw-r--r--   0     1001      123      756 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/files/small.parquet
+-rw-r--r--   0     1001      123     1884 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/test_avro.py
+-rw-r--r--   0     1001      123    41164 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/test_csv.py
+-rw-r--r--   0     1001      123     6271 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/test_database.py
+-rw-r--r--   0     1001      123     6172 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/test_delta.py
+-rw-r--r--   0     1001      123    11169 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/test_excel.py
+-rw-r--r--   0     1001      123     5483 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/test_ipc.py
+-rw-r--r--   0     1001      123     4389 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/test_json.py
+-rw-r--r--   0     1001      123     7379 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/test_lazy_csv.py
+-rw-r--r--   0     1001      123     2060 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/test_lazy_ipc.py
+-rw-r--r--   0     1001      123     2867 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/test_lazy_json.py
+-rw-r--r--   0     1001      123    11145 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/test_lazy_parquet.py
+-rw-r--r--   0     1001      123     2012 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/test_other.py
+-rw-r--r--   0     1001      123    14157 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/test_parquet.py
+-rw-r--r--   0     1001      123      612 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/test_pickle.py
+-rw-r--r--   0     1001      123     3706 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/io/test_pyarrow_dataset.py
+-rw-r--r--   0     1001      123      509 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/namespaces/__init__.py
+-rw-r--r--   0     1001      123      589 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/namespaces/test_array.py
+-rw-r--r--   0     1001      123     3218 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/namespaces/test_binary.py
+-rw-r--r--   0     1001      123     2489 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/namespaces/test_categorical.py
+-rw-r--r--   0     1001      123    23231 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/namespaces/test_datetime.py
+-rw-r--r--   0     1001      123    15528 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/namespaces/test_list.py
+-rw-r--r--   0     1001      123     2472 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/namespaces/test_meta.py
+-rw-r--r--   0     1001      123    24050 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/namespaces/test_string.py
+-rw-r--r--   0     1001      123    20819 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/namespaces/test_strptime.py
+-rw-r--r--   0     1001      123      982 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/namespaces/test_struct.py
+-rw-r--r--   0     1001      123       85 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/__init__.py
+-rw-r--r--   0     1001      123     8008 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_aggregations.py
+-rw-r--r--   0     1001      123    10613 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_apply.py
+-rw-r--r--   0     1001      123     6896 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_arithmetic.py
+-rw-r--r--   0     1001      123     4940 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_comparison.py
+-rw-r--r--   0     1001      123     3275 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_drop.py
+-rw-r--r--   0     1001      123     8813 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_explode.py
+-rw-r--r--   0     1001      123     3664 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_filter.py
+-rw-r--r--   0     1001      123     1801 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_folds.py
+-rw-r--r--   0     1001      123    25037 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_groupby.py
+-rw-r--r--   0     1001      123     7649 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_groupby_rolling.py
+-rw-r--r--   0     1001      123     2983 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_is_in.py
+-rw-r--r--   0     1001      123    18993 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_join.py
+-rw-r--r--   0     1001      123    14952 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_join_asof.py
+-rw-r--r--   0     1001      123      643 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_melt.py
+-rw-r--r--   0     1001      123    10253 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_pivot.py
+-rw-r--r--   0     1001      123     3187 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_random.py
+-rw-r--r--   0     1001      123    24274 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_rolling.py
+-rw-r--r--   0     1001      123     2389 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_select.py
+-rw-r--r--   0     1001      123    20770 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_sort.py
+-rw-r--r--   0     1001      123     7395 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_statistics.py
+-rw-r--r--   0     1001      123     4130 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_transpose.py
+-rw-r--r--   0     1001      123      771 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_unique.py
+-rw-r--r--   0     1001      123    11644 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_window.py
+-rw-r--r--   0     1001      123     5480 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/operations/test_with_columns.py
+-rw-r--r--   0     1001      123        0 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/streaming/__init__.py
+-rw-r--r--   0     1001      123      196 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/streaming/conftest.py
+-rw-r--r--   0     1001      123      908 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/streaming/test_ooc.py
+-rw-r--r--   0     1001      123    19789 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/streaming/test_streaming.py
+-rw-r--r--   0     1001      123     4831 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_api.py
+-rw-r--r--   0     1001      123     1969 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_arity.py
+-rw-r--r--   0     1001      123    20397 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_cfg.py
+-rw-r--r--   0     1001      123    43560 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_constructors.py
+-rw-r--r--   0     1001      123      454 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_context.py
+-rw-r--r--   0     1001      123     2626 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_cse.py
+-rw-r--r--   0     1001      123     5191 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_datatypes.py
+-rw-r--r--   0     1001      123   120452 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_df.py
+-rw-r--r--   0     1001      123     2741 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_empty.py
+-rw-r--r--   0     1001      123    19301 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_errors.py
+-rw-r--r--   0     1001      123     2741 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_expr_multi_cols.py
+-rw-r--r--   0     1001      123    33619 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_exprs.py
+-rw-r--r--   0     1001      123     3516 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_fmt.py
+-rw-r--r--   0     1001      123     3512 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_interchange.py
+-rw-r--r--   0     1001      123    38530 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_interop.py
+-rw-r--r--   0     1001      123    49654 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_lazy.py
+-rw-r--r--   0     1001      123     2463 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_polars_import.py
+-rw-r--r--   0     1001      123     4883 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_predicates.py
+-rw-r--r--   0     1001      123     7572 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_projections.py
+-rw-r--r--   0     1001      123    11551 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_queries.py
+-rw-r--r--   0     1001      123     8100 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_rows.py
+-rw-r--r--   0     1001      123    13961 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_schema.py
+-rw-r--r--   0     1001      123    12341 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_selectors.py
+-rw-r--r--   0     1001      123     4107 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_serde.py
+-rw-r--r--   0     1001      123    82889 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_series.py
+-rw-r--r--   0     1001      123      657 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_single.py
+-rw-r--r--   0     1001      123    16616 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_sql.py
+-rw-r--r--   0     1001      123    35314 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/test_testing.py
+-rw-r--r--   0     1001      123       41 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/utils/__init__.py
+-rw-r--r--   0     1001      123      306 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/utils/test_build_info.py
+-rw-r--r--   0     1001      123     2855 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/utils/test_parse_expr_input.py
+-rw-r--r--   0     1001      123      247 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/utils/test_show_versions.py
+-rw-r--r--   0     1001      123     5026 2023-07-06 16:19:17.000000 polars_lts_cpu-0.18.6/tests/unit/utils/test_utils.py
+-rw-r--r--   0     1001      123    65129 2023-07-06 16:20:28.000000 polars_lts_cpu-0.18.6/Cargo.lock
+-rw-r--r--   0        0        0    14286 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.6/PKG-INFO
```

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/Cargo.toml` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/LICENSE` & `polars_lts_cpu-0.18.6/local_dependencies/polars-algo/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/array/default_arrays.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/array/default_arrays.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/array/fixed_size_list.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/array/fixed_size_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/array/get.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/array/get.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/array/list.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/array/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/array/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/array/null.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/array/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/array/slice.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/array/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/array/utf8.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/array/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/bit_util.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/bit_util.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/bitmap/mutable.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/bitmap/mutable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/commutative.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/commutative.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/div.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/div.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mul.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mul.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/bitwise.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/bitwise.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/cast.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/decimal.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/take/boolean.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/take/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/take/fixed_size_list.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/take/fixed_size_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/take/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/compute/tile.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/compute/tile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/conversion.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/data_types.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/data_types.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/floats/ord.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/floats/ord.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/index.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/index.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/is_valid.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/is_valid.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/agg_mean.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/agg_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/comparison.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/concatenate.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/concatenate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/ewm/average.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/ewm/average.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/float.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/float.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/list.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/rolling/window.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/rolling/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/set.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/sort_partition.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/sort_partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/string.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/kernels/time.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/kernels/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/slice.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/trusted_len/boolean.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/trusted_len/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/trusted_len/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/trusted_len/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-arrow/src/utils.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/Cargo.toml` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 diagonal_concat = []
 unique_counts = ["polars-plan/unique_counts"]
 log = ["polars-plan/log"]
 list_eval = []
 cumulative_eval = []
 chunked_ids = ["polars-plan/chunked_ids", "polars-core/chunked_ids"]
 list_to_struct = ["polars-plan/list_to_struct"]
-python = ["pyo3", "polars-plan/python"]
+python = ["pyo3", "polars-plan/python", "polars-core/python"]
 row_hash = ["polars-plan/row_hash"]
 string_justify = ["polars-plan/string_justify"]
 string_from_radix = ["polars-plan/string_from_radix"]
 arg_where = ["polars-plan/arg_where"]
 search_sorted = ["polars-plan/search_sorted"]
 merge_sorted = ["polars-plan/merge_sorted"]
 meta = ["polars-plan/meta"]
```

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/LICENSE` & `polars_lts_cpu-0.18.6/local_dependencies/polars-json/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/dot.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/dsl/eval.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/dsl/eval.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/dsl/functions.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/dsl/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/dsl/list.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/dsl/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/dsl/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/dsl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/frame/csv.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/frame/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/frame/file_list_reader.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/frame/file_list_reader.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/frame/ipc.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/frame/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/frame/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/frame/ndjson.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/frame/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/frame/parquet.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/frame/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/frame/pivot.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/frame/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/lib.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/exotic.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/exotic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/cache.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/cache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/state.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/streaming/checks.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/streaming/checks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/streaming/construct_pipeline.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/streaming/construct_pipeline.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/streaming/convert_alp.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/streaming/convert_alp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/prelude.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/aggregations.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/aggregations.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/arity.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/cse.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/io.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/logical.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/logical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/optimization_checks.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/optimization_checks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/predicate_queries.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/projection_queries.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/queries.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/streaming.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/streaming.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/tests/tpch.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/tests/tpch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-lazy/src/utils.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/Cargo.toml` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/LICENSE` & `polars_lts_cpu-0.18.6/local_dependencies/polars-sql/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/array/min_max.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/array/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/array/namespace.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/array/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/array/sum_mean.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/array/sum_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/interpolate.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/interpolate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/list/any_all.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/list/any_all.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/list/count.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/list/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/list/hash.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/list/hash.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/list/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/list/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs`

 * *Files 1% similar despite different names*

```diff
@@ -404,15 +404,15 @@
                         #[cfg(feature = "dtype-struct")]
                         DataType::Struct(_) => s = s.rechunk(),
                         // nothing
                         _ => {}
                     }
                     s
                 });
-                builder.append_opt_series(opt_s.as_ref())
+                builder.append_opt_series(opt_s.as_ref()).unwrap();
             });
             builder.finish()
         } else {
             // normal path which may contain same length list or unit length lists
             cast_rhs(&mut other, &inner_super_type, dtype, length, true)?;
 
             let vals_size_other = other
@@ -466,15 +466,15 @@
                 match inner_super_type {
                     // structs don't have chunks, so we must first rechunk the underlying series
                     #[cfg(feature = "dtype-struct")]
                     DataType::Struct(_) => acc = acc.rechunk(),
                     // nothing
                     _ => {}
                 }
-                builder.append_series(&acc);
+                builder.append_series(&acc).unwrap();
             }
             builder.finish()
         };
         Ok(out)
     }
 }
```

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/list/sets.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/list/sets.rs`

 * *Files 12% similar despite different names*

```diff
@@ -11,43 +11,14 @@
 use polars_arrow::utils::combine_validities_and;
 use polars_core::prelude::*;
 use polars_core::utils::align_chunks_binary;
 use polars_core::with_match_physical_integer_type;
 #[cfg(feature = "serde")]
 use serde::{Deserialize, Serialize};
 
-struct Intersection<'a, T, I: Iterator<Item = T>> {
-    // iterator of the first set
-    iter: I,
-    // the second set
-    other: &'a PlIndexSet<T>,
-}
-
-impl<'a, T, I> Iterator for Intersection<'a, T, I>
-where
-    T: Eq + Hash,
-    I: Iterator<Item = T>,
-{
-    type Item = T;
-
-    fn next(&mut self) -> Option<T> {
-        loop {
-            let elt = self.iter.next()?;
-            if self.other.contains(&elt) {
-                return Some(elt);
-            }
-        }
-    }
-
-    fn size_hint(&self) -> (usize, Option<usize>) {
-        let (_, upper) = self.iter.size_hint();
-        (0, upper)
-    }
-}
-
 trait MaterializeValues<K> {
     // extends the iterator to the values and returns the current offset
     fn extend_buf<I: Iterator<Item = K>>(&mut self, values: I) -> usize;
 }
 
 impl<T> MaterializeValues<Option<T>> for MutablePrimitiveArray<T>
 where
@@ -68,38 +39,31 @@
 
 fn set_operation<K, I, R>(
     set: &mut PlIndexSet<K>,
     set2: &mut PlIndexSet<K>,
     a: I,
     b: I,
     out: &mut R,
-    set_type: SetOperation,
+    set_op: SetOperation,
 ) -> usize
 where
     K: Eq + Hash + Copy,
     I: IntoIterator<Item = K>,
     R: MaterializeValues<K>,
 {
     set.clear();
     let a = a.into_iter();
     let b = b.into_iter();
 
-    match set_type {
+    match set_op {
         SetOperation::Intersection => {
-            let (smaller, larger) = if a.size_hint().0 <= b.size_hint().0 {
-                (a, b)
-            } else {
-                (b, a)
-            };
-            set.extend(smaller);
-            let iter = Intersection {
-                iter: larger,
-                other: set,
-            };
-            out.extend_buf(iter)
+            set2.clear();
+            set.extend(a);
+            set2.extend(b);
+            out.extend_buf(set.intersection(set2).copied())
         }
         SetOperation::Union => {
             set.extend(a);
             set.extend(b);
             out.extend_buf(set.drain(..))
         }
         SetOperation::Difference => {
@@ -146,15 +110,15 @@
 }
 
 fn primitive<T>(
     a: &PrimitiveArray<T>,
     b: &PrimitiveArray<T>,
     offsets_a: &[i64],
     offsets_b: &[i64],
-    set_type: SetOperation,
+    set_op: SetOperation,
     validity: Option<Bitmap>,
 ) -> ListArray<i64>
 where
     T: NativeType + Hash + Copy + Eq,
 {
     assert_eq!(offsets_a.len(), offsets_b.len());
 
@@ -184,22 +148,16 @@
                 .map(copied_opt);
             let b_iter = b
                 .into_iter()
                 .skip(start_b)
                 .take(end_b - start_b)
                 .map(copied_opt);
 
-            let offset = set_operation(
-                &mut set,
-                &mut set2,
-                a_iter,
-                b_iter,
-                &mut values_out,
-                set_type,
-            );
+            let offset =
+                set_operation(&mut set, &mut set2, a_iter, b_iter, &mut values_out, set_op);
             offsets.push(offset as i64);
         }
     }
     let offsets = unsafe { OffsetsBuffer::new_unchecked(offsets.into()) };
     let dtype = ListArray::<i64>::default_datatype(values_out.data_type().clone());
 
     let values: PrimitiveArray<T> = values_out.into();
@@ -207,15 +165,15 @@
 }
 
 fn binary(
     a: &BinaryArray<i64>,
     b: &BinaryArray<i64>,
     offsets_a: &[i64],
     offsets_b: &[i64],
-    set_type: SetOperation,
+    set_op: SetOperation,
     validity: Option<Bitmap>,
     as_utf8: bool,
 ) -> ListArray<i64> {
     assert_eq!(offsets_a.len(), offsets_b.len());
 
     let mut set = Default::default();
     let mut set2 = Default::default();
@@ -235,22 +193,16 @@
             let start_b = *offsets_b.get_unchecked(i - 1) as usize;
             let end_b = *offsets_b.get_unchecked(i) as usize;
 
             // going via skip iterator instead of slice doesn't heap alloc nor trigger a bitcount
             let a_iter = a.into_iter().skip(start_a).take(end_a - start_a);
             let b_iter = b.into_iter().skip(start_b).take(end_b - start_b);
 
-            let offset = set_operation(
-                &mut set,
-                &mut set2,
-                a_iter,
-                b_iter,
-                &mut values_out,
-                set_type,
-            );
+            let offset =
+                set_operation(&mut set, &mut set2, a_iter, b_iter, &mut values_out, set_op);
             offsets.push(offset as i64);
         }
     }
     let offsets = unsafe { OffsetsBuffer::new_unchecked(offsets.into()) };
     let values: BinaryArray<i64> = values_out.into();
 
     if as_utf8 {
@@ -278,15 +230,15 @@
         arr.validity().cloned(),
     )
 }
 
 fn array_set_operation(
     a: &ListArray<i64>,
     b: &ListArray<i64>,
-    set_type: SetOperation,
+    set_op: SetOperation,
 ) -> ListArray<i64> {
     let offsets_a = a.offsets().as_slice();
     let offsets_b = b.offsets().as_slice();
 
     let values_a = a.values();
     let values_b = b.values();
     assert_eq!(values_a.data_type(), values_b.data_type());
@@ -297,48 +249,48 @@
     match dtype {
         ArrowDataType::LargeUtf8 => {
             let a = values_a.as_any().downcast_ref::<Utf8Array<i64>>().unwrap();
             let b = values_b.as_any().downcast_ref::<Utf8Array<i64>>().unwrap();
 
             let a = utf8_to_binary(a);
             let b = utf8_to_binary(b);
-            binary(&a, &b, offsets_a, offsets_b, set_type, validity, true)
+            binary(&a, &b, offsets_a, offsets_b, set_op, validity, true)
         }
         ArrowDataType::LargeBinary => {
             let a = values_a
                 .as_any()
                 .downcast_ref::<BinaryArray<i64>>()
                 .unwrap();
             let b = values_b
                 .as_any()
                 .downcast_ref::<BinaryArray<i64>>()
                 .unwrap();
-            binary(a, b, offsets_a, offsets_b, set_type, validity, false)
+            binary(a, b, offsets_a, offsets_b, set_op, validity, false)
         }
         ArrowDataType::Boolean => {
             todo!("boolean type not yet supported in list union operations")
         }
         _ => {
             with_match_physical_integer_type!(dtype.into(), |$T| {
                 let a = values_a.as_any().downcast_ref::<PrimitiveArray<$T>>().unwrap();
                 let b = values_b.as_any().downcast_ref::<PrimitiveArray<$T>>().unwrap();
 
-                primitive(&a, &b, offsets_a, offsets_b, set_type, validity)
+                primitive(&a, &b, offsets_a, offsets_b, set_op, validity)
             })
         }
     }
 }
 
-pub fn list_set_operation(a: &ListChunked, b: &ListChunked, set_type: SetOperation) -> ListChunked {
+pub fn list_set_operation(a: &ListChunked, b: &ListChunked, set_op: SetOperation) -> ListChunked {
     let (a, b) = align_chunks_binary(a, b);
 
     // no downcasting needed as lists
     // already have logical types
     let chunks = a
         .downcast_iter()
         .zip(b.downcast_iter())
-        .map(|(a, b)| array_set_operation(a, b, set_type).boxed())
+        .map(|(a, b)| array_set_operation(a, b, set_op).boxed())
         .collect::<Vec<_>>();
 
     // safety: dtypes are correct
     unsafe { a.with_chunks(chunks) }
 }
```

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/set.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/strings/case.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/strings/case.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/chunked_array/top_k.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/chunked_array/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/frame/join/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/frame/join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/frame/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/frame/pivot/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/frame/pivot/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/frame/pivot/positioning.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/frame/pivot/positioning.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/approx_unique.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/approx_unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/cut.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/cut.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/floor_divide.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/floor_divide.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/fused.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/fused.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/is_first.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/is_first.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/is_unique.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/is_unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/log.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/log.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/rolling.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/search_sorted.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/to_dummies.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/to_dummies.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-ops/src/series/ops/various.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/src/series/ops/various.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/Cargo.toml` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/LICENSE` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dot.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/arithmetic.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/arity.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/array.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/array.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/binary.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/cat.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/cat.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/dt.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/dt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/expr.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/expr_dyn_fn.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/expr_dyn_fn.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/from.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/array.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/array.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/correlation.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/correlation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/fused.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/fused.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/list.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/log.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/log.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/random.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/range.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/range.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/arity.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/coerce.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/coerce.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/concat.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/concat.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/correlation.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/correlation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/horizontal.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/horizontal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/index.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/index.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/range.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/range.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/selectors.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/selectors.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/syntactic_sugar.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/syntactic_sugar.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/functions/temporal.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/functions/temporal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/list.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/meta.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1467,18 +1467,14 @@
     #[cfg(feature = "cutqcut")]
     pub fn cut(self, breaks: Vec<f64>, labels: Option<Vec<String>>, left_closed: bool) -> Expr {
         self.apply_private(FunctionExpr::Cut {
             breaks,
             labels,
             left_closed,
         })
-        .with_function_options(|mut opt| {
-            opt.allow_group_aware = false;
-            opt
-        })
     }
 
     #[cfg(feature = "cutqcut")]
     pub fn qcut(
         self,
         probs: Vec<f64>,
         labels: Option<Vec<String>>,
@@ -1487,18 +1483,14 @@
     ) -> Expr {
         self.apply_private(FunctionExpr::QCut {
             probs,
             labels,
             left_closed,
             allow_duplicates,
         })
-        .with_function_options(|mut opt| {
-            opt.allow_group_aware = false;
-            opt
-        })
     }
 
     #[cfg(feature = "diff")]
     pub fn diff(self, n: i64, null_behavior: NullBehavior) -> Expr {
         self.apply_private(FunctionExpr::Diff(n, null_behavior))
     }
```

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/options.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/options.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/python_udf.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/python_udf.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/random.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/selector.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/selector.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/string.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/dsl/struct_.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/dsl/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/frame/opt_state.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/frame/opt_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/alp.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/alp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/apply.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/builder.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/conversion.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/format.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/format.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/functions/python_udf.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/functions/python_udf.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/iterator.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/lit.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/lit.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/fused.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/fused.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/options.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/options.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/projection.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/schema.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/tree_format.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/tree_format.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/visitor/expr.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/visitor/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/visitor/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/visitor/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/logical_plan/visitor/visitors.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/logical_plan/visitor/visitors.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/prelude.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-plan/src/utils.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/Cargo.toml` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/LICENSE` & `polars_lts_cpu-0.18.6/local_dependencies/polars-arrow/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/base_utc_offset.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/base_utc_offset.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/date.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/datetime.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/duration.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/kernels.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/kernels.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/time.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/date_range.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/date_range.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/dst_offset.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/dst_offset.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/groupby/dynamic.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/groupby/dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/lib.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/month_end.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/month_end.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/month_start.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/month_start.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/round.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/round.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/series/_trait.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/series/_trait.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/series/implementations/floats.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/series/implementations/integers.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/series/implementations/integers.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/series/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/truncate.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/truncate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/upsample.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/upsample.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/utils.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/windows/bounds.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/windows/bounds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/windows/calendar.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/windows/calendar.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/windows/duration.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/windows/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/windows/groupby.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/windows/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/windows/test.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/windows/test.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-time/src/windows/window.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/src/windows/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-row/Cargo.toml` & `polars_lts_cpu-0.18.6/local_dependencies/polars-row/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-row/LICENSE` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-row/src/decode.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-row/src/decode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-row/src/encode.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-row/src/encode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-row/src/fixed.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-row/src/fixed.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-row/src/lib.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-row/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-row/src/row.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-row/src/row.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-row/src/utils.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-row/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-row/src/variable.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-row/src/variable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/Cargo.toml` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/LICENSE` & `polars_lts_cpu-0.18.6/local_dependencies/polars-plan/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/operators/filter.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/operators/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/operators/function.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/operators/function.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/operators/pass.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/operators/pass.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/operators/projection.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/operators/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/operators/reproject.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/operators/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/source.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/source.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/io.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/memory.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/memory.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/slice.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sinks/utils.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sinks/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sources/csv.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sources/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sources/frame.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sources/frame.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sources/parquet.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sources/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sources/reproject.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sources/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/executors/sources/union.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/executors/sources/union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/operators/chunks.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/operators/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/operators/operator.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/operators/operator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/operators/sink.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/operators/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/pipeline/convert.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/pipeline/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-pipe/src/pipeline/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-pipe/src/pipeline/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/Cargo.toml` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/LICENSE` & `polars_lts_cpu-0.18.6/local_dependencies/polars-error/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/avro/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/avro/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/avro/read.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/avro/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/avro/write.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/avro/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/cloud/adaptors.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/cloud/adaptors.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/cloud/glob.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/cloud/glob.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/cloud/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/cloud/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/buffer.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/parser.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/parser.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/read.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/read_impl/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/read_impl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/splitfields.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/splitfields.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/utils.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/write.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/csv/write_impl.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/csv/write_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/ipc/ipc_file.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/ipc/ipc_file.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/ipc/ipc_stream.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/ipc/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/ipc/mmap.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/ipc/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/ipc/write.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/ipc/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/ipc/write_async.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/ipc/write_async.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/json/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/json/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/lib.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/mmap.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/ndjson/buffer.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/ndjson/buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/ndjson/core.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/ndjson/core.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/parquet/async_impl.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/parquet/async_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/parquet/mmap.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/parquet/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/parquet/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/parquet/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/parquet/predicates.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/parquet/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/parquet/read.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/parquet/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/parquet/read_impl.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/parquet/read_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/parquet/write.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/parquet/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/partition.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/predicates.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/prelude.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-io/src/utils.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/Cargo.toml` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/LICENSE` & `polars_lts_cpu-0.18.6/local_dependencies/polars-time/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/arithmetic/decimal.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/arithmetic/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/arithmetic/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/arithmetic/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/arithmetic/numeric.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/arithmetic/numeric.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/array/iterator.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/array/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/array/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/bitwise.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/bitwise.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/builder/binary.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/builder/fixed_size_list.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/fixed_size_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/builder/from.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/builder/list.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,709 +1,503 @@
-use polars_arrow::array::list::AnonymousBuilder;
-use polars_arrow::array::null::MutableNullArray;
-use polars_arrow::prelude::*;
+use arrow::offset::Offsets;
+use polars_arrow::kernels::concatenate::concatenate_owned_unchecked;
+use polars_utils::unwrap::UnwrapUncheckedRelease;
 
 use super::*;
+#[cfg(feature = "dtype-struct")]
+use crate::chunked_array::builder::AnonymousOwnedListBuilder;
 
-pub trait ListBuilderTrait {
-    fn append_opt_series(&mut self, opt_s: Option<&Series>) {
-        match opt_s {
-            Some(s) => self.append_series(s),
-            None => self.append_null(),
-        }
-    }
-    fn append_series(&mut self, s: &Series);
-    fn append_null(&mut self);
-    fn finish(&mut self) -> ListChunked;
-}
-
-impl<S: ?Sized> ListBuilderTrait for Box<S>
-where
-    S: ListBuilderTrait,
-{
-    fn append_opt_series(&mut self, opt_s: Option<&Series>) {
-        (**self).append_opt_series(opt_s)
-    }
-
-    fn append_series(&mut self, s: &Series) {
-        (**self).append_series(s)
-    }
-
-    fn append_null(&mut self) {
-        (**self).append_null()
-    }
-
-    fn finish(&mut self) -> ListChunked {
-        (**self).finish()
-    }
-}
-
-pub struct ListPrimitiveChunkedBuilder<T>
-where
-    T: PolarsNumericType,
-{
-    pub builder: LargePrimitiveBuilder<T::Native>,
-    field: Field,
-    fast_explode: bool,
-}
-
-macro_rules! finish_list_builder {
-    ($self:ident) => {{
-        let arr = $self.builder.as_box();
-
-        let mut ca = ListChunked {
-            field: Arc::new($self.field.clone()),
-            chunks: vec![arr],
-            phantom: PhantomData,
-            ..Default::default()
-        };
-        ca.compute_len();
-        if $self.fast_explode {
-            ca.set_fast_explode()
-        }
-        ca
-    }};
+pub trait AggList {
+    /// # Safety
+    ///
+    /// groups should be in bounds
+    unsafe fn agg_list(&self, _groups: &GroupsProxy) -> Series;
 }
 
-impl<T> ListPrimitiveChunkedBuilder<T>
+impl<T> AggList for ChunkedArray<T>
 where
     T: PolarsNumericType,
+    ChunkedArray<T>: IntoSeries,
 {
-    pub fn new(
-        name: &str,
-        capacity: usize,
-        values_capacity: usize,
-        logical_type: DataType,
-    ) -> Self {
-        let values = MutablePrimitiveArray::<T::Native>::with_capacity(values_capacity);
-        let builder = LargePrimitiveBuilder::<T::Native>::new_with_capacity(values, capacity);
-        let field = Field::new(name, DataType::List(Box::new(logical_type)));
-
-        Self {
-            builder,
-            field,
-            fast_explode: true,
-        }
-    }
+    unsafe fn agg_list(&self, groups: &GroupsProxy) -> Series {
+        let ca = self.rechunk();
 
-    #[inline]
-    pub fn append_slice(&mut self, items: &[T::Native]) {
-        let values = self.builder.mut_values();
-        values.extend_from_slice(items);
-        self.builder.try_push_valid().unwrap();
+        match groups {
+            GroupsProxy::Idx(groups) => {
+                let mut can_fast_explode = true;
+
+                let arr = ca.downcast_iter().next().unwrap();
+                let values = arr.values();
+
+                let mut offsets = Vec::<i64>::with_capacity(groups.len() + 1);
+                let mut length_so_far = 0i64;
+                offsets.push(length_so_far);
+
+                let mut list_values = Vec::<T::Native>::with_capacity(self.len());
+                groups.iter().for_each(|(_, idx)| {
+                    let idx_len = idx.len();
+                    if idx_len == 0 {
+                        can_fast_explode = false;
+                    }
 
-        if items.is_empty() {
-            self.fast_explode = false;
-        }
-    }
+                    length_so_far += idx_len as i64;
+                    // Safety:
+                    // group tuples are in bounds
+                    {
+                        list_values.extend(idx.iter().map(|idx| {
+                            debug_assert!((*idx as usize) < values.len());
+                            *values.get_unchecked(*idx as usize)
+                        }));
+                        // Safety:
+                        // we know that offsets has allocated enough slots
+                        offsets.push_unchecked(length_so_far);
+                    }
+                });
 
-    #[inline]
-    pub fn append_opt_slice(&mut self, opt_v: Option<&[T::Native]>) {
-        match opt_v {
-            Some(items) => self.append_slice(items),
-            None => {
-                self.builder.push_null();
+                let validity = if arr.null_count() > 0 {
+                    let old_validity = arr.validity().unwrap();
+                    let mut validity = MutableBitmap::from_len_set(list_values.len());
+
+                    let mut count = 0;
+                    groups.iter().for_each(|(_, idx)| {
+                        for i in idx {
+                            if !old_validity.get_bit_unchecked(*i as usize) {
+                                validity.set_bit_unchecked(count, false)
+                            }
+                            count += 1;
+                        }
+                    });
+                    Some(validity.into())
+                } else {
+                    None
+                };
+
+                let array =
+                    PrimitiveArray::new(T::get_dtype().to_arrow(), list_values.into(), validity);
+                let data_type = ListArray::<i64>::default_datatype(T::get_dtype().to_arrow());
+                // Safety:
+                // offsets are monotonically increasing
+                let arr = ListArray::<i64>::new(
+                    data_type,
+                    Offsets::new_unchecked(offsets).into(),
+                    Box::new(array),
+                    None,
+                );
+
+                let mut ca = unsafe { ListChunked::from_chunks(self.name(), vec![Box::new(arr)]) };
+                if can_fast_explode {
+                    ca.set_fast_explode()
+                }
+                ca.into()
             }
-        }
-    }
-    /// Appends from an iterator over values
-    #[inline]
-    pub fn append_iter_values<I: Iterator<Item = T::Native> + TrustedLen>(&mut self, iter: I) {
-        let values = self.builder.mut_values();
-
-        if iter.size_hint().0 == 0 {
-            self.fast_explode = false;
-        }
-        // Safety
-        // trusted len, trust the type system
-        unsafe { values.extend_trusted_len_values_unchecked(iter) };
-        self.builder.try_push_valid().unwrap();
-    }
+            GroupsProxy::Slice { groups, .. } => {
+                let mut can_fast_explode = true;
+                let arr = ca.downcast_iter().next().unwrap();
+                let values = arr.values();
+
+                let mut offsets = Vec::<i64>::with_capacity(groups.len() + 1);
+                let mut length_so_far = 0i64;
+                offsets.push(length_so_far);
+
+                let mut list_values = Vec::<T::Native>::with_capacity(self.len());
+                groups.iter().for_each(|&[first, len]| {
+                    if len == 0 {
+                        can_fast_explode = false;
+                    }
 
-    /// Appends from an iterator over values
-    #[inline]
-    pub fn append_iter<I: Iterator<Item = Option<T::Native>> + TrustedLen>(&mut self, iter: I) {
-        let values = self.builder.mut_values();
+                    length_so_far += len as i64;
+                    list_values.extend_from_slice(&values[first as usize..(first + len) as usize]);
+                    {
+                        // Safety:
+                        // we know that offsets has allocated enough slots
+                        offsets.push_unchecked(length_so_far);
+                    }
+                });
 
-        if iter.size_hint().0 == 0 {
-            self.fast_explode = false;
+                let validity = if arr.null_count() > 0 {
+                    let old_validity = arr.validity().unwrap();
+                    let mut validity = MutableBitmap::from_len_set(list_values.len());
+
+                    let mut count = 0;
+                    groups.iter().for_each(|[first, len]| {
+                        for i in *first..(*first + *len) {
+                            if !old_validity.get_bit_unchecked(i as usize) {
+                                validity.set_bit_unchecked(count, false)
+                            }
+                            count += 1;
+                        }
+                    });
+                    Some(validity.into())
+                } else {
+                    None
+                };
+
+                let array =
+                    PrimitiveArray::new(T::get_dtype().to_arrow(), list_values.into(), validity);
+                let data_type = ListArray::<i64>::default_datatype(T::get_dtype().to_arrow());
+                let arr = ListArray::<i64>::new(
+                    data_type,
+                    Offsets::new_unchecked(offsets).into(),
+                    Box::new(array),
+                    None,
+                );
+                let mut ca = unsafe { ListChunked::from_chunks(self.name(), vec![Box::new(arr)]) };
+                if can_fast_explode {
+                    ca.set_fast_explode()
+                }
+                ca.into()
+            }
         }
-        // Safety
-        // trusted len, trust the type system
-        unsafe { values.extend_trusted_len_unchecked(iter) };
-        self.builder.try_push_valid().unwrap();
     }
 }
 
-impl<T> ListBuilderTrait for ListPrimitiveChunkedBuilder<T>
-where
-    T: PolarsNumericType,
-{
-    #[inline]
-    fn append_opt_series(&mut self, opt_s: Option<&Series>) {
-        match opt_s {
-            Some(s) => {
-                self.append_series(s);
+impl AggList for BooleanChunked {
+    unsafe fn agg_list(&self, groups: &GroupsProxy) -> Series {
+        match groups {
+            GroupsProxy::Idx(groups) => {
+                let mut builder =
+                    ListBooleanChunkedBuilder::new(self.name(), groups.len(), self.len());
+                for idx in groups.all().iter() {
+                    let ca = { self.take_unchecked(idx.into()) };
+                    builder.append(&ca)
+                }
+                builder.finish().into_series()
             }
-            None => self.append_null(),
-        }
-    }
-
-    #[inline]
-    fn append_null(&mut self) {
-        self.fast_explode = false;
-        self.builder.push_null();
-    }
-
-    #[inline]
-    fn append_series(&mut self, s: &Series) {
-        if s.is_empty() {
-            self.fast_explode = false;
-        }
-        let physical = s.to_physical_repr();
-        let ca = physical.unpack::<T>().unwrap();
-        let values = self.builder.mut_values();
-
-        ca.downcast_iter().for_each(|arr| {
-            if !arr.has_validity() {
-                values.extend_from_slice(arr.values().as_slice())
-            } else {
-                // Safety:
-                // Arrow arrays are trusted length iterators.
-                unsafe { values.extend_trusted_len_unchecked(arr.into_iter()) }
+            GroupsProxy::Slice { groups, .. } => {
+                let mut builder =
+                    ListBooleanChunkedBuilder::new(self.name(), groups.len(), self.len());
+                for [first, len] in groups {
+                    let ca = self.slice(*first as i64, *len as usize);
+                    builder.append(&ca)
+                }
+                builder.finish().into_series()
             }
-        });
-        // overflow of i64 is far beyond polars capable lengths.
-        unsafe { self.builder.try_push_valid().unwrap_unchecked() };
-    }
-
-    fn finish(&mut self) -> ListChunked {
-        finish_list_builder!(self)
-    }
-}
-
-type LargePrimitiveBuilder<T> = MutableListArray<i64, MutablePrimitiveArray<T>>;
-type LargeListUtf8Builder = MutableListArray<i64, MutableUtf8Array<i64>>;
-type LargeListBinaryBuilder = MutableListArray<i64, MutableBinaryArray<i64>>;
-type LargeListBooleanBuilder = MutableListArray<i64, MutableBooleanArray>;
-type LargeListNullBuilder = MutableListArray<i64, MutableNullArray>;
-
-pub struct ListUtf8ChunkedBuilder {
-    builder: LargeListUtf8Builder,
-    field: Field,
-    fast_explode: bool,
-}
-
-impl ListUtf8ChunkedBuilder {
-    pub fn new(name: &str, capacity: usize, values_capacity: usize) -> Self {
-        let values = MutableUtf8Array::<i64>::with_capacity(values_capacity);
-        let builder = LargeListUtf8Builder::new_with_capacity(values, capacity);
-        let field = Field::new(name, DataType::List(Box::new(DataType::Utf8)));
-
-        ListUtf8ChunkedBuilder {
-            builder,
-            field,
-            fast_explode: true,
-        }
-    }
-
-    #[inline]
-    pub fn append_trusted_len_iter<'a, I: Iterator<Item = Option<&'a str>> + TrustedLen>(
-        &mut self,
-        iter: I,
-    ) {
-        let values = self.builder.mut_values();
-
-        if iter.size_hint().0 == 0 {
-            self.fast_explode = false;
-        }
-        // Safety
-        // trusted len, trust the type system
-        unsafe { values.extend_trusted_len_unchecked(iter) };
-        self.builder.try_push_valid().unwrap();
-    }
-
-    #[inline]
-    pub fn append_values_iter<'a, I: Iterator<Item = &'a str>>(&mut self, iter: I) {
-        let values = self.builder.mut_values();
-
-        if iter.size_hint().0 == 0 {
-            self.fast_explode = false;
         }
-        values.extend_values(iter);
-        self.builder.try_push_valid().unwrap();
-    }
-
-    #[inline]
-    pub(crate) fn append(&mut self, ca: &Utf8Chunked) {
-        let value_builder = self.builder.mut_values();
-        value_builder.try_extend(ca).unwrap();
-        self.builder.try_push_valid().unwrap();
     }
 }
 
-impl ListBuilderTrait for ListUtf8ChunkedBuilder {
-    #[inline]
-    fn append_opt_series(&mut self, opt_s: Option<&Series>) {
-        match opt_s {
-            Some(s) => self.append_series(s),
-            None => {
-                self.append_null();
+impl AggList for Utf8Chunked {
+    unsafe fn agg_list(&self, groups: &GroupsProxy) -> Series {
+        // TODO: dispatch via binary
+        match groups {
+            GroupsProxy::Idx(groups) => {
+                let mut builder =
+                    ListUtf8ChunkedBuilder::new(self.name(), groups.len(), self.len());
+                for idx in groups.all().iter() {
+                    let ca = { self.take_unchecked(idx.into()) };
+                    builder.append(&ca)
+                }
+                builder.finish().into_series()
+            }
+            GroupsProxy::Slice { groups, .. } => {
+                let mut builder =
+                    ListUtf8ChunkedBuilder::new(self.name(), groups.len(), self.len());
+                for [first, len] in groups {
+                    let ca = self.slice(*first as i64, *len as usize);
+                    builder.append(&ca)
+                }
+                builder.finish().into_series()
             }
         }
     }
-
-    #[inline]
-    fn append_null(&mut self) {
-        self.fast_explode = false;
-        self.builder.push_null();
-    }
-
-    #[inline]
-    fn append_series(&mut self, s: &Series) {
-        if s.is_empty() {
-            self.fast_explode = false;
-        }
-        let ca = s.utf8().unwrap();
-        self.append(ca)
-    }
-
-    fn finish(&mut self) -> ListChunked {
-        finish_list_builder!(self)
-    }
-}
-
-pub struct ListBinaryChunkedBuilder {
-    builder: LargeListBinaryBuilder,
-    field: Field,
-    fast_explode: bool,
-}
-
-impl ListBinaryChunkedBuilder {
-    pub fn new(name: &str, capacity: usize, values_capacity: usize) -> Self {
-        let values = MutableBinaryArray::<i64>::with_capacity(values_capacity);
-        let builder = LargeListBinaryBuilder::new_with_capacity(values, capacity);
-        let field = Field::new(name, DataType::List(Box::new(DataType::Binary)));
-
-        ListBinaryChunkedBuilder {
-            builder,
-            field,
-            fast_explode: true,
-        }
-    }
-
-    pub fn append_trusted_len_iter<'a, I: Iterator<Item = Option<&'a [u8]>> + TrustedLen>(
-        &mut self,
-        iter: I,
-    ) {
-        let values = self.builder.mut_values();
-
-        if iter.size_hint().0 == 0 {
-            self.fast_explode = false;
-        }
-        // Safety
-        // trusted len, trust the type system
-        unsafe { values.extend_trusted_len_unchecked(iter) };
-        self.builder.try_push_valid().unwrap();
-    }
-
-    pub fn append_values_iter<'a, I: Iterator<Item = &'a [u8]>>(&mut self, iter: I) {
-        let values = self.builder.mut_values();
-
-        if iter.size_hint().0 == 0 {
-            self.fast_explode = false;
-        }
-        values.extend_values(iter);
-        self.builder.try_push_valid().unwrap();
-    }
-
-    pub(crate) fn append(&mut self, ca: &BinaryChunked) {
-        let value_builder = self.builder.mut_values();
-        value_builder.try_extend(ca).unwrap();
-        self.builder.try_push_valid().unwrap();
-    }
 }
 
-impl ListBuilderTrait for ListBinaryChunkedBuilder {
-    fn append_opt_series(&mut self, opt_s: Option<&Series>) {
-        match opt_s {
-            Some(s) => self.append_series(s),
-            None => {
-                self.append_null();
+impl AggList for BinaryChunked {
+    unsafe fn agg_list(&self, groups: &GroupsProxy) -> Series {
+        match groups {
+            GroupsProxy::Idx(groups) => {
+                let mut builder =
+                    ListBinaryChunkedBuilder::new(self.name(), groups.len(), self.len());
+                for idx in groups.all().iter() {
+                    let ca = { self.take_unchecked(idx.into()) };
+                    builder.append(&ca)
+                }
+                builder.finish().into_series()
+            }
+            GroupsProxy::Slice { groups, .. } => {
+                let mut builder =
+                    ListBinaryChunkedBuilder::new(self.name(), groups.len(), self.len());
+                for [first, len] in groups {
+                    let ca = self.slice(*first as i64, *len as usize);
+                    builder.append(&ca)
+                }
+                builder.finish().into_series()
             }
         }
     }
-
-    #[inline]
-    fn append_null(&mut self) {
-        self.fast_explode = false;
-        self.builder.push_null();
-    }
-
-    fn append_series(&mut self, s: &Series) {
-        if s.is_empty() {
-            self.fast_explode = false;
-        }
-        let ca = s.binary().unwrap();
-        self.append(ca)
-    }
-
-    fn finish(&mut self) -> ListChunked {
-        finish_list_builder!(self)
-    }
 }
 
-pub struct ListBooleanChunkedBuilder {
-    builder: LargeListBooleanBuilder,
-    field: Field,
-    fast_explode: bool,
-}
-
-impl ListBooleanChunkedBuilder {
-    pub fn new(name: &str, capacity: usize, values_capacity: usize) -> Self {
-        let values = MutableBooleanArray::with_capacity(values_capacity);
-        let builder = LargeListBooleanBuilder::new_with_capacity(values, capacity);
-        let field = Field::new(name, DataType::List(Box::new(DataType::Boolean)));
-
-        Self {
-            builder,
-            field,
-            fast_explode: true,
-        }
-    }
-
-    #[inline]
-    pub fn append_iter<I: Iterator<Item = Option<bool>> + TrustedLen>(&mut self, iter: I) {
-        let values = self.builder.mut_values();
-
-        if iter.size_hint().0 == 0 {
-            self.fast_explode = false;
-        }
-        // Safety
-        // trusted len, trust the type system
-        unsafe { values.extend_trusted_len_unchecked(iter) };
-        self.builder.try_push_valid().unwrap();
-    }
-
-    #[inline]
-    pub(crate) fn append(&mut self, ca: &BooleanChunked) {
-        if ca.is_empty() {
-            self.fast_explode = false;
+fn agg_list_list<F: Fn(&ListChunked, bool, &mut Vec<i64>, &mut i64, &mut Vec<ArrayRef>) -> bool>(
+    ca: &ListChunked,
+    groups_len: usize,
+    func: F,
+) -> Series {
+    let inner_dtype = ca.inner_dtype();
+    let inner_dtype_physical = inner_dtype.to_physical();
+    let can_fast_explode = true;
+    let mut offsets = Vec::<i64>::with_capacity(groups_len + 1);
+    let mut length_so_far = 0i64;
+    offsets.push(length_so_far);
+
+    let mut list_values = Vec::with_capacity(groups_len);
+
+    let can_fast_explode = func(
+        ca,
+        can_fast_explode,
+        &mut offsets,
+        &mut length_so_far,
+        &mut list_values,
+    );
+    if groups_len == 0 {
+        list_values.push(ca.chunks[0].sliced(0, 0))
+    }
+    let list_values = concatenate_owned_unchecked(&list_values).unwrap();
+    let data_type = ListArray::<i64>::default_datatype(list_values.data_type().clone());
+    // Safety:
+    // offsets are monotonically increasing
+    let arr = unsafe {
+        Box::new(ListArray::<i64>::new(
+            data_type,
+            Offsets::new_unchecked(offsets).into(),
+            list_values,
+            None,
+        )) as ArrayRef
+    };
+    let mut listarr = unsafe { ListChunked::from_chunks(ca.name(), vec![arr]) };
+    if can_fast_explode {
+        listarr.set_fast_explode()
+    }
+    if inner_dtype_physical != inner_dtype {
+        listarr.to_physical(DataType::List(Box::new(inner_dtype)));
+    }
+    listarr.into_series()
+}
+
+impl AggList for ListChunked {
+    unsafe fn agg_list(&self, groups: &GroupsProxy) -> Series {
+        match groups {
+            GroupsProxy::Idx(groups) => {
+                let func = |ca: &ListChunked,
+                            mut can_fast_explode: bool,
+                            offsets: &mut Vec<i64>,
+                            length_so_far: &mut i64,
+                            list_values: &mut Vec<ArrayRef>| {
+                    assert!(list_values.capacity() >= groups.len());
+                    groups.iter().for_each(|(_, idx)| {
+                        let idx_len = idx.len();
+                        if idx_len == 0 {
+                            can_fast_explode = false;
+                        }
+
+                        *length_so_far += idx_len as i64;
+                        // Safety:
+                        // group tuples are in bounds
+                        {
+                            let mut s = ca.take_unchecked(idx.into());
+                            let arr = s.chunks.pop().unwrap_unchecked_release();
+                            list_values.push_unchecked(arr);
+
+                            // Safety:
+                            // we know that offsets has allocated enough slots
+                            offsets.push_unchecked(*length_so_far);
+                        }
+                    });
+                    can_fast_explode
+                };
+
+                agg_list_list(self, groups.len(), func)
+            }
+            GroupsProxy::Slice { groups, .. } => {
+                let func = |ca: &ListChunked,
+                            mut can_fast_explode: bool,
+                            offsets: &mut Vec<i64>,
+                            length_so_far: &mut i64,
+                            list_values: &mut Vec<ArrayRef>| {
+                    assert!(list_values.capacity() >= groups.len());
+                    groups.iter().for_each(|&[first, len]| {
+                        if len == 0 {
+                            can_fast_explode = false;
+                        }
+
+                        *length_so_far += len as i64;
+                        let mut s = ca.slice(first as i64, len as usize);
+                        let arr = s.chunks.pop().unwrap_unchecked_release();
+                        list_values.push_unchecked(arr);
+
+                        {
+                            // Safety:
+                            // we know that offsets has allocated enough slots
+                            offsets.push_unchecked(*length_so_far);
+                        }
+                    });
+                    can_fast_explode
+                };
+
+                agg_list_list(self, groups.len(), func)
+            }
         }
-        let value_builder = self.builder.mut_values();
-        value_builder.extend(ca);
-        self.builder.try_push_valid().unwrap();
     }
 }
 
-impl ListBuilderTrait for ListBooleanChunkedBuilder {
-    fn append_opt_series(&mut self, opt_s: Option<&Series>) {
-        match opt_s {
-            Some(s) => self.append_series(s),
-            None => {
-                self.append_null();
+#[cfg(feature = "dtype-array")]
+fn agg_list_fixed_size_list<F: Fn(&ArrayChunked, &mut Vec<ArrayRef>)>(
+    ca: &ArrayChunked,
+    groups_len: usize,
+    func: F,
+    width: usize,
+) -> Series {
+    let inner_dtype = ca.inner_dtype();
+    let inner_dtype_physical = inner_dtype.to_physical();
+    let mut list_values = Vec::with_capacity(groups_len);
+
+    func(ca, &mut list_values);
+    if groups_len == 0 {
+        list_values.push(ca.chunks[0].sliced(0, 0))
+    }
+    let list_values = concatenate_owned_unchecked(&list_values).unwrap();
+    let data_type = FixedSizeListArray::default_datatype(list_values.data_type().clone(), width);
+    let arr = Box::new(FixedSizeListArray::new(data_type, list_values, None)) as ArrayRef;
+    let mut listarr = unsafe { ListChunked::from_chunks(ca.name(), vec![arr]) };
+    if inner_dtype_physical != inner_dtype {
+        listarr.to_physical(DataType::List(Box::new(inner_dtype)));
+    }
+    listarr.into_series()
+}
+
+#[cfg(feature = "dtype-array")]
+impl AggList for ArrayChunked {
+    unsafe fn agg_list(&self, groups: &GroupsProxy) -> Series {
+        match groups {
+            GroupsProxy::Idx(groups) => {
+                let func = |ca: &ArrayChunked, list_values: &mut Vec<ArrayRef>| {
+                    assert!(list_values.capacity() >= groups.len());
+                    groups.iter().for_each(|(_, idx)| {
+                        // Safety:
+                        // group tuples are in bounds
+                        {
+                            let mut s = ca.take_unchecked(idx.into());
+                            let arr = s.chunks.pop().unwrap_unchecked_release();
+                            list_values.push_unchecked(arr);
+                        }
+                    });
+                };
+
+                agg_list_fixed_size_list(self, groups.len(), func, self.width())
+            }
+            GroupsProxy::Slice { groups, .. } => {
+                let func = |ca: &ArrayChunked, list_values: &mut Vec<ArrayRef>| {
+                    assert!(list_values.capacity() >= groups.len());
+                    groups.iter().for_each(|&[first, len]| {
+                        let mut s = ca.slice(first as i64, len as usize);
+                        let arr = s.chunks.pop().unwrap_unchecked_release();
+                        list_values.push_unchecked(arr);
+                    });
+                };
+
+                agg_list_fixed_size_list(self, groups.len(), func, self.width())
             }
         }
     }
-
-    #[inline]
-    fn append_null(&mut self) {
-        self.fast_explode = false;
-        self.builder.push_null();
-    }
-
-    #[inline]
-    fn append_series(&mut self, s: &Series) {
-        let ca = s.bool().unwrap();
-        self.append(ca)
-    }
-
-    fn finish(&mut self) -> ListChunked {
-        finish_list_builder!(self)
-    }
 }
 
-impl ListBuilderTrait for LargeListNullBuilder {
-    #[inline]
-    fn append_series(&mut self, _s: &Series) {
-        self.push_null()
-    }
-
-    #[inline]
-    fn append_null(&mut self) {
-        self.push_null()
-    }
+#[cfg(feature = "object")]
+impl<T: PolarsObject> AggList for ObjectChunked<T> {
+    unsafe fn agg_list(&self, groups: &GroupsProxy) -> Series {
+        let mut can_fast_explode = true;
+        let mut offsets = Vec::<i64>::with_capacity(groups.len() + 1);
+        let mut length_so_far = 0i64;
+        offsets.push(length_so_far);
+
+        //  we know that iterators length
+        let iter = {
+            groups
+                .iter()
+                .flat_map(|indicator| {
+                    let (group_vals, len) = match indicator {
+                        GroupsIndicator::Idx((_first, idx)) => {
+                            // Safety:
+                            // group tuples always in bounds
+                            let group_vals = self.take_unchecked(idx.into());
+
+                            (group_vals, idx.len() as IdxSize)
+                        }
+                        GroupsIndicator::Slice([first, len]) => {
+                            let group_vals = _slice_from_offsets(self, first, len);
+
+                            (group_vals, len)
+                        }
+                    };
 
-    fn finish(&mut self) -> ListChunked {
-        unsafe {
-            ListChunked::from_chunks_and_dtype_unchecked(
-                "",
-                vec![self.as_box()],
-                DataType::List(Box::new(DataType::Null)),
-            )
-        }
-    }
-}
+                    if len == 0 {
+                        can_fast_explode = false;
+                    }
+                    length_so_far += len as i64;
+                    // Safety:
+                    // we know that offsets has allocated enough slots
+                    offsets.push_unchecked(length_so_far);
+
+                    let arr = group_vals.downcast_iter().next().unwrap().clone();
+                    arr.into_iter_cloned()
+                })
+                .trust_my_length(self.len())
+        };
 
-pub fn get_list_builder(
-    inner_type_logical: &DataType,
-    value_capacity: usize,
-    list_capacity: usize,
-    name: &str,
-) -> PolarsResult<Box<dyn ListBuilderTrait>> {
-    let physical_type = inner_type_logical.to_physical();
-
-    match &physical_type {
-        #[cfg(feature = "object")]
-        DataType::Object(_) => polars_bail!(opq = list_builder, &physical_type),
-        #[cfg(feature = "dtype-struct")]
-        DataType::Struct(_) => Ok(Box::new(AnonymousOwnedListBuilder::new(
-            name,
-            list_capacity,
-            Some(inner_type_logical.clone()),
-        ))),
-        DataType::Null => Ok(Box::new(LargeListNullBuilder::with_capacity(list_capacity))),
-        DataType::List(_) => Ok(Box::new(AnonymousOwnedListBuilder::new(
-            name,
-            list_capacity,
-            Some(inner_type_logical.clone()),
-        ))),
-        _ => {
-            macro_rules! get_primitive_builder {
-                ($type:ty) => {{
-                    let builder = ListPrimitiveChunkedBuilder::<$type>::new(
-                        name,
-                        list_capacity,
-                        value_capacity,
-                        inner_type_logical.clone(),
-                    );
-                    Box::new(builder)
-                }};
-            }
-            macro_rules! get_bool_builder {
-                () => {{
-                    let builder =
-                        ListBooleanChunkedBuilder::new(&name, list_capacity, value_capacity);
-                    Box::new(builder)
-                }};
-            }
-            macro_rules! get_utf8_builder {
-                () => {{
-                    let builder =
-                        ListUtf8ChunkedBuilder::new(&name, list_capacity, 5 * value_capacity);
-                    Box::new(builder)
-                }};
-            }
-            macro_rules! get_binary_builder {
-                () => {{
-                    let builder =
-                        ListBinaryChunkedBuilder::new(&name, list_capacity, 5 * value_capacity);
-                    Box::new(builder)
-                }};
-            }
-            Ok(match_dtype_to_logical_apply_macro!(
-                physical_type,
-                get_primitive_builder,
-                get_utf8_builder,
-                get_binary_builder,
-                get_bool_builder
-            ))
-        }
-    }
-}
+        let mut pe = create_extension(iter);
 
-pub struct AnonymousListBuilder<'a> {
-    name: String,
-    builder: AnonymousBuilder<'a>,
-    fast_explode: bool,
-    inner_dtype: Option<DataType>,
-}
-
-impl Default for AnonymousListBuilder<'_> {
-    fn default() -> Self {
-        Self::new("", 0, None)
+        // Safety:
+        // this is safe because we just created the PolarsExtension
+        // meaning that the sentinel is heap allocated and the dereference of the
+        // pointer does not fail
+        pe.set_to_series_fn::<T>();
+        let extension_array = Box::new(pe.take_and_forget()) as ArrayRef;
+        let extension_dtype = extension_array.data_type();
+
+        let data_type = ListArray::<i64>::default_datatype(extension_dtype.clone());
+        // Safety:
+        // offsets are monotonically increasing
+        let arr = Box::new(ListArray::<i64>::new(
+            data_type,
+            Offsets::new_unchecked(offsets).into(),
+            extension_array,
+            None,
+        )) as ArrayRef;
+
+        let mut listarr = unsafe { ListChunked::from_chunks(self.name(), vec![arr]) };
+        if can_fast_explode {
+            listarr.set_fast_explode()
+        }
+        listarr.into_series()
     }
 }
 
-impl<'a> AnonymousListBuilder<'a> {
-    pub fn new(name: &str, capacity: usize, inner_dtype: Option<DataType>) -> Self {
-        Self {
-            name: name.into(),
-            builder: AnonymousBuilder::new(capacity),
-            fast_explode: true,
-            inner_dtype,
-        }
-    }
-
-    pub fn append_opt_series(&mut self, opt_s: Option<&'a Series>) {
-        match opt_s {
-            Some(s) => self.append_series(s),
-            None => {
-                self.append_null();
-            }
-        }
-    }
-
-    pub fn append_opt_array(&mut self, opt_s: Option<&'a dyn Array>) {
-        match opt_s {
-            Some(s) => self.append_array(s),
-            None => {
-                self.append_null();
-            }
-        }
-    }
-
-    pub fn append_array(&mut self, arr: &'a dyn Array) {
-        self.builder.push(arr)
-    }
-
-    #[inline]
-    pub fn append_null(&mut self) {
-        self.fast_explode = false;
-        self.builder.push_null();
-    }
-
-    #[inline]
-    pub fn append_empty(&mut self) {
-        self.fast_explode = false;
-        self.builder.push_empty()
-    }
-
-    pub fn append_series(&mut self, s: &'a Series) {
-        // empty arrays tend to be null type and thus differ
-        // if we would push it the concat would fail.
-        if s.is_empty() && matches!(s.dtype(), DataType::Null) {
-            self.append_empty();
-        } else {
-            match s.dtype() {
-                #[cfg(feature = "dtype-struct")]
-                DataType::Struct(_) => {
-                    let arr = &**s.array_ref(0);
-                    self.builder.push(arr)
-                }
-                _ => {
-                    self.builder.push_multiple(s.chunks());
+#[cfg(feature = "dtype-struct")]
+impl AggList for StructChunked {
+    unsafe fn agg_list(&self, groups: &GroupsProxy) -> Series {
+        let s = self.clone().into_series();
+        match groups {
+            GroupsProxy::Idx(groups) => {
+                let mut builder = AnonymousOwnedListBuilder::new(
+                    self.name(),
+                    groups.len(),
+                    Some(self.dtype().clone()),
+                );
+                for idx in groups.all().iter() {
+                    let taken = s.take_iter_unchecked(&mut idx.iter().map(|i| *i as usize));
+                    builder.append_series(&taken).unwrap();
                 }
+                builder.finish().into_series()
             }
-        }
-    }
-
-    pub fn finish(&mut self) -> ListChunked {
-        // don't use self from here on one
-        let slf = std::mem::take(self);
-        if slf.builder.is_empty() {
-            ListChunked::full_null_with_dtype(
-                &slf.name,
-                0,
-                &slf.inner_dtype.unwrap_or(DataType::Null),
-            )
-        } else {
-            let inner_dtype_physical = slf
-                .inner_dtype
-                .as_ref()
-                .map(|dt| dt.to_physical().to_arrow());
-            let arr = slf.builder.finish(inner_dtype_physical.as_ref()).unwrap();
-
-            let list_dtype_logical = match slf.inner_dtype {
-                None => DataType::from(arr.data_type()),
-                Some(dt) => DataType::List(Box::new(dt)),
-            };
-            let mut ca = unsafe { ListChunked::from_chunks("", vec![Box::new(arr)]) };
-
-            if slf.fast_explode {
-                ca.set_fast_explode();
-            }
-
-            ca.field = Arc::new(Field::new(&slf.name, list_dtype_logical));
-            ca
-        }
-    }
-}
-
-pub struct AnonymousOwnedListBuilder {
-    name: String,
-    builder: AnonymousBuilder<'static>,
-    owned: Vec<Series>,
-    inner_dtype: Option<DataType>,
-    fast_explode: bool,
-}
-
-impl Default for AnonymousOwnedListBuilder {
-    fn default() -> Self {
-        Self::new("", 0, None)
-    }
-}
-
-impl ListBuilderTrait for AnonymousOwnedListBuilder {
-    fn append_series(&mut self, s: &Series) {
-        if s.is_empty() {
-            self.append_empty();
-        } else {
-            // Safety
-            // we deref a raw pointer with a lifetime that is not static
-            // it is safe because we also clone Series (Arc +=1) and therefore the &dyn Arrays
-            // will not be dropped until the owned series are dropped
-            unsafe {
-                match s.dtype() {
-                    #[cfg(feature = "dtype-struct")]
-                    DataType::Struct(_) => {
-                        self.builder.push(&*(&**s.array_ref(0) as *const dyn Array))
-                    }
-                    _ => {
-                        self.builder
-                            .push_multiple(&*(s.chunks().as_ref() as *const [ArrayRef]));
-                    }
+            GroupsProxy::Slice { groups, .. } => {
+                let mut builder = AnonymousOwnedListBuilder::new(
+                    self.name(),
+                    groups.len(),
+                    Some(self.dtype().clone()),
+                );
+                for [first, len] in groups {
+                    let taken = s.slice(*first as i64, *len as usize);
+                    builder.append_series(&taken).unwrap();
                 }
+                builder.finish().into_series()
             }
-            // this make sure that the underlying ArrayRef's are not dropped
-            self.owned.push(s.clone());
-        }
-    }
-
-    #[inline]
-    fn append_null(&mut self) {
-        self.fast_explode = false;
-        self.builder.push_null()
-    }
-
-    fn finish(&mut self) -> ListChunked {
-        // don't use self from here on one
-        let slf = std::mem::take(self);
-        let inner_dtype_physical = slf
-            .inner_dtype
-            .as_ref()
-            .map(|dt| dt.to_physical().to_arrow());
-        let arr = slf.builder.finish(inner_dtype_physical.as_ref()).unwrap();
-
-        let list_dtype_logical = match slf.inner_dtype {
-            None => DataType::from(arr.data_type()),
-            Some(dt) => DataType::List(Box::new(dt)),
-        };
-        // safety: same type
-        let mut ca = unsafe { ListChunked::from_chunks("", vec![Box::new(arr)]) };
-
-        if slf.fast_explode {
-            ca.set_fast_explode();
         }
-
-        ca.field = Arc::new(Field::new(&slf.name, list_dtype_logical));
-        ca
-    }
-}
-
-impl AnonymousOwnedListBuilder {
-    pub fn new(name: &str, capacity: usize, inner_dtype: Option<DataType>) -> Self {
-        Self {
-            name: name.into(),
-            builder: AnonymousBuilder::new(capacity),
-            owned: Vec::with_capacity(capacity),
-            inner_dtype,
-            fast_explode: true,
-        }
-    }
-
-    #[inline]
-    pub fn append_empty(&mut self) {
-        self.fast_explode = false;
-        self.builder.push_empty()
     }
 }
```

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/builder/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/cast.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/drop.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/float.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/float.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/from.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/kernels/take.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/kernels/take.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/list/iterator.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/list/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/list/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/list/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,122 @@
 use std::sync::Arc;
 
 use arrow::bitmap::MutableBitmap;
 use arrow::offset::Offsets;
 
 use super::*;
 
-pub(crate) fn merge_categorical_map(
+fn slots_to_mut(slots: &Utf8Array<i64>) -> MutableUtf8Array<i64> {
+    // safety: invariants don't change, just the type
+    let offset_buf = unsafe { Offsets::new_unchecked(slots.offsets().as_slice().to_vec()) };
+    let values_buf = slots.values().as_slice().to_vec();
+
+    let validity_buf = if let Some(validity) = slots.validity() {
+        let mut validity_buf = MutableBitmap::new();
+        let (b, offset, len) = validity.as_slice();
+        validity_buf.extend_from_slice(b, offset, len);
+        Some(validity_buf)
+    } else {
+        None
+    };
+
+    // Safety
+    // all offsets are valid and the u8 data is valid utf8
+    unsafe {
+        MutableUtf8Array::new_unchecked(
+            DataType::Utf8.to_arrow(),
+            offset_buf,
+            values_buf,
+            validity_buf,
+        )
+    }
+}
+
+struct State {
+    map: PlHashMap<u32, u32>,
+    slots: MutableUtf8Array<i64>,
+}
+
+#[derive(Default)]
+pub(crate) struct RevMapMerger {
+    id: u128,
+    original: Arc<RevMapping>,
+    // only initiate state when
+    // we encounter a rev-map from a different source,
+    // but from the same string cache
+    state: Option<State>,
+}
+
+impl RevMapMerger {
+    pub(crate) fn new(rev_map: Arc<RevMapping>) -> Self {
+        let RevMapping::Global(_, _, id) = rev_map.as_ref() else { panic!("impl error") };
+        RevMapMerger {
+            state: None,
+            id: *id,
+            original: rev_map,
+        }
+    }
+
+    fn init_state(&mut self) {
+        let RevMapping::Global(map, slots, _) = self.original.as_ref() else { unreachable!() };
+        self.state = Some(State {
+            map: (*map).clone(),
+            slots: slots_to_mut(slots),
+        })
+    }
+
+    pub(crate) fn merge_map(&mut self, rev_map: &Arc<RevMapping>) -> PolarsResult<()> {
+        // happy path
+        // they come from the same source
+        if Arc::ptr_eq(&self.original, rev_map) {
+            return Ok(());
+        }
+        let RevMapping::Global(map, slots, id) = rev_map.as_ref() else { polars_bail!(ComputeError: "expected global rev-map") };
+        polars_ensure!(*id == self.id, ComputeError: "categoricals don't originate from the same string cache\n\
+    try setting a global string cache or increase the scope of the local string cache");
+
+        if self.state.is_none() {
+            self.init_state()
+        }
+        let state = self.state.as_mut().unwrap();
+
+        for (cat, idx) in map.iter() {
+            state.map.entry(*cat).or_insert_with(|| {
+                // Safety
+                // within bounds
+                let str_val = unsafe { slots.value_unchecked(*idx as usize) };
+                let new_idx = state.slots.len() as u32;
+                state.slots.push(Some(str_val));
+
+                new_idx
+            });
+        }
+        Ok(())
+    }
+
+    pub(crate) fn finish(self) -> Arc<RevMapping> {
+        match self.state {
+            None => self.original,
+            Some(state) => {
+                let new_rev = RevMapping::Global(state.map, state.slots.into(), self.id);
+                Arc::new(new_rev)
+            }
+        }
+    }
+}
+
+pub(crate) fn merge_rev_map(
     left: &Arc<RevMapping>,
     right: &Arc<RevMapping>,
 ) -> PolarsResult<Arc<RevMapping>> {
     match (&**left, &**right) {
-        (RevMapping::Global(l_map, l_slots, l_id), RevMapping::Global(r_map, r_slots, r_id)) => {
-            polars_ensure!(
-                l_id == r_id,
-                ComputeError: "unable to merge categorical arrays created under different global \
-                string caches (try setting a global string cache)"
-            );
-            let mut new_map = (*l_map).clone();
-
-            // safety: invariants don't change, just the type
-            let offset_buf =
-                unsafe { Offsets::new_unchecked(l_slots.offsets().as_slice().to_vec()) };
-            let values_buf = l_slots.values().as_slice().to_vec();
-
-            let validity_buf = if let Some(validity) = l_slots.validity() {
-                let mut validity_buf = MutableBitmap::new();
-                let (b, offset, len) = validity.as_slice();
-                validity_buf.extend_from_slice(b, offset, len);
-                Some(validity_buf)
-            } else {
-                None
-            };
-
-            // Safety
-            // all offsets are valid and the u8 data is valid utf8
-            let mut new_slots = unsafe {
-                MutableUtf8Array::new_unchecked(
-                    DataType::Utf8.to_arrow(),
-                    offset_buf,
-                    values_buf,
-                    validity_buf,
-                )
-            };
-
-            for (cat, idx) in r_map.iter() {
-                new_map.entry(*cat).or_insert_with(|| {
-                    // Safety
-                    // within bounds
-                    let str_val = unsafe { r_slots.value_unchecked(*idx as usize) };
-                    let new_idx = new_slots.len() as u32;
-                    new_slots.push(Some(str_val));
-
-                    new_idx
-                });
-            }
-            let new_rev = RevMapping::Global(new_map, new_slots.into(), *l_id);
-            Ok(Arc::new(new_rev))
+        (RevMapping::Global(_, _, _), RevMapping::Global(_, _, _)) => {
+            let mut merger = RevMapMerger::new(left.clone());
+            merger.merge_map(right)?;
+            Ok(merger.finish())
         }
         (RevMapping::Local(arr_l), RevMapping::Local(arr_r)) => {
             // they are from the same source, just clone
             if std::ptr::eq(arr_l, arr_r) {
                 return Ok(left.clone());
             }
 
@@ -77,30 +134,30 @@
             "unable to merge categorical under a global string cache with a non-cached one"
         ),
     }
 }
 
 impl CategoricalChunked {
     pub(crate) fn merge_categorical_map(&self, other: &Self) -> PolarsResult<Arc<RevMapping>> {
-        merge_categorical_map(self.get_rev_map(), other.get_rev_map())
+        merge_rev_map(self.get_rev_map(), other.get_rev_map())
     }
 }
 
 #[cfg(test)]
 #[cfg(feature = "single_thread")]
 mod test {
     use super::*;
     use crate::chunked_array::categorical::CategoricalChunkedBuilder;
-    use crate::{enable_string_cache, reset_string_cache};
+    use crate::{enable_string_cache, reset_string_cache, IUseStringCache};
 
     #[test]
     fn test_merge_rev_map() {
         let _lock = SINGLE_LOCK.lock();
         reset_string_cache();
-        enable_string_cache(true);
+        let _sc = IUseStringCache::hold();
 
         let mut builder1 = CategoricalChunkedBuilder::new("foo", 10);
         let mut builder2 = CategoricalChunkedBuilder::new("foo", 10);
         builder1.drain_iter(vec![None, Some("hello"), Some("vietnam")]);
         builder2.drain_iter(vec![Some("hello"), None, Some("world"), Some("bar")].into_iter());
         let ca1 = builder1.finish();
         let ca2 = builder2.finish();
```

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/date.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/duration.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/logical/time.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/logical/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -334,15 +334,15 @@
     }
 
     /// Get data type of ChunkedArray.
     pub fn dtype(&self) -> &DataType {
         self.field.data_type()
     }
 
-    #[cfg(feature = "dtype-struct")]
+    #[cfg(any(feature = "dtype-struct", feature = "dtype-categorical"))]
     pub(crate) unsafe fn set_dtype(&mut self, dtype: DataType) {
         self.field = Arc::new(Field::new(self.name(), dtype))
     }
 
     /// Name of the ChunkedArray.
     pub fn name(&self) -> &str {
         self.field.name()
```

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ndarray.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ndarray.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/object/builder.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/object/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs`

 * *Files 3% similar despite different names*

```diff
@@ -33,28 +33,26 @@
             offsets,
             fast_explode: true,
         }
     }
 }
 
 impl<T: PolarsObject> ListBuilderTrait for ExtensionListBuilder<T> {
-    fn append_series(&mut self, s: &Series) {
-        let arr = s
-            .as_any()
-            .downcast_ref::<ObjectChunked<T>>()
-            .expect("series of type object");
+    fn append_series(&mut self, s: &Series) -> PolarsResult<()> {
+        let arr = s.as_any().downcast_ref::<ObjectChunked<T>>().unwrap();
 
         for v in arr.into_iter() {
             self.values_builder.append_option(v.cloned())
         }
         if arr.is_empty() {
             self.fast_explode = false;
         }
         let len_so_far = self.offsets[self.offsets.len() - 1];
         self.offsets.push(len_so_far + arr.len() as i64);
+        Ok(())
     }
 
     fn append_null(&mut self) {
         self.values_builder.append_null();
         let len_so_far = self.offsets[self.offsets.len() - 1];
         self.offsets.push(len_so_far + 1);
     }
```

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/object/iterator.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/object/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/object/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/object/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/object/registry.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/object/registry.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/append.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/apply.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/decimal.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/explode.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/explode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/explode_and_offsets.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/explode_and_offsets.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/extend.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/extend.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/filter.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/full.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/full.rs`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 }
 
 impl ChunkFull<&Series> for ListChunked {
     fn full(name: &str, value: &Series, length: usize) -> ListChunked {
         let mut builder =
             get_list_builder(value.dtype(), value.len() * length, length, name).unwrap();
         for _ in 0..length {
-            builder.append_series(value)
+            builder.append_series(value).unwrap();
         }
         builder.finish()
     }
 }
 
 impl ChunkFullNull for ListChunked {
     fn full_null(name: &str, length: usize) -> ListChunked {
```

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/set.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/shift.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/shift.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/ops/zip.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/random.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/temporal/date.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/temporal/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/temporal/time.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/temporal/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/to_vec.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/to_vec.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/trusted_len.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/trusted_len.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs`

 * *Files 3% similar despite different names*

```diff
@@ -179,17 +179,17 @@
             Some(v) => v,
             None => return ListChunked::full_null("", 0),
         };
         // We don't know the needed capacity. We arbitrarily choose an average of 5 elements per series.
         let mut builder =
             get_list_builder(v.borrow().dtype(), capacity * 5, capacity, "collected").unwrap();
 
-        builder.append_series(v.borrow());
+        builder.append_series(v.borrow()).unwrap();
         for s in it {
-            builder.append_series(s.borrow());
+            builder.append_series(s.borrow()).unwrap();
         }
         builder.finish()
     }
 }
 
 impl FromIterator<Option<Series>> for ListChunked {
     fn from_iter<I: IntoIterator<Item = Option<Series>>>(iter: I) -> Self {
@@ -227,30 +227,30 @@
                     let mut builder = AnonymousOwnedListBuilder::new("collected", capacity, None);
                     for _ in 0..init_null_count {
                         builder.append_null();
                     }
                     builder.append_empty();
 
                     for opt_s in it {
-                        builder.append_opt_series(opt_s.as_ref());
+                        builder.append_opt_series(opt_s.as_ref()).unwrap();
                     }
                     builder.finish()
                 } else {
                     match first_s.dtype() {
                         #[cfg(feature = "object")]
                         DataType::Object(_) => {
                             let mut builder =
                                 first_s.get_list_builder("collected", capacity * 5, capacity);
                             for _ in 0..init_null_count {
                                 builder.append_null();
                             }
-                            builder.append_series(first_s);
+                            builder.append_series(first_s).unwrap();
 
                             for opt_s in it {
-                                builder.append_opt_series(opt_s.as_ref());
+                                builder.append_opt_series(opt_s.as_ref()).unwrap();
                             }
                             builder.finish()
                         }
                         _ => {
                             // We don't know the needed capacity. We arbitrarily choose an average of 5 elements per series.
                             let mut builder = get_list_builder(
                                 first_s.dtype(),
@@ -259,18 +259,18 @@
                                 "collected",
                             )
                             .unwrap();
 
                             for _ in 0..init_null_count {
                                 builder.append_null();
                             }
-                            builder.append_series(first_s);
+                            builder.append_series(first_s).unwrap();
 
                             for opt_s in it {
-                                builder.append_opt_series(opt_s.as_ref());
+                                builder.append_opt_series(opt_s.as_ref()).unwrap();
                             }
                             builder.finish()
                         }
                     }
                 }
             }
         }
@@ -717,25 +717,25 @@
                     .flatten()
                     .find_map(|opt_s| opt_s.as_ref())
                     .unwrap();
                 let mut builder = s.get_list_builder("collected", value_capacity, list_capacity);
 
                 for v in vectors {
                     for val in v {
-                        builder.append_opt_series(val.as_ref());
+                        builder.append_opt_series(val.as_ref()).unwrap();
                     }
                 }
                 builder.finish()
             }
             Some(dtype) => {
                 let mut builder =
                     get_list_builder(dtype, value_capacity, list_capacity, "collected").unwrap();
                 for v in &vectors {
                     for val in v {
-                        builder.append_opt_series(val.as_ref());
+                        builder.append_opt_series(val.as_ref()).unwrap();
                     }
                 }
                 builder.finish()
             }
             None => ListChunked::full_null_with_dtype("collected", list_capacity, &DataType::Null),
         }
     }
```

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/cloud.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/cloud.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/config.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/config.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/datatypes/_serde.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/datatypes/_serde.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/datatypes/aliases.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/datatypes/aliases.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/datatypes/any_value.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/datatypes/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/datatypes/dtype.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/datatypes/dtype.rs`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                 (Datetime(tu_l, tz_l), Datetime(tu_r, tz_r)) => tu_l == tu_r && tz_l == tz_r,
                 (List(left_inner), List(right_inner)) => left_inner == right_inner,
                 #[cfg(feature = "dtype-duration")]
                 (Duration(tu_l), Duration(tu_r)) => tu_l == tu_r,
                 #[cfg(feature = "object")]
                 (Object(lhs), Object(rhs)) => lhs == rhs,
                 #[cfg(feature = "dtype-struct")]
-                (Struct(lhs), Struct(rhs)) => lhs == rhs,
+                (Struct(lhs), Struct(rhs)) => Vec::as_ptr(lhs) == Vec::as_ptr(rhs) || lhs == rhs,
                 #[cfg(feature = "dtype-array")]
                 (Array(left_inner, left_width), Array(right_inner, right_width)) => {
                     left_width == right_width && left_inner == right_inner
                 }
                 _ => std::mem::discriminant(self) == std::mem::discriminant(other),
             }
         }
@@ -340,15 +340,15 @@
 
 pub fn merge_dtypes(left: &DataType, right: &DataType) -> PolarsResult<DataType> {
     // TODO! add struct
     use DataType::*;
     Ok(match (left, right) {
         #[cfg(feature = "dtype-categorical")]
         (Categorical(Some(rev_map_l)), Categorical(Some(rev_map_r))) => {
-            let rev_map = merge_categorical_map(rev_map_l, rev_map_r)?;
+            let rev_map = merge_rev_map(rev_map_l, rev_map_r)?;
             Categorical(Some(rev_map))
         }
         (List(inner_l), List(inner_r)) => {
             let merged = merge_dtypes(inner_l, inner_r)?;
             List(Box::new(merged))
         }
         #[cfg(feature = "dtype-array")]
```

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/datatypes/field.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/datatypes/field.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/datatypes/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/datatypes/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/datatypes/time_unit.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/datatypes/time_unit.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/doc/changelog/v0_7.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/doc/changelog/v0_7.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/doc/changelog/v0_8.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/doc/changelog/v0_8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/doc/changelog/v0_9.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/doc/changelog/v0_9.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/fmt.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/fmt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/arithmetic.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/asof_join/asof.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/asof_join/asof.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/asof_join/groups.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/asof_join/groups.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/asof_join/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/asof_join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/chunks.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/cross_join.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/cross_join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/explode.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/explode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/from.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/proxy.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,503 +1,648 @@
-use arrow::offset::Offsets;
-use polars_arrow::kernels::concatenate::concatenate_owned_unchecked;
-use polars_utils::unwrap::UnwrapUncheckedRelease;
-
-use super::*;
-#[cfg(feature = "dtype-struct")]
-use crate::chunked_array::builder::AnonymousOwnedListBuilder;
+use std::mem::ManuallyDrop;
+use std::ops::Deref;
 
-pub trait AggList {
-    /// # Safety
-    ///
-    /// groups should be in bounds
-    unsafe fn agg_list(&self, _groups: &GroupsProxy) -> Series;
-}
-
-impl<T> AggList for ChunkedArray<T>
-where
-    T: PolarsNumericType,
-    ChunkedArray<T>: IntoSeries,
-{
-    unsafe fn agg_list(&self, groups: &GroupsProxy) -> Series {
-        let ca = self.rechunk();
+use polars_arrow::utils::CustomIterTools;
+use polars_utils::sync::SyncPtr;
+use rayon::iter::plumbing::UnindexedConsumer;
+use rayon::prelude::*;
+
+use crate::prelude::*;
+use crate::utils::{flatten, slice_slice, NoNull};
+use crate::POOL;
+
+/// Indexes of the groups, the first index is stored separately.
+/// this make sorting fast.
+#[derive(Debug, Clone, PartialEq, Eq, Default)]
+pub struct GroupsIdx {
+    pub(crate) sorted: bool,
+    first: Vec<IdxSize>,
+    all: Vec<Vec<IdxSize>>,
+}
+
+pub type IdxItem = (IdxSize, Vec<IdxSize>);
+pub type BorrowIdxItem<'a> = (IdxSize, &'a Vec<IdxSize>);
+
+impl Drop for GroupsIdx {
+    fn drop(&mut self) {
+        let v = std::mem::take(&mut self.all);
+        // ~65k took approximately 1ms on local machine, so from that point we drop on other thread
+        // to stop query from being blocked
+        #[cfg(not(target_family = "wasm"))]
+        if v.len() > 1 << 16 {
+            std::thread::spawn(move || drop(v));
+        } else {
+            drop(v);
+        }
 
-        match groups {
-            GroupsProxy::Idx(groups) => {
-                let mut can_fast_explode = true;
+        #[cfg(target_family = "wasm")]
+        drop(v);
+    }
+}
 
-                let arr = ca.downcast_iter().next().unwrap();
-                let values = arr.values();
+impl From<Vec<IdxItem>> for GroupsIdx {
+    fn from(v: Vec<IdxItem>) -> Self {
+        v.into_iter().collect()
+    }
+}
 
-                let mut offsets = Vec::<i64>::with_capacity(groups.len() + 1);
-                let mut length_so_far = 0i64;
-                offsets.push(length_so_far);
-
-                let mut list_values = Vec::<T::Native>::with_capacity(self.len());
-                groups.iter().for_each(|(_, idx)| {
-                    let idx_len = idx.len();
-                    if idx_len == 0 {
-                        can_fast_explode = false;
-                    }
+impl From<Vec<(Vec<IdxSize>, Vec<Vec<IdxSize>>)>> for GroupsIdx {
+    fn from(v: Vec<(Vec<IdxSize>, Vec<Vec<IdxSize>>)>) -> Self {
+        // we have got the hash tables so we can determine the final
+        let cap = v.iter().map(|v| v.0.len()).sum::<usize>();
+        let offsets = v
+            .iter()
+            .scan(0_usize, |acc, v| {
+                let out = *acc;
+                *acc += v.0.len();
+                Some(out)
+            })
+            .collect::<Vec<_>>();
+        let mut global_first = Vec::with_capacity(cap);
+        let global_first_ptr = unsafe { SyncPtr::new(global_first.as_mut_ptr()) };
+        let mut global_all = Vec::with_capacity(cap);
+        let global_all_ptr = unsafe { SyncPtr::new(global_all.as_mut_ptr()) };
+
+        POOL.install(|| {
+            v.into_par_iter().zip(offsets).for_each(
+                |((local_first_vals, mut local_all_vals), offset)| unsafe {
+                    let global_first: *mut IdxSize = global_first_ptr.get();
+                    let global_all: *mut Vec<IdxSize> = global_all_ptr.get();
+                    let global_first = global_first.add(offset);
+                    let global_all = global_all.add(offset);
+
+                    std::ptr::copy_nonoverlapping(
+                        local_first_vals.as_ptr(),
+                        global_first,
+                        local_first_vals.len(),
+                    );
+                    std::ptr::copy_nonoverlapping(
+                        local_all_vals.as_ptr(),
+                        global_all,
+                        local_all_vals.len(),
+                    );
+                    // local_all_vals: Vec<Vec<IdxSize>>
+                    // we just copied the contents: Vec<IdxSize> to a new buffer
+                    // now, we want to free the outer vec, without freeing
+                    // the inner vecs as they are moved, so we set the len to 0
+                    local_all_vals.set_len(0);
+                },
+            );
+        });
+        unsafe {
+            global_all.set_len(cap);
+            global_first.set_len(cap);
+        }
+        GroupsIdx {
+            sorted: false,
+            first: global_first,
+            all: global_all,
+        }
+    }
+}
 
-                    length_so_far += idx_len as i64;
-                    // Safety:
-                    // group tuples are in bounds
-                    {
-                        list_values.extend(idx.iter().map(|idx| {
-                            debug_assert!((*idx as usize) < values.len());
-                            *values.get_unchecked(*idx as usize)
-                        }));
-                        // Safety:
-                        // we know that offsets has allocated enough slots
-                        offsets.push_unchecked(length_so_far);
+impl From<Vec<Vec<IdxItem>>> for GroupsIdx {
+    fn from(v: Vec<Vec<IdxItem>>) -> Self {
+        // single threaded flatten: 10% faster than `iter().flatten().collect()
+        // this is the multi-threaded impl of that
+        let (cap, offsets) = flatten::cap_and_offsets(&v);
+        let mut first = Vec::with_capacity(cap);
+        let first_ptr = first.as_ptr() as usize;
+        let mut all = Vec::with_capacity(cap);
+        let all_ptr = all.as_ptr() as usize;
+
+        POOL.install(|| {
+            v.into_par_iter()
+                .zip(offsets)
+                .for_each(|(mut inner, offset)| {
+                    unsafe {
+                        let first = (first_ptr as *const IdxSize as *mut IdxSize).add(offset);
+                        let all = (all_ptr as *const Vec<IdxSize> as *mut Vec<IdxSize>).add(offset);
+
+                        let inner_ptr = inner.as_mut_ptr();
+                        for i in 0..inner.len() {
+                            let (first_val, vals) = std::ptr::read(inner_ptr.add(i));
+                            std::ptr::write(first.add(i), first_val);
+                            std::ptr::write(all.add(i), vals);
+                        }
+                        // set len to 0 so that the contents will not get dropped
+                        // they are moved to `first` and `all`
+                        inner.set_len(0);
                     }
                 });
+        });
+        unsafe {
+            all.set_len(cap);
+            first.set_len(cap);
+        }
+        GroupsIdx {
+            sorted: false,
+            first,
+            all,
+        }
+    }
+}
 
-                let validity = if arr.null_count() > 0 {
-                    let old_validity = arr.validity().unwrap();
-                    let mut validity = MutableBitmap::from_len_set(list_values.len());
-
-                    let mut count = 0;
-                    groups.iter().for_each(|(_, idx)| {
-                        for i in idx {
-                            if !old_validity.get_bit_unchecked(*i as usize) {
-                                validity.set_bit_unchecked(count, false)
-                            }
-                            count += 1;
-                        }
-                    });
-                    Some(validity.into())
-                } else {
-                    None
-                };
+impl GroupsIdx {
+    pub fn new(first: Vec<IdxSize>, all: Vec<Vec<IdxSize>>, sorted: bool) -> Self {
+        Self { sorted, first, all }
+    }
+
+    pub fn sort(&mut self) {
+        let mut idx = 0;
+        let first = std::mem::take(&mut self.first);
+        // store index and values so that we can sort those
+        let mut idx_vals = first
+            .into_iter()
+            .map(|v| {
+                let out = [idx, v];
+                idx += 1;
+                out
+            })
+            .collect_trusted::<Vec<_>>();
+        idx_vals.sort_unstable_by_key(|v| v[1]);
+
+        let take_first = || idx_vals.iter().map(|v| v[1]).collect_trusted::<Vec<_>>();
+        let take_all = || {
+            idx_vals
+                .iter()
+                .map(|v| unsafe {
+                    let idx = v[0] as usize;
+                    std::mem::take(self.all.get_unchecked_mut(idx))
+                })
+                .collect_trusted::<Vec<_>>()
+        };
+        let (first, all) = POOL.install(|| rayon::join(take_first, take_all));
+        self.first = first;
+        self.all = all;
+        self.sorted = true
+    }
+    pub fn is_sorted_flag(&self) -> bool {
+        self.sorted
+    }
 
-                let array =
-                    PrimitiveArray::new(T::get_dtype().to_arrow(), list_values.into(), validity);
-                let data_type = ListArray::<i64>::default_datatype(T::get_dtype().to_arrow());
-                // Safety:
-                // offsets are monotonically increasing
-                let arr = ListArray::<i64>::new(
-                    data_type,
-                    Offsets::new_unchecked(offsets).into(),
-                    Box::new(array),
-                    None,
-                );
-
-                let mut ca = unsafe { ListChunked::from_chunks(self.name(), vec![Box::new(arr)]) };
-                if can_fast_explode {
-                    ca.set_fast_explode()
-                }
-                ca.into()
-            }
-            GroupsProxy::Slice { groups, .. } => {
-                let mut can_fast_explode = true;
-                let arr = ca.downcast_iter().next().unwrap();
-                let values = arr.values();
-
-                let mut offsets = Vec::<i64>::with_capacity(groups.len() + 1);
-                let mut length_so_far = 0i64;
-                offsets.push(length_so_far);
-
-                let mut list_values = Vec::<T::Native>::with_capacity(self.len());
-                groups.iter().for_each(|&[first, len]| {
-                    if len == 0 {
-                        can_fast_explode = false;
-                    }
+    pub fn iter(
+        &self,
+    ) -> std::iter::Zip<std::iter::Copied<std::slice::Iter<IdxSize>>, std::slice::Iter<Vec<IdxSize>>>
+    {
+        self.into_iter()
+    }
 
-                    length_so_far += len as i64;
-                    list_values.extend_from_slice(&values[first as usize..(first + len) as usize]);
-                    {
-                        // Safety:
-                        // we know that offsets has allocated enough slots
-                        offsets.push_unchecked(length_so_far);
-                    }
-                });
+    pub fn all(&self) -> &[Vec<IdxSize>] {
+        &self.all
+    }
 
-                let validity = if arr.null_count() > 0 {
-                    let old_validity = arr.validity().unwrap();
-                    let mut validity = MutableBitmap::from_len_set(list_values.len());
-
-                    let mut count = 0;
-                    groups.iter().for_each(|[first, len]| {
-                        for i in *first..(*first + *len) {
-                            if !old_validity.get_bit_unchecked(i as usize) {
-                                validity.set_bit_unchecked(count, false)
-                            }
-                            count += 1;
-                        }
-                    });
-                    Some(validity.into())
-                } else {
-                    None
-                };
+    pub fn first(&self) -> &[IdxSize] {
+        &self.first
+    }
 
-                let array =
-                    PrimitiveArray::new(T::get_dtype().to_arrow(), list_values.into(), validity);
-                let data_type = ListArray::<i64>::default_datatype(T::get_dtype().to_arrow());
-                let arr = ListArray::<i64>::new(
-                    data_type,
-                    Offsets::new_unchecked(offsets).into(),
-                    Box::new(array),
-                    None,
-                );
-                let mut ca = unsafe { ListChunked::from_chunks(self.name(), vec![Box::new(arr)]) };
-                if can_fast_explode {
-                    ca.set_fast_explode()
-                }
-                ca.into()
-            }
+    pub fn first_mut(&mut self) -> &mut Vec<IdxSize> {
+        &mut self.first
+    }
+
+    pub(crate) fn len(&self) -> usize {
+        self.first.len()
+    }
+
+    pub(crate) unsafe fn get_unchecked(&self, index: usize) -> BorrowIdxItem {
+        let first = *self.first.get_unchecked(index);
+        let all = self.all.get_unchecked(index);
+        (first, all)
+    }
+}
+
+impl FromIterator<IdxItem> for GroupsIdx {
+    fn from_iter<T: IntoIterator<Item = IdxItem>>(iter: T) -> Self {
+        let (first, all) = iter.into_iter().unzip();
+        GroupsIdx {
+            sorted: false,
+            first,
+            all,
         }
     }
 }
 
-impl AggList for BooleanChunked {
-    unsafe fn agg_list(&self, groups: &GroupsProxy) -> Series {
-        match groups {
-            GroupsProxy::Idx(groups) => {
-                let mut builder =
-                    ListBooleanChunkedBuilder::new(self.name(), groups.len(), self.len());
-                for idx in groups.all().iter() {
-                    let ca = { self.take_unchecked(idx.into()) };
-                    builder.append(&ca)
-                }
-                builder.finish().into_series()
-            }
-            GroupsProxy::Slice { groups, .. } => {
-                let mut builder =
-                    ListBooleanChunkedBuilder::new(self.name(), groups.len(), self.len());
-                for [first, len] in groups {
-                    let ca = self.slice(*first as i64, *len as usize);
-                    builder.append(&ca)
-                }
-                builder.finish().into_series()
-            }
+impl<'a> IntoIterator for &'a GroupsIdx {
+    type Item = BorrowIdxItem<'a>;
+    type IntoIter = std::iter::Zip<
+        std::iter::Copied<std::slice::Iter<'a, IdxSize>>,
+        std::slice::Iter<'a, Vec<IdxSize>>,
+    >;
+
+    fn into_iter(self) -> Self::IntoIter {
+        self.first.iter().copied().zip(self.all.iter())
+    }
+}
+
+impl IntoIterator for GroupsIdx {
+    type Item = IdxItem;
+    type IntoIter = std::iter::Zip<std::vec::IntoIter<IdxSize>, std::vec::IntoIter<Vec<IdxSize>>>;
+
+    fn into_iter(mut self) -> Self::IntoIter {
+        let first = std::mem::take(&mut self.first);
+        let all = std::mem::take(&mut self.all);
+        first.into_iter().zip(all.into_iter())
+    }
+}
+
+impl FromParallelIterator<IdxItem> for GroupsIdx {
+    fn from_par_iter<I>(par_iter: I) -> Self
+    where
+        I: IntoParallelIterator<Item = IdxItem>,
+    {
+        let (first, all) = par_iter.into_par_iter().unzip();
+        GroupsIdx {
+            sorted: false,
+            first,
+            all,
         }
     }
 }
 
-impl AggList for Utf8Chunked {
-    unsafe fn agg_list(&self, groups: &GroupsProxy) -> Series {
-        // TODO: dispatch via binary
-        match groups {
-            GroupsProxy::Idx(groups) => {
-                let mut builder =
-                    ListUtf8ChunkedBuilder::new(self.name(), groups.len(), self.len());
-                for idx in groups.all().iter() {
-                    let ca = { self.take_unchecked(idx.into()) };
-                    builder.append(&ca)
-                }
-                builder.finish().into_series()
-            }
+impl<'a> IntoParallelIterator for &'a GroupsIdx {
+    type Iter = rayon::iter::Zip<
+        rayon::iter::Copied<rayon::slice::Iter<'a, IdxSize>>,
+        rayon::slice::Iter<'a, Vec<IdxSize>>,
+    >;
+    type Item = BorrowIdxItem<'a>;
+
+    fn into_par_iter(self) -> Self::Iter {
+        self.first.par_iter().copied().zip(self.all.par_iter())
+    }
+}
+
+impl IntoParallelIterator for GroupsIdx {
+    type Iter = rayon::iter::Zip<rayon::vec::IntoIter<IdxSize>, rayon::vec::IntoIter<Vec<IdxSize>>>;
+    type Item = IdxItem;
+
+    fn into_par_iter(mut self) -> Self::Iter {
+        let first = std::mem::take(&mut self.first);
+        let all = std::mem::take(&mut self.all);
+        first.into_par_iter().zip(all.into_par_iter())
+    }
+}
+
+/// Every group is indicated by an array where the
+///  - first value is an index to the start of the group
+///  - second value is the length of the group
+/// Only used when group values are stored together
+///
+/// This type should have the invariant that it is always sorted in ascending order.
+pub type GroupsSlice = Vec<[IdxSize; 2]>;
+
+#[derive(Debug, Clone, PartialEq, Eq)]
+pub enum GroupsProxy {
+    Idx(GroupsIdx),
+    /// Slice is always sorted in ascending order.
+    Slice {
+        // the groups slices
+        groups: GroupsSlice,
+        // indicates if we do a rolling groupby
+        rolling: bool,
+    },
+}
+
+impl Default for GroupsProxy {
+    fn default() -> Self {
+        GroupsProxy::Idx(GroupsIdx::default())
+    }
+}
+
+impl GroupsProxy {
+    pub fn into_idx(self) -> GroupsIdx {
+        match self {
+            GroupsProxy::Idx(groups) => groups,
             GroupsProxy::Slice { groups, .. } => {
-                let mut builder =
-                    ListUtf8ChunkedBuilder::new(self.name(), groups.len(), self.len());
-                for [first, len] in groups {
-                    let ca = self.slice(*first as i64, *len as usize);
-                    builder.append(&ca)
-                }
-                builder.finish().into_series()
+                eprintln!("Had to reallocate groups, missed an optimization opportunity. Please open an issue.");
+                groups
+                    .iter()
+                    .map(|&[first, len]| (first, (first..first + len).collect_trusted::<Vec<_>>()))
+                    .collect()
             }
         }
     }
-}
 
-impl AggList for BinaryChunked {
-    unsafe fn agg_list(&self, groups: &GroupsProxy) -> Series {
-        match groups {
+    pub fn iter(&self) -> GroupsProxyIter {
+        GroupsProxyIter::new(self)
+    }
+
+    pub fn sort(&mut self) {
+        match self {
             GroupsProxy::Idx(groups) => {
-                let mut builder =
-                    ListBinaryChunkedBuilder::new(self.name(), groups.len(), self.len());
-                for idx in groups.all().iter() {
-                    let ca = { self.take_unchecked(idx.into()) };
-                    builder.append(&ca)
+                if !groups.is_sorted_flag() {
+                    groups.sort()
                 }
-                builder.finish().into_series()
             }
-            GroupsProxy::Slice { groups, .. } => {
-                let mut builder =
-                    ListBinaryChunkedBuilder::new(self.name(), groups.len(), self.len());
-                for [first, len] in groups {
-                    let ca = self.slice(*first as i64, *len as usize);
-                    builder.append(&ca)
-                }
-                builder.finish().into_series()
+            GroupsProxy::Slice { .. } => {
+                // invariant of the type
             }
         }
     }
-}
 
-fn agg_list_list<F: Fn(&ListChunked, bool, &mut Vec<i64>, &mut i64, &mut Vec<ArrayRef>) -> bool>(
-    ca: &ListChunked,
-    groups_len: usize,
-    func: F,
-) -> Series {
-    let inner_dtype = ca.inner_dtype();
-    let inner_dtype_physical = inner_dtype.to_physical();
-    let can_fast_explode = true;
-    let mut offsets = Vec::<i64>::with_capacity(groups_len + 1);
-    let mut length_so_far = 0i64;
-    offsets.push(length_so_far);
-
-    let mut list_values = Vec::with_capacity(groups_len);
-
-    let can_fast_explode = func(
-        ca,
-        can_fast_explode,
-        &mut offsets,
-        &mut length_so_far,
-        &mut list_values,
-    );
-    if groups_len == 0 {
-        list_values.push(ca.chunks[0].sliced(0, 0))
-    }
-    let list_values = concatenate_owned_unchecked(&list_values).unwrap();
-    let data_type = ListArray::<i64>::default_datatype(list_values.data_type().clone());
-    // Safety:
-    // offsets are monotonically increasing
-    let arr = unsafe {
-        Box::new(ListArray::<i64>::new(
-            data_type,
-            Offsets::new_unchecked(offsets).into(),
-            list_values,
-            None,
-        )) as ArrayRef
-    };
-    let mut listarr = unsafe { ListChunked::from_chunks(ca.name(), vec![arr]) };
-    if can_fast_explode {
-        listarr.set_fast_explode()
-    }
-    if inner_dtype_physical != inner_dtype {
-        listarr.to_physical(DataType::List(Box::new(inner_dtype)));
-    }
-    listarr.into_series()
-}
-
-impl AggList for ListChunked {
-    unsafe fn agg_list(&self, groups: &GroupsProxy) -> Series {
-        match groups {
-            GroupsProxy::Idx(groups) => {
-                let func = |ca: &ListChunked,
-                            mut can_fast_explode: bool,
-                            offsets: &mut Vec<i64>,
-                            length_so_far: &mut i64,
-                            list_values: &mut Vec<ArrayRef>| {
-                    assert!(list_values.capacity() >= groups.len());
-                    groups.iter().for_each(|(_, idx)| {
-                        let idx_len = idx.len();
-                        if idx_len == 0 {
-                            can_fast_explode = false;
-                        }
+    pub(crate) fn is_sorted_flag(&self) -> bool {
+        match self {
+            GroupsProxy::Idx(groups) => groups.is_sorted_flag(),
+            GroupsProxy::Slice { .. } => true,
+        }
+    }
 
-                        *length_so_far += idx_len as i64;
-                        // Safety:
-                        // group tuples are in bounds
-                        {
-                            let mut s = ca.take_unchecked(idx.into());
-                            let arr = s.chunks.pop().unwrap_unchecked_release();
-                            list_values.push_unchecked(arr);
-
-                            // Safety:
-                            // we know that offsets has allocated enough slots
-                            offsets.push_unchecked(*length_so_far);
-                        }
-                    });
-                    can_fast_explode
-                };
+    pub fn group_lengths(&self, name: &str) -> IdxCa {
+        let ca: NoNull<IdxCa> = match self {
+            GroupsProxy::Idx(groups) => groups
+                .iter()
+                .map(|(_, groups)| groups.len() as IdxSize)
+                .collect_trusted(),
+            GroupsProxy::Slice { groups, .. } => groups.iter().map(|g| g[1]).collect_trusted(),
+        };
+        let mut ca = ca.into_inner();
+        ca.rename(name);
+        ca
+    }
 
-                agg_list_list(self, groups.len(), func)
-            }
+    pub fn take_group_firsts(self) -> Vec<IdxSize> {
+        match self {
+            GroupsProxy::Idx(mut groups) => std::mem::take(&mut groups.first),
             GroupsProxy::Slice { groups, .. } => {
-                let func = |ca: &ListChunked,
-                            mut can_fast_explode: bool,
-                            offsets: &mut Vec<i64>,
-                            length_so_far: &mut i64,
-                            list_values: &mut Vec<ArrayRef>| {
-                    assert!(list_values.capacity() >= groups.len());
-                    groups.iter().for_each(|&[first, len]| {
-                        if len == 0 {
-                            can_fast_explode = false;
-                        }
+                groups.into_iter().map(|[first, _len]| first).collect()
+            }
+        }
+    }
 
-                        *length_so_far += len as i64;
-                        let mut s = ca.slice(first as i64, len as usize);
-                        let arr = s.chunks.pop().unwrap_unchecked_release();
-                        list_values.push_unchecked(arr);
-
-                        {
-                            // Safety:
-                            // we know that offsets has allocated enough slots
-                            offsets.push_unchecked(*length_so_far);
-                        }
-                    });
-                    can_fast_explode
-                };
+    pub fn par_iter(&self) -> GroupsProxyParIter {
+        GroupsProxyParIter::new(self)
+    }
+
+    /// Get a reference to the `GroupsIdx`.
+    ///
+    /// # Panic
+    ///
+    /// panics if the groups are a slice.
+    pub fn unwrap_idx(&self) -> &GroupsIdx {
+        match self {
+            GroupsProxy::Idx(groups) => groups,
+            GroupsProxy::Slice { .. } => panic!("groups are slices not index"),
+        }
+    }
+
+    /// Get a reference to the `GroupsSlice`.
+    ///
+    /// # Panic
+    ///
+    /// panics if the groups are an idx.
+    pub fn unwrap_slice(&self) -> &GroupsSlice {
+        match self {
+            GroupsProxy::Slice { groups, .. } => groups,
+            GroupsProxy::Idx(_) => panic!("groups are index not slices"),
+        }
+    }
 
-                agg_list_list(self, groups.len(), func)
+    pub fn get(&self, index: usize) -> GroupsIndicator {
+        match self {
+            GroupsProxy::Idx(groups) => {
+                let first = groups.first[index];
+                let all = &groups.all[index];
+                GroupsIndicator::Idx((first, all))
             }
+            GroupsProxy::Slice { groups, .. } => GroupsIndicator::Slice(groups[index]),
         }
     }
-}
 
-#[cfg(feature = "dtype-array")]
-fn agg_list_fixed_size_list<F: Fn(&ArrayChunked, &mut Vec<ArrayRef>)>(
-    ca: &ArrayChunked,
-    groups_len: usize,
-    func: F,
-    width: usize,
-) -> Series {
-    let inner_dtype = ca.inner_dtype();
-    let inner_dtype_physical = inner_dtype.to_physical();
-    let mut list_values = Vec::with_capacity(groups_len);
+    /// Get a mutable reference to the `GroupsIdx`.
+    ///
+    /// # Panic
+    ///
+    /// panics if the groups are a slice.
+    pub fn idx_mut(&mut self) -> &mut GroupsIdx {
+        match self {
+            GroupsProxy::Idx(groups) => groups,
+            GroupsProxy::Slice { .. } => panic!("groups are slices not index"),
+        }
+    }
 
-    func(ca, &mut list_values);
-    if groups_len == 0 {
-        list_values.push(ca.chunks[0].sliced(0, 0))
+    pub fn len(&self) -> usize {
+        match self {
+            GroupsProxy::Idx(groups) => groups.len(),
+            GroupsProxy::Slice { groups, .. } => groups.len(),
+        }
     }
-    let list_values = concatenate_owned_unchecked(&list_values).unwrap();
-    let data_type = FixedSizeListArray::default_datatype(list_values.data_type().clone(), width);
-    let arr = Box::new(FixedSizeListArray::new(data_type, list_values, None)) as ArrayRef;
-    let mut listarr = unsafe { ListChunked::from_chunks(ca.name(), vec![arr]) };
-    if inner_dtype_physical != inner_dtype {
-        listarr.to_physical(DataType::List(Box::new(inner_dtype)));
+
+    pub fn is_empty(&self) -> bool {
+        self.len() == 0
     }
-    listarr.into_series()
-}
 
-#[cfg(feature = "dtype-array")]
-impl AggList for ArrayChunked {
-    unsafe fn agg_list(&self, groups: &GroupsProxy) -> Series {
-        match groups {
+    pub fn group_count(&self) -> IdxCa {
+        match self {
             GroupsProxy::Idx(groups) => {
-                let func = |ca: &ArrayChunked, list_values: &mut Vec<ArrayRef>| {
-                    assert!(list_values.capacity() >= groups.len());
-                    groups.iter().for_each(|(_, idx)| {
-                        // Safety:
-                        // group tuples are in bounds
-                        {
-                            let mut s = ca.take_unchecked(idx.into());
-                            let arr = s.chunks.pop().unwrap_unchecked_release();
-                            list_values.push_unchecked(arr);
-                        }
-                    });
-                };
-
-                agg_list_fixed_size_list(self, groups.len(), func, self.width())
+                let ca: NoNull<IdxCa> = groups
+                    .iter()
+                    .map(|(_first, idx)| idx.len() as IdxSize)
+                    .collect_trusted();
+                ca.into_inner()
             }
             GroupsProxy::Slice { groups, .. } => {
-                let func = |ca: &ArrayChunked, list_values: &mut Vec<ArrayRef>| {
-                    assert!(list_values.capacity() >= groups.len());
-                    groups.iter().for_each(|&[first, len]| {
-                        let mut s = ca.slice(first as i64, len as usize);
-                        let arr = s.chunks.pop().unwrap_unchecked_release();
-                        list_values.push_unchecked(arr);
-                    });
-                };
-
-                agg_list_fixed_size_list(self, groups.len(), func, self.width())
+                let ca: NoNull<IdxCa> = groups.iter().map(|[_first, len]| *len).collect_trusted();
+                ca.into_inner()
             }
         }
     }
-}
-
-#[cfg(feature = "object")]
-impl<T: PolarsObject> AggList for ObjectChunked<T> {
-    unsafe fn agg_list(&self, groups: &GroupsProxy) -> Series {
-        let mut can_fast_explode = true;
-        let mut offsets = Vec::<i64>::with_capacity(groups.len() + 1);
-        let mut length_so_far = 0i64;
-        offsets.push(length_so_far);
-
-        //  we know that iterators length
-        let iter = {
-            groups
+    pub fn as_list_chunked(&self) -> ListChunked {
+        match self {
+            GroupsProxy::Idx(groups) => groups
+                .iter()
+                .map(|(_first, idx)| {
+                    let ca: NoNull<IdxCa> = idx.iter().map(|&v| v as IdxSize).collect();
+                    ca.into_inner().into_series()
+                })
+                .collect_trusted(),
+            GroupsProxy::Slice { groups, .. } => groups
                 .iter()
-                .flat_map(|indicator| {
-                    let (group_vals, len) = match indicator {
-                        GroupsIndicator::Idx((_first, idx)) => {
-                            // Safety:
-                            // group tuples always in bounds
-                            let group_vals = self.take_unchecked(idx.into());
+                .map(|&[first, len]| {
+                    let ca: NoNull<IdxCa> = (first..first + len).collect_trusted();
+                    ca.into_inner().into_series()
+                })
+                .collect_trusted(),
+        }
+    }
 
-                            (group_vals, idx.len() as IdxSize)
-                        }
-                        GroupsIndicator::Slice([first, len]) => {
-                            let group_vals = _slice_from_offsets(self, first, len);
+    pub fn unroll(self) -> GroupsProxy {
+        match self {
+            GroupsProxy::Idx(_) => self,
+            GroupsProxy::Slice { rolling: false, .. } => self,
+            GroupsProxy::Slice { mut groups, .. } => {
+                let mut offset = 0 as IdxSize;
+                for g in groups.iter_mut() {
+                    g[0] = offset;
+                    offset += g[1];
+                }
+                GroupsProxy::Slice {
+                    groups,
+                    rolling: false,
+                }
+            }
+        }
+    }
 
-                            (group_vals, len)
-                        }
-                    };
+    pub fn slice(&self, offset: i64, len: usize) -> SlicedGroups {
+        // Safety:
+        // we create new `Vec`s from the sliced groups. But we wrap them in ManuallyDrop
+        // so that we never call drop on them.
+        // These groups lifetimes are bounded to the `self`. This must remain valid
+        // for the scope of the aggregation.
+        let sliced = match self {
+            GroupsProxy::Idx(groups) => {
+                let first = unsafe {
+                    let first = slice_slice(groups.first(), offset, len);
+                    let ptr = first.as_ptr() as *mut _;
+                    Vec::from_raw_parts(ptr, first.len(), first.len())
+                };
 
-                    if len == 0 {
-                        can_fast_explode = false;
-                    }
-                    length_so_far += len as i64;
-                    // Safety:
-                    // we know that offsets has allocated enough slots
-                    offsets.push_unchecked(length_so_far);
+                let all = unsafe {
+                    let all = slice_slice(groups.all(), offset, len);
+                    let ptr = all.as_ptr() as *mut _;
+                    Vec::from_raw_parts(ptr, all.len(), all.len())
+                };
+                ManuallyDrop::new(GroupsProxy::Idx(GroupsIdx::new(
+                    first,
+                    all,
+                    groups.is_sorted_flag(),
+                )))
+            }
+            GroupsProxy::Slice { groups, rolling } => {
+                let groups = unsafe {
+                    let groups = slice_slice(groups, offset, len);
+                    let ptr = groups.as_ptr() as *mut _;
+                    Vec::from_raw_parts(ptr, groups.len(), groups.len())
+                };
 
-                    let arr = group_vals.downcast_iter().next().unwrap().clone();
-                    arr.into_iter_cloned()
+                ManuallyDrop::new(GroupsProxy::Slice {
+                    groups,
+                    rolling: *rolling,
                 })
-                .trust_my_length(self.len())
+            }
         };
 
-        let mut pe = create_extension(iter);
+        SlicedGroups {
+            sliced,
+            borrowed: self,
+        }
+    }
+}
 
-        // Safety:
-        // this is safe because we just created the PolarsExtension
-        // meaning that the sentinel is heap allocated and the dereference of the
-        // pointer does not fail
-        pe.set_to_series_fn::<T>();
-        let extension_array = Box::new(pe.take_and_forget()) as ArrayRef;
-        let extension_dtype = extension_array.data_type();
+impl From<GroupsIdx> for GroupsProxy {
+    fn from(groups: GroupsIdx) -> Self {
+        GroupsProxy::Idx(groups)
+    }
+}
 
-        let data_type = ListArray::<i64>::default_datatype(extension_dtype.clone());
-        // Safety:
-        // offsets are monotonically increasing
-        let arr = Box::new(ListArray::<i64>::new(
-            data_type,
-            Offsets::new_unchecked(offsets).into(),
-            extension_array,
-            None,
-        )) as ArrayRef;
-
-        let mut listarr = unsafe { ListChunked::from_chunks(self.name(), vec![arr]) };
-        if can_fast_explode {
-            listarr.set_fast_explode()
-        }
-        listarr.into_series()
+pub enum GroupsIndicator<'a> {
+    Idx(BorrowIdxItem<'a>),
+    Slice([IdxSize; 2]),
+}
+
+impl<'a> GroupsIndicator<'a> {
+    pub fn len(&self) -> usize {
+        match self {
+            GroupsIndicator::Idx(g) => g.1.len(),
+            GroupsIndicator::Slice([_, len]) => *len as usize,
+        }
+    }
+    pub fn first(&self) -> IdxSize {
+        match self {
+            GroupsIndicator::Idx(g) => g.0,
+            GroupsIndicator::Slice([first, _]) => *first,
+        }
+    }
+    pub fn is_empty(&self) -> bool {
+        self.len() == 0
     }
 }
 
-#[cfg(feature = "dtype-struct")]
-impl AggList for StructChunked {
-    unsafe fn agg_list(&self, groups: &GroupsProxy) -> Series {
-        let s = self.clone().into_series();
-        match groups {
-            GroupsProxy::Idx(groups) => {
-                let mut builder = AnonymousOwnedListBuilder::new(
-                    self.name(),
-                    groups.len(),
-                    Some(self.dtype().clone()),
-                );
-                for idx in groups.all().iter() {
-                    let taken = s.take_iter_unchecked(&mut idx.iter().map(|i| *i as usize));
-                    builder.append_series(&taken)
+pub struct GroupsProxyIter<'a> {
+    vals: &'a GroupsProxy,
+    len: usize,
+    idx: usize,
+}
+
+impl<'a> GroupsProxyIter<'a> {
+    fn new(vals: &'a GroupsProxy) -> Self {
+        let len = vals.len();
+        let idx = 0;
+        GroupsProxyIter { vals, len, idx }
+    }
+}
+
+impl<'a> Iterator for GroupsProxyIter<'a> {
+    type Item = GroupsIndicator<'a>;
+
+    fn nth(&mut self, n: usize) -> Option<Self::Item> {
+        self.idx = self.idx.saturating_add(n);
+        self.next()
+    }
+
+    fn next(&mut self) -> Option<Self::Item> {
+        if self.idx >= self.len {
+            return None;
+        }
+
+        let out = unsafe {
+            match self.vals {
+                GroupsProxy::Idx(groups) => {
+                    let item = groups.get_unchecked(self.idx);
+                    Some(GroupsIndicator::Idx(item))
                 }
-                builder.finish().into_series()
-            }
-            GroupsProxy::Slice { groups, .. } => {
-                let mut builder = AnonymousOwnedListBuilder::new(
-                    self.name(),
-                    groups.len(),
-                    Some(self.dtype().clone()),
-                );
-                for [first, len] in groups {
-                    let taken = s.slice(*first as i64, *len as usize);
-                    builder.append_series(&taken)
+                GroupsProxy::Slice { groups, .. } => {
+                    Some(GroupsIndicator::Slice(*groups.get_unchecked(self.idx)))
                 }
-                builder.finish().into_series()
             }
-        }
+        };
+        self.idx += 1;
+        out
+    }
+}
+
+pub struct GroupsProxyParIter<'a> {
+    vals: &'a GroupsProxy,
+    len: usize,
+}
+
+impl<'a> GroupsProxyParIter<'a> {
+    fn new(vals: &'a GroupsProxy) -> Self {
+        let len = vals.len();
+        GroupsProxyParIter { vals, len }
+    }
+}
+
+impl<'a> ParallelIterator for GroupsProxyParIter<'a> {
+    type Item = GroupsIndicator<'a>;
+
+    fn drive_unindexed<C>(self, consumer: C) -> C::Result
+    where
+        C: UnindexedConsumer<Self::Item>,
+    {
+        (0..self.len)
+            .into_par_iter()
+            .map(|i| unsafe {
+                match self.vals {
+                    GroupsProxy::Idx(groups) => GroupsIndicator::Idx(groups.get_unchecked(i)),
+                    GroupsProxy::Slice { groups, .. } => {
+                        GroupsIndicator::Slice(*groups.get_unchecked(i))
+                    }
+                }
+            })
+            .drive_unindexed(consumer)
+    }
+}
+
+pub struct SlicedGroups<'a> {
+    sliced: ManuallyDrop<GroupsProxy>,
+    #[allow(dead_code)]
+    // we need the lifetime to ensure the slice remains valid
+    borrowed: &'a GroupsProxy,
+}
+
+impl Deref for SlicedGroups<'_> {
+    type Target = GroupsProxy;
+
+    fn deref(&self) -> &Self::Target {
+        self.sliced.deref()
     }
 }
```

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/groupby/hashing.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/hashing.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/groupby/into_groups.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/into_groups.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/groupby/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/groupby/perfect.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/groupby/perfect.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/args.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/args.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/hash_join/zip_outer.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/hash_join/zip_outer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/row/av_buffer.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/row/av_buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/row/dataframe.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/row/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/row/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/row/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/row/transpose.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/row/transpose.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/top_k.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/frame/upstream_traits.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/frame/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/functions.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/hashing/fx.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/hashing/fx.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/hashing/identity.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/hashing/identity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/hashing/partition.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/hashing/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/hashing/vector_hasher.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/hashing/vector_hasher.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/lib.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/named_from.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/named_from.rs`

 * *Files 1% similar despite different names*

```diff
@@ -125,23 +125,23 @@
 
         let dt = series_slice[0].dtype();
 
         // inner type is also list so we need the anonymous builder
         if let DataType::List(_) = dt {
             let mut builder = AnonymousListBuilder::new(name, list_cap, Some(dt.clone()));
             for s in series_slice {
-                builder.append_series(s)
+                builder.append_series(s).unwrap();
             }
             builder.finish().into_series()
         } else {
             let values_cap = series_slice.iter().fold(0, |acc, s| acc + s.len());
 
             let mut builder = get_list_builder(dt, values_cap, list_cap, name).unwrap();
             for series in series_slice {
-                builder.append_series(series)
+                builder.append_series(series).unwrap();
             }
             builder.finish().into_series()
         }
     }
 }
 
 impl<T: AsRef<[Option<Series>]>> NamedFrom<T, [Option<Series>]> for Series {
@@ -153,15 +153,15 @@
         let dt = match series_slice.iter().filter_map(|opt| opt.as_ref()).next() {
             Some(series) => series.dtype(),
             None => &DataType::Null,
         };
 
         let mut builder = get_list_builder(dt, values_cap, series_slice.len(), name).unwrap();
         for series in series_slice {
-            builder.append_opt_series(series.as_ref())
+            builder.append_opt_series(series.as_ref()).unwrap();
         }
         builder.finish().into_series()
     }
 }
 impl<'a, T: AsRef<[&'a str]>> NamedFrom<T, [&'a str]> for Series {
     fn new(name: &str, v: T) -> Self {
         Utf8Chunked::from_slice(name, v.as_ref()).into_series()
```

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/prelude.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/schema.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/serde/chunked_array.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/serde/chunked_array.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/serde/df.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/serde/df.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/serde/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/serde/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/serde/series.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/serde/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/any_value.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/arithmetic/owned.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/arithmetic/owned.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/comparison.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/from.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/array.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/array.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/binary.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/boolean.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/categorical.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/dates_time.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/dates_time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/datetime.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/decimal.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/duration.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/floats.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/list.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/null.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/object.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/object.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/struct_.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/implementations/utf8.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/implementations/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/into.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/into.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/iterator.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/diff.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/diff.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/downcast.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/ewm.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/ewm.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/moment.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/moment.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/null.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/pct_change.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/pct_change.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/round.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/round.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/to_list.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/to_list.rs`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
                 let mut builder =
                     get_list_builder(s_ref.dtype(), s_ref.len(), rows as usize, self.name())?;
 
                 let mut offset = 0i64;
                 for _ in 0..rows {
                     let row = s_ref.slice(offset, cols as usize);
-                    builder.append_series(&row);
+                    builder.append_series(&row).unwrap();
                     offset += cols;
                 }
                 Ok(builder.finish().into_series())
             }
             _ => {
                 panic!("more than two dimensions not yet supported");
             }
```

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/ops/unique.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/series_trait.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/series_trait.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/series/unstable.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/series/unstable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/testing.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/testing.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/utils/flatten.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/utils/flatten.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/utils/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/utils/series.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/utils/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-core/src/utils/supertype.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-core/src/utils/supertype.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-json/Cargo.toml` & `polars_lts_cpu-0.18.6/local_dependencies/polars-json/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-json/LICENSE` & `polars_lts_cpu-0.18.6/local_dependencies/polars/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-json/src/json/deserialize.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-json/src/json/deserialize.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-json/src/json/infer_schema.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-json/src/json/infer_schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-json/src/ndjson/deserialize.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-json/src/ndjson/deserialize.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-json/src/ndjson/file.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-json/src/ndjson/file.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/Cargo.toml` & `polars_lts_cpu-0.18.6/local_dependencies/polars/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/LICENSE` & `polars_lts_cpu-0.18.6/local_dependencies/polars-utils/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/Makefile` & `polars_lts_cpu-0.18.6/local_dependencies/polars/Makefile`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/src/docs/eager.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/src/docs/eager.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/src/docs/lazy.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/src/docs/lazy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/src/docs/performance.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/src/docs/performance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/src/lib.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/core/date_like.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/core/date_like.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/core/groupby.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/core/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/core/joins.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/core/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/core/list.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/core/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/core/pivot.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/core/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/core/random.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/core/random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/core/rolling_window.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/core/rolling_window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/core/series.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/core/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/io/csv.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/io/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/io/ipc_stream.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/io/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/io/json.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/io/json.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/io/parquet.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/io/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/joins.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/aggregation.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/cse.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/expressions/apply.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/expressions/arity.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/expressions/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/expressions/expand.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/expressions/expand.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/expressions/filter.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/expressions/slice.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/expressions/window.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/folds.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/folds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/functions.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/groupby.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/mod.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/predicate_queries.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/projection_queries.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/lazy/queries.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/lazy/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/schema.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars/tests/it/time/date_range.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars/tests/it/time/date_range.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-error/Cargo.toml` & `polars_lts_cpu-0.18.6/local_dependencies/polars-error/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-error/LICENSE` & `polars_lts_cpu-0.18.6/local_dependencies/polars-lazy/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-error/src/lib.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-error/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-algo/Cargo.toml` & `polars_lts_cpu-0.18.6/local_dependencies/polars-algo/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-algo/LICENSE` & `polars_lts_cpu-0.18.6/local_dependencies/polars-ops/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-algo/src/algo.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-algo/src/algo.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-utils/Cargo.toml` & `polars_lts_cpu-0.18.6/local_dependencies/polars-utils/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-utils/LICENSE` & `polars_lts_cpu-0.18.6/local_dependencies/polars-row/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/arena.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/arena.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/atomic.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/atomic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/cell.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/cell.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/contention_pool.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/contention_pool.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/functions.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/iter/enumerate_idx.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/iter/enumerate_idx.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/macros.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/macros.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/slice.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/sort.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/sync.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/sync.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/unwrap.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/unwrap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/vec.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/vec.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-utils/src/wasm.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-utils/src/wasm.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-sql/Cargo.toml` & `polars_lts_cpu-0.18.6/local_dependencies/polars-sql/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-sql/LICENSE` & `polars_lts_cpu-0.18.6/local_dependencies/polars-io/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-sql/src/context.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-sql/src/context.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-sql/src/functions.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-sql/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-sql/src/keywords.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-sql/src/keywords.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-sql/src/sql_expr.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-sql/src/sql_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-sql/src/table_functions.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-sql/src/table_functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/functions_cumulative.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/functions_cumulative.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/functions_io.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/functions_io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/functions_math.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/functions_math.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/functions_meta.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/functions_meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/functions_string.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/functions_string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/iss_7436.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/iss_7436.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/iss_7437.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/iss_7437.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/iss_7440.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/iss_7440.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/iss_8395.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/iss_8395.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/iss_8419.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/iss_8419.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/ops_distinct_on.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/ops_distinct_on.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/simple_exprs.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/simple_exprs.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/local_dependencies/polars-sql/tests/statements.rs` & `polars_lts_cpu-0.18.6/local_dependencies/polars-sql/tests/statements.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/Cargo.toml` & `polars_lts_cpu-0.18.6/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "py-polars"
-version = "0.18.5"
+version = "0.18.6"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [workspace]
 # prevents package from thinking it's in the workspace
 [target.'cfg(any(not(target_os = "linux"), use_mimalloc))'.dependencies]
```

### Comparing `polars_lts_cpu-0.18.5/LICENSE` & `polars_lts_cpu-0.18.6/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/Makefile` & `polars_lts_cpu-0.18.6/Makefile`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/README.md` & `polars_lts_cpu-0.18.6/README.md`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/build.rs` & `polars_lts_cpu-0.18.6/build.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/Makefile` & `polars_lts_cpu-0.18.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/_templates/autosummary/class.rst` & `polars_lts_cpu-0.18.6/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/requirements-docs.txt` & `polars_lts_cpu-0.18.6/docs/requirements-docs.txt`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/run_live_docs_server.py` & `polars_lts_cpu-0.18.6/docs/run_live_docs_server.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/_static/css/custom.css` & `polars_lts_cpu-0.18.6/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/conf.py` & `polars_lts_cpu-0.18.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/api.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/api.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/config.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/config.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/dataframe/modify_select.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/dataframe/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/datatypes.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/datatypes.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/expressions/computation.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/expressions/computation.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/expressions/functions.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/expressions/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/expressions/list.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/expressions/list.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/expressions/modify_select.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/expressions/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/expressions/operators.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/expressions/operators.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/expressions/string.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/expressions/string.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/expressions/temporal.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/expressions/temporal.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/functions.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/io.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/io.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/lazyframe/modify_select.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/lazyframe/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/selectors.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/selectors.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/series/computation.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/series/computation.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/series/descriptive.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/series/descriptive.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/series/list.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/series/list.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/series/modify_select.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/series/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/series/string.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/series/string.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/series/temporal.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/series/temporal.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/docs/source/reference/testing.rst` & `polars_lts_cpu-0.18.6/docs/source/reference/testing.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/__init__.py` & `polars_lts_cpu-0.18.6/polars/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/api.py` & `polars_lts_cpu-0.18.6/polars/api.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/config.py` & `polars_lts_cpu-0.18.6/polars/config.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/convert.py` & `polars_lts_cpu-0.18.6/polars/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/dataframe/_html.py` & `polars_lts_cpu-0.18.6/polars/dataframe/_html.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/dataframe/frame.py` & `polars_lts_cpu-0.18.6/polars/dataframe/frame.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/dataframe/groupby.py` & `polars_lts_cpu-0.18.6/polars/dataframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/datatypes/__init__.py` & `polars_lts_cpu-0.18.6/polars/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/datatypes/classes.py` & `polars_lts_cpu-0.18.6/polars/datatypes/classes.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/datatypes/constants.py` & `polars_lts_cpu-0.18.6/polars/datatypes/constants.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/datatypes/constructor.py` & `polars_lts_cpu-0.18.6/polars/datatypes/constructor.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/datatypes/convert.py` & `polars_lts_cpu-0.18.6/polars/datatypes/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/dependencies.py` & `polars_lts_cpu-0.18.6/polars/dependencies.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/exceptions.py` & `polars_lts_cpu-0.18.6/polars/exceptions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/expr/array.py` & `polars_lts_cpu-0.18.6/polars/expr/array.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/expr/binary.py` & `polars_lts_cpu-0.18.6/polars/expr/binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/expr/categorical.py` & `polars_lts_cpu-0.18.6/polars/expr/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/expr/datetime.py` & `polars_lts_cpu-0.18.6/polars/expr/datetime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/expr/expr.py` & `polars_lts_cpu-0.18.6/polars/expr/expr.py`

 * *Files 2% similar despite different names*

```diff
@@ -3248,14 +3248,52 @@
         breaks
             A list of unique cut points.
         labels
             Labels to assign to bins. If given, the length must be len(probs) + 1.
         left_closed
             Whether intervals should be [) instead of the default of (]
 
+        Examples
+        --------
+        >>> g = pl.repeat("a", 5, eager=True).append(pl.repeat("b", 5, eager=True))
+        >>> df = pl.DataFrame(dict(g=g, x=range(10)))
+        >>> df.with_columns(q=pl.col("x").cut([2, 5]))
+        shape: (10, 3)
+        ┌─────┬─────┬───────────┐
+        │ g   ┆ x   ┆ q         │
+        │ --- ┆ --- ┆ ---       │
+        │ str ┆ i64 ┆ cat       │
+        ╞═════╪═════╪═══════════╡
+        │ a   ┆ 0   ┆ (-inf, 2] │
+        │ a   ┆ 1   ┆ (-inf, 2] │
+        │ a   ┆ 2   ┆ (-inf, 2] │
+        │ a   ┆ 3   ┆ (2, 5]    │
+        │ …   ┆ …   ┆ …         │
+        │ b   ┆ 6   ┆ (5, inf]  │
+        │ b   ┆ 7   ┆ (5, inf]  │
+        │ b   ┆ 8   ┆ (5, inf]  │
+        │ b   ┆ 9   ┆ (5, inf]  │
+        └─────┴─────┴───────────┘
+        >>> df.with_columns(q=pl.col("x").cut([2, 5], left_closed=True))
+        shape: (10, 3)
+        ┌─────┬─────┬───────────┐
+        │ g   ┆ x   ┆ q         │
+        │ --- ┆ --- ┆ ---       │
+        │ str ┆ i64 ┆ cat       │
+        ╞═════╪═════╪═══════════╡
+        │ a   ┆ 0   ┆ [-inf, 2) │
+        │ a   ┆ 1   ┆ [-inf, 2) │
+        │ a   ┆ 2   ┆ [2, 5)    │
+        │ a   ┆ 3   ┆ [2, 5)    │
+        │ …   ┆ …   ┆ …         │
+        │ b   ┆ 6   ┆ [5, inf)  │
+        │ b   ┆ 7   ┆ [5, inf)  │
+        │ b   ┆ 8   ┆ [5, inf)  │
+        │ b   ┆ 9   ┆ [5, inf)  │
+        └─────┴─────┴───────────┘
         """
         return self._from_pyexpr(self._pyexpr.cut(breaks, labels, left_closed))
 
     def qcut(
         self,
         probs: list[float],
         labels: list[str] | None = None,
@@ -3268,22 +3306,79 @@
         Parameters
         ----------
         probs
             Probabilities for which to find the corresponding quantiles
             For p in probs, we assume 0 <= p <= 1
         labels
             Labels to assign to bins. If given, the length must be len(probs) + 1.
-            If computing over a grouping variable we recommend this be set.
+            If computing over groups this must be set for now.
         left_closed
             Whether intervals should be [) instead of the default of (]
         allow_duplicates
             If True, the resulting quantile breaks don't have to be unique. This can
             happen even with unique probs depending on the data. Duplicates will be
             dropped, resulting in fewer bins.
 
+
+        Examples
+        --------
+        >>> g = pl.repeat("a", 5, eager=True).append(pl.repeat("b", 5, eager=True))
+        >>> df = pl.DataFrame(dict(g=g, x=range(10)))
+        >>> df.with_columns(q=pl.col("x").qcut([0.5]))
+        shape: (10, 3)
+        ┌─────┬─────┬─────────────┐
+        │ g   ┆ x   ┆ q           │
+        │ --- ┆ --- ┆ ---         │
+        │ str ┆ i64 ┆ cat         │
+        ╞═════╪═════╪═════════════╡
+        │ a   ┆ 0   ┆ (-inf, 4.5] │
+        │ a   ┆ 1   ┆ (-inf, 4.5] │
+        │ a   ┆ 2   ┆ (-inf, 4.5] │
+        │ a   ┆ 3   ┆ (-inf, 4.5] │
+        │ …   ┆ …   ┆ …           │
+        │ b   ┆ 6   ┆ (4.5, inf]  │
+        │ b   ┆ 7   ┆ (4.5, inf]  │
+        │ b   ┆ 8   ┆ (4.5, inf]  │
+        │ b   ┆ 9   ┆ (4.5, inf]  │
+        └─────┴─────┴─────────────┘
+        >>> df.with_columns(q=pl.col("x").qcut([0.5], ["lo", "hi"]).over("g"))
+        shape: (10, 3)
+        ┌─────┬─────┬─────┐
+        │ g   ┆ x   ┆ q   │
+        │ --- ┆ --- ┆ --- │
+        │ str ┆ i64 ┆ cat │
+        ╞═════╪═════╪═════╡
+        │ a   ┆ 0   ┆ lo  │
+        │ a   ┆ 1   ┆ lo  │
+        │ a   ┆ 2   ┆ lo  │
+        │ a   ┆ 3   ┆ hi  │
+        │ …   ┆ …   ┆ …   │
+        │ b   ┆ 6   ┆ lo  │
+        │ b   ┆ 7   ┆ lo  │
+        │ b   ┆ 8   ┆ hi  │
+        │ b   ┆ 9   ┆ hi  │
+        └─────┴─────┴─────┘
+        >>> df.with_columns(q=pl.col("x").qcut([0.5], ["lo", "hi"], True).over("g"))
+        shape: (10, 3)
+        ┌─────┬─────┬─────┐
+        │ g   ┆ x   ┆ q   │
+        │ --- ┆ --- ┆ --- │
+        │ str ┆ i64 ┆ cat │
+        ╞═════╪═════╪═════╡
+        │ a   ┆ 0   ┆ lo  │
+        │ a   ┆ 1   ┆ lo  │
+        │ a   ┆ 2   ┆ hi  │
+        │ a   ┆ 3   ┆ hi  │
+        │ …   ┆ …   ┆ …   │
+        │ b   ┆ 6   ┆ lo  │
+        │ b   ┆ 7   ┆ hi  │
+        │ b   ┆ 8   ┆ hi  │
+        │ b   ┆ 9   ┆ hi  │
+        └─────┴─────┴─────┘
+
         """
         return self._from_pyexpr(
             self._pyexpr.qcut(probs, labels, left_closed, allow_duplicates)
         )
 
     def filter(self, predicate: Expr) -> Self:
         """
```

### Comparing `polars_lts_cpu-0.18.5/polars/expr/list.py` & `polars_lts_cpu-0.18.6/polars/expr/list.py`

 * *Files 4% similar despite different names*

```diff
@@ -970,15 +970,15 @@
         ┌───────────┬──────────────┬──────────────┐
         │ a         ┆ b            ┆ intersection │
         │ ---       ┆ ---          ┆ ---          │
         │ list[i64] ┆ list[i64]    ┆ list[i64]    │
         ╞═══════════╪══════════════╪══════════════╡
         │ [1, 2, 3] ┆ [2, 3, 4]    ┆ [2, 3]       │
         │ []        ┆ [3]          ┆ []           │
-        │ [null, 3] ┆ [3, 4, null] ┆ [3, null]    │
+        │ [null, 3] ┆ [3, 4, null] ┆ [null, 3]    │
         │ [5, 6, 7] ┆ [6, 8]       ┆ [6]          │
         └───────────┴──────────────┴──────────────┘
 
         """  # noqa: W505.
         other = parse_as_expression(other, str_as_lit=False)
         return wrap_expr(self._pyexpr.list_set_operation(other, "intersection"))
 
@@ -987,10 +987,31 @@
         Compute the SET SYMMETRIC DIFFERENCE between the elements in this list and the elements of ``other``.
 
         Parameters
         ----------
         other
             Right hand side of the set operation.
 
+
+        Examples
+        --------
+        >>> df = pl.DataFrame(
+        ...     {
+        ...         "a": [[1, 2, 3], [], [None, 3], [5, 6, 7]],
+        ...         "b": [[2, 3, 4], [3], [3, 4, None], [6, 8]],
+        ...     }
+        ... )
+        >>> df.with_columns(pl.col("b").list.symmetric_difference("a").alias("sdiff"))
+        shape: (4, 3)
+        ┌───────────┬──────────────┬───────────┐
+        │ a         ┆ b            ┆ sdiff     │
+        │ ---       ┆ ---          ┆ ---       │
+        │ list[i64] ┆ list[i64]    ┆ list[i64] │
+        ╞═══════════╪══════════════╪═══════════╡
+        │ [1, 2, 3] ┆ [2, 3, 4]    ┆ [4, 1]    │
+        │ []        ┆ [3]          ┆ [3]       │
+        │ [null, 3] ┆ [3, 4, null] ┆ [4]       │
+        │ [5, 6, 7] ┆ [6, 8]       ┆ [8, 5, 7] │
+        └───────────┴──────────────┴───────────┘
         """  # noqa: W505.
         other = parse_as_expression(other, str_as_lit=False)
         return wrap_expr(self._pyexpr.list_set_operation(other, "symmetric_difference"))
```

### Comparing `polars_lts_cpu-0.18.5/polars/expr/meta.py` & `polars_lts_cpu-0.18.6/polars/expr/meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/expr/string.py` & `polars_lts_cpu-0.18.6/polars/expr/string.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/expr/struct.py` & `polars_lts_cpu-0.18.6/polars/expr/struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/functions/__init__.py` & `polars_lts_cpu-0.18.6/polars/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/functions/as_datatype.py` & `polars_lts_cpu-0.18.6/polars/functions/as_datatype.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/functions/eager.py` & `polars_lts_cpu-0.18.6/polars/functions/eager.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/functions/lazy.py` & `polars_lts_cpu-0.18.6/polars/functions/lazy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/functions/range.py` & `polars_lts_cpu-0.18.6/polars/functions/range.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/functions/repeat.py` & `polars_lts_cpu-0.18.6/polars/functions/repeat.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/functions/whenthen.py` & `polars_lts_cpu-0.18.6/polars/functions/whenthen.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/io/__init__.py` & `polars_lts_cpu-0.18.6/polars/io/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/io/_utils.py` & `polars_lts_cpu-0.18.6/polars/io/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/io/avro.py` & `polars_lts_cpu-0.18.6/polars/io/avro.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/io/csv/_utils.py` & `polars_lts_cpu-0.18.6/polars/io/csv/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/io/csv/batched_reader.py` & `polars_lts_cpu-0.18.6/polars/io/csv/batched_reader.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/io/csv/functions.py` & `polars_lts_cpu-0.18.6/polars/io/csv/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/io/database.py` & `polars_lts_cpu-0.18.6/polars/io/database.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/io/delta.py` & `polars_lts_cpu-0.18.6/polars/io/delta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/io/excel/_write_utils.py` & `polars_lts_cpu-0.18.6/polars/io/excel/_write_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/io/excel/functions.py` & `polars_lts_cpu-0.18.6/polars/io/excel/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/io/ipc/anonymous_scan.py` & `polars_lts_cpu-0.18.6/polars/io/ipc/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/io/ipc/functions.py` & `polars_lts_cpu-0.18.6/polars/io/ipc/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/io/ndjson.py` & `polars_lts_cpu-0.18.6/polars/io/ndjson.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/io/parquet/anonymous_scan.py` & `polars_lts_cpu-0.18.6/polars/io/parquet/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/io/parquet/functions.py` & `polars_lts_cpu-0.18.6/polars/io/parquet/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/io/pyarrow_dataset/anonymous_scan.py` & `polars_lts_cpu-0.18.6/polars/io/pyarrow_dataset/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/io/pyarrow_dataset/functions.py` & `polars_lts_cpu-0.18.6/polars/io/pyarrow_dataset/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/lazyframe/frame.py` & `polars_lts_cpu-0.18.6/polars/lazyframe/frame.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/lazyframe/groupby.py` & `polars_lts_cpu-0.18.6/polars/lazyframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/selectors.py` & `polars_lts_cpu-0.18.6/polars/selectors.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/series/_numpy.py` & `polars_lts_cpu-0.18.6/polars/series/_numpy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/series/array.py` & `polars_lts_cpu-0.18.6/polars/series/array.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/series/binary.py` & `polars_lts_cpu-0.18.6/polars/series/binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/series/categorical.py` & `polars_lts_cpu-0.18.6/polars/series/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/series/datetime.py` & `polars_lts_cpu-0.18.6/polars/series/datetime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/series/list.py` & `polars_lts_cpu-0.18.6/polars/series/list.py`

 * *Files 0% similar despite different names*

```diff
@@ -619,15 +619,15 @@
         >>> b = pl.Series([[2, 3, 4], [3], [3, 4, None], [6, 8]])
         >>> a.list.intersection(b)
         shape: (4,)
         Series: '' [list[i64]]
         [
                 [2, 3]
                 []
-                [3, null]
+                [null, 3]
                 [6]
         ]
 
         """  # noqa: W505.
 
     def symmetric_difference(self, other: Series) -> Series:
         """
```

### Comparing `polars_lts_cpu-0.18.5/polars/series/series.py` & `polars_lts_cpu-0.18.6/polars/series/series.py`

 * *Files 2% similar despite different names*

```diff
@@ -1649,15 +1649,48 @@
         │ -1.5 ┆ -1.0        ┆ (-inf, -1.0] │
         │ …    ┆ …           ┆ …            │
         │ 1.0  ┆ 1.0         ┆ (-1.0, 1.0]  │
         │ 1.5  ┆ inf         ┆ (1.0, inf]   │
         │ 2.0  ┆ inf         ┆ (1.0, inf]   │
         │ 2.5  ┆ inf         ┆ (1.0, inf]   │
         └──────┴─────────────┴──────────────┘
-
+        >>> a.cut([-1, 1], series=True)
+        shape: (12,)
+        Series: 'a' [cat]
+        [
+            "(-inf, -1]"
+            "(-inf, -1]"
+            "(-inf, -1]"
+            "(-inf, -1]"
+            "(-inf, -1]"
+            "(-1, 1]"
+            "(-1, 1]"
+            "(-1, 1]"
+            "(-1, 1]"
+            "(1, inf]"
+            "(1, inf]"
+            "(1, inf]"
+        ]
+        >>> a.cut([-1, 1], series=True, left_closed=True)
+        shape: (12,)
+        Series: 'a' [cat]
+        [
+            "[-inf, -1)"
+            "[-inf, -1)"
+            "[-inf, -1)"
+            "[-inf, -1)"
+            "[-1, 1)"
+            "[-1, 1)"
+            "[-1, 1)"
+            "[-1, 1)"
+            "[1, inf)"
+            "[1, inf)"
+            "[1, inf)"
+            "[1, inf)"
+        ]
         """
         if series:
             return (
                 self.to_frame()
                 .select(F.col(self._s.name()).cut(bins, labels, left_closed))
                 .to_series()
             )
@@ -1691,21 +1724,21 @@
         quantiles
             List of quantiles to create.
             We expect quantiles ``0.0 <= quantile <= 1``
         labels
             Labels to assign to the quantiles. If given the length of labels must be
             len(bins) + 1.
         break_point_label
-            Name given to the breakpoint column.
+            Name given to the breakpoint column. Only used if series == False.
         category_label
-            Name given to the category column.
+            Name given to the category column. Only used if series == False.
         maintain_order
-            Keep the order of the original `Series`.
+            Keep the order of the original `Series`. Only used if series == False.
         series
-            If True, return the a categorical series in the data's original order
+            If True, return a categorical series in the data's original order
         left_closed
             Whether intervals should be [) instead of (]
         allow_duplicates
             If True, the resulting quantile breaks don't have to be unique. This can
             happen even with unique probs depending on the data. Duplicates will be
             dropped, resulting in fewer bins.
 
@@ -1733,15 +1766,40 @@
         │ -3.0 ┆ 0.25        ┆ (-3.25, 0.25] │
         │ -2.0 ┆ 0.25        ┆ (-3.25, 0.25] │
         │ -1.0 ┆ 0.25        ┆ (-3.25, 0.25] │
         │ 0.0  ┆ 0.25        ┆ (-3.25, 0.25] │
         │ 1.0  ┆ inf         ┆ (0.25, inf]   │
         │ 2.0  ┆ inf         ┆ (0.25, inf]   │
         └──────┴─────────────┴───────────────┘
-
+        >>> a.qcut([0.0, 0.25, 0.75], series=True)
+        shape: (8,)
+        Series: 'a' [cat]
+        [
+            "(-inf, -5]"
+            "(-5, -3.25]"
+            "(-3.25, 0.25]"
+            "(-3.25, 0.25]"
+            "(-3.25, 0.25]"
+            "(-3.25, 0.25]"
+            "(0.25, inf]"
+            "(0.25, inf]"
+        ]
+        >>> a.qcut([0.0, 0.25, 0.75], series=True, left_closed=True)
+        shape: (8,)
+        Series: 'a' [cat]
+        [
+            "[-5, -3.25)"
+            "[-5, -3.25)"
+            "[-3.25, 0.25)"
+            "[-3.25, 0.25)"
+            "[-3.25, 0.25)"
+            "[-3.25, 0.25)"
+            "[0.25, inf)"
+            "[0.25, inf)"
+        ]
         """
         if series:
             return (
                 self.to_frame()
                 .select(
                     F.col(self._s.name()).qcut(
                         quantiles, labels, left_closed, allow_duplicates
```

### Comparing `polars_lts_cpu-0.18.5/polars/series/string.py` & `polars_lts_cpu-0.18.6/polars/series/string.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/series/struct.py` & `polars_lts_cpu-0.18.6/polars/series/struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/series/utils.py` & `polars_lts_cpu-0.18.6/polars/series/utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/slice.py` & `polars_lts_cpu-0.18.6/polars/slice.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/sql/context.py` & `polars_lts_cpu-0.18.6/polars/sql/context.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/string_cache.py` & `polars_lts_cpu-0.18.6/polars/string_cache.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/testing/_private.py` & `polars_lts_cpu-0.18.6/polars/testing/_private.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/testing/asserts.py` & `polars_lts_cpu-0.18.6/polars/testing/asserts.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/testing/parametric/__init__.py` & `polars_lts_cpu-0.18.6/polars/testing/parametric/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/testing/parametric/primitives.py` & `polars_lts_cpu-0.18.6/polars/testing/parametric/primitives.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/testing/parametric/profiles.py` & `polars_lts_cpu-0.18.6/polars/testing/parametric/profiles.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/testing/parametric/strategies.py` & `polars_lts_cpu-0.18.6/polars/testing/parametric/strategies.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/type_aliases.py` & `polars_lts_cpu-0.18.6/polars/type_aliases.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/utils/__init__.py` & `polars_lts_cpu-0.18.6/polars/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/utils/_construction.py` & `polars_lts_cpu-0.18.6/polars/utils/_construction.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/utils/_parse_expr_input.py` & `polars_lts_cpu-0.18.6/polars/utils/_parse_expr_input.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/utils/_scan.py` & `polars_lts_cpu-0.18.6/polars/utils/_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/utils/_wrap.py` & `polars_lts_cpu-0.18.6/polars/utils/_wrap.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/utils/build_info.py` & `polars_lts_cpu-0.18.6/polars/utils/build_info.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/utils/convert.py` & `polars_lts_cpu-0.18.6/polars/utils/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/utils/decorators.py` & `polars_lts_cpu-0.18.6/polars/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/utils/meta.py` & `polars_lts_cpu-0.18.6/polars/utils/meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/utils/polars_version.py` & `polars_lts_cpu-0.18.6/polars/utils/polars_version.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/utils/show_versions.py` & `polars_lts_cpu-0.18.6/polars/utils/show_versions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/polars/utils/various.py` & `polars_lts_cpu-0.18.6/polars/utils/various.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/pyproject.toml` & `polars_lts_cpu-0.18.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/requirements-dev.txt` & `polars_lts_cpu-0.18.6/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/scripts/check_stacklevels.py` & `polars_lts_cpu-0.18.6/scripts/check_stacklevels.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/apply/dataframe.rs` & `polars_lts_cpu-0.18.6/src/apply/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/apply/lazy.rs` & `polars_lts_cpu-0.18.6/src/apply/lazy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/apply/mod.rs` & `polars_lts_cpu-0.18.6/src/apply/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -255,22 +255,26 @@
     capacity: usize,
 ) -> PyResult<ListChunked> {
     let mut builder =
         get_list_builder(dt, capacity * 5, capacity, name).map_err(PyPolarsErr::from)?;
     for _ in 0..init_null_count {
         builder.append_null()
     }
-    builder.append_opt_series(first_value);
+    builder
+        .append_opt_series(first_value)
+        .map_err(PyPolarsErr::from)?;
     for opt_val in it {
         match opt_val {
             None => builder.append_null(),
             Some(s) => {
                 if s.len() == 0 && s.dtype() != dt {
-                    builder.append_series(&Series::full_null("", 0, dt))
+                    builder
+                        .append_series(&Series::full_null("", 0, dt))
+                        .unwrap()
                 } else {
-                    builder.append_series(&s)
+                    builder.append_series(&s).map_err(PyPolarsErr::from)?
                 }
             }
         }
     }
     Ok(builder.finish())
 }
```

### Comparing `polars_lts_cpu-0.18.5/src/apply/series.rs` & `polars_lts_cpu-0.18.6/src/apply/series.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1126,18 +1126,20 @@
     match out {
         Ok(out) => {
             // unpack the wrapper in a PySeries
             let py_pyseries = out
                 .getattr("_s")
                 .expect("could net get series attribute '_s'");
             let pyseries = py_pyseries.extract::<PySeries>()?;
-            builder.append_series(&pyseries.series);
+            builder
+                .append_series(&pyseries.series)
+                .map_err(PyPolarsErr::from)?;
         }
         Err(_) => {
-            builder.append_opt_series(None);
+            builder.append_opt_series(None).map_err(PyPolarsErr::from)?;
         }
     };
     Ok(())
 }
 
 fn call_series_lambda(pypolars: &PyModule, lambda: &PyAny, series: Series) -> Option<Series> {
     // create a PySeries struct/object for Python
@@ -1207,15 +1209,17 @@
                     // use first value to get dtype and replace default builder
                     if let Some(series) = it.next() {
                         let out_series = call_series_lambda(pypolars, lambda, series)
                             .expect("Cannot determine dtype because lambda failed; Make sure that your udf returns a Series");
                         let dt = out_series.dtype();
                         builder = get_list_builder(dt, self.len() * 5, self.len(), self.name())
                             .map_err(PyPolarsErr::from)?;
-                        builder.append_opt_series(Some(&out_series));
+                        builder
+                            .append_opt_series(Some(&out_series))
+                            .map_err(PyPolarsErr::from)?;
                     } else {
                         let mut builder =
                             get_list_builder(dt, 0, 1, self.name()).map_err(PyPolarsErr::from)?;
                         let ca = builder.finish();
                         return Ok(PySeries::new(ca.into_series()));
                     }
                     for series in it {
@@ -1230,28 +1234,30 @@
                     for opt_series in &mut it {
                         if let Some(series) = opt_series {
                             let out_series = call_series_lambda(pypolars, lambda, series)
                                 .expect("Cannot determine dtype because lambda failed; Make sure that your udf returns a Series");
                             let dt = out_series.dtype();
                             builder = get_list_builder(dt, self.len() * 5, self.len(), self.name())
                                 .map_err(PyPolarsErr::from)?;
-                            builder.append_opt_series(Some(&out_series));
+                            builder
+                                .append_opt_series(Some(&out_series))
+                                .map_err(PyPolarsErr::from)?;
                             break;
                         } else {
                             nulls += 1;
                         }
                     }
                     for _ in 0..nulls {
-                        builder.append_opt_series(None);
+                        builder.append_opt_series(None).map_err(PyPolarsErr::from)?;
                     }
                     for opt_series in it {
                         if let Some(series) = opt_series {
                             append_series(pypolars, &mut *builder, lambda, series)?;
                         } else {
-                            builder.append_opt_series(None)
+                            builder.append_opt_series(None).unwrap()
                         }
                     }
                 };
                 let ca = builder.finish();
                 Ok(PySeries::new(ca.into_series()))
             }
             _ => unimplemented!(),
```

### Comparing `polars_lts_cpu-0.18.5/src/arrow_interop/to_py.rs` & `polars_lts_cpu-0.18.6/src/arrow_interop/to_py.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/arrow_interop/to_rust.rs` & `polars_lts_cpu-0.18.6/src/arrow_interop/to_rust.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/batched_csv.rs` & `polars_lts_cpu-0.18.6/src/batched_csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/conversion.rs` & `polars_lts_cpu-0.18.6/src/conversion.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1303,15 +1303,15 @@
 #[cfg(feature = "list_sets")]
 impl FromPyObject<'_> for Wrap<SetOperation> {
     fn extract(ob: &PyAny) -> PyResult<Self> {
         let parsed = match ob.extract::<&str>()? {
             "union" => SetOperation::Union,
             "difference" => SetOperation::Difference,
             "intersection" => SetOperation::Intersection,
-            "symmetric_difference" => SetOperation::Difference,
+            "symmetric_difference" => SetOperation::SymmetricDifference,
             v => {
                 return Err(PyValueError::new_err(format!(
                     "validate must be one of {{'union', 'difference', 'intersection', 'symmetric_difference'}}, got {v}",
                 )))
             }
         };
         Ok(Wrap(parsed))
```

### Comparing `polars_lts_cpu-0.18.5/src/dataframe.rs` & `polars_lts_cpu-0.18.6/src/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/datatypes.rs` & `polars_lts_cpu-0.18.6/src/datatypes.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/error.rs` & `polars_lts_cpu-0.18.6/src/error.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/expr/array.rs` & `polars_lts_cpu-0.18.6/src/expr/array.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/expr/binary.rs` & `polars_lts_cpu-0.18.6/src/expr/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/expr/datetime.rs` & `polars_lts_cpu-0.18.6/src/expr/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/expr/general.rs` & `polars_lts_cpu-0.18.6/src/expr/general.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/expr/list.rs` & `polars_lts_cpu-0.18.6/src/expr/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/expr/meta.rs` & `polars_lts_cpu-0.18.6/src/expr/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/expr/mod.rs` & `polars_lts_cpu-0.18.6/src/expr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/expr/string.rs` & `polars_lts_cpu-0.18.6/src/expr/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/file.rs` & `polars_lts_cpu-0.18.6/src/file.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/functions/eager.rs` & `polars_lts_cpu-0.18.6/src/functions/eager.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/functions/io.rs` & `polars_lts_cpu-0.18.6/src/functions/io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/functions/lazy.rs` & `polars_lts_cpu-0.18.6/src/functions/lazy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/functions/meta.rs` & `polars_lts_cpu-0.18.6/src/functions/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/functions/range.rs` & `polars_lts_cpu-0.18.6/src/functions/range.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/functions/whenthen.rs` & `polars_lts_cpu-0.18.6/src/functions/whenthen.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/lazyframe.rs` & `polars_lts_cpu-0.18.6/src/lazyframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/lazygroupby.rs` & `polars_lts_cpu-0.18.6/src/lazygroupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/lib.rs` & `polars_lts_cpu-0.18.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/on_startup.rs` & `polars_lts_cpu-0.18.6/src/on_startup.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/series/aggregation.rs` & `polars_lts_cpu-0.18.6/src/series/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/series/arithmetic.rs` & `polars_lts_cpu-0.18.6/src/series/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/series/comparison.rs` & `polars_lts_cpu-0.18.6/src/series/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/series/construction.rs` & `polars_lts_cpu-0.18.6/src/series/construction.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/series/export.rs` & `polars_lts_cpu-0.18.6/src/series/export.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/series/mod.rs` & `polars_lts_cpu-0.18.6/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/series/numpy_ufunc.rs` & `polars_lts_cpu-0.18.6/src/series/numpy_ufunc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/series/set_at_idx.rs` & `polars_lts_cpu-0.18.6/src/series/set_at_idx.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/sql.rs` & `polars_lts_cpu-0.18.6/src/sql.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/src/utils.rs` & `polars_lts_cpu-0.18.6/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/README.md` & `polars_lts_cpu-0.18.6/tests/README.md`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/benchmark/groupby-datagen.R` & `polars_lts_cpu-0.18.6/tests/benchmark/groupby-datagen.R`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/benchmark/run_h2oai_benchmark.py` & `polars_lts_cpu-0.18.6/tests/benchmark/run_h2oai_benchmark.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/benchmark/test_release.py` & `polars_lts_cpu-0.18.6/tests/benchmark/test_release.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/docs/run_doctest.py` & `polars_lts_cpu-0.18.6/tests/docs/run_doctest.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/parametric/test_dataframe.py` & `polars_lts_cpu-0.18.6/tests/parametric/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/parametric/test_groupby_rolling.py` & `polars_lts_cpu-0.18.6/tests/parametric/test_groupby_rolling.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/parametric/test_lazyframe.py` & `polars_lts_cpu-0.18.6/tests/parametric/test_lazyframe.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/parametric/test_lit.py` & `polars_lts_cpu-0.18.6/tests/parametric/test_lit.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/parametric/test_series.py` & `polars_lts_cpu-0.18.6/tests/parametric/test_series.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/parametric/test_testing.py` & `polars_lts_cpu-0.18.6/tests/parametric/test_testing.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/parametric/time_series/test_to_datetime.py` & `polars_lts_cpu-0.18.6/tests/parametric/time_series/test_to_datetime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/conftest.py` & `polars_lts_cpu-0.18.6/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/datatypes/test_array.py` & `polars_lts_cpu-0.18.6/tests/unit/datatypes/test_array.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/datatypes/test_binary.py` & `polars_lts_cpu-0.18.6/tests/unit/datatypes/test_binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/datatypes/test_bool.py` & `polars_lts_cpu-0.18.6/tests/unit/datatypes/test_bool.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/datatypes/test_categorical.py` & `polars_lts_cpu-0.18.6/tests/unit/datatypes/test_categorical.py`

 * *Files 2% similar despite different names*

```diff
@@ -407,7 +407,18 @@
     with pl.StringCache():
         df1 = pl.DataFrame({"x": ["A"]}).with_columns(pl.col("x").cast(pl.Categorical))
         df2 = pl.DataFrame({"x": ["B"]}).with_columns(pl.col("x").cast(pl.Categorical))
 
     out = pl.concat([df1, df2])
     assert out.dtypes == [pl.Categorical]
     assert out["x"].to_list() == ["A", "B"]
+
+
+def test_list_builder_different_categorical_rev_maps() -> None:
+    with pl.StringCache():
+        # built with different values, so different rev-map
+        s1 = pl.Series(["a", "b"], dtype=pl.Categorical)
+        s2 = pl.Series(["c", "d"], dtype=pl.Categorical)
+
+    assert pl.DataFrame({"c": [s1, s2]}).to_dict(False) == {
+        "c": [["a", "b"], ["c", "d"]]
+    }
```

### Comparing `polars_lts_cpu-0.18.5/tests/unit/datatypes/test_decimal.py` & `polars_lts_cpu-0.18.6/tests/unit/datatypes/test_decimal.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/datatypes/test_duration.py` & `polars_lts_cpu-0.18.6/tests/unit/datatypes/test_duration.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/datatypes/test_list.py` & `polars_lts_cpu-0.18.6/tests/unit/datatypes/test_list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/datatypes/test_object.py` & `polars_lts_cpu-0.18.6/tests/unit/datatypes/test_object.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/datatypes/test_struct.py` & `polars_lts_cpu-0.18.6/tests/unit/datatypes/test_struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/datatypes/test_temporal.py` & `polars_lts_cpu-0.18.6/tests/unit/datatypes/test_temporal.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/functions/test_as_datatype.py` & `polars_lts_cpu-0.18.6/tests/unit/functions/test_as_datatype.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/functions/test_functions.py` & `polars_lts_cpu-0.18.6/tests/unit/functions/test_functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/functions/test_range.py` & `polars_lts_cpu-0.18.6/tests/unit/functions/test_range.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/functions/test_repeat.py` & `polars_lts_cpu-0.18.6/tests/unit/functions/test_repeat.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json` & `polars_lts_cpu-0.18.6/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json` & `polars_lts_cpu-0.18.6/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet` & `polars_lts_cpu-0.18.6/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet` & `polars_lts_cpu-0.18.6/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/files/example.xlsx` & `polars_lts_cpu-0.18.6/tests/unit/io/files/example.xlsx`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/files/foods1.ipc` & `polars_lts_cpu-0.18.6/tests/unit/io/files/foods1.ipc`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/files/foods1.ndjson` & `polars_lts_cpu-0.18.6/tests/unit/io/files/foods1.ndjson`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/files/foods1.parquet` & `polars_lts_cpu-0.18.6/tests/unit/io/files/foods1.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/files/foods2.ipc` & `polars_lts_cpu-0.18.6/tests/unit/io/files/foods2.ipc`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/files/foods2.ndjson` & `polars_lts_cpu-0.18.6/tests/unit/io/files/foods2.ndjson`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/files/foods2.parquet` & `polars_lts_cpu-0.18.6/tests/unit/io/files/foods2.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/files/small.parquet` & `polars_lts_cpu-0.18.6/tests/unit/io/files/small.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/test_avro.py` & `polars_lts_cpu-0.18.6/tests/unit/io/test_avro.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/test_csv.py` & `polars_lts_cpu-0.18.6/tests/unit/io/test_csv.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/test_database.py` & `polars_lts_cpu-0.18.6/tests/unit/io/test_database.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/test_delta.py` & `polars_lts_cpu-0.18.6/tests/unit/io/test_delta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/test_excel.py` & `polars_lts_cpu-0.18.6/tests/unit/io/test_excel.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/test_ipc.py` & `polars_lts_cpu-0.18.6/tests/unit/io/test_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/test_json.py` & `polars_lts_cpu-0.18.6/tests/unit/io/test_json.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/test_lazy_csv.py` & `polars_lts_cpu-0.18.6/tests/unit/io/test_lazy_csv.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/test_lazy_ipc.py` & `polars_lts_cpu-0.18.6/tests/unit/io/test_lazy_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/test_lazy_json.py` & `polars_lts_cpu-0.18.6/tests/unit/io/test_lazy_json.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/test_lazy_parquet.py` & `polars_lts_cpu-0.18.6/tests/unit/io/test_lazy_parquet.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/test_other.py` & `polars_lts_cpu-0.18.6/tests/unit/io/test_other.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/test_parquet.py` & `polars_lts_cpu-0.18.6/tests/unit/io/test_parquet.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/test_pickle.py` & `polars_lts_cpu-0.18.6/tests/unit/io/test_pickle.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/io/test_pyarrow_dataset.py` & `polars_lts_cpu-0.18.6/tests/unit/io/test_pyarrow_dataset.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/namespaces/test_array.py` & `polars_lts_cpu-0.18.6/tests/unit/namespaces/test_array.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/namespaces/test_binary.py` & `polars_lts_cpu-0.18.6/tests/unit/namespaces/test_binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/namespaces/test_categorical.py` & `polars_lts_cpu-0.18.6/tests/unit/namespaces/test_categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/namespaces/test_datetime.py` & `polars_lts_cpu-0.18.6/tests/unit/namespaces/test_datetime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/namespaces/test_list.py` & `polars_lts_cpu-0.18.6/tests/unit/namespaces/test_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -461,15 +461,15 @@
 
     assert df.select(pl.col("a").list.union("b"))["a"].to_list() == [
         [1, 2, 3, 4],
         [1, 2, 12],
         [4],
     ]
     assert df.select(pl.col("a").list.intersection("b"))["a"].to_list() == [
-        [2, 1],
+        [1, 2],
         [1],
         [4],
     ]
     assert df.select(pl.col("a").list.difference("b"))["a"].to_list() == [[3], [], []]
     assert df.select(pl.col("b").list.difference("a"))["b"].to_list() == [
         [4],
         [2, 12],
@@ -492,7 +492,19 @@
         }
     )
 
     assert df.select(pl.col("a").list.union("b"))["a"].to_list() == [
         ["a", "b", "c", "s"],
         ["b", "e", "z", "a", "f"],
     ]
+
+    df = pl.DataFrame(
+        {
+            "a": [[2, 3, 3], [3, 1], [1, 2, 3]],
+            "b": [[2, 3, 4], [3, 3, 1], [3, 3]],
+        }
+    )
+    r1 = df.with_columns(pl.col("a").list.intersection("b"))["a"].to_list()
+    r2 = df.with_columns(pl.col("b").list.intersection("a"))["b"].to_list()
+    exp = [[2, 3], [3, 1], [3]]
+    assert r1 == exp
+    assert r2 == exp
```

### Comparing `polars_lts_cpu-0.18.5/tests/unit/namespaces/test_meta.py` & `polars_lts_cpu-0.18.6/tests/unit/namespaces/test_meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/namespaces/test_string.py` & `polars_lts_cpu-0.18.6/tests/unit/namespaces/test_string.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/namespaces/test_strptime.py` & `polars_lts_cpu-0.18.6/tests/unit/namespaces/test_strptime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/namespaces/test_struct.py` & `polars_lts_cpu-0.18.6/tests/unit/namespaces/test_struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_aggregations.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_apply.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_apply.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_arithmetic.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_comparison.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_comparison.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_drop.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_drop.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_explode.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_explode.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_filter.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_filter.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_folds.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_folds.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_groupby.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_groupby_rolling.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_groupby_rolling.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_is_in.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_is_in.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_join.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_join.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_join_asof.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_join_asof.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_melt.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_melt.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_pivot.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_pivot.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_random.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_random.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_rolling.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_rolling.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_select.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_select.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_sort.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_sort.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_statistics.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_statistics.py`

 * *Files 19% similar despite different names*

```diff
@@ -186,7 +186,64 @@
     ) == {"A": [timedelta(seconds=43200)]}
 
 
 def test_correlation_cast_supertype() -> None:
     df = pl.DataFrame({"a": [1, 8, 3], "b": [4.0, 5.0, 2.0]})
     df = df.with_columns(pl.col("b"))
     assert df.select(pl.corr("a", "b")).to_dict(False) == {"a": [0.5447047794019223]}
+
+
+def test_cut_over() -> None:
+    with pl.StringCache():
+        x = pl.Series(range(20))
+    r = pl.Series(
+        [pl.repeat("a", 10, eager=True), pl.repeat("b", 10, eager=True)]
+    ).explode()
+    df = pl.DataFrame({"x": x, "g": r})
+
+    out = df.with_columns(pl.col("x").qcut([0.5]).over("g")).to_dict(False)
+    assert out == {
+        "x": [
+            "(-inf, 4.5]",
+            "(-inf, 4.5]",
+            "(-inf, 4.5]",
+            "(-inf, 4.5]",
+            "(-inf, 4.5]",
+            "(4.5, inf]",
+            "(4.5, inf]",
+            "(4.5, inf]",
+            "(4.5, inf]",
+            "(4.5, inf]",
+            "(-inf, 14.5]",
+            "(-inf, 14.5]",
+            "(-inf, 14.5]",
+            "(-inf, 14.5]",
+            "(-inf, 14.5]",
+            "(14.5, inf]",
+            "(14.5, inf]",
+            "(14.5, inf]",
+            "(14.5, inf]",
+            "(14.5, inf]",
+        ],
+        "g": [
+            "a",
+            "a",
+            "a",
+            "a",
+            "a",
+            "a",
+            "a",
+            "a",
+            "a",
+            "a",
+            "b",
+            "b",
+            "b",
+            "b",
+            "b",
+            "b",
+            "b",
+            "b",
+            "b",
+            "b",
+        ],
+    }
```

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_transpose.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_transpose.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_unique.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_unique.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_window.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_window.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/operations/test_with_columns.py` & `polars_lts_cpu-0.18.6/tests/unit/operations/test_with_columns.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/streaming/test_ooc.py` & `polars_lts_cpu-0.18.6/tests/unit/streaming/test_ooc.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/streaming/test_streaming.py` & `polars_lts_cpu-0.18.6/tests/unit/streaming/test_streaming.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_api.py` & `polars_lts_cpu-0.18.6/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_arity.py` & `polars_lts_cpu-0.18.6/tests/unit/test_arity.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_cfg.py` & `polars_lts_cpu-0.18.6/tests/unit/test_cfg.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_constructors.py` & `polars_lts_cpu-0.18.6/tests/unit/test_constructors.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_cse.py` & `polars_lts_cpu-0.18.6/tests/unit/test_cse.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_datatypes.py` & `polars_lts_cpu-0.18.6/tests/unit/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_df.py` & `polars_lts_cpu-0.18.6/tests/unit/test_df.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_empty.py` & `polars_lts_cpu-0.18.6/tests/unit/test_empty.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_errors.py` & `polars_lts_cpu-0.18.6/tests/unit/test_errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -665,19 +665,7 @@
         {"a": [1, 1, 1], "b": [3, 2, 1], "c": [1, 1, 2]},
         schema={"a": pl.Float32, "b": pl.Float32, "c": pl.Float32},
     )
     with pytest.raises(pl.ComputeError):
         df.lazy().groupby("c").agg(
             [pl.col("a").sort_by(pl.col("b").filter(pl.col("b") > 100)).sum()]
         ).collect()
-
-
-def test_raise_cut_in_over() -> None:
-    with pl.StringCache():
-        x = pl.Series(range(20))
-    r = pl.Series(
-        [pl.repeat("a", 10, eager=True), pl.repeat("b", 10, eager=True)]
-    ).explode()
-    df = pl.DataFrame({"x": x, "g": r})
-
-    with pytest.raises(pl.ComputeError):
-        df.with_columns(pl.col("x").qcut([0.5]).over("g").to_physical())
```

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_expr_multi_cols.py` & `polars_lts_cpu-0.18.6/tests/unit/test_expr_multi_cols.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_exprs.py` & `polars_lts_cpu-0.18.6/tests/unit/test_exprs.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_fmt.py` & `polars_lts_cpu-0.18.6/tests/unit/test_fmt.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_interchange.py` & `polars_lts_cpu-0.18.6/tests/unit/test_interchange.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_interop.py` & `polars_lts_cpu-0.18.6/tests/unit/test_interop.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_lazy.py` & `polars_lts_cpu-0.18.6/tests/unit/test_lazy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_polars_import.py` & `polars_lts_cpu-0.18.6/tests/unit/test_polars_import.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_predicates.py` & `polars_lts_cpu-0.18.6/tests/unit/test_predicates.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_projections.py` & `polars_lts_cpu-0.18.6/tests/unit/test_projections.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_queries.py` & `polars_lts_cpu-0.18.6/tests/unit/test_queries.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_rows.py` & `polars_lts_cpu-0.18.6/tests/unit/test_rows.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_schema.py` & `polars_lts_cpu-0.18.6/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_selectors.py` & `polars_lts_cpu-0.18.6/tests/unit/test_selectors.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_serde.py` & `polars_lts_cpu-0.18.6/tests/unit/test_serde.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_series.py` & `polars_lts_cpu-0.18.6/tests/unit/test_series.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_single.py` & `polars_lts_cpu-0.18.6/tests/unit/test_single.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_sql.py` & `polars_lts_cpu-0.18.6/tests/unit/test_sql.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/test_testing.py` & `polars_lts_cpu-0.18.6/tests/unit/test_testing.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/utils/test_parse_expr_input.py` & `polars_lts_cpu-0.18.6/tests/unit/utils/test_parse_expr_input.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/tests/unit/utils/test_utils.py` & `polars_lts_cpu-0.18.6/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.5/Cargo.lock` & `polars_lts_cpu-0.18.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1714,15 +1714,15 @@
 checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py-polars"
-version = "0.18.5"
+version = "0.18.6"
 dependencies = [
  "ahash",
  "built",
  "ciborium",
  "jemallocator",
  "lexical-core",
  "libc",
```

### Comparing `polars_lts_cpu-0.18.5/PKG-INFO` & `polars_lts_cpu-0.18.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars-lts-cpu
-Version: 0.18.5
+Version: 0.18.6
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: polars-lts-cpu Version: 0.18.5 Classifier:
+Metadata-Version: 2.1 Name: polars-lts-cpu Version: 0.18.6 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

