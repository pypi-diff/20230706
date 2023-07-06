# Comparing `tmp/pysipfenn-0.12.1.tar.gz` & `tmp/pysipfenn-0.12.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysipfenn-0.12.1.tar", last modified: Sun Jun 25 16:55:46 2023, max compression
+gzip compressed data, was "pysipfenn-0.12.2.tar", last modified: Thu Jul  6 18:32:29 2023, max compression
```

## Comparing `pysipfenn-0.12.1.tar` & `pysipfenn-0.12.2.tar`

### file list

```diff
@@ -1,97 +1,90 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.027309 pysipfenn-0.12.1/
--rw-r--r--   0 adam       (501) staff       (20)      104 2023-03-17 23:08:06.000000 pysipfenn-0.12.1/.gitattributes
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.008392 pysipfenn-0.12.1/.github/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.011235 pysipfenn-0.12.1/.github/workflows/
--rw-r--r--   0 adam       (501) staff       (20)     1327 2023-04-06 22:05:43.000000 pysipfenn-0.12.1/.github/workflows/benchmarks.yml
--rw-r--r--   0 adam       (501) staff       (20)     2667 2023-04-06 15:18:55.000000 pysipfenn-0.12.1/.github/workflows/fullTest.yml
--rw-r--r--   0 adam       (501) staff       (20)      885 2023-04-06 15:18:55.000000 pysipfenn-0.12.1/.github/workflows/partialTest.yml
--rwx------   0 adam       (501) staff       (20)      408 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/.readthedocs.yaml
--rwx------   0 adam       (501) staff       (20)    35149 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/LICENSE
--rwx------   0 adam       (501) staff       (20)      309 2023-06-25 16:55:13.000000 pysipfenn-0.12.1/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)     8456 2023-06-25 16:55:46.027138 pysipfenn-0.12.1/PKG-INFO
--rwx------   0 adam       (501) staff       (20)     7231 2023-04-06 16:22:26.000000 pysipfenn-0.12.1/README.md
--rwx------   0 adam       (501) staff       (20)     1522 2023-06-25 16:52:20.000000 pysipfenn-0.12.1/pyproject.toml
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.011515 pysipfenn-0.12.1/pysipfenn/
--rwx------   0 adam       (501) staff       (20)       38 2023-04-05 20:03:47.000000 pysipfenn-0.12.1/pysipfenn/__init__.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.012436 pysipfenn-0.12.1/pysipfenn/core/
--rwx------   0 adam       (501) staff       (20)        0 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/core/__init__.py
--rw-r--r--   0 adam       (501) staff       (20)    39207 2023-06-25 16:52:20.000000 pysipfenn-0.12.1/pysipfenn/core/pysipfenn.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.016272 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/
--rwx------   0 adam       (501) staff       (20)    28375 2023-04-06 16:33:34.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/KS2022.py
--rw-r--r--   0 adam       (501) staff       (20)     2036 2023-04-06 16:33:38.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/KS2022_TestResult.csv
--rwx------   0 adam       (501) staff       (20)    23904 2023-04-06 16:39:11.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/KS2022_dilute.py
--rw-r--r--   0 adam       (501) staff       (20)     2035 2023-04-06 16:39:13.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/KS2022_dilute_TestResult.csv
--rwx------   0 adam       (501) staff       (20)   141363 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/Magpie_element_properties.csv
--rwx------   0 adam       (501) staff       (20)      702 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/Magpie_property_names.txt
--rwx------   0 adam       (501) staff       (20)      151 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/README.md
--rw-r--r--   0 adam       (501) staff       (20)    33100 2023-04-06 16:33:34.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/Ward2017.py
--rwx------   0 adam       (501) staff       (20)        0 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/__init__.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.017272 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/__pycache__/
--rw-------   0 adam       (501) staff       (20)    18404 2023-04-06 21:56:10.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/__pycache__/KS2022.cpython-39.pyc
--rw-------   0 adam       (501) staff       (20)    15449 2023-04-06 21:56:10.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/__pycache__/KS2022_dilute.cpython-39.pyc
--rw-r--r--   0 adam       (501) staff       (20)    20791 2023-04-06 21:56:09.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/__pycache__/Ward2017.cpython-39.pyc
--rw-------   0 adam       (501) staff       (20)      172 2023-02-27 19:53:51.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/__pycache__/__init__.cpython-39.pyc
--rwx------   0 adam       (501) staff       (20)     5796 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/labels_KS2022.csv
--rwx------   0 adam       (501) staff       (20)     5796 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/labels_KS2022_dilute.csv
--rwx------   0 adam       (501) staff       (20)     6206 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/labels_Ward2017.csv
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.017757 pysipfenn-0.12.1/pysipfenn/modelsSIPFENN/
--rwx------   0 adam       (501) staff       (20)       86 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/modelsSIPFENN/README.md
--rwx------   0 adam       (501) staff       (20)        0 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/modelsSIPFENN/__init__.py
--rwx------   0 adam       (501) staff       (20)     1420 2023-02-28 15:23:16.000000 pysipfenn-0.12.1/pysipfenn/modelsSIPFENN/models.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.019647 pysipfenn-0.12.1/pysipfenn/tests/
--rwx------   0 adam       (501) staff       (20)        0 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/__init__.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.020479 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/
--rw-r--r--   0 adam       (501) staff       (20)    13122 2023-04-05 21:14:25.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_enumerated.csv
--rw-r--r--   0 adam       (501) staff       (20)    18296 2023-04-05 21:14:25.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_named.csv
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.026126 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/
--rwx------   0 adam       (501) staff       (20)     1021 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/0-Cr8Fe18Ni4.POSCAR
--rwx------   0 adam       (501) staff       (20)     1021 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/1-Cr16Fe8Ni6.POSCAR
--rwx------   0 adam       (501) staff       (20)      916 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/10-Ce4Ti4O12.POSCAR
--rwx------   0 adam       (501) staff       (20)     1014 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/11-Fe10Ni20.POSCAR
--rwx------   0 adam       (501) staff       (20)      916 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/12-Gd4Cr4O12.POSCAR
--rwx------   0 adam       (501) staff       (20)     1016 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/13-Fe16Ni14.POSCAR
--rwx------   0 adam       (501) staff       (20)     1014 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/14-Fe24Ni6.POSCAR
--rwx------   0 adam       (501) staff       (20)      916 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/15-Ta4Tl4O12.POSCAR
--rwx------   0 adam       (501) staff       (20)     1016 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/16-Fe18Ni12.POSCAR
--rwx------   0 adam       (501) staff       (20)      916 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/17-Pr4Ga4O12.POSCAR
--rwx------   0 adam       (501) staff       (20)     1015 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/18-Fe28Ni2.POSCAR
--rwx------   0 adam       (501) staff       (20)     1016 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/19-Fe4Ni26.POSCAR
--rwx------   0 adam       (501) staff       (20)     1012 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/2-Fe8Ni22.POSCAR
--rwx------   0 adam       (501) staff       (20)     1012 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/20-Fe8Ni22.POSCAR
--rwx------   0 adam       (501) staff       (20)     1014 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/21-Fe10Ni20.POSCAR
--rwx------   0 adam       (501) staff       (20)     1018 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/22-Fe10Ni20.POSCAR
--rwx------   0 adam       (501) staff       (20)     1018 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/23-Fe12Ni18.POSCAR
--rwx------   0 adam       (501) staff       (20)     1016 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/24-Fe16Ni14.POSCAR
--rwx------   0 adam       (501) staff       (20)     1020 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/25-Fe12Ni18.POSCAR
--rwx------   0 adam       (501) staff       (20)     1014 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/26-Fe8Ni22.POSCAR
--rwx------   0 adam       (501) staff       (20)     1012 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/27-Cr28Fe2.POSCAR
--rwx------   0 adam       (501) staff       (20)     1018 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/28-Fe26Ni4.POSCAR
--rwx------   0 adam       (501) staff       (20)     1019 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/29-Fe12Ni18.POSCAR
--rwx------   0 adam       (501) staff       (20)     1018 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/3-Cr18Fe12.POSCAR
--rwx------   0 adam       (501) staff       (20)     1012 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/30-Cr26Fe4.POSCAR
--rwx------   0 adam       (501) staff       (20)     1923 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/31-Li24Al4Ni32.POSCAR
--rwx------   0 adam       (501) staff       (20)     1003 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/4-Fe30.POSCAR
--rwx------   0 adam       (501) staff       (20)     1014 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/5-Cr22Fe8.POSCAR
--rwx------   0 adam       (501) staff       (20)     1014 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/6-Fe2Ni28.POSCAR
--rwx------   0 adam       (501) staff       (20)     1016 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/7-Cr18Fe12.POSCAR
--rwx------   0 adam       (501) staff       (20)     1023 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/8-Cr2Fe16Ni12.POSCAR
--rwx------   0 adam       (501) staff       (20)      908 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/9-Pb8O12.POSCAR
--rwx------   0 adam       (501) staff       (20)    68010 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFilesDescriptorTable.csv
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.026766 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/
--rwx------   0 adam       (501) staff       (20)    15121 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/1-Zr220Cu280.POSCAR
--rwx------   0 adam       (501) staff       (20)    15121 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/2-Zr220Cu280.POSCAR
--rwx------   0 adam       (501) staff       (20)    15121 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/3-Zr220Cu280.POSCAR
--rwx------   0 adam       (501) staff       (20)      743 2023-03-31 18:23:39.000000 pysipfenn-0.12.1/pysipfenn/tests/test_AllCompatibleONNX_Ward2017.py
--rwx------   0 adam       (501) staff       (20)     3152 2023-04-06 22:01:56.000000 pysipfenn-0.12.1/pysipfenn/tests/test_KS2022.py
--rwx------   0 adam       (501) staff       (20)    21509 2023-04-06 22:01:56.000000 pysipfenn-0.12.1/pysipfenn/tests/test_KS2022_dilute.py
--rwx------   0 adam       (501) staff       (20)     1578 2023-03-31 18:23:39.000000 pysipfenn-0.12.1/pysipfenn/tests/test_Krajewski2020_NN9NN20NN24_ONNX.py
--rwx------   0 adam       (501) staff       (20)     2338 2023-04-06 22:01:56.000000 pysipfenn-0.12.1/pysipfenn/tests/test_Ward2017.py
--rw-r--r--   0 adam       (501) staff       (20)     2221 2023-03-31 18:23:39.000000 pysipfenn-0.12.1/pysipfenn/tests/test_customModel.py
--rwx------   0 adam       (501) staff       (20)    12132 2023-04-05 21:17:25.000000 pysipfenn-0.12.1/pysipfenn/tests/test_pysipfenn.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.012214 pysipfenn-0.12.1/pysipfenn.egg-info/
--rwx------   0 adam       (501) staff       (20)     8456 2023-06-25 16:55:45.000000 pysipfenn-0.12.1/pysipfenn.egg-info/PKG-INFO
--rwx------   0 adam       (501) staff       (20)     4311 2023-06-25 16:55:46.000000 pysipfenn-0.12.1/pysipfenn.egg-info/SOURCES.txt
--rwx------   0 adam       (501) staff       (20)        1 2023-06-25 16:55:45.000000 pysipfenn-0.12.1/pysipfenn.egg-info/dependency_links.txt
--rwx------   0 adam       (501) staff       (20)      147 2023-06-25 16:55:45.000000 pysipfenn-0.12.1/pysipfenn.egg-info/requires.txt
--rwx------   0 adam       (501) staff       (20)       10 2023-06-25 16:55:45.000000 pysipfenn-0.12.1/pysipfenn.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)       38 2023-06-25 16:55:46.027357 pysipfenn-0.12.1/setup.cfg
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-06 18:32:29.509366 pysipfenn-0.12.2/
+-rw-r--r--   0 adam       (501) staff       (20)      104 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/.gitattributes
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-06 18:32:29.495835 pysipfenn-0.12.2/.github/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-06 18:32:29.498249 pysipfenn-0.12.2/.github/workflows/
+-rw-r--r--   0 adam       (501) staff       (20)     1327 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/.github/workflows/benchmarks.yml
+-rw-r--r--   0 adam       (501) staff       (20)     2667 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/.github/workflows/fullTest.yml
+-rw-r--r--   0 adam       (501) staff       (20)      885 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/.github/workflows/partialTest.yml
+-rw-r--r--   0 adam       (501) staff       (20)     1721 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/.github/workflows/weeklyTesting.yml
+-rw-r--r--   0 adam       (501) staff       (20)      408 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/.readthedocs.yaml
+-rw-r--r--   0 adam       (501) staff       (20)     7805 2023-07-06 18:11:32.000000 pysipfenn-0.12.2/LICENSE.md
+-rw-r--r--   0 adam       (501) staff       (20)      231 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/MANIFEST.in
+-rw-r--r--   0 adam       (501) staff       (20)     8905 2023-07-06 18:32:29.509204 pysipfenn-0.12.2/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     7659 2023-07-06 18:22:50.000000 pysipfenn-0.12.2/README.md
+-rw-r--r--   0 adam       (501) staff       (20)     1540 2023-07-06 18:32:04.000000 pysipfenn-0.12.2/pyproject.toml
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-06 18:32:29.498400 pysipfenn-0.12.2/pysipfenn/
+-rw-r--r--   0 adam       (501) staff       (20)       38 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/__init__.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-06 18:32:29.499425 pysipfenn-0.12.2/pysipfenn/core/
+-rw-r--r--   0 adam       (501) staff       (20)        0 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/core/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)    39186 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/core/pysipfenn.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-06 18:32:29.501592 pysipfenn-0.12.2/pysipfenn/descriptorDefinitions/
+-rw-r--r--   0 adam       (501) staff       (20)    28375 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/descriptorDefinitions/KS2022.py
+-rw-r--r--   0 adam       (501) staff       (20)    23904 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/descriptorDefinitions/KS2022_dilute.py
+-rw-r--r--   0 adam       (501) staff       (20)   141363 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/descriptorDefinitions/Magpie_element_properties.csv
+-rw-r--r--   0 adam       (501) staff       (20)      702 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/descriptorDefinitions/Magpie_property_names.txt
+-rw-r--r--   0 adam       (501) staff       (20)      151 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/descriptorDefinitions/README.md
+-rw-r--r--   0 adam       (501) staff       (20)    33100 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/descriptorDefinitions/Ward2017.py
+-rw-r--r--   0 adam       (501) staff       (20)        0 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/descriptorDefinitions/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     5796 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/descriptorDefinitions/labels_KS2022.csv
+-rw-r--r--   0 adam       (501) staff       (20)     5796 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/descriptorDefinitions/labels_KS2022_dilute.csv
+-rw-r--r--   0 adam       (501) staff       (20)     6206 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/descriptorDefinitions/labels_Ward2017.csv
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-06 18:32:29.501972 pysipfenn-0.12.2/pysipfenn/modelsSIPFENN/
+-rw-r--r--   0 adam       (501) staff       (20)       86 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/modelsSIPFENN/README.md
+-rw-r--r--   0 adam       (501) staff       (20)        0 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/modelsSIPFENN/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)     1420 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/modelsSIPFENN/models.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-06 18:32:29.503644 pysipfenn-0.12.2/pysipfenn/tests/
+-rw-r--r--   0 adam       (501) staff       (20)        0 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/__init__.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-06 18:32:29.504307 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/
+-rw-r--r--   0 adam       (501) staff       (20)    13122 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_enumerated.csv
+-rw-r--r--   0 adam       (501) staff       (20)    18296 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_named.csv
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-06 18:32:29.508516 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/
+-rw-r--r--   0 adam       (501) staff       (20)     1021 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/0-Cr8Fe18Ni4.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1021 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/1-Cr16Fe8Ni6.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)      916 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/10-Ce4Ti4O12.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1014 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/11-Fe10Ni20.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)      916 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/12-Gd4Cr4O12.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1016 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/13-Fe16Ni14.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1014 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/14-Fe24Ni6.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)      916 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/15-Ta4Tl4O12.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1016 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/16-Fe18Ni12.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)      916 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/17-Pr4Ga4O12.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1015 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/18-Fe28Ni2.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1016 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/19-Fe4Ni26.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1012 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/2-Fe8Ni22.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1012 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/20-Fe8Ni22.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1014 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/21-Fe10Ni20.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1018 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/22-Fe10Ni20.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1018 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/23-Fe12Ni18.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1016 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/24-Fe16Ni14.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1020 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/25-Fe12Ni18.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1014 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/26-Fe8Ni22.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1012 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/27-Cr28Fe2.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1018 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/28-Fe26Ni4.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1019 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/29-Fe12Ni18.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1018 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/3-Cr18Fe12.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1012 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/30-Cr26Fe4.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1003 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/4-Fe30.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1014 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/5-Cr22Fe8.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1014 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/6-Fe2Ni28.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1016 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/7-Cr18Fe12.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)     1023 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/8-Cr2Fe16Ni12.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)      908 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/9-Pb8O12.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)    68010 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFilesDescriptorTable.csv
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-06 18:32:29.508942 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/
+-rw-r--r--   0 adam       (501) staff       (20)    15121 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/1-Zr220Cu280.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)    15121 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/2-Zr220Cu280.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)    15121 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/3-Zr220Cu280.POSCAR
+-rw-r--r--   0 adam       (501) staff       (20)      743 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/test_AllCompatibleONNX_Ward2017.py
+-rw-r--r--   0 adam       (501) staff       (20)     3152 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/test_KS2022.py
+-rw-r--r--   0 adam       (501) staff       (20)    21509 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/test_KS2022_dilute.py
+-rw-r--r--   0 adam       (501) staff       (20)     1578 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/test_Krajewski2020_NN9NN20NN24_ONNX.py
+-rw-r--r--   0 adam       (501) staff       (20)     2338 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/test_Ward2017.py
+-rw-r--r--   0 adam       (501) staff       (20)     2221 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/test_customModel.py
+-rw-r--r--   0 adam       (501) staff       (20)    12132 2023-07-06 18:04:50.000000 pysipfenn-0.12.2/pysipfenn/tests/test_pysipfenn.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-07-06 18:32:29.499189 pysipfenn-0.12.2/pysipfenn.egg-info/
+-rw-r--r--   0 adam       (501) staff       (20)     8905 2023-07-06 18:32:29.000000 pysipfenn-0.12.2/pysipfenn.egg-info/PKG-INFO
+-rw-r--r--   0 adam       (501) staff       (20)     3890 2023-07-06 18:32:29.000000 pysipfenn-0.12.2/pysipfenn.egg-info/SOURCES.txt
+-rw-r--r--   0 adam       (501) staff       (20)        1 2023-07-06 18:32:29.000000 pysipfenn-0.12.2/pysipfenn.egg-info/dependency_links.txt
+-rw-r--r--   0 adam       (501) staff       (20)      147 2023-07-06 18:32:29.000000 pysipfenn-0.12.2/pysipfenn.egg-info/requires.txt
+-rw-r--r--   0 adam       (501) staff       (20)       10 2023-07-06 18:32:29.000000 pysipfenn-0.12.2/pysipfenn.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)       38 2023-07-06 18:32:29.509407 pysipfenn-0.12.2/setup.cfg
```

### Comparing `pysipfenn-0.12.1/.github/workflows/benchmarks.yml` & `pysipfenn-0.12.2/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/.github/workflows/fullTest.yml` & `pysipfenn-0.12.2/.github/workflows/fullTest.yml`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/.github/workflows/partialTest.yml` & `pysipfenn-0.12.2/.github/workflows/partialTest.yml`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/PKG-INFO` & `pysipfenn-0.12.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: pysipfenn
-Version: 0.12.1
+Version: 0.12.2
 Summary: Easily extensible Python package for featurizing periodic atomic structures and running Structure-Informed Prediction of Formation Energy using Neural Networks (SIPFENN)
 Author-email: Adam Krajewski <ak@psu.edu>, Jonathan Siegel <jwsiegel@tamu.edu>
 Project-URL: Research Page, https://phaseslab.com/sipfenn
 Project-URL: Homepage, https://pysipfenn.org
 Project-URL: Bug Tracker, https://github.com/PhasesResearchLab/pySIPFENN/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.md
 
 ## pySIPFENN
 ![GitHub top language](https://img.shields.io/github/languages/top/PhasesResearchLab/pysipfenn)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pysipfenn)
 ![PyPI](https://img.shields.io/pypi/v/pysipfenn)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pysipfenn)
 
@@ -40,16 +40,19 @@
 ![GitHub Release Date - Published_At](https://img.shields.io/github/release-date/PhasesResearchLab/pysipfenn?label=Last%20Release)
 ![GitHub commits since tagged version](https://img.shields.io/github/commits-since/PhasesResearchLab/pysipfenn/v0.12.0?color=g)
 ![GitHub issues](https://img.shields.io/github/issues/PhasesResearchLab/pysipfenn)
 
 [![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.commatsci.2022.111254-blue)](https://doi.org/10.1016/j.commatsci.2022.111254)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7373089.svg)](https://doi.org/10.5281/zenodo.7373089)
 
-### News
+### Major News
 
+- **(v.12.2)** The license has been changed to LGPLv3 to allow for integration with proprietary software developed
+by CALPHAD community, while supporting the development of new pySIPFENN features for all users. Many thanks to our colleagues from 
+[GTT-Technologies](https://gtt-technologies.de) and other participants of [50th CALPHAD 2023 conference in Boston](https://calphad.org/calphad-2023) for fruitful discussions.
 - **(v.12.0)** Official Python 3.11 support. 
 - **(v.12.0)** Automated matrix-testing on Linux / Mac / Windows with Python 3.9 / 3.10 / 3.11 through GitHub Actions CLI
 and test coverage report through Codecov. Tests are also generally improved and more extensive.
 - **(v0.11.0)** Some common questions are now addressed in the [documentation FAQ section](https://pysipfenn.readthedocs.io/en/stable/faq.html).
 - **(v0.11.0)** The model downloads from Zenodo are now multithreaded and are 15 times faster.
 - **(March 2023 Workshop)** We would like to thank all of our amazing attendees for making our workshop, co-organized with the
 [Materials Genome Foundation](https://materialsgenomefoundation.org), such a success! Over 100 of you simultaneously followed
```

### Comparing `pysipfenn-0.12.1/README.md` & `pysipfenn-0.12.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,16 +16,19 @@
 ![GitHub Release Date - Published_At](https://img.shields.io/github/release-date/PhasesResearchLab/pysipfenn?label=Last%20Release)
 ![GitHub commits since tagged version](https://img.shields.io/github/commits-since/PhasesResearchLab/pysipfenn/v0.12.0?color=g)
 ![GitHub issues](https://img.shields.io/github/issues/PhasesResearchLab/pysipfenn)
 
 [![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.commatsci.2022.111254-blue)](https://doi.org/10.1016/j.commatsci.2022.111254)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7373089.svg)](https://doi.org/10.5281/zenodo.7373089)
 
-### News
+### Major News
 
+- **(v.12.2)** The license has been changed to LGPLv3 to allow for integration with proprietary software developed
+by CALPHAD community, while supporting the development of new pySIPFENN features for all users. Many thanks to our colleagues from 
+[GTT-Technologies](https://gtt-technologies.de) and other participants of [50th CALPHAD 2023 conference in Boston](https://calphad.org/calphad-2023) for fruitful discussions.
 - **(v.12.0)** Official Python 3.11 support. 
 - **(v.12.0)** Automated matrix-testing on Linux / Mac / Windows with Python 3.9 / 3.10 / 3.11 through GitHub Actions CLI
 and test coverage report through Codecov. Tests are also generally improved and more extensive.
 - **(v0.11.0)** Some common questions are now addressed in the [documentation FAQ section](https://pysipfenn.readthedocs.io/en/stable/faq.html).
 - **(v0.11.0)** The model downloads from Zenodo are now multithreaded and are 15 times faster.
 - **(March 2023 Workshop)** We would like to thank all of our amazing attendees for making our workshop, co-organized with the
 [Materials Genome Foundation](https://materialsgenomefoundation.org), such a success! Over 100 of you simultaneously followed
```

### Comparing `pysipfenn-0.12.1/pyproject.toml` & `pysipfenn-0.12.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysipfenn"
-version = "0.12.1"
+version = "0.12.2"
 authors = [
   { name="Adam Krajewski", email="ak@psu.edu" },
     { name="Jonathan Siegel", email="jwsiegel@tamu.edu" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Chemistry",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 description = "Easily extensible Python package for featurizing periodic atomic structures and running Structure-Informed Prediction of Formation Energy using Neural Networks (SIPFENN)"
```

### Comparing `pysipfenn-0.12.1/pysipfenn/core/pysipfenn.py` & `pysipfenn-0.12.2/pysipfenn/core/pysipfenn.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from typing import List, Union, Dict
 
 # Descriptor Generators
 from pysipfenn.descriptorDefinitions import Ward2017, KS2022, KS2022_dilute
 
 # - add new ones here if extending the code
 
-__version__ = '0.12.1'
+__version__ = '0.11.0post1'
 __authors__ = [["Adam Krajewski", "ak@psu.edu"],
                ["Jonathan Siegel", "jwsiegel@tamu.edu"]]
 __name__ = 'pysipfenn'
 
 
 class Calculator:
     """
@@ -72,15 +72,15 @@
             print(f'Loading all available models (autoLoad=True)')
             self.loadModels()
 
         self.toRun = []
         self.descriptorData = []
         self.predictions = []
         self.inputFiles = []
-        print(f'*********  PySIPFENN Calculator v{__version__} Successfully Initialized  **********')
+        print(f'*********  PySIPFENN Successfully Initialized  **********')
 
     def __str__(self):
         printOut = f'PySIPFENN Calculator Object. Version: {__version__}\n'
         printOut += f'Models are located in:\n{resources.files("pysipfenn.modelsSIPFENN")}\n{"-" * 80}\n'
         printOut += f'Loaded Networks: {list(self.loadedModels.keys())}\n'
         if len(self.inputFiles) > 0:
             printOut += f'Last files selected as input: {len(self.inputFiles)}\n'
```

### Comparing `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/KS2022.py` & `pysipfenn-0.12.2/pysipfenn/descriptorDefinitions/KS2022.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/KS2022_dilute.py` & `pysipfenn-0.12.2/pysipfenn/descriptorDefinitions/KS2022_dilute.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/Magpie_element_properties.csv` & `pysipfenn-0.12.2/pysipfenn/descriptorDefinitions/Magpie_element_properties.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/Magpie_property_names.txt` & `pysipfenn-0.12.2/pysipfenn/descriptorDefinitions/Magpie_property_names.txt`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/Ward2017.py` & `pysipfenn-0.12.2/pysipfenn/descriptorDefinitions/Ward2017.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/labels_KS2022.csv` & `pysipfenn-0.12.2/pysipfenn/descriptorDefinitions/labels_KS2022.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/labels_KS2022_dilute.csv` & `pysipfenn-0.12.2/pysipfenn/descriptorDefinitions/labels_KS2022_dilute.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/labels_Ward2017.csv` & `pysipfenn-0.12.2/pysipfenn/descriptorDefinitions/labels_Ward2017.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/modelsSIPFENN/models.json` & `pysipfenn-0.12.2/pysipfenn/modelsSIPFENN/models.json`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_enumerated.csv` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_enumerated.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_named.csv` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_named.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/0-Cr8Fe18Ni4.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/0-Cr8Fe18Ni4.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/1-Cr16Fe8Ni6.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/1-Cr16Fe8Ni6.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/10-Ce4Ti4O12.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/10-Ce4Ti4O12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/11-Fe10Ni20.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/11-Fe10Ni20.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/12-Gd4Cr4O12.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/12-Gd4Cr4O12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/13-Fe16Ni14.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/13-Fe16Ni14.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/14-Fe24Ni6.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/14-Fe24Ni6.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/15-Ta4Tl4O12.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/15-Ta4Tl4O12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/16-Fe18Ni12.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/16-Fe18Ni12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/17-Pr4Ga4O12.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/17-Pr4Ga4O12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/18-Fe28Ni2.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/18-Fe28Ni2.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/19-Fe4Ni26.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/19-Fe4Ni26.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/2-Fe8Ni22.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/2-Fe8Ni22.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/20-Fe8Ni22.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/20-Fe8Ni22.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/21-Fe10Ni20.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/21-Fe10Ni20.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/22-Fe10Ni20.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/22-Fe10Ni20.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/23-Fe12Ni18.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/23-Fe12Ni18.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/24-Fe16Ni14.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/24-Fe16Ni14.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/25-Fe12Ni18.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/25-Fe12Ni18.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/26-Fe8Ni22.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/26-Fe8Ni22.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/27-Cr28Fe2.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/27-Cr28Fe2.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/28-Fe26Ni4.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/28-Fe26Ni4.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/29-Fe12Ni18.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/29-Fe12Ni18.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/3-Cr18Fe12.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/3-Cr18Fe12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/30-Cr26Fe4.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/30-Cr26Fe4.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/4-Fe30.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/4-Fe30.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/5-Cr22Fe8.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/5-Cr22Fe8.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/6-Fe2Ni28.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/6-Fe2Ni28.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/7-Cr18Fe12.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/7-Cr18Fe12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/8-Cr2Fe16Ni12.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/8-Cr2Fe16Ni12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/9-Pb8O12.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles/9-Pb8O12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFilesDescriptorTable.csv` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFilesDescriptorTable.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/1-Zr220Cu280.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/1-Zr220Cu280.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/2-Zr220Cu280.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/2-Zr220Cu280.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/3-Zr220Cu280.POSCAR` & `pysipfenn-0.12.2/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/3-Zr220Cu280.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/test_AllCompatibleONNX_Ward2017.py` & `pysipfenn-0.12.2/pysipfenn/tests/test_AllCompatibleONNX_Ward2017.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/test_KS2022.py` & `pysipfenn-0.12.2/pysipfenn/tests/test_KS2022.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/test_KS2022_dilute.py` & `pysipfenn-0.12.2/pysipfenn/tests/test_KS2022_dilute.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/test_Krajewski2020_NN9NN20NN24_ONNX.py` & `pysipfenn-0.12.2/pysipfenn/tests/test_Krajewski2020_NN9NN20NN24_ONNX.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/test_Ward2017.py` & `pysipfenn-0.12.2/pysipfenn/tests/test_Ward2017.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/test_customModel.py` & `pysipfenn-0.12.2/pysipfenn/tests/test_customModel.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn/tests/test_pysipfenn.py` & `pysipfenn-0.12.2/pysipfenn/tests/test_pysipfenn.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.1/pysipfenn.egg-info/PKG-INFO` & `pysipfenn-0.12.2/pysipfenn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: pysipfenn
-Version: 0.12.1
+Version: 0.12.2
 Summary: Easily extensible Python package for featurizing periodic atomic structures and running Structure-Informed Prediction of Formation Energy using Neural Networks (SIPFENN)
 Author-email: Adam Krajewski <ak@psu.edu>, Jonathan Siegel <jwsiegel@tamu.edu>
 Project-URL: Research Page, https://phaseslab.com/sipfenn
 Project-URL: Homepage, https://pysipfenn.org
 Project-URL: Bug Tracker, https://github.com/PhasesResearchLab/pySIPFENN/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
+License-File: LICENSE.md
 
 ## pySIPFENN
 ![GitHub top language](https://img.shields.io/github/languages/top/PhasesResearchLab/pysipfenn)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pysipfenn)
 ![PyPI](https://img.shields.io/pypi/v/pysipfenn)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/pysipfenn)
 
@@ -40,16 +40,19 @@
 ![GitHub Release Date - Published_At](https://img.shields.io/github/release-date/PhasesResearchLab/pysipfenn?label=Last%20Release)
 ![GitHub commits since tagged version](https://img.shields.io/github/commits-since/PhasesResearchLab/pysipfenn/v0.12.0?color=g)
 ![GitHub issues](https://img.shields.io/github/issues/PhasesResearchLab/pysipfenn)
 
 [![DOI](https://img.shields.io/badge/DOI-10.1016%2Fj.commatsci.2022.111254-blue)](https://doi.org/10.1016/j.commatsci.2022.111254)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7373089.svg)](https://doi.org/10.5281/zenodo.7373089)
 
-### News
+### Major News
 
+- **(v.12.2)** The license has been changed to LGPLv3 to allow for integration with proprietary software developed
+by CALPHAD community, while supporting the development of new pySIPFENN features for all users. Many thanks to our colleagues from 
+[GTT-Technologies](https://gtt-technologies.de) and other participants of [50th CALPHAD 2023 conference in Boston](https://calphad.org/calphad-2023) for fruitful discussions.
 - **(v.12.0)** Official Python 3.11 support. 
 - **(v.12.0)** Automated matrix-testing on Linux / Mac / Windows with Python 3.9 / 3.10 / 3.11 through GitHub Actions CLI
 and test coverage report through Codecov. Tests are also generally improved and more extensive.
 - **(v0.11.0)** Some common questions are now addressed in the [documentation FAQ section](https://pysipfenn.readthedocs.io/en/stable/faq.html).
 - **(v0.11.0)** The model downloads from Zenodo are now multithreaded and are 15 times faster.
 - **(March 2023 Workshop)** We would like to thank all of our amazing attendees for making our workshop, co-organized with the
 [Materials Genome Foundation](https://materialsgenomefoundation.org), such a success! Over 100 of you simultaneously followed
```

### Comparing `pysipfenn-0.12.1/pysipfenn.egg-info/SOURCES.txt` & `pysipfenn-0.12.2/pysipfenn.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 .gitattributes
 .readthedocs.yaml
-LICENSE
+LICENSE.md
 MANIFEST.in
 README.md
 pyproject.toml
 .github/workflows/benchmarks.yml
 .github/workflows/fullTest.yml
 .github/workflows/partialTest.yml
+.github/workflows/weeklyTesting.yml
 pysipfenn/__init__.py
 pysipfenn.egg-info/PKG-INFO
 pysipfenn.egg-info/SOURCES.txt
 pysipfenn.egg-info/dependency_links.txt
 pysipfenn.egg-info/requires.txt
 pysipfenn.egg-info/top_level.txt
 pysipfenn/core/__init__.py
 pysipfenn/core/pysipfenn.py
 pysipfenn/descriptorDefinitions/KS2022.py
-pysipfenn/descriptorDefinitions/KS2022_TestResult.csv
 pysipfenn/descriptorDefinitions/KS2022_dilute.py
-pysipfenn/descriptorDefinitions/KS2022_dilute_TestResult.csv
 pysipfenn/descriptorDefinitions/Magpie_element_properties.csv
 pysipfenn/descriptorDefinitions/Magpie_property_names.txt
 pysipfenn/descriptorDefinitions/README.md
 pysipfenn/descriptorDefinitions/Ward2017.py
 pysipfenn/descriptorDefinitions/__init__.py
 pysipfenn/descriptorDefinitions/labels_KS2022.csv
 pysipfenn/descriptorDefinitions/labels_KS2022_dilute.csv
 pysipfenn/descriptorDefinitions/labels_Ward2017.csv
-pysipfenn/descriptorDefinitions/__pycache__/KS2022.cpython-39.pyc
-pysipfenn/descriptorDefinitions/__pycache__/KS2022_dilute.cpython-39.pyc
-pysipfenn/descriptorDefinitions/__pycache__/Ward2017.cpython-39.pyc
-pysipfenn/descriptorDefinitions/__pycache__/__init__.cpython-39.pyc
 pysipfenn/modelsSIPFENN/README.md
 pysipfenn/modelsSIPFENN/__init__.py
 pysipfenn/modelsSIPFENN/models.json
 pysipfenn/tests/__init__.py
 pysipfenn/tests/test_AllCompatibleONNX_Ward2017.py
 pysipfenn/tests/test_KS2022.py
 pysipfenn/tests/test_KS2022_dilute.py
@@ -66,15 +61,14 @@
 pysipfenn/tests/testCaseFiles/exampleInputFiles/25-Fe12Ni18.POSCAR
 pysipfenn/tests/testCaseFiles/exampleInputFiles/26-Fe8Ni22.POSCAR
 pysipfenn/tests/testCaseFiles/exampleInputFiles/27-Cr28Fe2.POSCAR
 pysipfenn/tests/testCaseFiles/exampleInputFiles/28-Fe26Ni4.POSCAR
 pysipfenn/tests/testCaseFiles/exampleInputFiles/29-Fe12Ni18.POSCAR
 pysipfenn/tests/testCaseFiles/exampleInputFiles/3-Cr18Fe12.POSCAR
 pysipfenn/tests/testCaseFiles/exampleInputFiles/30-Cr26Fe4.POSCAR
-pysipfenn/tests/testCaseFiles/exampleInputFiles/31-Li24Al4Ni32.POSCAR
 pysipfenn/tests/testCaseFiles/exampleInputFiles/4-Fe30.POSCAR
 pysipfenn/tests/testCaseFiles/exampleInputFiles/5-Cr22Fe8.POSCAR
 pysipfenn/tests/testCaseFiles/exampleInputFiles/6-Fe2Ni28.POSCAR
 pysipfenn/tests/testCaseFiles/exampleInputFiles/7-Cr18Fe12.POSCAR
 pysipfenn/tests/testCaseFiles/exampleInputFiles/8-Cr2Fe16Ni12.POSCAR
 pysipfenn/tests/testCaseFiles/exampleInputFiles/9-Pb8O12.POSCAR
 pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/1-Zr220Cu280.POSCAR
```

