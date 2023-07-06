# Comparing `tmp/CollabConnector-0.1.1683892264.tar.gz` & `tmp/CollabConnector-0.1.1688663438.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CollabConnector-0.1.1683892264.tar", last modified: Fri May 12 11:51:12 2023, max compression
+gzip compressed data, was "CollabConnector-0.1.1688663438.tar", last modified: Thu Jul  6 17:10:45 2023, max compression
```

## Comparing `CollabConnector-0.1.1683892264.tar` & `CollabConnector-0.1.1688663438.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.627653 CollabConnector-0.1.1683892264/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1068 2022-10-25 21:11:47.000000 CollabConnector-0.1.1683892264/LICENSE
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3417 2023-05-12 11:51:12.627841 CollabConnector-0.1.1683892264/PKG-INFO
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2772 2022-10-28 16:12:38.000000 CollabConnector-0.1.1683892264/README.md
--rw-r--r--   0 jonsnipes   (501) staff       (20)       84 2022-10-26 13:12:59.000000 CollabConnector-0.1.1683892264/pyproject.toml
--rw-r--r--   0 jonsnipes   (501) staff       (20)      933 2023-05-12 11:51:12.628776 CollabConnector-0.1.1683892264/setup.cfg
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.338181 CollabConnector-0.1.1683892264/src/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.354029 CollabConnector-0.1.1683892264/src/CollabConnector/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.359654 CollabConnector-0.1.1683892264/src/CollabConnector/CER/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2582 2023-02-22 19:34:55.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CER/CER.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CER/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.361491 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.363304 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AST/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    10783 2023-02-22 19:35:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AST/AST.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AST/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.377045 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2111 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/AXL.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.381075 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/Add/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   300285 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/Add/Add.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/Add/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.382850 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/Do/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2439 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/Do/Do.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       17 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/Do/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.386251 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/Get/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   185512 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/Get/Get.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/Get/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.389722 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/List/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   234451 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/List/List.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/List/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.392033 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/Remove/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    18840 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/Remove/Remove.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/Remove/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.395402 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/Update/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   282551 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/Update/Update.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/Update/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      138 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.346357 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.402405 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/10.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   769959 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   128245 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3395256 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.422172 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/10.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   770694 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   130699 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3413507 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.441732 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/11.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   787404 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   132691 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3488840 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.461118 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/11.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   801501 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   134780 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3541419 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.480822 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/12.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   809784 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   136574 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3574456 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.515363 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/12.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   141548 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3700703 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd
--rw-r--r--   0 jonsnipes   (501) staff       (20)    14032 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)    14090 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)    18688 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.524219 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/14.0/
--rw-r--r--   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl
--rw-r--r--   0 jonsnipes   (501) staff       (20)   147593 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd
--rw-r--r--   0 jonsnipes   (501) staff       (20)  3718998 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.542981 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/7.1/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   106483 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   247739 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   324873 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)     4901 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.549778 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/8.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   479490 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   285148 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2239698 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.564208 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/8.5/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   495675 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   316422 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2321578 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.579247 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/9.0/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   554463 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   352279 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2538639 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.594545 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/9.1/
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   555159 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)   485786 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd
--rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2547044 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.605300 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/CDR/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    20618 2023-01-24 14:18:53.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/CDR/CDR.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9803 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/CDR/CDROnDemand.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2023-01-24 14:06:12.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/CDR/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)    13353 2023-04-27 16:08:41.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/CUCM.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.607064 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/DIME/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2951 2022-11-15 18:23:49.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/DIME/DIME.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/DIME/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.608410 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/Logs/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2390 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/Logs/Logs.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/Logs/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.609921 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/Risport/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     1509 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/Risport/Risport.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/Risport/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.611392 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/Serviceability/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9277 2022-11-15 19:11:35.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/Serviceability/Serviceability.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2022-11-15 18:23:37.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/Serviceability/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.612964 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/UDS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     2098 2023-02-22 19:35:33.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/UDS/UDS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/UDS/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.614637 CollabConnector-0.1.1683892264/src/CollabConnector/CUCX/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    15080 2023-02-22 19:34:48.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCX/CUCX.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/CUCX/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.616310 CollabConnector-0.1.1683892264/src/CollabConnector/Expressway/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3525 2023-02-22 19:35:10.000000 CollabConnector-0.1.1683892264/src/CollabConnector/Expressway/Expressway.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       25 2022-11-17 23:27:57.000000 CollabConnector-0.1.1683892264/src/CollabConnector/Expressway/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.618348 CollabConnector-0.1.1683892264/src/CollabConnector/IOS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    20124 2022-12-10 21:17:21.000000 CollabConnector-0.1.1683892264/src/CollabConnector/IOS/IOS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-12-10 02:10:29.000000 CollabConnector-0.1.1683892264/src/CollabConnector/IOS/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.620691 CollabConnector-0.1.1683892264/src/CollabConnector/PAWS/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     5894 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/PAWS/PAWS.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/PAWS/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.622443 CollabConnector-0.1.1683892264/src/CollabConnector/Phone/
--rw-r--r--   0 jonsnipes   (501) staff       (20)    30949 2023-02-22 19:35:02.000000 CollabConnector-0.1.1683892264/src/CollabConnector/Phone/Phone.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/Phone/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.624149 CollabConnector-0.1.1683892264/src/CollabConnector/UCCX/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     8550 2023-02-22 19:34:41.000000 CollabConnector-0.1.1683892264/src/CollabConnector/UCCX/UCCX.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/UCCX/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.627329 CollabConnector-0.1.1683892264/src/CollabConnector/Webex/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3205 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/Webex/CallControl.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     9430 2023-05-12 11:49:22.000000 CollabConnector-0.1.1683892264/src/CollabConnector/Webex/ContactCenter.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      954 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/Webex/OutputStyle.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)     7891 2023-05-12 11:50:53.000000 CollabConnector-0.1.1683892264/src/CollabConnector/Webex/Webex.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)        0 2022-10-25 21:12:20.000000 CollabConnector-0.1.1683892264/src/CollabConnector/Webex/__init__.py
--rw-r--r--   0 jonsnipes   (501) staff       (20)      186 2022-12-10 02:10:29.000000 CollabConnector-0.1.1683892264/src/CollabConnector/__init__.py
-drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-05-12 11:51:12.357847 CollabConnector-0.1.1683892264/src/CollabConnector.egg-info/
--rw-r--r--   0 jonsnipes   (501) staff       (20)     3417 2023-05-12 11:51:12.000000 CollabConnector-0.1.1683892264/src/CollabConnector.egg-info/PKG-INFO
--rw-r--r--   0 jonsnipes   (501) staff       (20)     4444 2023-05-12 11:51:12.000000 CollabConnector-0.1.1683892264/src/CollabConnector.egg-info/SOURCES.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)        1 2023-05-12 11:51:12.000000 CollabConnector-0.1.1683892264/src/CollabConnector.egg-info/dependency_links.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)       47 2023-05-12 11:51:12.000000 CollabConnector-0.1.1683892264/src/CollabConnector.egg-info/requires.txt
--rw-r--r--   0 jonsnipes   (501) staff       (20)       16 2023-05-12 11:51:12.000000 CollabConnector-0.1.1683892264/src/CollabConnector.egg-info/top_level.txt
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.774444 CollabConnector-0.1.1688663438/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1068 2022-10-25 21:11:47.000000 CollabConnector-0.1.1688663438/LICENSE
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3417 2023-07-06 17:10:45.774562 CollabConnector-0.1.1688663438/PKG-INFO
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2772 2022-10-28 16:12:38.000000 CollabConnector-0.1.1688663438/README.md
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       84 2022-10-26 13:12:59.000000 CollabConnector-0.1.1688663438/pyproject.toml
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      933 2023-07-06 17:10:45.775113 CollabConnector-0.1.1688663438/setup.cfg
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.552323 CollabConnector-0.1.1688663438/src/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.560589 CollabConnector-0.1.1688663438/src/CollabConnector/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.564092 CollabConnector-0.1.1688663438/src/CollabConnector/CER/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2582 2023-02-22 19:34:55.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CER/CER.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CER/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.565819 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.567036 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AST/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    10787 2023-07-06 17:10:27.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AST/AST.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AST/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.568756 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2111 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/AXL.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.571845 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/Add/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   300285 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/Add/Add.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/Add/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.572804 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/Do/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2439 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/Do/Do.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       17 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/Do/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.574813 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/Get/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   185512 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/Get/Get.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/Get/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.576744 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/List/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   234451 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/List/List.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/List/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.577966 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/Remove/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    18840 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/Remove/Remove.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/Remove/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.579433 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/Update/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   282551 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/Update/Update.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/Update/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      138 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.556442 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.583791 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/10.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   769959 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   128245 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3395256 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.600683 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/10.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   770694 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   130699 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3413507 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.617308 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/11.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   787404 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   132691 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3488840 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.631928 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/11.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   801501 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   134780 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3541419 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.648839 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/12.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   809784 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   136574 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3574456 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.677336 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/12.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   141548 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  3700703 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    14032 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    14090 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    18688 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.683718 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/14.0/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   834720 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl
+-rw-r--r--   0 jonsnipes   (501) staff       (20)   147593 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd
+-rw-r--r--   0 jonsnipes   (501) staff       (20)  3718998 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.702684 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/7.1/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   106483 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   247739 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   324873 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)     4901 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.708943 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/8.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   479490 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   285148 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2239698 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.723385 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/8.5/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   495675 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   316422 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2321578 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.736862 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/9.0/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   554463 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   352279 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2538639 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.751066 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/9.1/
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   555159 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)   485786 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd
+-rwxr-xr-x   0 jonsnipes   (501) staff       (20)  2547044 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.760069 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/CDR/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    20618 2023-01-24 14:18:53.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/CDR/CDR.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9803 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/CDR/CDROnDemand.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       21 2023-01-24 14:06:12.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/CDR/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    13353 2023-04-27 16:08:41.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/CUCM.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.761188 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/DIME/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2951 2022-11-15 18:23:49.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/DIME/DIME.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/DIME/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.762087 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/Logs/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2390 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/Logs/Logs.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/Logs/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.762990 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/Risport/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     1509 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/Risport/Risport.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       22 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/Risport/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.763956 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/Serviceability/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9277 2022-11-15 19:11:35.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/Serviceability/Serviceability.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       29 2022-11-15 18:23:37.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/Serviceability/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.765171 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/UDS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     2098 2023-02-22 19:35:33.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/UDS/UDS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       18 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/UDS/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.766404 CollabConnector-0.1.1688663438/src/CollabConnector/CUCX/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    15080 2023-02-22 19:34:48.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCX/CUCX.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/CUCX/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.767619 CollabConnector-0.1.1688663438/src/CollabConnector/Expressway/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3525 2023-02-22 19:35:10.000000 CollabConnector-0.1.1688663438/src/CollabConnector/Expressway/Expressway.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       25 2022-11-17 23:27:57.000000 CollabConnector-0.1.1688663438/src/CollabConnector/Expressway/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.768844 CollabConnector-0.1.1688663438/src/CollabConnector/IOS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    20124 2022-12-10 21:17:21.000000 CollabConnector-0.1.1688663438/src/CollabConnector/IOS/IOS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-12-10 02:10:29.000000 CollabConnector-0.1.1688663438/src/CollabConnector/IOS/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.769910 CollabConnector-0.1.1688663438/src/CollabConnector/PAWS/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     5894 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/PAWS/PAWS.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       19 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/PAWS/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.771069 CollabConnector-0.1.1688663438/src/CollabConnector/Phone/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)    30949 2023-02-22 19:35:02.000000 CollabConnector-0.1.1688663438/src/CollabConnector/Phone/Phone.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/Phone/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.772114 CollabConnector-0.1.1688663438/src/CollabConnector/UCCX/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     8550 2023-02-22 19:34:41.000000 CollabConnector-0.1.1688663438/src/CollabConnector/UCCX/UCCX.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       20 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/UCCX/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.774247 CollabConnector-0.1.1688663438/src/CollabConnector/Webex/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3205 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/Webex/CallControl.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     9430 2023-05-12 11:49:22.000000 CollabConnector-0.1.1688663438/src/CollabConnector/Webex/ContactCenter.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      954 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/Webex/OutputStyle.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     7891 2023-05-12 11:50:53.000000 CollabConnector-0.1.1688663438/src/CollabConnector/Webex/Webex.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)        0 2022-10-25 21:12:20.000000 CollabConnector-0.1.1688663438/src/CollabConnector/Webex/__init__.py
+-rw-r--r--   0 jonsnipes   (501) staff       (20)      186 2022-12-10 02:10:29.000000 CollabConnector-0.1.1688663438/src/CollabConnector/__init__.py
+drwxr-xr-x   0 jonsnipes   (501) staff       (20)        0 2023-07-06 17:10:45.562878 CollabConnector-0.1.1688663438/src/CollabConnector.egg-info/
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     3417 2023-07-06 17:10:45.000000 CollabConnector-0.1.1688663438/src/CollabConnector.egg-info/PKG-INFO
+-rw-r--r--   0 jonsnipes   (501) staff       (20)     4444 2023-07-06 17:10:45.000000 CollabConnector-0.1.1688663438/src/CollabConnector.egg-info/SOURCES.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)        1 2023-07-06 17:10:45.000000 CollabConnector-0.1.1688663438/src/CollabConnector.egg-info/dependency_links.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       47 2023-07-06 17:10:45.000000 CollabConnector-0.1.1688663438/src/CollabConnector.egg-info/requires.txt
+-rw-r--r--   0 jonsnipes   (501) staff       (20)       16 2023-07-06 17:10:45.000000 CollabConnector-0.1.1688663438/src/CollabConnector.egg-info/top_level.txt
```

### Comparing `CollabConnector-0.1.1683892264/LICENSE` & `CollabConnector-0.1.1688663438/LICENSE`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/PKG-INFO` & `CollabConnector-0.1.1688663438/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CollabConnector
-Version: 0.1.1683892264
+Version: 0.1.1688663438
 Summary: An attempt at a simplified API collection for Cisco Collab products
 Home-page: https://github.com/mycollablab/CollabConnector
 Author: Jon Snipes
 Author-email: jsnipes@mycollablab.org
 Project-URL: Bug Tracker, https://github.com/mycollablab/CollabConnector/issues
 Project-URL: repository, https://github.com/mycollablab/CollabConnector
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CollabConnector-0.1.1683892264/README.md` & `CollabConnector-0.1.1688663438/README.md`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/setup.cfg` & `CollabConnector-0.1.1688663438/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = CollabConnector
-version = 0.1.1683892264
+version = 0.1.1688663438
 author = Jon Snipes
 author_email = jsnipes@mycollablab.org
 description = An attempt at a simplified API collection for Cisco Collab products
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/mycollablab/CollabConnector
 project_urls =
