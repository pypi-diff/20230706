# Comparing `tmp/ReverseBox-0.6.0.tar.gz` & `tmp/ReverseBox-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReverseBox-0.6.0.tar", last modified: Mon May  8 21:55:58 2023, max compression
+gzip compressed data, was "ReverseBox-0.6.1.tar", last modified: Thu Jul  6 21:22:02 2023, max compression
```

## Comparing `ReverseBox-0.6.0.tar` & `ReverseBox-0.6.1.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.180420 ReverseBox-0.6.0/
--rw-rw-rw-   0        0        0    35821 2022-03-18 16:59:47.000000 ReverseBox-0.6.0/LICENSE
--rw-rw-rw-   0        0        0     5768 2023-05-08 21:55:58.180420 ReverseBox-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     4506 2023-05-08 21:41:35.000000 ReverseBox-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.114849 ReverseBox-0.6.0/ReverseBox.egg-info/
--rw-rw-rw-   0        0        0     5768 2023-05-08 21:55:57.000000 ReverseBox-0.6.0/ReverseBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1840 2023-05-08 21:55:58.000000 ReverseBox-0.6.0/ReverseBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 21:55:57.000000 ReverseBox-0.6.0/ReverseBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-08 21:55:58.000000 ReverseBox-0.6.0/ReverseBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-08 21:55:58.000000 ReverseBox-0.6.0/ReverseBox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.115849 ReverseBox-0.6.0/reversebox/
--rw-rw-rw-   0        0        0        0 2022-06-25 12:19:26.000000 ReverseBox-0.6.0/reversebox/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.119850 ReverseBox-0.6.0/reversebox/checksum/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.6.0/reversebox/checksum/__init__.py
--rw-rw-rw-   0        0        0      404 2023-01-08 20:51:07.000000 ReverseBox-0.6.0/reversebox/checksum/checksum_adler32.py
--rw-rw-rw-   0        0        0      403 2023-01-09 21:19:57.000000 ReverseBox-0.6.0/reversebox/checksum/checksum_fletcher16.py
--rw-rw-rw-   0        0        0      510 2023-01-09 22:41:53.000000 ReverseBox-0.6.0/reversebox/checksum/checksum_fletcher32.py
-drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.122851 ReverseBox-0.6.0/reversebox/common/
--rw-rw-rw-   0        0        0        0 2022-06-25 16:29:13.000000 ReverseBox-0.6.0/reversebox/common/__init__.py
--rw-rw-rw-   0        0        0      394 2023-04-15 13:54:42.000000 ReverseBox-0.6.0/reversebox/common/common.py
--rw-rw-rw-   0        0        0      730 2022-09-07 19:55:27.000000 ReverseBox-0.6.0/reversebox/common/logger.py
-drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.127014 ReverseBox-0.6.0/reversebox/compression/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.6.0/reversebox/compression/__init__.py
--rw-rw-rw-   0        0        0      482 2023-04-23 00:00:01.000000 ReverseBox-0.6.0/reversebox/compression/compression_jcalg1.py
--rw-rw-rw-   0        0        0      335 2022-12-27 14:56:59.000000 ReverseBox-0.6.0/reversebox/compression/compression_lzo.py
--rw-rw-rw-   0        0        0      330 2022-10-15 10:41:38.000000 ReverseBox-0.6.0/reversebox/compression/compression_zlib.py
-drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.135205 ReverseBox-0.6.0/reversebox/crc/
--rw-rw-rw-   0        0        0        0 2023-01-09 18:26:29.000000 ReverseBox-0.6.0/reversebox/crc/__init__.py
--rw-rw-rw-   0        0        0     1018 2022-07-17 23:25:19.000000 ReverseBox-0.6.0/reversebox/crc/crc16_arc.py
--rw-rw-rw-   0        0        0     1656 2022-07-24 14:41:31.000000 ReverseBox-0.6.0/reversebox/crc/crc16_ccitt.py
--rw-rw-rw-   0        0        0     1189 2022-07-21 21:16:06.000000 ReverseBox-0.6.0/reversebox/crc/crc16_dnp.py
--rw-rw-rw-   0        0        0     1211 2022-07-17 23:25:19.000000 ReverseBox-0.6.0/reversebox/crc/crc16_kermit.py
--rw-rw-rw-   0        0        0     1103 2022-07-24 15:12:37.000000 ReverseBox-0.6.0/reversebox/crc/crc16_modbus.py
--rw-rw-rw-   0        0        0      735 2022-07-21 21:35:31.000000 ReverseBox-0.6.0/reversebox/crc/crc16_sick.py
--rw-rw-rw-   0        0        0     1008 2022-07-17 23:25:19.000000 ReverseBox-0.6.0/reversebox/crc/crc32_iso_hdlc.py
-drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.140806 ReverseBox-0.6.0/reversebox/encryption/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.6.0/reversebox/encryption/__init__.py
--rw-rw-rw-   0        0        0      579 2022-07-17 23:25:19.000000 ReverseBox-0.6.0/reversebox/encryption/encryption_xor_basic.py
--rw-rw-rw-   0        0        0     1175 2023-04-15 13:23:01.000000 ReverseBox-0.6.0/reversebox/encryption/encryption_xor_gianas_return_zda.py
--rw-rw-rw-   0        0        0      574 2022-07-17 23:25:19.000000 ReverseBox-0.6.0/reversebox/encryption/encryption_xor_retro64_eco.py
-drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.144807 ReverseBox-0.6.0/reversebox/hash/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.6.0/reversebox/hash/__init__.py
--rw-rw-rw-   0        0        0      280 2022-09-11 18:48:36.000000 ReverseBox-0.6.0/reversebox/hash/hash_md5.py
--rw-rw-rw-   0        0        0      283 2023-01-08 14:05:01.000000 ReverseBox-0.6.0/reversebox/hash/hash_sha1.py
--rw-rw-rw-   0        0        0      289 2023-01-08 14:07:31.000000 ReverseBox-0.6.0/reversebox/hash/hash_sha2.py
-drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.148808 ReverseBox-0.6.0/reversebox/image/
--rw-rw-rw-   0        0        0        0 2022-12-27 21:18:24.000000 ReverseBox-0.6.0/reversebox/image/__init__.py
--rw-rw-rw-   0        0        0    13727 2023-01-06 23:05:19.000000 ReverseBox-0.6.0/reversebox/image/image_finder_gui.py
--rw-rw-rw-   0        0        0      713 2023-04-23 00:00:01.000000 ReverseBox-0.6.0/reversebox/image/image_finder_main.py
--rw-rw-rw-   0        0        0     1507 2023-04-15 13:20:43.000000 ReverseBox-0.6.0/reversebox/image/psp_swizzle.py
-drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.162812 ReverseBox-0.6.0/reversebox/io_files/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.6.0/reversebox/io_files/__init__.py
--rw-rw-rw-   0        0        0      931 2023-04-23 15:32:28.000000 ReverseBox-0.6.0/reversebox/io_files/bytes_handler.py
--rw-rw-rw-   0        0        0     1026 2023-04-22 01:54:49.000000 ReverseBox-0.6.0/reversebox/io_files/check_file.py
--rw-rw-rw-   0        0        0     8126 2023-04-23 18:16:41.000000 ReverseBox-0.6.0/reversebox/io_files/file_handler.py
--rw-rw-rw-   0        0        0     5195 2023-05-08 21:42:14.000000 ReverseBox-0.6.0/reversebox/io_files/mod_handler.py
--rw-rw-rw-   0        0        0    11372 2023-05-08 21:44:23.000000 ReverseBox-0.6.0/reversebox/io_files/translation_text_handler.py
--rw-rw-rw-   0        0        0       42 2023-05-08 21:55:58.180420 ReverseBox-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1825 2023-05-08 21:39:10.000000 ReverseBox-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.164811 ReverseBox-0.6.0/tests/
--rw-rw-rw-   0        0        0        0 2022-07-19 22:27:10.000000 ReverseBox-0.6.0/tests/__init__.py
--rw-rw-rw-   0        0        0      626 2023-04-12 20:56:38.000000 ReverseBox-0.6.0/tests/common.py
-drwxrwxrwx   0        0        0        0 2023-05-08 21:55:58.180420 ReverseBox-0.6.0/tests/tests_crc/
--rw-rw-rw-   0        0        0        0 2023-01-09 18:28:33.000000 ReverseBox-0.6.0/tests/tests_crc/__init__.py
--rw-rw-rw-   0        0        0     2301 2023-01-09 18:34:08.000000 ReverseBox-0.6.0/tests/tests_crc/test_crc16_arc.py
--rw-rw-rw-   0        0        0     4539 2023-01-09 18:34:08.000000 ReverseBox-0.6.0/tests/tests_crc/test_crc16_ccitt.py
--rw-rw-rw-   0        0        0     1633 2023-01-09 18:34:08.000000 ReverseBox-0.6.0/tests/tests_crc/test_crc16_dnp.py
--rw-rw-rw-   0        0        0     1651 2023-01-09 18:34:08.000000 ReverseBox-0.6.0/tests/tests_crc/test_crc16_kermit.py
--rw-rw-rw-   0        0        0     1660 2023-01-09 18:34:08.000000 ReverseBox-0.6.0/tests/tests_crc/test_crc16_modbus.py
--rw-rw-rw-   0        0        0     1632 2023-01-09 18:34:08.000000 ReverseBox-0.6.0/tests/tests_crc/test_crc16_sick.py
--rw-rw-rw-   0        0        0     2655 2023-04-23 00:00:01.000000 ReverseBox-0.6.0/tests/tests_crc/test_crc32_iso_hdlc.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:22:02.549997 ReverseBox-0.6.1/
+-rw-rw-rw-   0        0        0    35821 2022-03-18 16:59:47.000000 ReverseBox-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0     5787 2023-07-06 21:22:02.549997 ReverseBox-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4525 2023-07-06 21:19:41.000000 ReverseBox-0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 21:22:02.492323 ReverseBox-0.6.1/ReverseBox.egg-info/
+-rw-rw-rw-   0        0        0     5787 2023-07-06 21:22:02.000000 ReverseBox-0.6.1/ReverseBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1878 2023-07-06 21:22:02.000000 ReverseBox-0.6.1/ReverseBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 21:22:02.000000 ReverseBox-0.6.1/ReverseBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-06 21:22:02.000000 ReverseBox-0.6.1/ReverseBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-06 21:22:02.000000 ReverseBox-0.6.1/ReverseBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 21:22:02.493324 ReverseBox-0.6.1/reversebox/
+-rw-rw-rw-   0        0        0        0 2022-06-25 12:19:26.000000 ReverseBox-0.6.1/reversebox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:22:02.498634 ReverseBox-0.6.1/reversebox/checksum/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.6.1/reversebox/checksum/__init__.py
+-rw-rw-rw-   0        0        0      404 2023-01-08 20:51:07.000000 ReverseBox-0.6.1/reversebox/checksum/checksum_adler32.py
+-rw-rw-rw-   0        0        0      404 2023-07-06 21:19:50.000000 ReverseBox-0.6.1/reversebox/checksum/checksum_bsd16.py
+-rw-rw-rw-   0        0        0      403 2023-01-09 21:19:57.000000 ReverseBox-0.6.1/reversebox/checksum/checksum_fletcher16.py
+-rw-rw-rw-   0        0        0      510 2023-01-09 22:41:53.000000 ReverseBox-0.6.1/reversebox/checksum/checksum_fletcher32.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:22:02.501692 ReverseBox-0.6.1/reversebox/common/
+-rw-rw-rw-   0        0        0        0 2022-06-25 16:29:13.000000 ReverseBox-0.6.1/reversebox/common/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-07-05 21:46:47.000000 ReverseBox-0.6.1/reversebox/common/common.py
+-rw-rw-rw-   0        0        0      730 2022-09-07 19:55:27.000000 ReverseBox-0.6.1/reversebox/common/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:22:02.505693 ReverseBox-0.6.1/reversebox/compression/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.6.1/reversebox/compression/__init__.py
+-rw-rw-rw-   0        0        0      482 2023-04-23 00:00:01.000000 ReverseBox-0.6.1/reversebox/compression/compression_jcalg1.py
+-rw-rw-rw-   0        0        0      335 2022-12-27 14:56:59.000000 ReverseBox-0.6.1/reversebox/compression/compression_lzo.py
+-rw-rw-rw-   0        0        0      330 2022-10-15 10:41:38.000000 ReverseBox-0.6.1/reversebox/compression/compression_zlib.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:22:02.514755 ReverseBox-0.6.1/reversebox/crc/
+-rw-rw-rw-   0        0        0        0 2023-01-09 18:26:29.000000 ReverseBox-0.6.1/reversebox/crc/__init__.py
+-rw-rw-rw-   0        0        0     1018 2022-07-17 23:25:19.000000 ReverseBox-0.6.1/reversebox/crc/crc16_arc.py
+-rw-rw-rw-   0        0        0     1656 2022-07-24 14:41:31.000000 ReverseBox-0.6.1/reversebox/crc/crc16_ccitt.py
+-rw-rw-rw-   0        0        0     1189 2022-07-21 21:16:06.000000 ReverseBox-0.6.1/reversebox/crc/crc16_dnp.py
+-rw-rw-rw-   0        0        0     1211 2022-07-17 23:25:19.000000 ReverseBox-0.6.1/reversebox/crc/crc16_kermit.py
+-rw-rw-rw-   0        0        0     1103 2022-07-24 15:12:37.000000 ReverseBox-0.6.1/reversebox/crc/crc16_modbus.py
+-rw-rw-rw-   0        0        0      735 2022-07-21 21:35:31.000000 ReverseBox-0.6.1/reversebox/crc/crc16_sick.py
+-rw-rw-rw-   0        0        0     1008 2022-07-17 23:25:19.000000 ReverseBox-0.6.1/reversebox/crc/crc32_iso_hdlc.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:22:02.520757 ReverseBox-0.6.1/reversebox/encryption/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.6.1/reversebox/encryption/__init__.py
+-rw-rw-rw-   0        0        0      579 2022-07-17 23:25:19.000000 ReverseBox-0.6.1/reversebox/encryption/encryption_xor_basic.py
+-rw-rw-rw-   0        0        0     1175 2023-04-15 13:23:01.000000 ReverseBox-0.6.1/reversebox/encryption/encryption_xor_gianas_return_zda.py
+-rw-rw-rw-   0        0        0      574 2022-07-17 23:25:19.000000 ReverseBox-0.6.1/reversebox/encryption/encryption_xor_retro64_eco.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:22:02.524841 ReverseBox-0.6.1/reversebox/hash/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.6.1/reversebox/hash/__init__.py
+-rw-rw-rw-   0        0        0      280 2022-09-11 18:48:36.000000 ReverseBox-0.6.1/reversebox/hash/hash_md5.py
+-rw-rw-rw-   0        0        0      283 2023-01-08 14:05:01.000000 ReverseBox-0.6.1/reversebox/hash/hash_sha1.py
+-rw-rw-rw-   0        0        0      289 2023-01-08 14:07:31.000000 ReverseBox-0.6.1/reversebox/hash/hash_sha2.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:22:02.528842 ReverseBox-0.6.1/reversebox/image/
+-rw-rw-rw-   0        0        0        0 2022-12-27 21:18:24.000000 ReverseBox-0.6.1/reversebox/image/__init__.py
+-rw-rw-rw-   0        0        0    13727 2023-01-06 23:05:19.000000 ReverseBox-0.6.1/reversebox/image/image_finder_gui.py
+-rw-rw-rw-   0        0        0      713 2023-04-23 00:00:01.000000 ReverseBox-0.6.1/reversebox/image/image_finder_main.py
+-rw-rw-rw-   0        0        0     1507 2023-04-15 13:20:43.000000 ReverseBox-0.6.1/reversebox/image/psp_swizzle.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:22:02.536913 ReverseBox-0.6.1/reversebox/io_files/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:13.000000 ReverseBox-0.6.1/reversebox/io_files/__init__.py
+-rw-rw-rw-   0        0        0      931 2023-04-23 15:32:28.000000 ReverseBox-0.6.1/reversebox/io_files/bytes_handler.py
+-rw-rw-rw-   0        0        0     1026 2023-04-22 01:54:49.000000 ReverseBox-0.6.1/reversebox/io_files/check_file.py
+-rw-rw-rw-   0        0        0     8126 2023-04-23 18:16:41.000000 ReverseBox-0.6.1/reversebox/io_files/file_handler.py
+-rw-rw-rw-   0        0        0     5195 2023-05-08 21:42:14.000000 ReverseBox-0.6.1/reversebox/io_files/mod_handler.py
+-rw-rw-rw-   0        0        0    11372 2023-05-08 21:44:23.000000 ReverseBox-0.6.1/reversebox/io_files/translation_text_handler.py
+-rw-rw-rw-   0        0        0       42 2023-07-06 21:22:02.549997 ReverseBox-0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1825 2023-07-06 21:19:41.000000 ReverseBox-0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:22:02.538914 ReverseBox-0.6.1/tests/
+-rw-rw-rw-   0        0        0        0 2022-07-19 22:27:10.000000 ReverseBox-0.6.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-04-12 20:56:38.000000 ReverseBox-0.6.1/tests/common.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:22:02.547998 ReverseBox-0.6.1/tests/tests_crc/
+-rw-rw-rw-   0        0        0        0 2023-01-09 18:28:33.000000 ReverseBox-0.6.1/tests/tests_crc/__init__.py
+-rw-rw-rw-   0        0        0     2301 2023-01-09 18:34:08.000000 ReverseBox-0.6.1/tests/tests_crc/test_crc16_arc.py
+-rw-rw-rw-   0        0        0     4539 2023-01-09 18:34:08.000000 ReverseBox-0.6.1/tests/tests_crc/test_crc16_ccitt.py
+-rw-rw-rw-   0        0        0     1633 2023-01-09 18:34:08.000000 ReverseBox-0.6.1/tests/tests_crc/test_crc16_dnp.py
+-rw-rw-rw-   0        0        0     1651 2023-01-09 18:34:08.000000 ReverseBox-0.6.1/tests/tests_crc/test_crc16_kermit.py
+-rw-rw-rw-   0        0        0     1660 2023-01-09 18:34:08.000000 ReverseBox-0.6.1/tests/tests_crc/test_crc16_modbus.py
+-rw-rw-rw-   0        0        0     1632 2023-01-09 18:34:08.000000 ReverseBox-0.6.1/tests/tests_crc/test_crc16_sick.py
+-rw-rw-rw-   0        0        0     2655 2023-04-23 00:00:01.000000 ReverseBox-0.6.1/tests/tests_crc/test_crc32_iso_hdlc.py
```

### Comparing `ReverseBox-0.6.0/LICENSE` & `ReverseBox-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/PKG-INFO` & `ReverseBox-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseBox
-Version: 0.6.0
+Version: 0.6.1
 Summary: A set of functions useful in reverse engineering.
 Home-page: https://github.com/bartlomiejduda/ReverseBox
 Author: Bartlomiej Duda
 Author-email: ikskoks@gmail.com
 Keywords: ReverseBox,reverse engineering,RE,CRC,Hash,Encryption,Compression,Checksum,Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -48,14 +48,15 @@
 Mostly developers and reverse engineers (e.g. file format researchers
 or software researchers).
 
 # List of functionalities
 
 * Checksum
   - Adler-32 ✔️
+  - BSD-16 ✔️
   - Fletcher-16 ✔️
   - Fletcher-32 ✔️
 
 * CRC
   - CRC-8 (TODO) ❌
   - CRC-16 (ARC) ✔️
   - CRC-16 (Modbus) ✔️
```

### Comparing `ReverseBox-0.6.0/README.md` & `ReverseBox-0.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 Mostly developers and reverse engineers (e.g. file format researchers
 or software researchers).
 
 # List of functionalities
 
 * Checksum
   - Adler-32 ✔️
+  - BSD-16 ✔️
   - Fletcher-16 ✔️
   - Fletcher-32 ✔️
 
 * CRC
   - CRC-8 (TODO) ❌
   - CRC-16 (ARC) ✔️
   - CRC-16 (Modbus) ✔️
```

### Comparing `ReverseBox-0.6.0/ReverseBox.egg-info/PKG-INFO` & `ReverseBox-0.6.1/ReverseBox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseBox
-Version: 0.6.0
+Version: 0.6.1
 Summary: A set of functions useful in reverse engineering.
 Home-page: https://github.com/bartlomiejduda/ReverseBox
 Author: Bartlomiej Duda
 Author-email: ikskoks@gmail.com
 Keywords: ReverseBox,reverse engineering,RE,CRC,Hash,Encryption,Compression,Checksum,Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -48,14 +48,15 @@
 Mostly developers and reverse engineers (e.g. file format researchers
 or software researchers).
 
 # List of functionalities
 
 * Checksum
   - Adler-32 ✔️