```

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CER/CER.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/CER/CER.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AST/AST.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AST/AST.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import requests
 from requests.auth import HTTPBasicAuth
 import sys
 import xmltodict
 import urllib
 
 requests.packages.urllib3.disable_warnings()
-requests.packages.urllib3.util.ssl_.DEFAULT_CIPHERS += ':HIGH:!DH:!aNULL'
 try:
+    requests.packages.urllib3.util.ssl_.DEFAULT_CIPHERS += ':HIGH:!DH:!aNULL'
     requests.packages.urllib3.contrib.pyopenssl.util.ssl_.DEFAULT_CIPHERS += ':HIGH:!DH:!aNULL'
 except AttributeError:
     # no pyopenssl support used / needed / available
     pass
 
 
 class Connect:
```

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/AXL.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/AXL.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/Add/Add.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/Add/Add.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/Do/Do.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/Do/Do.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/Get/Get.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/Get/Get.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/List/List.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/List/List.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/Remove/Remove.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/Remove/Remove.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/Update/Update.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/Update/Update.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/10.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/10.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/10.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/10.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/10.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/10.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/11.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/11.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/11.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/11.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/11.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/11.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/12.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/12.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/12.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/12.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/12.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/12.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/12.5/ControlCenterServices.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/12.5/PerfmonService.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/12.5/RISService70.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/14.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/14.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/14.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/7.1/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/7.1/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/7.1/axl.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/7.1/axlmessage.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/8.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/8.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/8.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/8.5/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/8.5/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/8.5/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/9.0/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/9.0/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/9.0/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/9.1/AXLAPI.wsdl`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/9.1/AXLEnums.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/AXL/schema/9.1/AXLSoap.xsd`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/CDR/CDR.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/CDR/CDR.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/CDR/CDROnDemand.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/CDR/CDROnDemand.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/CUCM.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/CUCM.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/DIME/DIME.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/DIME/DIME.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/Logs/Logs.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/Logs/Logs.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/Risport/Risport.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/Risport/Risport.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/Serviceability/Serviceability.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/Serviceability/Serviceability.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCM/UDS/UDS.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCM/UDS/UDS.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/CUCX/CUCX.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/CUCX/CUCX.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/Expressway/Expressway.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/Expressway/Expressway.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/IOS/IOS.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/IOS/IOS.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/PAWS/PAWS.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/PAWS/PAWS.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/Phone/Phone.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/Phone/Phone.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/UCCX/UCCX.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/UCCX/UCCX.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/Webex/CallControl.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/Webex/CallControl.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/Webex/ContactCenter.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/Webex/ContactCenter.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/Webex/OutputStyle.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/Webex/OutputStyle.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector/Webex/Webex.py` & `CollabConnector-0.1.1688663438/src/CollabConnector/Webex/Webex.py`

 * *Files identical despite different names*

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector.egg-info/PKG-INFO` & `CollabConnector-0.1.1688663438/src/CollabConnector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CollabConnector
-Version: 0.1.1683892264
+Version: 0.1.1688663438
 Summary: An attempt at a simplified API collection for Cisco Collab products
 Home-page: https://github.com/mycollablab/CollabConnector
 Author: Jon Snipes
 Author-email: jsnipes@mycollablab.org
 Project-URL: Bug Tracker, https://github.com/mycollablab/CollabConnector/issues
 Project-URL: repository, https://github.com/mycollablab/CollabConnector
 Classifier: Programming Language :: Python :: 3
```

### Comparing `CollabConnector-0.1.1683892264/src/CollabConnector.egg-info/SOURCES.txt` & `CollabConnector-0.1.1688663438/src/CollabConnector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