+  - BSD-16 ✔️
   - Fletcher-16 ✔️
   - Fletcher-32 ✔️
 
 * CRC
   - CRC-8 (TODO) ❌
   - CRC-16 (ARC) ✔️
   - CRC-16 (Modbus) ✔️
```

### Comparing `ReverseBox-0.6.0/ReverseBox.egg-info/SOURCES.txt` & `ReverseBox-0.6.1/ReverseBox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 ReverseBox.egg-info/SOURCES.txt
 ReverseBox.egg-info/dependency_links.txt
 ReverseBox.egg-info/requires.txt
 ReverseBox.egg-info/top_level.txt
 reversebox/__init__.py
 reversebox/checksum/__init__.py
 reversebox/checksum/checksum_adler32.py
+reversebox/checksum/checksum_bsd16.py
 reversebox/checksum/checksum_fletcher16.py
 reversebox/checksum/checksum_fletcher32.py
 reversebox/common/__init__.py
 reversebox/common/common.py
 reversebox/common/logger.py
 reversebox/compression/__init__.py
 reversebox/compression/compression_jcalg1.py
```

### Comparing `ReverseBox-0.6.0/reversebox/common/logger.py` & `ReverseBox-0.6.1/reversebox/common/logger.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/reversebox/crc/crc16_arc.py` & `ReverseBox-0.6.1/reversebox/crc/crc16_arc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/reversebox/crc/crc16_ccitt.py` & `ReverseBox-0.6.1/reversebox/crc/crc16_ccitt.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/reversebox/crc/crc16_dnp.py` & `ReverseBox-0.6.1/reversebox/crc/crc16_dnp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/reversebox/crc/crc16_kermit.py` & `ReverseBox-0.6.1/reversebox/crc/crc16_kermit.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/reversebox/crc/crc16_modbus.py` & `ReverseBox-0.6.1/reversebox/crc/crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/reversebox/crc/crc16_sick.py` & `ReverseBox-0.6.1/reversebox/crc/crc16_sick.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/reversebox/crc/crc32_iso_hdlc.py` & `ReverseBox-0.6.1/reversebox/crc/crc32_iso_hdlc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/reversebox/encryption/encryption_xor_basic.py` & `ReverseBox-0.6.1/reversebox/encryption/encryption_xor_basic.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/reversebox/encryption/encryption_xor_gianas_return_zda.py` & `ReverseBox-0.6.1/reversebox/encryption/encryption_xor_gianas_return_zda.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/reversebox/encryption/encryption_xor_retro64_eco.py` & `ReverseBox-0.6.1/reversebox/encryption/encryption_xor_retro64_eco.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/reversebox/image/image_finder_gui.py` & `ReverseBox-0.6.1/reversebox/image/image_finder_gui.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/reversebox/image/image_finder_main.py` & `ReverseBox-0.6.1/reversebox/image/image_finder_main.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/reversebox/image/psp_swizzle.py` & `ReverseBox-0.6.1/reversebox/image/psp_swizzle.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/reversebox/io_files/bytes_handler.py` & `ReverseBox-0.6.1/reversebox/io_files/bytes_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/reversebox/io_files/check_file.py` & `ReverseBox-0.6.1/reversebox/io_files/check_file.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/reversebox/io_files/file_handler.py` & `ReverseBox-0.6.1/reversebox/io_files/file_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/reversebox/io_files/mod_handler.py` & `ReverseBox-0.6.1/reversebox/io_files/mod_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/reversebox/io_files/translation_text_handler.py` & `ReverseBox-0.6.1/reversebox/io_files/translation_text_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/setup.py` & `ReverseBox-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 License: GPL-3.0 License
 """
 
 import os
 
 import setuptools
 
-VERSION_NUM = "0.6.0"
+VERSION_NUM = "0.6.1"
 
 
 def get_long_description() -> str:
     with open(
         os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf8"
     ) as readme:
         readme_text = readme.read()
```

### Comparing `ReverseBox-0.6.0/tests/common.py` & `ReverseBox-0.6.1/tests/common.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/tests/tests_crc/test_crc16_arc.py` & `ReverseBox-0.6.1/tests/tests_crc/test_crc16_arc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/tests/tests_crc/test_crc16_ccitt.py` & `ReverseBox-0.6.1/tests/tests_crc/test_crc16_ccitt.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/tests/tests_crc/test_crc16_dnp.py` & `ReverseBox-0.6.1/tests/tests_crc/test_crc16_dnp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/tests/tests_crc/test_crc16_kermit.py` & `ReverseBox-0.6.1/tests/tests_crc/test_crc16_kermit.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/tests/tests_crc/test_crc16_modbus.py` & `ReverseBox-0.6.1/tests/tests_crc/test_crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/tests/tests_crc/test_crc16_sick.py` & `ReverseBox-0.6.1/tests/tests_crc/test_crc16_sick.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.6.0/tests/tests_crc/test_crc32_iso_hdlc.py` & `ReverseBox-0.6.1/tests/tests_crc/test_crc32_iso_hdlc.py`

 * *Files identical despite different names*

