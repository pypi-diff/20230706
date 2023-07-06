# Comparing `tmp/pyocf-1.0.1.tar.gz` & `tmp/pyocf-1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyocf-1.0.1.tar", last modified: Thu Jul  6 11:16:45 2023, max compression
+gzip compressed data, was "pyocf-1.0b1.tar", last modified: Wed Mar 15 20:14:42 2023, max compression
```

## Comparing `pyocf-1.0.1.tar` & `pyocf-1.0b1.tar`

### file list

```diff
@@ -1,260 +1,259 @@
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.889949 pyocf-1.0.1/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      442 2023-07-06 11:16:45.000000 pyocf-1.0.1/.pre-commit-config.yaml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      339 2023-07-06 11:16:45.000000 pyocf-1.0.1/.readthedocs.yaml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      331 2023-07-06 11:16:45.000000 pyocf-1.0.1/CHANGES.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1092 2023-07-06 11:16:45.000000 pyocf-1.0.1/LICENSE.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      217 2023-07-06 11:16:45.000000 pyocf-1.0.1/MANIFEST.in
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1551 2023-07-06 11:16:45.000000 pyocf-1.0.1/Makefile
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1682 2023-07-06 11:16:45.889949 pyocf-1.0.1/PKG-INFO
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      301 2023-07-06 11:16:45.000000 pyocf-1.0.1/README.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1401 2023-07-06 11:16:45.889949 pyocf-1.0.1/setup.cfg
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       38 2023-07-06 11:16:45.000000 pyocf-1.0.1/setup.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.865949 pyocf-1.0.1/src/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.869949 pyocf-1.0.1/src/pyocf/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    13995 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/api.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7774 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/captable.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.873949 pyocf-1.0.1/src/pyocf/enums/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      641 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/accrualperiodtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      525 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/addresstype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1748 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/allocationtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      526 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/compensationtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      544 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/compoundingtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      912 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/conversionmechanismtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      695 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/conversionrighttype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      749 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/conversiontimingtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1239 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/conversiontriggertype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      585 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/convertibletype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      580 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/daycounttype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      525 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/emailtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1043 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/filetype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      594 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/interestpayouttype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2833 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/objecttype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      607 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/ocfversiontype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      507 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/optiontype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      664 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/parentsecuritytype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      527 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/periodtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      558 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/phonetype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      531 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/roundingtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      997 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/stakeholderrelationshiptype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      624 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/stakeholdertype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      520 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/stockclasstype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      859 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/terminationwindowtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      477 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/valuationtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3007 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/vestingdayofmonth.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      698 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/enums/vestingtriggertype.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.873949 pyocf-1.0.1/src/pyocf/files/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/files/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4600 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/files/ocfmanifestfile.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      920 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/files/stakeholdersfile.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      921 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/files/stockclassesfile.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1019 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/files/stocklegendtemplatesfile.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      905 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/files/stockplansfile.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5557 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/files/transactionsfile.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      900 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/files/valuationsfile.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      929 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/files/vestingtermsfile.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.877949 pyocf-1.0.1/src/pyocf/objects/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2688 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/issuer.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2418 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/stakeholder.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4509 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/stockclass.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1200 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/stocklegendtemplate.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2187 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/stockplan.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.877949 pyocf-1.0.1/src/pyocf/objects/transactions/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       23 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/__init__.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.877949 pyocf-1.0.1/src/pyocf/objects/transactions/acceptance/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/acceptance/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2200 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/acceptance/convertibleacceptance.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2210 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/acceptance/plansecurityacceptance.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2161 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/acceptance/stockacceptance.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2173 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/acceptance/warrantacceptance.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.877949 pyocf-1.0.1/src/pyocf/objects/transactions/adjustment/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/adjustment/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2217 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/adjustment/stockclassauthorizedsharesadjustment.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2974 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/adjustment/stockclassconversionratioadjustment.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2576 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/adjustment/stockplanpooladjustment.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.877949 pyocf-1.0.1/src/pyocf/objects/transactions/cancellation/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       23 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/cancellation/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2697 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/cancellation/convertiblecancellation.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2717 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/cancellation/plansecuritycancellation.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2689 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/cancellation/stockcancellation.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2701 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/cancellation/warrantcancellation.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.877949 pyocf-1.0.1/src/pyocf/objects/transactions/conversion/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/conversion/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3841 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/conversion/convertibleconversion.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2762 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/conversion/stockconversion.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.877949 pyocf-1.0.1/src/pyocf/objects/transactions/exercise/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/exercise/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2759 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/exercise/plansecurityexercise.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2779 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/exercise/warrantexercise.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.877949 pyocf-1.0.1/src/pyocf/objects/transactions/issuance/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/issuance/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5800 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/issuance/convertibleissuance.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4772 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/issuance/plansecurityissuance.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4929 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/issuance/stockissuance.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5692 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/issuance/warrantissuance.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.877949 pyocf-1.0.1/src/pyocf/objects/transactions/reissuance/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/reissuance/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2845 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/reissuance/stockreissuance.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.877949 pyocf-1.0.1/src/pyocf/objects/transactions/release/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/release/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3232 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/release/plansecurityrelease.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.877949 pyocf-1.0.1/src/pyocf/objects/transactions/repurchase/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/repurchase/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2973 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/repurchase/stockrepurchase.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.877949 pyocf-1.0.1/src/pyocf/objects/transactions/retraction/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/retraction/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2284 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/retraction/convertibleretraction.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2276 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/retraction/plansecurityretraction.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2245 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/retraction/stockretraction.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2257 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/retraction/warrantretraction.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.877949 pyocf-1.0.1/src/pyocf/objects/transactions/split/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/split/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1813 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/split/stockclasssplit.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.877949 pyocf-1.0.1/src/pyocf/objects/transactions/transfer/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/transfer/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3097 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/transfer/convertibletransfer.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3076 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/transfer/plansecuritytransfer.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3084 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/transfer/stocktransfer.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3096 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/transfer/warranttransfer.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.877949 pyocf-1.0.1/src/pyocf/objects/transactions/vesting/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/vesting/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2537 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/vesting/vestingacceleration.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2425 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/vesting/vestingevent.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2432 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/transactions/vesting/vestingstart.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2059 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/valuation.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1702 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/objects/vestingterms.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.877949 pyocf-1.0.1/src/pyocf/primitives/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/__init__.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.881949 pyocf-1.0.1/src/pyocf/primitives/files/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/files/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      763 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/files/file.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.881949 pyocf-1.0.1/src/pyocf/primitives/objects/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      999 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/object.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.881949 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       23 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/__init__.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.881949 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/acceptance/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/acceptance/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      561 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/acceptance/acceptance.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.881949 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/cancellation/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       23 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/cancellation/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1032 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/cancellation/cancellation.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.881949 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/conversion/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/conversion/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      848 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/conversion/conversion.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.881949 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/exercise/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/exercise/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1119 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/exercise/exercise.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.881949 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/issuance/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/issuance/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1618 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/issuance/issuance.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.881949 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/reissuance/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/reissuance/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1374 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/reissuance/reissuance.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.881949 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/release/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/release/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1756 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/release/release.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.881949 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/repurchase/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/repurchase/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1482 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/repurchase/repurchase.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.881949 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/retraction/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/retraction/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      698 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/retraction/retraction.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1401 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/securitytransaction.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      881 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/stockclasstransaction.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      872 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/stockplantransaction.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      757 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/transaction.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.881949 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/transfer/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/transfer/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1404 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/objects/transactions/transfer/transfer.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.881949 pyocf-1.0.1/src/pyocf/primitives/types/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/types/__init__.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.881949 pyocf-1.0.1/src/pyocf/primitives/types/conversion_mechanisms/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       32 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/types/conversion_mechanisms/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      882 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/types/conversion_mechanisms/conversionmechanism.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.881949 pyocf-1.0.1/src/pyocf/primitives/types/conversion_rights/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       28 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/types/conversion_rights/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2721 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/types/conversion_rights/conversionright.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.881949 pyocf-1.0.1/src/pyocf/primitives/types/conversion_triggers/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       30 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/types/conversion_triggers/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2260 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/types/conversion_triggers/conversiontrigger.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.881949 pyocf-1.0.1/src/pyocf/primitives/types/vesting/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/types/vesting/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      993 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/types/vesting/vestingconditiontrigger.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1356 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/primitives/types/vesting/vestingperiod.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1513 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/simplebase.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.885949 pyocf-1.0.1/src/pyocf/types/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1555 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/address.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2050 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/capitalizationdefinition.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      991 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/contactinfo.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.885949 pyocf-1.0.1/src/pyocf/types/conversion_mechanisms/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       32 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/conversion_mechanisms/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1340 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/conversion_mechanisms/customconversionmechanism.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1119 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/conversion_mechanisms/fixedamountconversionmechanism.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2931 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/conversion_mechanisms/noteconversionmechanism.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1744 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/conversion_mechanisms/percentcapitalizationconversionmechanism.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1681 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/conversion_mechanisms/ratioconversionmechanism.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2421 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/conversion_mechanisms/safeconversionmechanism.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.885949 pyocf-1.0.1/src/pyocf/types/conversion_rights/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       28 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/conversion_rights/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2433 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/conversion_rights/convertibleconversionright.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1686 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/conversion_rights/stockclassconversionright.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2276 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/conversion_rights/warrantconversionright.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.889949 pyocf-1.0.1/src/pyocf/types/conversion_triggers/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       30 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/conversion_triggers/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2444 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/conversion_triggers/automaticconversiononconditiontrigger.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2316 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/conversion_triggers/automaticconversionondatetrigger.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2210 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/conversion_triggers/electiveconversionatwilltrigger.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2414 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/conversion_triggers/electiveconversionindaterangetrigger.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2452 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/conversion_triggers/electiveconversiononconditiontrigger.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2186 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/conversion_triggers/unspecifiedconversiontrigger.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      608 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/countrycode.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      681 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/countrysubdivisioncode.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      592 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/currencycode.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      563 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/date.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      782 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/email.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      707 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/file.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1452 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/interestrate.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      778 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/md5.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      834 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/monetary.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      899 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/name.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      637 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/numeric.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      763 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/percentage.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      982 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/phone.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1177 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/ratio.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1359 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/securityexemption.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1418 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/sharenumberrange.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1304 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/stockparent.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      979 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/taxid.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1150 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/terminationwindow.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.889949 pyocf-1.0.1/src/pyocf/types/vesting/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/vesting/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2711 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/vesting/vestingcondition.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1964 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/vesting/vestingconditionportion.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      854 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/vesting/vestingeventtrigger.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1255 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/vesting/vestingperiodindays.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1467 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/vesting/vestingperiodinmonths.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1000 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/vesting/vestingscheduleabsolutetrigger.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1793 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/vesting/vestingschedulerelativetrigger.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      882 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf/types/vesting/vestingstarttrigger.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.873949 pyocf-1.0.1/src/pyocf.egg-info/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1682 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf.egg-info/PKG-INFO
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     9738 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf.egg-info/SOURCES.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf.egg-info/dependency_links.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      163 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf.egg-info/requires.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        6 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf.egg-info/top_level.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-07-06 11:16:45.000000 pyocf-1.0.1/src/pyocf.egg-info/zip-safe
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.889949 pyocf-1.0.1/tests/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.000000 pyocf-1.0.1/tests/__init__.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.889949 pyocf-1.0.1/tests/samples/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    12054 2023-07-06 11:16:45.000000 pyocf-1.0.1/tests/samples/Captable.ocf.zip
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2262 2023-07-06 11:16:45.000000 pyocf-1.0.1/tests/test_basic.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    12312 2023-07-06 11:16:45.000000 pyocf-1.0.1/tests/test_load.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2156 2023-07-06 11:16:45.000000 pyocf-1.0.1/tests/test_save.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-07-06 11:16:45.889949 pyocf-1.0.1/utils/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      362 2023-07-06 11:16:45.000000 pyocf-1.0.1/utils/enum.mako
--rwxrwxr-x   0 lregebro  (1000) lregebro  (1000)    14641 2023-07-06 11:16:45.000000 pyocf-1.0.1/utils/generate.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      546 2023-07-06 11:16:45.000000 pyocf-1.0.1/utils/object.mako
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.347033 pyocf-1.0b1/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      443 2023-03-15 20:14:42.000000 pyocf-1.0b1/.pre-commit-config.yaml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       70 2023-03-15 20:14:42.000000 pyocf-1.0b1/CHANGES.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1092 2023-03-15 20:14:42.000000 pyocf-1.0b1/LICENSE.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      192 2023-03-15 20:14:42.000000 pyocf-1.0b1/MANIFEST.in
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1340 2023-03-15 20:14:42.000000 pyocf-1.0b1/Makefile
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1188 2023-03-15 20:14:42.347033 pyocf-1.0b1/PKG-INFO
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      270 2023-03-15 20:14:42.000000 pyocf-1.0b1/README.rst
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1240 2023-03-15 20:14:42.351033 pyocf-1.0b1/setup.cfg
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       38 2023-03-15 20:14:42.000000 pyocf-1.0b1/setup.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.327033 pyocf-1.0b1/src/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.331033 pyocf-1.0b1/src/pyocf/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7744 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/captable.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.335033 pyocf-1.0b1/src/pyocf/enums/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      660 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/accrualperiodtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      544 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/addresstype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1376 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/allocationtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      545 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/compensationtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      563 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/compoundingtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      931 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/conversionmechanismtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      714 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/conversionrighttype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      716 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/conversiontimingtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1080 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/conversiontriggertype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      604 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/convertibletype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      599 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/daycounttype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      544 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/emailtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1047 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/filetype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      613 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/interestpayouttype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2852 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/objecttype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      626 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/ocfversiontype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      526 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/optiontype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      683 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/parentsecuritytype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      546 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/periodtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      577 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/phonetype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      550 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/roundingtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1016 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/stakeholderrelationshiptype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      643 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/stakeholdertype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      539 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/stockclasstype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      878 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/terminationwindowtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      496 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/valuationtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2241 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/vestingdayofmonth.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      717 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/vestingtriggertype.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.335033 pyocf-1.0b1/src/pyocf/files/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/files/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3522 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/files/ocfmanifestfile.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      794 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/files/stakeholdersfile.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      795 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/files/stockclassesfile.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      898 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/files/stocklegendtemplatesfile.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      779 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/files/stockplansfile.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5318 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/files/transactionsfile.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      774 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/files/valuationsfile.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      803 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/files/vestingtermsfile.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.335033 pyocf-1.0b1/src/pyocf/objects/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1922 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/issuer.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1750 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/stakeholder.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3271 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/stockclass.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      928 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/stocklegendtemplate.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1621 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/stockplan.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.335033 pyocf-1.0b1/src/pyocf/objects/transactions/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       23 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/__init__.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.335033 pyocf-1.0b1/src/pyocf/objects/transactions/acceptance/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/acceptance/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1835 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/acceptance/convertibleacceptance.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1845 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/acceptance/plansecurityacceptance.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1796 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/acceptance/stockacceptance.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1808 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/acceptance/warrantacceptance.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.335033 pyocf-1.0b1/src/pyocf/objects/transactions/adjustment/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/adjustment/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1721 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/adjustment/stockclassauthorizedsharesadjustment.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2240 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/adjustment/stockclassconversionratioadjustment.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2010 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/adjustment/stockplanpooladjustment.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.335033 pyocf-1.0b1/src/pyocf/objects/transactions/cancellation/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       23 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/cancellation/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2160 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/cancellation/convertiblecancellation.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2180 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/cancellation/plansecuritycancellation.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2135 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/cancellation/stockcancellation.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2150 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/cancellation/warrantcancellation.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.335033 pyocf-1.0b1/src/pyocf/objects/transactions/conversion/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/conversion/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2972 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/conversion/convertibleconversion.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2166 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/conversion/stockconversion.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.335033 pyocf-1.0b1/src/pyocf/objects/transactions/exercise/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/exercise/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2177 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/exercise/plansecurityexercise.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2152 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/exercise/warrantexercise.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/objects/transactions/issuance/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/issuance/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4651 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/issuance/convertibleissuance.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4014 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/issuance/plansecurityissuance.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3679 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/issuance/stockissuance.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4535 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/issuance/warrantissuance.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/objects/transactions/reissuance/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/reissuance/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2206 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/reissuance/stockreissuance.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/objects/transactions/release/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/release/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2482 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/release/plansecurityrelease.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/objects/transactions/repurchase/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/repurchase/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2290 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/repurchase/stockrepurchase.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/objects/transactions/retraction/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/retraction/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1892 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/retraction/convertibleretraction.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1884 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/retraction/plansecurityretraction.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1853 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/retraction/stockretraction.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1865 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/retraction/warrantretraction.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/objects/transactions/split/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/split/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1416 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/split/stockclasssplit.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/objects/transactions/transfer/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/transfer/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2375 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/transfer/convertibletransfer.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2345 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/transfer/plansecuritytransfer.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2353 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/transfer/stocktransfer.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2365 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/transfer/warranttransfer.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/objects/transactions/vesting/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/vesting/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2027 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/vesting/vestingacceleration.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1953 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/vesting/vestingevent.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1960 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/vesting/vestingstart.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1515 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/valuation.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1294 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/vestingterms.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/primitives/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/__init__.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/primitives/files/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/files/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      654 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/files/file.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/primitives/objects/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      802 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/object.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       23 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/__init__.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/acceptance/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/acceptance/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      580 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/acceptance/acceptance.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/cancellation/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       23 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/cancellation/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      850 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/cancellation/cancellation.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/conversion/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/conversion/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      739 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/conversion/conversion.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/exercise/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/exercise/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      892 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/exercise/exercise.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/issuance/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/issuance/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1237 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/issuance/issuance.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.343033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/reissuance/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/reissuance/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1063 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/reissuance/reissuance.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.343033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/release/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/release/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1334 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/release/release.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.343033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/repurchase/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/repurchase/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1127 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/repurchase/repurchase.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.343033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/retraction/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/retraction/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      634 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/retraction/retraction.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1214 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/securitytransaction.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      749 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/stockclasstransaction.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      740 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/stockplantransaction.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      693 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/transaction.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.343033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/transfer/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/transfer/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1051 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/transfer/transfer.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.343033 pyocf-1.0b1/src/pyocf/primitives/types/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/types/__init__.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.343033 pyocf-1.0b1/src/pyocf/primitives/types/conversion_mechanisms/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       32 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/types/conversion_mechanisms/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      795 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/types/conversion_mechanisms/conversionmechanism.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.343033 pyocf-1.0b1/src/pyocf/primitives/types/conversion_rights/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       28 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/types/conversion_rights/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2350 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/types/conversion_rights/conversionright.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.343033 pyocf-1.0b1/src/pyocf/primitives/types/conversion_triggers/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       30 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/types/conversion_triggers/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1921 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/types/conversion_triggers/conversiontrigger.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.343033 pyocf-1.0b1/src/pyocf/primitives/types/vesting/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/types/vesting/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      837 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/types/vesting/vestingconditiontrigger.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1066 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/types/vesting/vestingperiod.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1484 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/simplebase.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.347033 pyocf-1.0b1/src/pyocf/types/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1183 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/address.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1588 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/capitalizationdefinition.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      859 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/contactinfo.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.347033 pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       32 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1090 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/customconversionmechanism.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      962 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/fixedamountconversionmechanism.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2187 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/noteconversionmechanism.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1374 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/percentcapitalizationconversionmechanism.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1320 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/ratioconversionmechanism.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1796 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/safeconversionmechanism.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.347033 pyocf-1.0b1/src/pyocf/types/conversion_rights/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       28 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_rights/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2152 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_rights/convertibleconversionright.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1333 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_rights/stockclassconversionright.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1945 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_rights/warrantconversionright.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.347033 pyocf-1.0b1/src/pyocf/types/conversion_triggers/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       30 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_triggers/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2056 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_triggers/automaticconversiononconditiontrigger.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1944 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_triggers/automaticconversionondatetrigger.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1886 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_triggers/electiveconversionatwilltrigger.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2040 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_triggers/electiveconversionindaterangetrigger.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2064 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_triggers/electiveconversiononconditiontrigger.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1868 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_triggers/unspecifiedconversiontrigger.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      627 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/countrycode.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      700 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/countrysubdivisioncode.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      611 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/currencycode.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      582 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/date.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      668 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/email.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      602 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/file.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1133 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/interestrate.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      729 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/md5.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      743 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/monetary.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      739 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/name.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      645 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/numeric.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      742 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/percentage.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      815 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/phone.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      946 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/prereleaseomission.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      953 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/ratio.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1074 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/securityexemption.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1091 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/sharenumberrange.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1018 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/stockparent.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      805 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/taxid.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      933 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/terminationwindow.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.347033 pyocf-1.0b1/src/pyocf/types/vesting/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/vesting/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2278 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/vesting/vestingcondition.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1567 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/vesting/vestingconditionportion.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      776 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/vesting/vestingeventtrigger.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1018 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/vesting/vestingperiodindays.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1171 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/vesting/vestingperiodinmonths.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      874 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/vesting/vestingscheduleabsolutetrigger.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1575 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/vesting/vestingschedulerelativetrigger.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      790 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/vesting/vestingstarttrigger.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.331033 pyocf-1.0b1/src/pyocf.egg-info/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1188 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf.egg-info/PKG-INFO
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     9741 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf.egg-info/SOURCES.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf.egg-info/dependency_links.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      163 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf.egg-info/requires.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        6 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf.egg-info/top_level.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf.egg-info/zip-safe
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.347033 pyocf-1.0b1/tests/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.000000 pyocf-1.0b1/tests/__init__.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.347033 pyocf-1.0b1/tests/samples/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    12054 2023-03-15 20:14:42.000000 pyocf-1.0b1/tests/samples/Captable.ocf.zip
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4086 2023-03-15 20:14:42.000000 pyocf-1.0b1/tests/test_basic.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    14197 2023-03-15 20:14:42.000000 pyocf-1.0b1/tests/test_load.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1529 2023-03-15 20:14:42.000000 pyocf-1.0b1/tests/test_save.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.347033 pyocf-1.0b1/utils/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      399 2023-03-15 20:14:42.000000 pyocf-1.0b1/utils/enum.mako
+-rwxrwxr-x   0 lregebro  (1000) lregebro  (1000)    14740 2023-03-15 20:14:42.000000 pyocf-1.0b1/utils/generate.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      723 2023-03-15 20:14:42.000000 pyocf-1.0b1/utils/object.mako
```

### Comparing `pyocf-1.0.1/LICENSE.txt` & `pyocf-1.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyocf-1.0.1/Makefile` & `pyocf-1.0b1/Makefile`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,56 @@
 root_dir := $(shell dirname $(realpath $(lastword $(MAKEFILE_LIST))))
-ifdef NO_VENV
-bin_dir :=
-python_exe := python3
-endif
-ifndef NO_VENV
-bin_dir := $(root_dir)/ve/bin/
-python_exe := $(bin_dir)python3
-endif
+bin_dir := $(root_dir)/ve/bin
 git_source := https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF.git
-git_branch := release-v1.0.0
+git_branch := main
 
 all: devenv fetch build
 
 build: generate check docs
 
 # The fullrelease script is a part of zest.releaser, which is the last
 # package installed, so if it exists, the devenv is installed.
-devenv:	$(bin_dir)fullrelease
+devenv:	ve/bin/fullrelease
 
-$(bin_dir):
+ve/bin/fullrelease:
 	virtualenv ve --python python3.9
-
-$(bin_dir)fullrelease: $(bin_dir)
-	$(python_exe) -m pip install -e .[build]
+	$(bin_dir)/pip install -e .[build]
 
 fetch: Open-Cap-Format-OCF update
 
 Open-Cap-Format-OCF:
 	git clone $(git_source)
 
 update:
 	cd Open-Cap-Format-OCF; \
 	git checkout $(git_branch); \
 	git pull
 
 generate:
-	$(bin_dir)python3 utils/generate.py
-	$(bin_dir)black src/
+	$(bin_dir)/python3 utils/generate.py
+	$(bin_dir)/black src/
 
 check:
-	$(bin_dir)black src utils tests docs
-	$(bin_dir)flake8 src utils tests docs
-	$(bin_dir)pyroma -d .
+	$(bin_dir)/black src utils tests
+	$(bin_dir)/flake8 src utils tests
+	$(bin_dir)/pyroma -d .
 
 coverage:
-	$(bin_dir)coverage run $(bin_dir)pytest
-	$(bin_dir)coverage html
-	$(bin_dir)coverage report
+	$(bin_dir)/coverage run $(bin_dir)/pytest
+	$(bin_dir)/coverage html
+	$(bin_dir)/coverage report
 
 .PHONY: docs
 docs:
 	cd ./docs; make html doctest
 
-Open-Cap-Format-OCF/samples/*.json: devenv fetch generate
-
 tests/samples/Captable.ocf.zip: Open-Cap-Format-OCF/samples/*.json
 	zip -j tests/samples/Captable.ocf.zip Open-Cap-Format-OCF/samples/*.json
 
 test: tests/samples/Captable.ocf.zip
-	$(bin_dir)pytest
+	$(bin_dir)/pytest
 
 release:
-	$(bin_dir)fullrelease
+	$(bin_dir)/fullrelease
 
 clean:
 	rm -rf Open-Cap-Format-OCF ve .coverage htmlcov build .pytest_cache docs/source/generated docs/build
```

### Comparing `pyocf-1.0.1/setup.cfg` & `pyocf-1.0b1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 [metadata]
 name = pyocf
-version = 1.0.1
+version = 1.0b1
 description = Open Captable Format objects and parser
 long_description = file: README.rst, CONTRIBUTORS.txt, CHANGES.txt
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3 :: Only
 	Topic :: Office/Business :: Financial
 keywords = captable, ocf
 author = Lennart Regebro
-author_email = lennart.regebro@fidelity.com
+author_email = lregebro@shoobx.com
+url = https://open-cap-table-coalition.github.io/Open-Cap-Format-OCF/
 license = MIT
-project_urls = 
-	Documentation = https://pyocf.readthedocs.io/
-	Source Code = https://github.com/Shoobx/pyocf
-	OCF = https://open-cap-table-coalition.github.io/Open-Cap-Format-OCF/
 
 [options]
-python_requires = >=3.9
+python_requires = >3.9
 install_requires = 
 	setuptools
 	pydantic >= 1.10.0
 zip_safe = True
 include_package_data = True
 packages = find:
 package_dir = 
@@ -53,14 +49,14 @@
 	sphinx_rtd_theme
 	zest.releaser[recommended]
 
 [bdist_wheel]
 universal = 1
 
 [flake8]
-max-line-length = 120
+max-line-length = 90
 ignore = F722, W503
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pyocf-1.0.1/src/pyocf/captable.py` & `pyocf-1.0b1/src/pyocf/captable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 """OCF Captable object"""
-
-# Copyright © 2023 FMR LLC
-
 import datetime
 import hashlib
 import json
 import pathlib
 import zipfile
 
 from packaging import version
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/accrualperiodtype.py` & `pyocf-1.0b1/src/pyocf/enums/periodtype.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-"""Enumeration of interest accrual period types"""
+"""Enumeration of time period types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/AccrualPeriodType.schema.json
+# OCF/tree/main/schema/enums/PeriodType.schema.json
 
 from enum import Enum
 
 
-class AccrualPeriodType(Enum):
-    """Enumeration of interest accrual period types"""
+class PeriodType(Enum):
+    """Enumeration of time period types"""
 
-    ENUM_DAILY = "DAILY"
-    ENUM_MONTHLY = "MONTHLY"
-    ENUM_QUARTERLY = "QUARTERLY"
-    ENUM_SEMI_ANNUAL = "SEMI_ANNUAL"
-    ENUM_ANNUAL = "ANNUAL"
+    ENUM_DAYS = "DAYS"
+    ENUM_MONTHS = "MONTHS"
+    ENUM_YEARS = "YEARS"
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/addresstype.py` & `pyocf-1.0b1/src/pyocf/enums/addresstype.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of address types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/AddressType.schema.json
+# OCF/tree/main/schema/enums/AddressType.schema.json
 
 from enum import Enum
 
 
 class AddressType(Enum):
     """Enumeration of address types"""
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/allocationtype.py` & `pyocf-1.0b1/src/pyocf/enums/allocationtype.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,16 @@
-"""Enumeration of allocation types for vesting terms. Using an example of 18 shares
-split across 4 tranches, each allocation type results in a different schedule as
-follows:
-  1.  Cumulative Rounding (5 - 4 - 5 - 4)
-  2.  Cumulative Round Down (4 - 5 - 4 - 5)
-  3.  Front Loaded (5 - 5 - 4 - 4)
-  4.  Back Loaded (4 - 4 - 5 - 5)
-  5.  Front Loaded to Single Tranche (6 - 4 - 4 - 4)
-  6.  Back Loaded to Single Tranche (4 - 4 - 4 - 6)
-  7.  Fractional (4.5 - 4.5 - 4.5 - 4.5)"""
+"""Enumeration of allocation types for vesting terms. Using an example of 18 shares"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/AllocationType.schema.json
+# OCF/tree/main/schema/enums/AllocationType.schema.json
 
 from enum import Enum
 
 
 class AllocationType(Enum):
     """Enumeration of allocation types for vesting terms. Using an example of 18 shares
     split across 4 tranches, each allocation type results in a different schedule as
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/compensationtype.py` & `pyocf-1.0b1/src/pyocf/enums/compensationtype.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of stock compensation types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/CompensationType.schema.json
+# OCF/tree/main/schema/enums/CompensationType.schema.json
 
 from enum import Enum
 
 
 class CompensationType(Enum):
     """Enumeration of stock compensation types"""
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/compoundingtype.py` & `pyocf-1.0b1/src/pyocf/enums/optiontype.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-"""Enumeration of interest compounding types"""
+"""Enumeration of option types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/CompoundingType.schema.json
+# OCF/tree/main/schema/enums/OptionType.schema.json
 
 from enum import Enum
 
 
-class CompoundingType(Enum):
-    """Enumeration of interest compounding types"""
+class OptionType(Enum):
+    """Enumeration of option types"""
 
-    ENUM_COMPOUNDING = "COMPOUNDING"
-    ENUM_SIMPLE = "SIMPLE"
+    ENUM_NSO = "NSO"
+    ENUM_ISO = "ISO"
+    ENUM_INTL = "INTL"
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/conversionmechanismtype.py` & `pyocf-1.0b1/src/pyocf/enums/conversionmechanismtype.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of convertible conversion calculation types."""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/ConversionMechanismType.schema.json
+# OCF/tree/main/schema/enums/ConversionMechanismType.schema.json
 
 from enum import Enum
 
 
 class ConversionMechanismType(Enum):
     """Enumeration of convertible conversion calculation types."""
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/conversiontimingtype.py` & `pyocf-1.0b1/src/pyocf/enums/conversiontimingtype.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Enumeration of convertible conversion timing for calculation purposes (e.g. does
-the instrument convert based on pre or post money)."""
+"""Enumeration of convertible conversion timing for calculation purposes (e.g. does"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/ConversionTimingType.schema.json
+# OCF/tree/main/schema/enums/ConversionTimingType.schema.json
 
 from enum import Enum
 
 
 class ConversionTimingType(Enum):
     """Enumeration of convertible conversion timing for calculation purposes (e.g. does
     the instrument convert based on pre or post money).
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/conversiontriggertype.py` & `pyocf-1.0b1/src/pyocf/enums/conversiontriggertype.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-"""Enumeration of types of triggers common to various legal rights - e.g. does the
-satisfaction of a condition trigger an automatic conversion or merely a right to
-convert? If `UNSPECIFIED`, the system of record cannot represent this data in a
-structured form."""
+"""Enumeration of types of triggers common to various legal rights - e.g. does the"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/ConversionTriggerType.schema.json
+# OCF/tree/main/schema/enums/ConversionTriggerType.schema.json
 
 from enum import Enum
 
 
 class ConversionTriggerType(Enum):
     """Enumeration of types of triggers common to various legal rights - e.g. does the
     satisfaction of a condition trigger an automatic conversion or merely a right to
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/convertibletype.py` & `pyocf-1.0b1/src/pyocf/enums/phonetype.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-"""Enumeration of convertible instrument types"""
+"""Enumeration of phone number types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/ConvertibleType.schema.json
+# OCF/tree/main/schema/enums/PhoneType.schema.json
 
 from enum import Enum
 
 
-class ConvertibleType(Enum):
-    """Enumeration of convertible instrument types"""
+class PhoneType(Enum):
+    """Enumeration of phone number types"""
 
-    ENUM_NOTE = "NOTE"
-    ENUM_SAFE = "SAFE"
-    ENUM_CONVERTIBLE_SECURITY = "CONVERTIBLE_SECURITY"
+    ENUM_HOME = "HOME"
+    ENUM_MOBILE = "MOBILE"
+    ENUM_BUSINESS = "BUSINESS"
+    ENUM_OTHER = "OTHER"
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/daycounttype.py` & `pyocf-1.0b1/src/pyocf/enums/daycounttype.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of how the number of days are determined per period"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/DayCountType.schema.json
+# OCF/tree/main/schema/enums/DayCountType.schema.json
 
 from enum import Enum
 
 
 class DayCountType(Enum):
     """Enumeration of how the number of days are determined per period"""
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/emailtype.py` & `pyocf-1.0b1/src/pyocf/enums/emailtype.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of email types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/EmailType.schema.json
+# OCF/tree/main/schema/enums/EmailType.schema.json
 
 from enum import Enum
 
 
 class EmailType(Enum):
     """Enumeration of email types"""
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/filetype.py` & `pyocf-1.0b1/src/pyocf/enums/filetype.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Enumeration of different OCF file types which are used to load proper schemas
-for validation"""
+"""Enumeration of different OCF file types which are used to load proper schemas"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/FileType.schema.json
+# OCF/tree/main/schema/enums/FileType.schema.json
 
 from enum import Enum
 
 
 class FileType(Enum):
     """Enumeration of different OCF file types which are used to load proper schemas
     for validation
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/objecttype.py` & `pyocf-1.0b1/src/pyocf/enums/objecttype.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of object types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/ObjectType.schema.json
+# OCF/tree/main/schema/enums/ObjectType.schema.json
 
 from enum import Enum
 
 
 class ObjectType(Enum):
     """Enumeration of object types"""
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/ocfversiontype.py` & `pyocf-1.0b1/src/pyocf/enums/ocfversiontype.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of recognized OCF versions"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/OCFVersionType.schema.json
+# OCF/tree/main/schema/enums/OCFVersionType.schema.json
 
 from enum import Enum
 
 
 class OCFVersionType(Enum):
     """Enumeration of recognized OCF versions"""
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/parentsecuritytype.py` & `pyocf-1.0b1/src/pyocf/enums/parentsecuritytype.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of parent sources a stock can be issued or created from"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/ParentSecurityType.schema.json
+# OCF/tree/main/schema/enums/ParentSecurityType.schema.json
 
 from enum import Enum
 
 
 class ParentSecurityType(Enum):
     """Enumeration of parent sources a stock can be issued or created from"""
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/periodtype.py` & `pyocf-1.0b1/src/pyocf/enums/stakeholdertype.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-"""Enumeration of time period types"""
+"""Enumeration of stakeholder types - individual (human) or institution (entity)"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/PeriodType.schema.json
+# OCF/tree/main/schema/enums/StakeholderType.schema.json
 
 from enum import Enum
 
 
-class PeriodType(Enum):
-    """Enumeration of time period types"""
+class StakeholderType(Enum):
+    """Enumeration of stakeholder types - individual (human) or institution (entity)"""
 
-    ENUM_DAYS = "DAYS"
-    ENUM_MONTHS = "MONTHS"
-    ENUM_YEARS = "YEARS"
+    ENUM_INDIVIDUAL = "INDIVIDUAL"
+    ENUM_INSTITUTION = "INSTITUTION"
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/phonetype.py` & `pyocf-1.0b1/src/pyocf/enums/stockclasstype.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-"""Enumeration of phone number types"""
+"""Enumeration of stock class types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/PhoneType.schema.json
+# OCF/tree/main/schema/enums/StockClassType.schema.json
 
 from enum import Enum
 
 
-class PhoneType(Enum):
-    """Enumeration of phone number types"""
+class StockClassType(Enum):
+    """Enumeration of stock class types"""
 
-    ENUM_HOME = "HOME"
-    ENUM_MOBILE = "MOBILE"
-    ENUM_BUSINESS = "BUSINESS"
-    ENUM_OTHER = "OTHER"
+    ENUM_COMMON = "COMMON"
+    ENUM_PREFERRED = "PREFERRED"
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/roundingtype.py` & `pyocf-1.0b1/src/pyocf/enums/roundingtype.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of rounding types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/RoundingType.schema.json
+# OCF/tree/main/schema/enums/RoundingType.schema.json
 
 from enum import Enum
 
 
 class RoundingType(Enum):
     """Enumeration of rounding types"""
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/stakeholderrelationshiptype.py` & `pyocf-1.0b1/src/pyocf/enums/stakeholderrelationshiptype.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of types of relationships between stakeholder and issuer"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/StakeholderRelationshipType.schema.json
+# OCF/tree/main/schema/enums/StakeholderRelationshipType.schema.json
 
 from enum import Enum
 
 
 class StakeholderRelationshipType(Enum):
     """Enumeration of types of relationships between stakeholder and issuer"""
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/stakeholdertype.py` & `pyocf-1.0b1/src/pyocf/enums/interestpayouttype.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-"""Enumeration of stakeholder types - individual (human) or institution (entity)"""
+"""Enumeration of interest payout types (e.g. deferred or cash payment)"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/StakeholderType.schema.json
+# OCF/tree/main/schema/enums/InterestPayoutType.schema.json
 
 from enum import Enum
 
 
-class StakeholderType(Enum):
-    """Enumeration of stakeholder types - individual (human) or institution (entity)"""
+class InterestPayoutType(Enum):
+    """Enumeration of interest payout types (e.g. deferred or cash payment)"""
 
-    ENUM_INDIVIDUAL = "INDIVIDUAL"
-    ENUM_INSTITUTION = "INSTITUTION"
+    ENUM_DEFERRED = "DEFERRED"
+    ENUM_CASH = "CASH"
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/stockclasstype.py` & `pyocf-1.0b1/src/pyocf/enums/compoundingtype.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-"""Enumeration of stock class types"""
+"""Enumeration of interest compounding types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/StockClassType.schema.json
+# OCF/tree/main/schema/enums/CompoundingType.schema.json
 
 from enum import Enum
 
 
-class StockClassType(Enum):
-    """Enumeration of stock class types"""
+class CompoundingType(Enum):
+    """Enumeration of interest compounding types"""
 
-    ENUM_COMMON = "COMMON"
-    ENUM_PREFERRED = "PREFERRED"
+    ENUM_COMPOUNDING = "COMPOUNDING"
+    ENUM_SIMPLE = "SIMPLE"
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/terminationwindowtype.py` & `pyocf-1.0b1/src/pyocf/enums/terminationwindowtype.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of termination window types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/TerminationWindowType.schema.json
+# OCF/tree/main/schema/enums/TerminationWindowType.schema.json
 
 from enum import Enum
 
 
 class TerminationWindowType(Enum):
     """Enumeration of termination window types"""
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/vestingdayofmonth.py` & `pyocf-1.0b1/src/pyocf/enums/vestingdayofmonth.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,23 @@
-"""Enumeration representing a vesting \"day of month\". Since not all months have
-29, 30, or 31 days, this enum requires those values to also specify an overflow
-behavior.
- - `01` - `28` : Day 1, 2... 28 of the month; e.g. `03` means vesting occurs on
-the 3rd of the month.
- - `29_OR_LAST_DAY_OF_MONTH` - `31_OR_LAST_DAY_OF_MONTH` : Day 29, 30, or 31 of
-the month, defaulting to the last day of the month for shorter months; e.g.
-`31_OR_LAST_DAY_OF_MONTH` means monthly vesting occurs on Jan 31, Feb 28/29, Mar
-31, Apr 30, etc.
- - `VESTING_START_DAY_OR_LAST_DAY_OF_MONTH` vests on the same day of month as
-the day of the `VESTING_START` condition; e.g. if vesting commences on Jan 15
-then any vesting will accrue on the 15th of future vesting months. If vesting
-commencement occurs on days 29-31, this has the same behavior as the other
-`*_LAST_DAY_OF_MONTH` values."""
+"""Enumeration representing a vesting "day of month". Since not all months have 29,"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/VestingDayOfMonth.schema.json
+# OCF/tree/main/schema/enums/VestingDayOfMonth.schema.json
 
 from enum import Enum
 
 
 class VestingDayOfMonth(Enum):
-    """Enumeration representing a vesting \"day of month\". Since not all months have
-    29, 30, or 31 days, this enum requires those values to also specify an overflow
+    """Enumeration representing a vesting "day of month". Since not all months have 29,
+    30, or 31 days, this enum requires those values to also specify an overflow
     behavior.
      - `01` - `28` : Day 1, 2... 28 of the month; e.g. `03` means vesting occurs on
     the 3rd of the month.
      - `29_OR_LAST_DAY_OF_MONTH` - `31_OR_LAST_DAY_OF_MONTH` : Day 29, 30, or 31 of
     the month, defaulting to the last day of the month for shorter months; e.g.
     `31_OR_LAST_DAY_OF_MONTH` means monthly vesting occurs on Jan 31, Feb 28/29, Mar
     31, Apr 30, etc.
```

### Comparing `pyocf-1.0.1/src/pyocf/enums/vestingtriggertype.py` & `pyocf-1.0b1/src/pyocf/enums/vestingtriggertype.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of vesting trigger types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/VestingTriggerType.schema.json
+# OCF/tree/main/schema/enums/VestingTriggerType.schema.json
 
 from enum import Enum
 
 
 class VestingTriggerType(Enum):
     """Enumeration of vesting trigger types"""
```

### Comparing `pyocf-1.0.1/src/pyocf/files/stakeholdersfile.py` & `pyocf-1.0b1/src/pyocf/files/stakeholdersfile.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 """JSON containing file type identifier and list of stakeholders"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/files/StakeholdersFile.schema.json
+# OCF/tree/main/schema/files/StakeholdersFile.schema.json
 
-from pydantic import Field
 from pyocf.objects.stakeholder import Stakeholder
 from pyocf.primitives.files.file import FileObject
-from typing import Annotated
 from typing import Literal
 
 
 class StakeholdersFile(FileObject):
     """JSON containing file type identifier and list of stakeholders"""
 
-    items: Annotated[
-        list[Stakeholder], Field(description="List of OCF stakeholder objects")
-    ]
-    file_type: Annotated[
-        Literal["OCF_STAKEHOLDERS_FILE"], Field(description="")
-    ] = "OCF_STAKEHOLDERS_FILE"
+    # List of OCF stakeholder objects
+    items: list[Stakeholder]
+    file_type: Literal["OCF_STAKEHOLDERS_FILE"] = "OCF_STAKEHOLDERS_FILE"
```

### Comparing `pyocf-1.0.1/src/pyocf/files/stocklegendtemplatesfile.py` & `pyocf-1.0b1/src/pyocf/files/stocklegendtemplatesfile.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 """JSON containing file type identifier and list of stock legend templates"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/files/StockLegendTemplatesFile.schema.json
+# OCF/tree/main/schema/files/StockLegendTemplatesFile.schema.json
 
-from pydantic import Field
 from pyocf.objects.stocklegendtemplate import StockLegendTemplate
 from pyocf.primitives.files.file import FileObject
-from typing import Annotated
 from typing import Literal
 
 
 class StockLegendTemplatesFile(FileObject):
     """JSON containing file type identifier and list of stock legend templates"""
 
-    items: Annotated[
-        list[StockLegendTemplate],
-        Field(description="List of OCF stock legend template objects"),
-    ]
-    file_type: Annotated[
-        Literal["OCF_STOCK_LEGEND_TEMPLATES_FILE"], Field(description="")
+    # List of OCF stock legend template objects
+    items: list[StockLegendTemplate]
+    file_type: Literal[
+        "OCF_STOCK_LEGEND_TEMPLATES_FILE"
     ] = "OCF_STOCK_LEGEND_TEMPLATES_FILE"
```

### Comparing `pyocf-1.0.1/src/pyocf/files/stockplansfile.py` & `pyocf-1.0b1/src/pyocf/files/stockplansfile.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 """JSON containing file type identifier and list of stock plans"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/files/StockPlansFile.schema.json
+# OCF/tree/main/schema/files/StockPlansFile.schema.json
 
-from pydantic import Field
 from pyocf.objects.stockplan import StockPlan
 from pyocf.primitives.files.file import FileObject
-from typing import Annotated
 from typing import Literal
 
 
 class StockPlansFile(FileObject):
     """JSON containing file type identifier and list of stock plans"""
 
-    items: Annotated[
-        list[StockPlan], Field(description="List of OCF stock plan objects")
-    ]
-    file_type: Annotated[
-        Literal["OCF_STOCK_PLANS_FILE"], Field(description="")
-    ] = "OCF_STOCK_PLANS_FILE"
+    # List of OCF stock plan objects
+    items: list[StockPlan]
+    file_type: Literal["OCF_STOCK_PLANS_FILE"] = "OCF_STOCK_PLANS_FILE"
```

### Comparing `pyocf-1.0.1/src/pyocf/files/transactionsfile.py` & `pyocf-1.0b1/src/pyocf/files/transactionsfile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """JSON containing file type identifier and list transactions"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/files/TransactionsFile.schema.json
+# OCF/tree/main/schema/files/TransactionsFile.schema.json
 
 from pydantic import Field
 from pyocf.objects.transactions.acceptance.convertibleacceptance import (
     ConvertibleAcceptance,
 )
 from pyocf.objects.transactions.acceptance.plansecurityacceptance import (
     PlanSecurityAcceptance,
@@ -76,54 +76,50 @@
 from typing import Literal
 from typing import Union
 
 
 class TransactionsFile(FileObject):
     """JSON containing file type identifier and list transactions"""
 
-    items: Annotated[
-        list[
-            Annotated[
-                Union[
-                    ConvertibleAcceptance,
-                    PlanSecurityAcceptance,
-                    StockAcceptance,
-                    WarrantAcceptance,
-                    ConvertibleCancellation,
-                    PlanSecurityCancellation,
-                    StockCancellation,
-                    WarrantCancellation,
-                    ConvertibleConversion,
-                    StockConversion,
-                    PlanSecurityExercise,
-                    WarrantExercise,
-                    ConvertibleIssuance,
-                    PlanSecurityIssuance,
-                    StockIssuance,
-                    WarrantIssuance,
-                    StockReissuance,
-                    StockRepurchase,
-                    PlanSecurityRelease,
-                    ConvertibleRetraction,
-                    PlanSecurityRetraction,
-                    StockRetraction,
-                    WarrantRetraction,
-                    StockClassSplit,
-                    StockClassConversionRatioAdjustment,
-                    StockClassAuthorizedSharesAdjustment,
-                    ConvertibleTransfer,
-                    PlanSecurityTransfer,
-                    StockTransfer,
-                    WarrantTransfer,
-                    VestingAcceleration,
-                    VestingStart,
-                    VestingEvent,
-                    StockPlanPoolAdjustment,
-                ],
-                Field(discriminator="object_type"),
-            ]
-        ],
-        Field(description="List of OCF transaction objects"),
+    # List of OCF transaction objects
+    items: list[
+        Annotated[
+            Union[
+                ConvertibleAcceptance,
+                PlanSecurityAcceptance,
+                StockAcceptance,
+                WarrantAcceptance,
+                ConvertibleCancellation,
+                PlanSecurityCancellation,
+                StockCancellation,
+                WarrantCancellation,
+                ConvertibleConversion,
+                StockConversion,
+                PlanSecurityExercise,
+                WarrantExercise,
+                ConvertibleIssuance,
+                PlanSecurityIssuance,
+                StockIssuance,
+                WarrantIssuance,
+                StockReissuance,
+                StockRepurchase,
+                PlanSecurityRelease,
+                ConvertibleRetraction,
+                PlanSecurityRetraction,
+                StockRetraction,
+                WarrantRetraction,
+                StockClassSplit,
+                StockClassConversionRatioAdjustment,
+                StockClassAuthorizedSharesAdjustment,
+                ConvertibleTransfer,
+                PlanSecurityTransfer,
+                StockTransfer,
+                WarrantTransfer,
+                VestingAcceleration,
+                VestingStart,
+                VestingEvent,
+                StockPlanPoolAdjustment,
+            ],
+            Field(discriminator="object_type"),
+        ]
     ]
-    file_type: Annotated[
-        Literal["OCF_TRANSACTIONS_FILE"], Field(description="")
-    ] = "OCF_TRANSACTIONS_FILE"
+    file_type: Literal["OCF_TRANSACTIONS_FILE"] = "OCF_TRANSACTIONS_FILE"
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/acceptance/convertibleacceptance.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/transfer/convertibletransfer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,51 @@
-"""Object describing a convertible acceptance transaction"""
+"""Object describing a transfer or secondary sale of a convertible security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/acceptance/ConvertibleAcceptance.schema.j
-# son
+# ree/main/schema/objects/transactions/transfer/ConvertibleTransfer.schema.json
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
-from pyocf.primitives.objects.transactions.acceptance.acceptance import Acceptance
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
+from pyocf.primitives.objects.transactions.transfer.transfer import Transfer
 from pyocf.types.date import Date
-from typing import Annotated
+from pyocf.types.monetary import Monetary
 from typing import Literal
 from typing import Optional
 
 
-class ConvertibleAcceptance(Object, Transaction, SecurityTransaction, Acceptance):
-    """Object describing a convertible acceptance transaction"""
+class ConvertibleTransfer(Object, Transaction, SecurityTransaction, Transfer):
+    """Object describing a transfer or secondary sale of a convertible security"""
 
-    object_type: Annotated[
-        Literal["TX_CONVERTIBLE_ACCEPTANCE"], Field(description="")
-    ] = "TX_CONVERTIBLE_ACCEPTANCE"
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
+    object_type: Literal["TX_CONVERTIBLE_TRANSFER"] = "TX_CONVERTIBLE_TRANSFER"
+    # Amount of monetary value transferred
+    amount: Monetary
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # Unstructured text description of consideration provided in exchange for security
+    # transfer
+    consideration_text: Optional[str]
+    # Identifier for the security that holds the remainder balance (for partial
+    # transfers)
+    balance_security_id: Optional[str]
+    # Array of identifiers for new security (or securities) created as a result of the
+    # transaction
+    resulting_security_ids: list[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/acceptance/plansecurityacceptance.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/release/plansecurityrelease.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,55 @@
-"""Object describing a plan security acceptance transaction"""
+"""Object describing a plan security release transaction"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/acceptance/PlanSecurityAcceptance.schema.
-# json
+# ree/main/schema/objects/transactions/release/PlanSecurityRelease.schema.json
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
-from pyocf.primitives.objects.transactions.acceptance.acceptance import Acceptance
+from pyocf.primitives.objects.transactions.release.release import Release
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
-from typing import Annotated
+from pyocf.types.monetary import Monetary
+from pyocf.types.numeric import Numeric
 from typing import Literal
 from typing import Optional
 
 
-class PlanSecurityAcceptance(Object, Transaction, SecurityTransaction, Acceptance):
-    """Object describing a plan security acceptance transaction"""
+class PlanSecurityRelease(Object, Transaction, SecurityTransaction, Release):
+    """Object describing a plan security release transaction"""
 
-    object_type: Annotated[
-        Literal["TX_PLAN_SECURITY_ACCEPTANCE"], Field(description="")
-    ] = "TX_PLAN_SECURITY_ACCEPTANCE"
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
+    object_type: Literal["TX_PLAN_SECURITY_RELEASE"] = "TX_PLAN_SECURITY_RELEASE"
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # The settlement date for the shares released, typically after the release
+    # transaction date
+    settlement_date: Date
+    # The release price used to determine the value of the security at the time of
+    # release
+    release_price: Monetary
+    # Quantity of shares released
+    quantity: Numeric
+    # Unstructured text description of consideration provided in exchange for security
+    # release
+    consideration_text: Optional[str]
+    # Identifier of the new security (or securities) issuance resulting from a release
+    # transaction
+    resulting_security_ids: list[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/acceptance/stockacceptance.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/acceptance/convertibleacceptance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,40 @@
-"""Object describing a stock acceptance transaction"""
+"""Object describing a convertible acceptance transaction"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/acceptance/StockAcceptance.schema.json
+# ree/main/schema/objects/transactions/acceptance/ConvertibleAcceptance.schema.jso
+# n
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.acceptance.acceptance import Acceptance
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
-from typing import Annotated
 from typing import Literal
 from typing import Optional
 
 
-class StockAcceptance(Object, Transaction, SecurityTransaction, Acceptance):
-    """Object describing a stock acceptance transaction"""
+class ConvertibleAcceptance(Object, Transaction, SecurityTransaction, Acceptance):
+    """Object describing a convertible acceptance transaction"""
 
-    object_type: Annotated[
-        Literal["TX_STOCK_ACCEPTANCE"], Field(description="")
-    ] = "TX_STOCK_ACCEPTANCE"
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
+    object_type: Literal["TX_CONVERTIBLE_ACCEPTANCE"] = "TX_CONVERTIBLE_ACCEPTANCE"
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/acceptance/warrantacceptance.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/transfer/stocktransfer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-"""Object describing a warrant acceptance transaction"""
+"""Object describing a transfer or secondary sale of a stock security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/acceptance/WarrantAcceptance.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
+# OCF/tree/main/schema/objects/transactions/transfer/StockTransfer.schema.json
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
-from pyocf.primitives.objects.transactions.acceptance.acceptance import Acceptance
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
+from pyocf.primitives.objects.transactions.transfer.transfer import Transfer
 from pyocf.types.date import Date
-from typing import Annotated
+from pyocf.types.numeric import Numeric
 from typing import Literal
 from typing import Optional
 
 
-class WarrantAcceptance(Object, Transaction, SecurityTransaction, Acceptance):
-    """Object describing a warrant acceptance transaction"""
+class StockTransfer(Object, Transaction, SecurityTransaction, Transfer):
+    """Object describing a transfer or secondary sale of a stock security"""
 
-    object_type: Annotated[
-        Literal["TX_WARRANT_ACCEPTANCE"], Field(description="")
-    ] = "TX_WARRANT_ACCEPTANCE"
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
+    object_type: Literal["TX_STOCK_TRANSFER"] = "TX_STOCK_TRANSFER"
+    # Quantity of non-monetary security units transferred
+    quantity: Numeric
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # Unstructured text description of consideration provided in exchange for security
+    # transfer
+    consideration_text: Optional[str]
+    # Identifier for the security that holds the remainder balance (for partial
+    # transfers)
+    balance_security_id: Optional[str]
+    # Array of identifiers for new security (or securities) created as a result of the
+    # transaction
+    resulting_security_ids: list[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/adjustment/stockclassauthorizedsharesadjustment.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/adjustment/stockclassauthorizedsharesadjustment.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,43 @@
-"""Object describing an event to change the number of authoried shares of a stock
-class."""
+"""Object describing an event to change the number of authoried shares of a stock"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/adjustment/StockClassAuthorizedSharesAdju
-# stment.schema.json
+# ree/main/schema/objects/transactions/adjustment/StockClassAuthorizedSharesAdjust
+# ment.schema.json
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.stockclasstransaction import (
     StockClassTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
 from pyocf.types.numeric import Numeric
-from typing import Annotated
 from typing import Literal
 from typing import Optional
 
 
 class StockClassAuthorizedSharesAdjustment(Object, Transaction, StockClassTransaction):
     """Object describing an event to change the number of authoried shares of a stock
     class.
     """
 
-    object_type: Annotated[
-        Literal["TX_STOCK_CLASS_AUTHORIZED_SHARES_ADJUSTMENT"], Field(description="")
+    object_type: Literal[
+        "TX_STOCK_CLASS_AUTHORIZED_SHARES_ADJUSTMENT"
     ] = "TX_STOCK_CLASS_AUTHORIZED_SHARES_ADJUSTMENT"
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    stock_class_id: Annotated[
-        str,
-        Field(
-            description="Identifier of the StockClass object, a subject of this transaction"
-        ),
-    ]
-    new_shares_authorized: Annotated[
-        Numeric,
-        Field(
-            description="The new number of shares authorized for this stock class as of the event of this"
-            "transaction"
-        ),
-    ]
-    board_approval_date: Optional[
-        Annotated[
-            Date,
-            Field(
-                description="Date on which the board approved the change to the stock class"
-            ),
-        ]
-    ]
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Date on which the transaction occurred
+    date: Date
+    # Identifier of the StockClass object, a subject of this transaction
+    stock_class_id: str
+    # The new number of shares authorized for this stock class as of the event of this
+    # transaction
+    new_shares_authorized: Numeric
+    # Date on which the board approved the change to the stock class
+    board_approval_date: Optional[Date]
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/adjustment/stockclassconversionratioadjustment.py` & `pyocf-1.0b1/src/pyocf/types/conversion_triggers/electiveconversiononconditiontrigger.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,52 @@
-"""Object describing the conversion ratio adjustment of a stock class that has a
-RatioConversionMechanism conversion mechanism where there was an actual
-repricing due to a down-round. The actual determination of the new conversion
-ratio / conversion price is calculated outside of OCF, so the specific mechanism
-- e.g. broad-based weighted-average anti-dilution protection vs. full ratchet
-anti-dilution protection."""
+"""Type representation of elective trigger on fulfillment of a condition."""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/adjustment/StockClassConversionRatioAdjus
-# tment.schema.json
+# ree/main/schema/types/conversion_triggers/ElectiveConversionOnConditionTrigger.s
+# chema.json
 
 from pydantic import Field
-from pyocf.primitives.objects.object import Object
-from pyocf.primitives.objects.transactions.stockclasstransaction import (
-    StockClassTransaction,
+from pyocf.primitives.types.conversion_triggers.conversiontrigger import (
+    ConversionTrigger,
 )
-from pyocf.primitives.objects.transactions.transaction import Transaction
-from pyocf.types.conversion_mechanisms.ratioconversionmechanism import (
-    RatioConversionMechanism,
+from pyocf.types.conversion_rights.convertibleconversionright import (
+    ConvertibleConversionRight,
 )
-from pyocf.types.date import Date
+from pyocf.types.conversion_rights.stockclassconversionright import (
+    StockClassConversionRight,
+)
+from pyocf.types.conversion_rights.warrantconversionright import WarrantConversionRight
 from typing import Annotated
 from typing import Literal
 from typing import Optional
+from typing import Union
 
 
-class StockClassConversionRatioAdjustment(Object, Transaction, StockClassTransaction):
-    """Object describing the conversion ratio adjustment of a stock class that has a
-    RatioConversionMechanism conversion mechanism where there was an actual
-    repricing due to a down-round. The actual determination of the new conversion
-    ratio / conversion price is calculated outside of OCF, so the specific mechanism
-    - e.g. broad-based weighted-average anti-dilution protection vs. full ratchet
-    anti-dilution protection.
-    """
+class ElectiveConversionOnConditionTrigger(ConversionTrigger):
+    """Type representation of elective trigger on fulfillment of a condition."""
 
-    object_type: Annotated[
-        Literal["TX_STOCK_CLASS_CONVERSION_RATIO_ADJUSTMENT"], Field(description="")
-    ] = "TX_STOCK_CLASS_CONVERSION_RATIO_ADJUSTMENT"
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    stock_class_id: Annotated[
-        str,
-        Field(
-            description="Identifier of the StockClass object, a subject of this transaction"
-        ),
-    ]
-    new_ratio_conversion_mechanism: Annotated[
-        RatioConversionMechanism,
-        Field(
-            description="New conversion ratio mechanism describing new conversion price and conversion"
-            "ratio in effect following a repricing - based on original issue price to new"
-            "conversion price (provided in this transaction). For 2-for-1 split the numerator"
-            "of the ratio is 2 and the denominator is 1."
-        ),
+    # Legal language describing what conditions must be satisfied for the conversion
+    # to take place (ideally, this should be excerpted from the instrument where
+    # possible)
+    trigger_condition: str
+    # Id for this conversion trigger, unique within list of ConversionTriggers in
+    # parent convertible issuance's `conversion_triggers` field.
+    trigger_id: str
+    # Human-friendly nickname to describe the conversion right
+    nickname: Optional[str]
+    # Long-form description of the trigger
+    trigger_description: Optional[str]
+    type: Literal["ELECTIVE_ON_CONDITION"] = "ELECTIVE_ON_CONDITION"
+    # When the conditions of the trigger are met, how does the convertible convert?
+    conversion_right: Annotated[
+        Union[
+            ConvertibleConversionRight,
+            WarrantConversionRight,
+            StockClassConversionRight,
+        ],
+        Field(discriminator="type"),
     ]
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/adjustment/stockplanpooladjustment.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/adjustment/stockplanpooladjustment.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,46 @@
 """Object describing the change in the size of a Stock Plan pool."""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/adjustment/StockPlanPoolAdjustment.schema
-# .json
+# ree/main/schema/objects/transactions/adjustment/StockPlanPoolAdjustment.schema.j
+# son
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.stockplantransaction import (
     StockPlanTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
 from pyocf.types.numeric import Numeric
-from typing import Annotated
 from typing import Literal
 from typing import Optional
 
 
 class StockPlanPoolAdjustment(Object, Transaction, StockPlanTransaction):
     """Object describing the change in the size of a Stock Plan pool."""
 
-    object_type: Annotated[
-        Literal["TX_STOCK_PLAN_POOL_ADJUSTMENT"], Field(description="")
+    object_type: Literal[
+        "TX_STOCK_PLAN_POOL_ADJUSTMENT"
     ] = "TX_STOCK_PLAN_POOL_ADJUSTMENT"
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    stock_plan_id: Annotated[
-        str,
-        Field(
-            description="Identifier of the Stock Plan object, a subject of this transaction"
-        ),
-    ]
-    board_approval_date: Annotated[
-        Date, Field(description="Date on which board approved the change to the plan.")
-    ]
-    stockholder_approval_date: Optional[
-        Annotated[
-            Date,
-            Field(
-                description="This optional field tracks when the stockholders approved this change to the"
-                "stock plan. This is intended for use by US companies that want to issue"
-                "Incentive Stock Options (ISOs), as the issuing StockPlan must receive"
-                "shareholder approval within a specified time frame in order to issue valid ISOs."
-            ),
-        ]
-    ]
-    shares_reserved: Annotated[
-        Numeric,
-        Field(
-            description="The number of shares reserved in the pool for this stock plan by the Board or"
-            "equivalent body as of the effective date of this pool adjustment."
-        ),
-    ]
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Date on which the transaction occurred
+    date: Date
+    # Identifier of the Stock Plan object, a subject of this transaction
+    stock_plan_id: str
+    # Date on which board approved the change to the plan.
+    board_approval_date: Date
+    # This optional field tracks when the stockholders approved this change to the
+    # stock plan. This is intended for use by US companies that want to issue
+    # Incentive Stock Options (ISOs), as the issuing StockPlan must receive
+    # shareholder approval within a specified time frame in order to issue valid ISOs.
+    stockholder_approval_date: Optional[Date]
+    # The number of shares reserved in the pool for this stock plan by the Board or
+    # equivalent body as of the effective date of this pool adjustment.
+    shares_reserved: Numeric
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/cancellation/convertiblecancellation.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/vesting/vestingacceleration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,45 @@
-"""Object describing a cancellation of a convertible security"""
+"""Object describing an acceleration of vesting, in which additional shares vest"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/cancellation/ConvertibleCancellation.sche
-# ma.json
+# ree/main/schema/objects/transactions/vesting/VestingAcceleration.schema.json
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
-from pyocf.primitives.objects.transactions.cancellation.cancellation import Cancellation
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
-from pyocf.types.monetary import Monetary
-from typing import Annotated
+from pyocf.types.numeric import Numeric
 from typing import Literal
 from typing import Optional
 
 
-class ConvertibleCancellation(Object, Transaction, SecurityTransaction, Cancellation):
-    """Object describing a cancellation of a convertible security"""
+class VestingAcceleration(Object, Transaction, SecurityTransaction):
+    """Object describing an acceleration of vesting, in which additional shares vest
+    ahead of the schedule specified in security's vesting terms.
+    """
 
-    object_type: Annotated[
-        Literal["TX_CONVERTIBLE_CANCELLATION"], Field(description="")
-    ] = "TX_CONVERTIBLE_CANCELLATION"
-    amount: Annotated[Monetary, Field(description="Amount of monetary value cancelled")]
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    balance_security_id: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Identifier for the security that holds the remainder balance (for partial"
-                "cancellations)"
-            ),
-        ]
-    ]
-    reason_text: Annotated[str, Field(description="Reason for the cancellation")]
+    object_type: Literal["TX_VESTING_ACCELERATION"] = "TX_VESTING_ACCELERATION"
+    # Number of shares vesting ahead of schedule
+    quantity: Numeric
+    # Reason for the acceleration; unstructured text
+    reason_text: str
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Date on which the transaction occurred
+    date: Date
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/cancellation/plansecuritycancellation.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/cancellation/warrantcancellation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,48 @@
-"""Object describing a cancellation of a plan security"""
+"""Object describing a cancellation of a warrant security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/cancellation/PlanSecurityCancellation.sch
-# ema.json
+# ree/main/schema/objects/transactions/cancellation/WarrantCancellation.schema.jso
+# n
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.cancellation.cancellation import Cancellation
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
 from pyocf.types.numeric import Numeric
-from typing import Annotated
 from typing import Literal
 from typing import Optional
 
 
-class PlanSecurityCancellation(Object, Transaction, SecurityTransaction, Cancellation):
-    """Object describing a cancellation of a plan security"""
+class WarrantCancellation(Object, Transaction, SecurityTransaction, Cancellation):
+    """Object describing a cancellation of a warrant security"""
 
-    object_type: Annotated[
-        Literal["TX_PLAN_SECURITY_CANCELLATION"], Field(description="")
-    ] = "TX_PLAN_SECURITY_CANCELLATION"
-    quantity: Annotated[
-        Numeric, Field(description="Quantity of non-monetary security units cancelled")
-    ]
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    balance_security_id: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Identifier for the security that holds the remainder balance (for partial"
-                "cancellations)"
-            ),
-        ]
-    ]
-    reason_text: Annotated[str, Field(description="Reason for the cancellation")]
+    object_type: Literal["TX_WARRANT_CANCELLATION"] = "TX_WARRANT_CANCELLATION"
+    # Quantity of non-monetary security units cancelled
+    quantity: Numeric
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # Identifier for the security that holds the remainder balance (for partial
+    # cancellations)
+    balance_security_id: Optional[str]
+    # Reason for the cancellation
+    reason_text: str
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/cancellation/stockcancellation.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/cancellation/convertiblecancellation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,48 @@
-"""Object describing a cancellation of a stock security"""
+"""Object describing a cancellation of a convertible security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/cancellation/StockCancellation.schema.jso
-# n
+# ree/main/schema/objects/transactions/cancellation/ConvertibleCancellation.schema
+# .json
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.cancellation.cancellation import Cancellation
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
-from pyocf.types.numeric import Numeric
-from typing import Annotated
+from pyocf.types.monetary import Monetary
 from typing import Literal
 from typing import Optional
 
 
-class StockCancellation(Object, Transaction, SecurityTransaction, Cancellation):
-    """Object describing a cancellation of a stock security"""
+class ConvertibleCancellation(Object, Transaction, SecurityTransaction, Cancellation):
+    """Object describing a cancellation of a convertible security"""
 
-    object_type: Annotated[
-        Literal["TX_STOCK_CANCELLATION"], Field(description="")
-    ] = "TX_STOCK_CANCELLATION"
-    quantity: Annotated[
-        Numeric, Field(description="Quantity of non-monetary security units cancelled")
-    ]
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    balance_security_id: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Identifier for the security that holds the remainder balance (for partial"
-                "cancellations)"
-            ),
-        ]
-    ]
-    reason_text: Annotated[str, Field(description="Reason for the cancellation")]
+    object_type: Literal["TX_CONVERTIBLE_CANCELLATION"] = "TX_CONVERTIBLE_CANCELLATION"
+    # Amount of monetary value cancelled
+    amount: Monetary
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # Identifier for the security that holds the remainder balance (for partial
+    # cancellations)
+    balance_security_id: Optional[str]
+    # Reason for the cancellation
+    reason_text: str
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/conversion/convertibleconversion.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/issuance/plansecurityissuance.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,93 +1,90 @@
-"""Object describing a conversion of a convertible security"""
+"""Object describing securities issuance transaction from a plan by the issuer and"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/conversion/ConvertibleConversion.schema.j
-# son
+# ree/main/schema/objects/transactions/issuance/PlanSecurityIssuance.schema.json
 
-from pydantic import Field
+from pydantic import root_validator
+from pyocf.enums.compensationtype import CompensationType
+from pyocf.enums.optiontype import OptionType
 from pyocf.primitives.objects.object import Object
-from pyocf.primitives.objects.transactions.conversion.conversion import Conversion
+from pyocf.primitives.objects.transactions.issuance.issuance import Issuance
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
-from pyocf.types.capitalizationdefinition import CapitalizationDefinition
 from pyocf.types.date import Date
+from pyocf.types.monetary import Monetary
 from pyocf.types.numeric import Numeric
-from typing import Annotated
+from pyocf.types.securityexemption import SecurityExemption
+from pyocf.types.terminationwindow import TerminationWindow
 from typing import Literal
 from typing import Optional
+from typing import Union
 
 
-class ConvertibleConversion(Object, Transaction, SecurityTransaction, Conversion):
-    """Object describing a conversion of a convertible security"""
+class PlanSecurityIssuance(Object, Transaction, SecurityTransaction, Issuance):
+    """Object describing securities issuance transaction from a plan by the issuer and
+    held by a stakeholder
+    """
 
-    object_type: Annotated[
-        Literal["TX_CONVERTIBLE_CONVERSION"], Field(description="")
-    ] = "TX_CONVERTIBLE_CONVERSION"
-    reason_text: Annotated[str, Field(description="Reason for the conversion")]
-    quantity_converted: Optional[
-        Annotated[Numeric, Field(description="Quantity of security units converted")]
-    ]
-    balance_security_id: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Identifier for the convertible that holds the remainder balance (for partial"
-                "conversions)"
-            ),
-        ]
-    ]
-    trigger_id: Annotated[
-        str,
-        Field(
-            description="What is the id of the convertible's conversion trigger that resulted in this"
-            "conversion"
-        ),
-    ]
-    capitalization_definition: Optional[
-        Annotated[
-            CapitalizationDefinition,
-            Field(
-                description="If this conversion event and its `quantity_converted` value was based on the"
-                "company's capitalization, please specify what stock classes, stock plans and"
-                "securities were aggregated to calculate the capitalization value used in the"
-                'calculation (e.g. if it was based on "fully diluted" capitalization, please'
-                "provide details on how this was calculated using the capitalization type"
-                "datastructure)."
-            ),
-        ]
-    ]
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    resulting_security_ids: Annotated[
-        list[str],
-        Field(
-            description="Identifier for the security (or securities) that resulted from the conversion"
-        ),
-    ]
+    object_type: Literal["TX_PLAN_SECURITY_ISSUANCE"] = "TX_PLAN_SECURITY_ISSUANCE"
+    # Identifier of StockPlan the PlanSecurities were issued from
+    stock_plan_id: str
+    # If the plan security is compensation, what kind?
+    compensation_type: CompensationType
+    # If the plan security is an option, what kind?
+    option_grant_type: Optional[OptionType]
+    # How many shares are subject to this plan security?
+    quantity: Numeric
+    # What is the exercise price?
+    exercise_price: Monetary
+    # Identifier of the VestingTerms to which this security is subject.  If not
+    # present, security is fully vested on issuance.
+    vesting_terms_id: Optional[str]
+    # Expiration date of the plan security
+    expiration_date: Union[None, Date]
+    # Exercise periods applicable to plan security after a termination for a given,
+    # enumerated reason
+    termination_exercise_windows: list[TerminationWindow]
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # A custom ID for this security (e.g. CN-1.)
+    custom_id: str
+    # Identifier for the stakeholder that holds legal title to this security
+    stakeholder_id: str
+    # Date of board approval for the security
+    board_approval_date: Optional[Date]
+    # Unstructured text description of consideration provided in exchange for security
+    # issuance
+    consideration_text: Optional[str]
+    # List of security law exemptions (and applicable jurisdictions) for this security
+    security_law_exemptions: list[SecurityExemption]
+
+    @root_validator(pre=True)
+    def validator_compensation_type(cls, values):
+        if (
+            values.get("compensation_type") == "OPTION"
+            and values.get("option_grant_type") is None
+        ):
+            raise ValueError(
+                "When compensation_type is 'OPTION' then option_grant_type is required"
+            )
+
+        return values
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/conversion/stockconversion.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/conversion/stockconversion.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,47 @@
 """Object describing a conversion of stock"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/conversion/StockConversion.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
+# OCF/tree/main/schema/objects/transactions/conversion/StockConversion.schema.json
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.conversion.conversion import Conversion
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
 from pyocf.types.numeric import Numeric
-from typing import Annotated
 from typing import Literal
 from typing import Optional
 
 
 class StockConversion(Object, Transaction, SecurityTransaction, Conversion):
     """Object describing a conversion of stock"""
 
-    object_type: Annotated[
-        Literal["TX_STOCK_CONVERSION"], Field(description="")
-    ] = "TX_STOCK_CONVERSION"
-    balance_security_id: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Identifier for the security that holds the remainder balance (for partial"
-                "conversions)"
-            ),
-        ]
-    ]
-    quantity_converted: Annotated[
-        Numeric, Field(description="Quantity of non-monetary security units converted")
-    ]
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    resulting_security_ids: Annotated[
-        list[str],
-        Field(
-            description="Identifier for the security (or securities) that resulted from the conversion"
-        ),
-    ]
+    object_type: Literal["TX_STOCK_CONVERSION"] = "TX_STOCK_CONVERSION"
+    # Identifier for the security that holds the remainder balance (for partial
+    # conversions)
+    balance_security_id: Optional[str]
+    # Quantity of non-monetary security units converted
+    quantity_converted: Numeric
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # Identifier for the security (or securities) that resulted from the conversion
+    resulting_security_ids: list[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/exercise/plansecurityexercise.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/transfer/warranttransfer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,51 @@
-"""Object describing a plan security exercise transaction"""
+"""Object describing a transfer or secondary sale of a warrant security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/exercise/PlanSecurityExercise.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
+# OCF/tree/main/schema/objects/transactions/transfer/WarrantTransfer.schema.json
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
-from pyocf.primitives.objects.transactions.exercise.exercise import Exercise
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
+from pyocf.primitives.objects.transactions.transfer.transfer import Transfer
 from pyocf.types.date import Date
 from pyocf.types.numeric import Numeric
-from typing import Annotated
 from typing import Literal
 from typing import Optional
 
 
-class PlanSecurityExercise(Object, Transaction, SecurityTransaction, Exercise):
-    """Object describing a plan security exercise transaction"""
+class WarrantTransfer(Object, Transaction, SecurityTransaction, Transfer):
+    """Object describing a transfer or secondary sale of a warrant security"""
 
-    object_type: Annotated[
-        Literal["TX_PLAN_SECURITY_EXERCISE"], Field(description="")
-    ] = "TX_PLAN_SECURITY_EXERCISE"
-    quantity: Annotated[Numeric, Field(description="Quantity of shares exercised")]
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    consideration_text: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Unstructured text description of consideration provided in exchange for security"
-                "exercise"
-            ),
-        ]
-    ]
-    resulting_security_ids: Annotated[
-        list[str],
-        Field(
-            description="Identifier for the security (or securities) that resulted from the exercise"
-        ),
-    ]
+    object_type: Literal["TX_WARRANT_TRANSFER"] = "TX_WARRANT_TRANSFER"
+    # Quantity of non-monetary security units transferred
+    quantity: Numeric
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # Unstructured text description of consideration provided in exchange for security
+    # transfer
+    consideration_text: Optional[str]
+    # Identifier for the security that holds the remainder balance (for partial
+    # transfers)
+    balance_security_id: Optional[str]
+    # Array of identifiers for new security (or securities) created as a result of the
+    # transaction
+    resulting_security_ids: list[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/exercise/warrantexercise.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/retraction/convertibleretraction.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,42 @@
-"""Object describing a warrant exercise transaction"""
+"""Object describing a retraction of a convertible security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/objects/transactions/exercise/WarrantExercise.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
+# ree/main/schema/objects/transactions/retraction/ConvertibleRetraction.schema.jso
+# n
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
-from pyocf.primitives.objects.transactions.exercise.exercise import Exercise
+from pyocf.primitives.objects.transactions.retraction.retraction import Retraction
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
-from typing import Annotated
 from typing import Literal
 from typing import Optional
 
 
-class WarrantExercise(Object, Transaction, SecurityTransaction, Exercise):
-    """Object describing a warrant exercise transaction"""
+class ConvertibleRetraction(Object, Transaction, SecurityTransaction, Retraction):
+    """Object describing a retraction of a convertible security"""
 
-    object_type: Annotated[
-        Literal["TX_WARRANT_EXERCISE"], Field(description="")
-    ] = "TX_WARRANT_EXERCISE"
-    trigger_id: Annotated[
-        str,
-        Field(
-            description="What is the id of the warrant's exercise trigger that resulted in this exercise"
-        ),
-    ]
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    consideration_text: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Unstructured text description of consideration provided in exchange for security"
-                "exercise"
-            ),
-        ]
-    ]
-    resulting_security_ids: Annotated[
-        list[str],
-        Field(
-            description="Identifier for the security (or securities) that resulted from the exercise"
-        ),
-    ]
+    object_type: Literal["TX_CONVERTIBLE_RETRACTION"] = "TX_CONVERTIBLE_RETRACTION"
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # Reason for the retraction
+    reason_text: str
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/issuance/convertibleissuance.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/issuance/convertibleissuance.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Object describing convertible instrument issuance transaction by the issuer and
-held by a stakeholder"""
+"""Object describing convertible instrument issuance transaction by the issuer and"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/issuance/ConvertibleIssuance.schema.json
+# ree/main/schema/objects/transactions/issuance/ConvertibleIssuance.schema.json
 
 from pydantic import Field
 from pyocf.enums.convertibletype import ConvertibleType
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.issuance.issuance import Issuance
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
@@ -46,107 +45,59 @@
 
 
 class ConvertibleIssuance(Object, Transaction, SecurityTransaction, Issuance):
     """Object describing convertible instrument issuance transaction by the issuer and
     held by a stakeholder
     """
 
-    object_type: Annotated[
-        Literal["TX_CONVERTIBLE_ISSUANCE"], Field(description="")
-    ] = "TX_CONVERTIBLE_ISSUANCE"
-    investment_amount: Annotated[
-        Monetary,
-        Field(
-            description="Amount invested and outstanding on date of issuance of this convertible"
-        ),
-    ]
-    convertible_type: Annotated[
-        ConvertibleType,
-        Field(
-            description="What kind of convertible instrument is this (of the supported, enumerated types)"
-        ),
-    ]
-    conversion_triggers: Annotated[
-        list[
-            Annotated[
-                Union[
-                    AutomaticConversionOnConditionTrigger,
-                    AutomaticConversionOnDateTrigger,
-                    ElectiveConversionAtWillTrigger,
-                    ElectiveConversionInDateRangeTrigger,
-                    ElectiveConversionOnConditionTrigger,
-                    UnspecifiedConversionTrigger,
-                ],
-                Field(discriminator="type"),
-            ]
-        ],
-        Field(
-            description="In event the convertible can convert due to trigger events (e.g. Maturity, Next"
-            "Qualified Financing, Change of Control, at Election of Holder), what are the"
-            "terms?"
-        ),
-    ]
-    pro_rata: Optional[
-        Annotated[
-            Numeric,
-            Field(
-                description="What pro-rata (if any) is the holder entitled to buy at the next round?"
-            ),
-        ]
-    ]
-    seniority: Annotated[
-        int,
-        Field(
-            description="If different convertible instruments have seniorty over one another, use this"
-            "value to build a seniority stack, with 1 being highest seniority and equal"
-            "seniority values assumed to be equal priority"
-        ),
-    ]
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
+    object_type: Literal["TX_CONVERTIBLE_ISSUANCE"] = "TX_CONVERTIBLE_ISSUANCE"
+    # Amount invested and outstanding on date of issuance of this convertible
+    investment_amount: Monetary
+    # What kind of convertible instrument is this (of the supported, enumerated types)
+    convertible_type: ConvertibleType
+    # In event the convertible can convert due to trigger events (e.g. Maturity, Next
+    # Qualified Financing, Change of Control, at Election of Holder), what are the
+    # terms?
+    conversion_triggers: list[
         Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
+            Union[
+                AutomaticConversionOnConditionTrigger,
+                AutomaticConversionOnDateTrigger,
+                ElectiveConversionAtWillTrigger,
+                ElectiveConversionInDateRangeTrigger,
+                ElectiveConversionOnConditionTrigger,
+                UnspecifiedConversionTrigger,
+            ],
+            Field(discriminator="type"),
         ]
     ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    custom_id: Annotated[
-        str, Field(description="A custom ID for this security (e.g. CN-1.)")
-    ]
-    stakeholder_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the stakeholder that holds legal title to this security"
-        ),
-    ]
-    board_approval_date: Optional[
-        Annotated[Date, Field(description="Date of board approval for the security")]
-    ]
-    consideration_text: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Unstructured text description of consideration provided in exchange for security"
-                "issuance"
-            ),
-        ]
-    ]
-    security_law_exemptions: Annotated[
-        list[SecurityExemption],
-        Field(
-            description="List of security law exemptions (and applicable jurisdictions) for this security"
-        ),
-    ]
+    # What pro-rata (if any) is the holder entitled to buy at the next round?
+    pro_rata: Optional[Numeric]
+    # If different convertible instruments have seniorty over one another, use this
+    # value to build a seniority stack, with 1 being highest seniority and equal
+    # seniority values assumed to be equal priority
+    seniority: int
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # A custom ID for this security (e.g. CN-1.)
+    custom_id: str
+    # Identifier for the stakeholder that holds legal title to this security
+    stakeholder_id: str
+    # Date of board approval for the security
+    board_approval_date: Optional[Date]
+    # Unstructured text description of consideration provided in exchange for security
+    # issuance
+    consideration_text: Optional[str]
+    # List of security law exemptions (and applicable jurisdictions) for this security
+    security_law_exemptions: list[SecurityExemption]
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/issuance/plansecurityissuance.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/issuance/warrantissuance.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,127 +1,104 @@
-"""Object describing securities issuance transaction from a plan by the issuer and
-held by a stakeholder"""
+"""Object describing warrant issuance transaction by the issuer and held by a"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/issuance/PlanSecurityIssuance.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
+# OCF/tree/main/schema/objects/transactions/issuance/WarrantIssuance.schema.json
 
 from pydantic import Field
-from pyocf.enums.compensationtype import CompensationType
-from pyocf.enums.optiontype import OptionType
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.issuance.issuance import Issuance
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
+from pyocf.types.conversion_triggers.automaticconversiononconditiontrigger import (
+    AutomaticConversionOnConditionTrigger,
+)
+from pyocf.types.conversion_triggers.automaticconversionondatetrigger import (
+    AutomaticConversionOnDateTrigger,
+)
+from pyocf.types.conversion_triggers.electiveconversionatwilltrigger import (
+    ElectiveConversionAtWillTrigger,
+)
+from pyocf.types.conversion_triggers.electiveconversionindaterangetrigger import (
+    ElectiveConversionInDateRangeTrigger,
+)
+from pyocf.types.conversion_triggers.electiveconversiononconditiontrigger import (
+    ElectiveConversionOnConditionTrigger,
+)
+from pyocf.types.conversion_triggers.unspecifiedconversiontrigger import (
+    UnspecifiedConversionTrigger,
+)
 from pyocf.types.date import Date
 from pyocf.types.monetary import Monetary
 from pyocf.types.numeric import Numeric
 from pyocf.types.securityexemption import SecurityExemption
-from pyocf.types.terminationwindow import TerminationWindow
 from typing import Annotated
 from typing import Literal
 from typing import Optional
 from typing import Union
 
 
-class PlanSecurityIssuance(Object, Transaction, SecurityTransaction, Issuance):
-    """Object describing securities issuance transaction from a plan by the issuer and
-    held by a stakeholder
+class WarrantIssuance(Object, Transaction, SecurityTransaction, Issuance):
+    """Object describing warrant issuance transaction by the issuer and held by a
+    stakeholder
     """
 
-    object_type: Annotated[
-        Literal["TX_PLAN_SECURITY_ISSUANCE"], Field(description="")
-    ] = "TX_PLAN_SECURITY_ISSUANCE"
-    stock_plan_id: Annotated[
-        str,
-        Field(
-            description="Identifier of StockPlan the PlanSecurities were issued from"
-        ),
-    ]
-    compensation_type: Annotated[
-        CompensationType,
-        Field(description="If the plan security is compensation, what kind?"),
-    ]
-    option_grant_type: Optional[
-        Annotated[
-            OptionType,
-            Field(description="If the plan security is an option, what kind?"),
-        ]
-    ]
-    quantity: Annotated[
-        Numeric, Field(description="How many shares are subject to this plan security?")
-    ]
-    exercise_price: Annotated[
-        Monetary, Field(description="What is the exercise price?")
-    ]
-    vesting_terms_id: Optional[
+    object_type: Literal["TX_WARRANT_ISSUANCE"] = "TX_WARRANT_ISSUANCE"
+    # Quantity of shares the warrant is exercisable for
+    quantity: Numeric
+    # The exercise price of the warrant
+    exercise_price: Monetary
+    # Actual purchase price of the warrant (sum up purported value of all
+    # consideration, including in-kind)
+    purchase_price: Monetary
+    # In event the Warrant can convert due to trigger events (e.g. Maturity, Next
+    # Qualified Financing, Change of Control, at Election of Holder), what are the
+    # terms?
+    exercise_triggers: list[
         Annotated[
-            str,
-            Field(
-                description="Identifier of the VestingTerms to which this security is subject.  If not"
-                "present, security is fully vested on issuance."
-            ),
+            Union[
+                AutomaticConversionOnConditionTrigger,
+                AutomaticConversionOnDateTrigger,
+                ElectiveConversionAtWillTrigger,
+                ElectiveConversionInDateRangeTrigger,
+                ElectiveConversionOnConditionTrigger,
+                UnspecifiedConversionTrigger,
+            ],
+            Field(discriminator="type"),
         ]
     ]
-    expiration_date: Union[None, Date]
-    termination_exercise_windows: Annotated[
-        list[TerminationWindow],
-        Field(
-            description="Exercise periods applicable to plan security after a termination for a given,"
-            "enumerated reason"
-        ),
-    ]
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    custom_id: Annotated[
-        str, Field(description="A custom ID for this security (e.g. CN-1.)")
-    ]
-    stakeholder_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the stakeholder that holds legal title to this security"
-        ),
-    ]
-    board_approval_date: Optional[
-        Annotated[Date, Field(description="Date of board approval for the security")]
-    ]
-    consideration_text: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Unstructured text description of consideration provided in exchange for security"
-                "issuance"
-            ),
-        ]
-    ]
-    security_law_exemptions: Annotated[
-        list[SecurityExemption],
-        Field(
-            description="List of security law exemptions (and applicable jurisdictions) for this security"
-        ),
-    ]
+    # What is expiration date of the warrant (if applicable)
+    warrant_expiration_date: Optional[Date]
+    # Identifier of the VestingTerms to which this security is subject. If not
+    # present, security is fully vested on issuance.
+    vesting_terms_id: Optional[str]
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # A custom ID for this security (e.g. CN-1.)
+    custom_id: str
+    # Identifier for the stakeholder that holds legal title to this security
+    stakeholder_id: str
+    # Date of board approval for the security
+    board_approval_date: Optional[Date]
+    # Unstructured text description of consideration provided in exchange for security
+    # issuance
+    consideration_text: Optional[str]
+    # List of security law exemptions (and applicable jurisdictions) for this security
+    security_law_exemptions: list[SecurityExemption]
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/reissuance/stockreissuance.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/reissuance/stockreissuance.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,47 @@
 """Object describing a re-issuance of stock"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/reissuance/StockReissuance.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
+# OCF/tree/main/schema/objects/transactions/reissuance/StockReissuance.schema.json
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.reissuance.reissuance import Reissuance
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
-from typing import Annotated
 from typing import Literal
 from typing import Optional
 
 
 class StockReissuance(Object, Transaction, SecurityTransaction, Reissuance):
     """Object describing a re-issuance of stock"""
 
-    object_type: Annotated[
-        Literal["TX_STOCK_REISSUANCE"], Field(description="")
-    ] = "TX_STOCK_REISSUANCE"
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    resulting_security_ids: Annotated[
-        list[str],
-        Field(
-            description="Identifier of the new security (or securities) issuance resulting from a"
-            "reissuance"
-        ),
-    ]
-    split_transaction_id: Optional[
-        Annotated[
-            str,
-            Field(
-                description="When stock is reissued as a result of a stock split, this field contains id of"
-                "the respective stock class split transaction. It is not set otherwise."
-            ),
-        ]
-    ]
-    reason_text: Optional[
-        Annotated[
-            str,
-            Field(description="Free-form human-readable reason for stock reissuance"),
-        ]
-    ]
+    object_type: Literal["TX_STOCK_REISSUANCE"] = "TX_STOCK_REISSUANCE"
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # Identifier of the new security (or securities) issuance resulting from a
+    # reissuance
+    resulting_security_ids: list[str]
+    # When stock is reissued as a result of a stock split, this field contains id of
+    # the respective stock class split transaction. It is not set otherwise.
+    split_transaction_id: Optional[str]
+    # Free-form human-readable reason for stock reissuance
+    reason_text: Optional[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/repurchase/stockrepurchase.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/repurchase/stockrepurchase.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,51 @@
 """Object describing a stock repurchase transaction"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/repurchase/StockRepurchase.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
+# OCF/tree/main/schema/objects/transactions/repurchase/StockRepurchase.schema.json
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.repurchase.repurchase import Repurchase
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
 from pyocf.types.monetary import Monetary
 from pyocf.types.numeric import Numeric
-from typing import Annotated
 from typing import Literal
 from typing import Optional
 
 
 class StockRepurchase(Object, Transaction, SecurityTransaction, Repurchase):
     """Object describing a stock repurchase transaction"""
 
-    object_type: Annotated[
-        Literal["TX_STOCK_REPURCHASE"], Field(description="")
-    ] = "TX_STOCK_REPURCHASE"
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    price: Annotated[
-        Monetary, Field(description="Repurchase price per share of the stock")
-    ]
-    quantity: Annotated[
-        Numeric, Field(description="Number of shares of stock repurchased")
-    ]
-    consideration_text: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Unstructured text description of consideration provided in exchange for security"
-                "repurchase"
-            ),
-        ]
-    ]
-    balance_security_id: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Identifier for the security that holds the remainder balance (for partial"
-                "repurchases)"
-            ),
-        ]
-    ]
+    object_type: Literal["TX_STOCK_REPURCHASE"] = "TX_STOCK_REPURCHASE"
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # Repurchase price per share of the stock
+    price: Monetary
+    # Number of shares of stock repurchased
+    quantity: Numeric
+    # Unstructured text description of consideration provided in exchange for security
+    # repurchase
+    consideration_text: Optional[str]
+    # Identifier for the security that holds the remainder balance (for partial
+    # repurchases)
+    balance_security_id: Optional[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/retraction/convertibleretraction.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/retraction/plansecurityretraction.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,42 @@
-"""Object describing a retraction of a convertible security"""
+"""Object describing a retraction of a plan security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/retraction/ConvertibleRetraction.schema.j
-# son
+# ree/main/schema/objects/transactions/retraction/PlanSecurityRetraction.schema.js
+# on
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.retraction.retraction import Retraction
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
-from typing import Annotated
 from typing import Literal
 from typing import Optional
 
 
-class ConvertibleRetraction(Object, Transaction, SecurityTransaction, Retraction):
-    """Object describing a retraction of a convertible security"""
+class PlanSecurityRetraction(Object, Transaction, SecurityTransaction, Retraction):
+    """Object describing a retraction of a plan security"""
 
-    object_type: Annotated[
-        Literal["TX_CONVERTIBLE_RETRACTION"], Field(description="")
-    ] = "TX_CONVERTIBLE_RETRACTION"
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    reason_text: Annotated[str, Field(description="Reason for the retraction")]
+    object_type: Literal["TX_PLAN_SECURITY_RETRACTION"] = "TX_PLAN_SECURITY_RETRACTION"
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # Reason for the retraction
+    reason_text: str
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/retraction/plansecurityretraction.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/retraction/warrantretraction.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,41 @@
-"""Object describing a retraction of a plan security"""
+"""Object describing a retraction of a warrant security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/retraction/PlanSecurityRetraction.schema.
-# json
+# ree/main/schema/objects/transactions/retraction/WarrantRetraction.schema.json
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.retraction.retraction import Retraction
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
-from typing import Annotated
 from typing import Literal
 from typing import Optional
 
 
-class PlanSecurityRetraction(Object, Transaction, SecurityTransaction, Retraction):
-    """Object describing a retraction of a plan security"""
+class WarrantRetraction(Object, Transaction, SecurityTransaction, Retraction):
+    """Object describing a retraction of a warrant security"""
 
-    object_type: Annotated[
-        Literal["TX_PLAN_SECURITY_RETRACTION"], Field(description="")
-    ] = "TX_PLAN_SECURITY_RETRACTION"
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    reason_text: Annotated[str, Field(description="Reason for the retraction")]
+    object_type: Literal["TX_WARRANT_RETRACTION"] = "TX_WARRANT_RETRACTION"
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # Reason for the retraction
+    reason_text: str
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/retraction/stockretraction.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/retraction/stockretraction.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,41 @@
 """Object describing a retraction of a stock security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/retraction/StockRetraction.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
+# OCF/tree/main/schema/objects/transactions/retraction/StockRetraction.schema.json
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.retraction.retraction import Retraction
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
-from typing import Annotated
 from typing import Literal
 from typing import Optional
 
 
 class StockRetraction(Object, Transaction, SecurityTransaction, Retraction):
     """Object describing a retraction of a stock security"""
 
-    object_type: Annotated[
-        Literal["TX_STOCK_RETRACTION"], Field(description="")
-    ] = "TX_STOCK_RETRACTION"
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    reason_text: Annotated[str, Field(description="Reason for the retraction")]
+    object_type: Literal["TX_STOCK_RETRACTION"] = "TX_STOCK_RETRACTION"
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # Reason for the retraction
+    reason_text: str
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/retraction/warrantretraction.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/vesting/vestingevent.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,43 @@
-"""Object describing a retraction of a warrant security"""
+"""Object describing the transaction of an non-schedule-driven vesting event"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/retraction/WarrantRetraction.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
+# OCF/tree/main/schema/objects/transactions/vesting/VestingEvent.schema.json
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
-from pyocf.primitives.objects.transactions.retraction.retraction import Retraction
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
-from typing import Annotated
 from typing import Literal
 from typing import Optional
 
 
-class WarrantRetraction(Object, Transaction, SecurityTransaction, Retraction):
-    """Object describing a retraction of a warrant security"""
+class VestingEvent(Object, Transaction, SecurityTransaction):
+    """Object describing the transaction of an non-schedule-driven vesting event
+    associated with a security
+    """
 
-    object_type: Annotated[
-        Literal["TX_WARRANT_RETRACTION"], Field(description="")
-    ] = "TX_WARRANT_RETRACTION"
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    reason_text: Annotated[str, Field(description="Reason for the retraction")]
+    object_type: Literal["TX_VESTING_EVENT"] = "TX_VESTING_EVENT"
+    # Reference to the `id` of a VestingCondition in this security's VestingTerms.
+    # This condition should have a trigger type of `VESTING_EVENT`.
+    vesting_condition_id: str
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Date on which the transaction occurred
+    date: Date
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/split/stockclasssplit.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/acceptance/warrantacceptance.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,52 +1,39 @@
-"""Object describing a split of a stock class"""
+"""Object describing a warrant acceptance transaction"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/objects/transactions/split/StockClassSplit.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
+# ree/main/schema/objects/transactions/acceptance/WarrantAcceptance.schema.json
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
-from pyocf.primitives.objects.transactions.stockclasstransaction import (
-    StockClassTransaction,
+from pyocf.primitives.objects.transactions.acceptance.acceptance import Acceptance
+from pyocf.primitives.objects.transactions.securitytransaction import (
+    SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
-from pyocf.types.ratio import Ratio
-from typing import Annotated
 from typing import Literal
 from typing import Optional
 
 
-class StockClassSplit(Object, Transaction, StockClassTransaction):
-    """Object describing a split of a stock class"""
+class WarrantAcceptance(Object, Transaction, SecurityTransaction, Acceptance):
+    """Object describing a warrant acceptance transaction"""
 
-    object_type: Annotated[
-        Literal["TX_STOCK_CLASS_SPLIT"], Field(description="")
-    ] = "TX_STOCK_CLASS_SPLIT"
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    stock_class_id: Annotated[
-        str,
-        Field(
-            description="Identifier of the StockClass object, a subject of this transaction"
-        ),
-    ]
-    split_ratio: Annotated[
-        Ratio,
-        Field(
-            description="Ratio of new shares to old shares. For 2-for-1 split the numerator of the ratio"
-            "is 2 and the denominator is 1."
-        ),
-    ]
+    object_type: Literal["TX_WARRANT_ACCEPTANCE"] = "TX_WARRANT_ACCEPTANCE"
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/transfer/convertibletransfer.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/cancellation/stockcancellation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,47 @@
-"""Object describing a transfer or secondary sale of a convertible security"""
+"""Object describing a cancellation of a stock security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/transfer/ConvertibleTransfer.schema.json
+# ree/main/schema/objects/transactions/cancellation/StockCancellation.schema.json
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
+from pyocf.primitives.objects.transactions.cancellation.cancellation import Cancellation
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
-from pyocf.primitives.objects.transactions.transfer.transfer import Transfer
 from pyocf.types.date import Date
-from pyocf.types.monetary import Monetary
-from typing import Annotated
+from pyocf.types.numeric import Numeric
 from typing import Literal
 from typing import Optional
 
 
-class ConvertibleTransfer(Object, Transaction, SecurityTransaction, Transfer):
-    """Object describing a transfer or secondary sale of a convertible security"""
+class StockCancellation(Object, Transaction, SecurityTransaction, Cancellation):
+    """Object describing a cancellation of a stock security"""
 
-    object_type: Annotated[
-        Literal["TX_CONVERTIBLE_TRANSFER"], Field(description="")
-    ] = "TX_CONVERTIBLE_TRANSFER"
-    amount: Annotated[
-        Monetary, Field(description="Amount of monetary value transferred")
-    ]
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    consideration_text: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Unstructured text description of consideration provided in exchange for security"
-                "transfer"
-            ),
-        ]
-    ]
-    balance_security_id: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Identifier for the security that holds the remainder balance (for partial"
-                "transfers)"
-            ),
-        ]
-    ]
-    resulting_security_ids: Annotated[
-        list[str],
-        Field(
-            description="Array of identifiers for new security (or securities) created as a result of the"
-            "transaction"
-        ),
-    ]
+    object_type: Literal["TX_STOCK_CANCELLATION"] = "TX_STOCK_CANCELLATION"
+    # Quantity of non-monetary security units cancelled
+    quantity: Numeric
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # Identifier for the security that holds the remainder balance (for partial
+    # cancellations)
+    balance_security_id: Optional[str]
+    # Reason for the cancellation
+    reason_text: str
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/transfer/plansecuritytransfer.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/transfer/plansecuritytransfer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,81 +1,51 @@
 """Object describing a transfer of a plan security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/transfer/PlanSecurityTransfer.schema.json
+# ree/main/schema/objects/transactions/transfer/PlanSecurityTransfer.schema.json
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.primitives.objects.transactions.transfer.transfer import Transfer
 from pyocf.types.date import Date
 from pyocf.types.numeric import Numeric
-from typing import Annotated
 from typing import Literal
 from typing import Optional
 
 
 class PlanSecurityTransfer(Object, Transaction, SecurityTransaction, Transfer):
     """Object describing a transfer of a plan security"""
 
-    object_type: Annotated[
-        Literal["TX_PLAN_SECURITY_TRANSFER"], Field(description="")
-    ] = "TX_PLAN_SECURITY_TRANSFER"
-    quantity: Annotated[
-        Numeric,
-        Field(description="Quantity of non-monetary security units transferred"),
-    ]
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    consideration_text: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Unstructured text description of consideration provided in exchange for security"
-                "transfer"
-            ),
-        ]
-    ]
-    balance_security_id: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Identifier for the security that holds the remainder balance (for partial"
-                "transfers)"
-            ),
-        ]
-    ]
-    resulting_security_ids: Annotated[
-        list[str],
-        Field(
-            description="Array of identifiers for new security (or securities) created as a result of the"
-            "transaction"
-        ),
-    ]
+    object_type: Literal["TX_PLAN_SECURITY_TRANSFER"] = "TX_PLAN_SECURITY_TRANSFER"
+    # Quantity of non-monetary security units transferred
+    quantity: Numeric
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # Unstructured text description of consideration provided in exchange for security
+    # transfer
+    consideration_text: Optional[str]
+    # Identifier for the security that holds the remainder balance (for partial
+    # transfers)
+    balance_security_id: Optional[str]
+    # Array of identifiers for new security (or securities) created as a result of the
+    # transaction
+    resulting_security_ids: list[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/transfer/stocktransfer.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/cancellation/plansecuritycancellation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,50 @@
-"""Object describing a transfer or secondary sale of a stock security"""
+"""Object describing a cancellation of a plan security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/objects/transactions/transfer/StockTransfer.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
+# ree/main/schema/objects/transactions/cancellation/PlanSecurityCancellation.schem
+# a.json
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
+from pyocf.primitives.objects.transactions.cancellation.cancellation import Cancellation
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
-from pyocf.primitives.objects.transactions.transfer.transfer import Transfer
 from pyocf.types.date import Date
 from pyocf.types.numeric import Numeric
-from typing import Annotated
 from typing import Literal
 from typing import Optional
 
 
-class StockTransfer(Object, Transaction, SecurityTransaction, Transfer):
-    """Object describing a transfer or secondary sale of a stock security"""
+class PlanSecurityCancellation(Object, Transaction, SecurityTransaction, Cancellation):
+    """Object describing a cancellation of a plan security"""
 
-    object_type: Annotated[
-        Literal["TX_STOCK_TRANSFER"], Field(description="")
-    ] = "TX_STOCK_TRANSFER"
-    quantity: Annotated[
-        Numeric,
-        Field(description="Quantity of non-monetary security units transferred"),
-    ]
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    consideration_text: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Unstructured text description of consideration provided in exchange for security"
-                "transfer"
-            ),
-        ]
-    ]
-    balance_security_id: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Identifier for the security that holds the remainder balance (for partial"
-                "transfers)"
-            ),
-        ]
-    ]
-    resulting_security_ids: Annotated[
-        list[str],
-        Field(
-            description="Array of identifiers for new security (or securities) created as a result of the"
-            "transaction"
-        ),
-    ]
+    object_type: Literal[
+        "TX_PLAN_SECURITY_CANCELLATION"
+    ] = "TX_PLAN_SECURITY_CANCELLATION"
+    # Quantity of non-monetary security units cancelled
+    quantity: Numeric
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # Identifier for the security that holds the remainder balance (for partial
+    # cancellations)
+    balance_security_id: Optional[str]
+    # Reason for the cancellation
+    reason_text: str
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/transfer/warranttransfer.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/exercise/warrantexercise.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,46 @@
-"""Object describing a transfer or secondary sale of a warrant security"""
+"""Object describing a warrant exercise transaction"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/objects/transactions/transfer/WarrantTransfer.schema.json
+# OCF/tree/main/schema/objects/transactions/exercise/WarrantExercise.schema.json
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
+from pyocf.primitives.objects.transactions.exercise.exercise import Exercise
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
-from pyocf.primitives.objects.transactions.transfer.transfer import Transfer
 from pyocf.types.date import Date
-from pyocf.types.numeric import Numeric
-from typing import Annotated
 from typing import Literal
 from typing import Optional
 
 
-class WarrantTransfer(Object, Transaction, SecurityTransaction, Transfer):
-    """Object describing a transfer or secondary sale of a warrant security"""
+class WarrantExercise(Object, Transaction, SecurityTransaction, Exercise):
+    """Object describing a warrant exercise transaction"""
 
-    object_type: Annotated[
-        Literal["TX_WARRANT_TRANSFER"], Field(description="")
-    ] = "TX_WARRANT_TRANSFER"
-    quantity: Annotated[
-        Numeric,
-        Field(description="Quantity of non-monetary security units transferred"),
-    ]
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    consideration_text: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Unstructured text description of consideration provided in exchange for security"
-                "transfer"
-            ),
-        ]
-    ]
-    balance_security_id: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Identifier for the security that holds the remainder balance (for partial"
-                "transfers)"
-            ),
-        ]
-    ]
-    resulting_security_ids: Annotated[
-        list[str],
-        Field(
-            description="Array of identifiers for new security (or securities) created as a result of the"
-            "transaction"
-        ),
-    ]
+    object_type: Literal["TX_WARRANT_EXERCISE"] = "TX_WARRANT_EXERCISE"
+    # What is the id of the warrant's exercise trigger that resulted in this exercise
+    trigger_id: str
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # Unstructured text description of consideration provided in exchange for security
+    # exercise
+    consideration_text: Optional[str]
+    # Identifier for the security (or securities) that resulted from the exercise
+    resulting_security_ids: list[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/objects/transactions/vesting/vestingevent.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/exercise/plansecurityexercise.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,47 @@
-"""Object describing the transaction of an non-schedule-driven vesting event
-associated with a security"""
+"""Object describing a plan security exercise transaction"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/objects/transactions/vesting/VestingEvent.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
+# ree/main/schema/objects/transactions/exercise/PlanSecurityExercise.schema.json
 
-from pydantic import Field
 from pyocf.primitives.objects.object import Object
+from pyocf.primitives.objects.transactions.exercise.exercise import Exercise
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
-from typing import Annotated
+from pyocf.types.numeric import Numeric
 from typing import Literal
 from typing import Optional
 
 
-class VestingEvent(Object, Transaction, SecurityTransaction):
-    """Object describing the transaction of an non-schedule-driven vesting event
-    associated with a security
-    """
+class PlanSecurityExercise(Object, Transaction, SecurityTransaction, Exercise):
+    """Object describing a plan security exercise transaction"""
 
-    object_type: Annotated[
-        Literal["TX_VESTING_EVENT"], Field(description="")
-    ] = "TX_VESTING_EVENT"
-    vesting_condition_id: Annotated[
-        str,
-        Field(
-            description="Reference to the `id` of a VestingCondition in this security's VestingTerms."
-            "This condition should have a trigger type of `VESTING_EVENT`."
-        ),
-    ]
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
+    object_type: Literal["TX_PLAN_SECURITY_EXERCISE"] = "TX_PLAN_SECURITY_EXERCISE"
+    # Quantity of shares exercised
+    quantity: Numeric
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
+    # Date on which the transaction occurred
+    date: Date
+    # Unstructured text description of consideration provided in exchange for security
+    # exercise
+    consideration_text: Optional[str]
+    # Identifier for the security (or securities) that resulted from the exercise
+    resulting_security_ids: list[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/primitives/files/file.py` & `pyocf-1.0b1/src/pyocf/primitives/types/vesting/vestingconditiontrigger.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,21 @@
-"""Abstract file to be extended by all other files"""
+"""Abstract type describing fields needed in all triggers types, with a 'trigger'"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/primitives/files/File.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
+# ree/main/schema/primitives/types/vesting/VestingConditionTrigger.schema.json
 
 from pydantic import BaseModel
-from pydantic import Field
-from pyocf.enums.filetype import FileType
-from typing import Annotated
+from pyocf.enums.vestingtriggertype import VestingTriggerType
 
 
-class FileObject(BaseModel):
-    """Abstract file to be extended by all other files"""
+class VestingConditionTrigger(BaseModel):
+    """Abstract type describing fields needed in all triggers types, with a 'trigger'
+    being a condition that must be satisfied for a VestingCondition to be met
+    """
 
-    file_type: Annotated[
-        FileType,
-        Field(
-            description="File type field (used to select proper schema for validation)"
-        ),
-    ]
+    # Identifies the sub-type of trigger
+    type: VestingTriggerType
```

### Comparing `pyocf-1.0.1/src/pyocf/primitives/objects/object.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/object.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 """Abstract object to be extended by all other objects"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/primitives/objects/Object.schema.json
+# OCF/tree/main/schema/primitives/objects/Object.schema.json
 
 from pydantic import BaseModel
-from pydantic import Field
 from pyocf.enums.objecttype import ObjectType
-from typing import Annotated
 from typing import Optional
 
 
 class Object(BaseModel):
     """Abstract object to be extended by all other objects"""
 
-    id: Annotated[str, Field(description="Identifier for the object")]
-    comments: Optional[
-        Annotated[
-            list[str],
-            Field(
-                description="Unstructured text comments related to and stored for the object"
-            ),
-        ]
-    ]
-    object_type: Annotated[ObjectType, Field(description="Object type field")]
+    # Identifier for the object
+    id: str
+    # Unstructured text comments related to and stored for the object
+    comments: Optional[list[str]]
+    # Object type field
+    object_type: ObjectType
```

### Comparing `pyocf-1.0.1/src/pyocf/primitives/objects/transactions/acceptance/acceptance.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/acceptance/acceptance.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Abstract object describing a security acceptance transaction"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/objects/transactions/acceptance/Acceptance.schema.j
-# son
+# ree/main/schema/primitives/objects/transactions/acceptance/Acceptance.schema.jso
+# n
 
 from pydantic import BaseModel
 
 
 class Acceptance(BaseModel):
     """Abstract object describing a security acceptance transaction"""
```

### Comparing `pyocf-1.0.1/src/pyocf/primitives/objects/transactions/cancellation/cancellation.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/issuance/issuance.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-"""Abstract object describing fields common to all cancellation transaction objects"""
+"""Abstract object describing fields common to all issuance objects"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/objects/transactions/cancellation/Cancellation.sche
-# ma.json
+# ree/main/schema/primitives/objects/transactions/issuance/Issuance.schema.json
 
 from pydantic import BaseModel
-from pydantic import Field
-from typing import Annotated
+from pyocf.types.date import Date
+from pyocf.types.securityexemption import SecurityExemption
 from typing import Optional
 
 
-class Cancellation(BaseModel):
-    """Abstract object describing fields common to all cancellation transaction objects"""
+class Issuance(BaseModel):
+    """Abstract object describing fields common to all issuance objects"""
 
-    balance_security_id: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Identifier for the security that holds the remainder balance (for partial"
-                "cancellations)"
-            ),
-        ]
-    ]
-    reason_text: Annotated[str, Field(description="Reason for the cancellation")]
+    # A custom ID for this security (e.g. CN-1.)
+    custom_id: str
+    # Identifier for the stakeholder that holds legal title to this security
+    stakeholder_id: str
+    # Date of board approval for the security
+    board_approval_date: Optional[Date]
+    # Unstructured text description of consideration provided in exchange for security
+    # issuance
+    consideration_text: Optional[str]
+    # List of security law exemptions (and applicable jurisdictions) for this security
+    security_law_exemptions: list[SecurityExemption]
```

### Comparing `pyocf-1.0.1/src/pyocf/primitives/objects/transactions/exercise/exercise.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/exercise/exercise.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,22 @@
 """Abstract object describing fields common to all exercise transaction objects"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/objects/transactions/exercise/Exercise.schema.json
+# ree/main/schema/primitives/objects/transactions/exercise/Exercise.schema.json
 
 from pydantic import BaseModel
-from pydantic import Field
-from typing import Annotated
 from typing import Optional
 
 
 class Exercise(BaseModel):
     """Abstract object describing fields common to all exercise transaction objects"""
 
-    consideration_text: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Unstructured text description of consideration provided in exchange for security"
-                "exercise"
-            ),
-        ]
-    ]
-    resulting_security_ids: Annotated[
-        list[str],
-        Field(
-            description="Identifier for the security (or securities) that resulted from the exercise"
-        ),
-    ]
+    # Unstructured text description of consideration provided in exchange for security
+    # exercise
+    consideration_text: Optional[str]
+    # Identifier for the security (or securities) that resulted from the exercise
+    resulting_security_ids: list[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/primitives/objects/transactions/release/release.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/release/release.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,34 @@
 """Abstract object describing fields common to all release transaction objects"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/objects/transactions/release/Release.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
+# OCF/tree/main/schema/primitives/objects/transactions/release/Release.schema.json
 
 from pydantic import BaseModel
-from pydantic import Field
 from pyocf.types.date import Date
 from pyocf.types.monetary import Monetary
 from pyocf.types.numeric import Numeric
-from typing import Annotated
 from typing import Optional
 
 
 class Release(BaseModel):
     """Abstract object describing fields common to all release transaction objects"""
 
-    settlement_date: Annotated[
-        Date,
-        Field(
-            description="The settlement date for the shares released, typically after the release"
-            "transaction date"
-        ),
-    ]
-    release_price: Annotated[
-        Monetary,
-        Field(
-            description="The release price used to determine the value of the security at the time of"
-            "release"
-        ),
-    ]
-    quantity: Annotated[Numeric, Field(description="Quantity of shares released")]
-    consideration_text: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Unstructured text description of consideration provided in exchange for security"
-                "release"
-            ),
-        ]
-    ]
-    resulting_security_ids: Annotated[
-        list[str],
-        Field(
-            description="Identifier of the new security (or securities) issuance resulting from a release"
-            "transaction"
-        ),
-    ]
+    # The settlement date for the shares released, typically after the release
+    # transaction date
+    settlement_date: Date
+    # The release price used to determine the value of the security at the time of
+    # release
+    release_price: Monetary
+    # Quantity of shares released
+    quantity: Numeric
+    # Unstructured text description of consideration provided in exchange for security
+    # release
+    consideration_text: Optional[str]
+    # Identifier of the new security (or securities) issuance resulting from a release
+    # transaction
+    resulting_security_ids: list[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/primitives/objects/transactions/repurchase/repurchase.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/repurchase/repurchase.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,30 @@
 """Abstract object describing common properties to a repurchase transaction"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/objects/transactions/repurchase/Repurchase.schema.j
-# son
+# ree/main/schema/primitives/objects/transactions/repurchase/Repurchase.schema.jso
+# n
 
 from pydantic import BaseModel
-from pydantic import Field
 from pyocf.types.monetary import Monetary
 from pyocf.types.numeric import Numeric
-from typing import Annotated
 from typing import Optional
 
 
 class Repurchase(BaseModel):
     """Abstract object describing common properties to a repurchase transaction"""
 
-    price: Annotated[
-        Monetary, Field(description="Repurchase price per share of the stock")
-    ]
-    quantity: Annotated[
-        Numeric, Field(description="Number of shares of stock repurchased")
-    ]
-    consideration_text: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Unstructured text description of consideration provided in exchange for security"
-                "repurchase"
-            ),
-        ]
-    ]
-    balance_security_id: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Identifier for the security that holds the remainder balance (for partial"
-                "repurchases)"
-            ),
-        ]
-    ]
+    # Repurchase price per share of the stock
+    price: Monetary
+    # Number of shares of stock repurchased
+    quantity: Numeric
+    # Unstructured text description of consideration provided in exchange for security
+    # repurchase
+    consideration_text: Optional[str]
+    # Identifier for the security that holds the remainder balance (for partial
+    # repurchases)
+    balance_security_id: Optional[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/primitives/objects/transactions/retraction/retraction.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/stockplantransaction.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-"""Abstract object describing a security retraction transaction"""
+"""Abstract transaction object to be extended by all transaction objects that"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/objects/transactions/retraction/Retraction.schema.j
-# son
+# ree/main/schema/primitives/objects/transactions/StockPlanTransaction.schema.json
 
 from pydantic import BaseModel
-from pydantic import Field
-from typing import Annotated
 
 
-class Retraction(BaseModel):
-    """Abstract object describing a security retraction transaction"""
+class StockPlanTransaction(BaseModel):
+    """Abstract transaction object to be extended by all transaction objects that
+    affect a stock plan
+    """
 
-    reason_text: Annotated[str, Field(description="Reason for the retraction")]
+    # Identifier of the Stock Plan object, a subject of this transaction
+    stock_plan_id: str
```

### Comparing `pyocf-1.0.1/src/pyocf/primitives/objects/transactions/securitytransaction.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/securitytransaction.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,26 @@
-"""Abstract transaction object to be extended by all transaction objects that deal
-with individual securities"""
+"""Abstract transaction object to be extended by all transaction objects that deal"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/objects/transactions/SecurityTransaction.schema.jso
-# n
+# ree/main/schema/primitives/objects/transactions/SecurityTransaction.schema.json
 
 from pydantic import BaseModel
-from pydantic import Field
-from typing import Annotated
 
 
 class SecurityTransaction(BaseModel):
     """Abstract transaction object to be extended by all transaction objects that deal
     with individual securities
     """
 
-    security_id: Annotated[
-        str,
-        Field(
-            description="Identifier for the security (stock, plan security, warrant, or convertible) by"
-            "which it can be referenced by other transaction objects. Note that while this"
-            "identifier is created with an issuance object, it should be different than the"
-            "issuance object's `id` field which identifies the issuance transaction object"
-            "itself. All future transactions on the security (e.g. acceptance, transfer,"
-            "cancel, etc.) must reference this `security_id` to qualify which security the"
-            "transaction applies to."
-        ),
-    ]
+    # Identifier for the security (stock, plan security, warrant, or convertible) by
+    # which it can be referenced by other transaction objects. Note that while this
+    # identifier is created with an issuance object, it should be different than the
+    # issuance object's `id` field which identifies the issuance transaction object
+    # itself. All future transactions on the security (e.g. acceptance, transfer,
+    # cancel, etc.) must reference this `security_id` to qualify which security the
+    # transaction applies to.
+    security_id: str
```

### Comparing `pyocf-1.0.1/src/pyocf/primitives/objects/transactions/stockplantransaction.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/stockclasstransaction.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,21 @@
-"""Abstract transaction object to be extended by all transaction objects that
-affect a stock plan"""
+"""Abstract transaction object to be extended by all transaction objects that"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/objects/transactions/StockPlanTransaction.schema.js
-# on
+# ree/main/schema/primitives/objects/transactions/StockClassTransaction.schema.jso
+# n
 
 from pydantic import BaseModel
-from pydantic import Field
-from typing import Annotated
 
 
-class StockPlanTransaction(BaseModel):
+class StockClassTransaction(BaseModel):
     """Abstract transaction object to be extended by all transaction objects that
-    affect a stock plan
+    affect the stock class
     """
 
-    stock_plan_id: Annotated[
-        str,
-        Field(
-            description="Identifier of the Stock Plan object, a subject of this transaction"
-        ),
-    ]
+    # Identifier of the StockClass object, a subject of this transaction
+    stock_class_id: str
```

### Comparing `pyocf-1.0.1/src/pyocf/primitives/objects/transactions/transaction.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/transaction.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """Abstract transaction object to be extended by all other transaction objects"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/primitives/objects/transactions/Transaction.schema.json
+# OCF/tree/main/schema/primitives/objects/transactions/Transaction.schema.json
 
 from pydantic import BaseModel
-from pydantic import Field
 from pyocf.types.date import Date
-from typing import Annotated
 
 
 class Transaction(BaseModel):
     """Abstract transaction object to be extended by all other transaction objects"""
 
-    date: Annotated[Date, Field(description="Date on which the transaction occurred")]
+    # Date on which the transaction occurred
+    date: Date
```

### Comparing `pyocf-1.0.1/src/pyocf/primitives/types/conversion_mechanisms/conversionmechanism.py` & `pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/customconversionmechanism.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-"""Abstract type setting forth required field(s) for ALL conversion mechanism types"""
+"""Sets forth inputs and conversion mechanism of a custom conversion, a conversion"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/types/conversion_mechanisms/ConversionMechanism.sch
-# ema.json
+# ree/main/schema/types/conversion_mechanisms/CustomConversionMechanism.schema.jso
+# n
 
-from pydantic import BaseModel
-from pydantic import Field
-from pyocf.enums.conversionmechanismtype import ConversionMechanismType
-from typing import Annotated
+from pyocf.primitives.types.conversion_mechanisms.conversionmechanism import (
+    ConversionMechanism,
+)
+from typing import Literal
 
 
-class ConversionMechanism(BaseModel):
-    """Abstract type setting forth required field(s) for ALL conversion mechanism types"""
+class CustomConversionMechanism(ConversionMechanism):
+    """Sets forth inputs and conversion mechanism of a custom conversion, a conversion
+    type that cannot be accurately modelled with any other OCF conversion mechanism
+    type
+    """
 
-    type: Annotated[
-        ConversionMechanismType,
-        Field(description="Identifies the specific conversion trigger type"),
-    ]
+    type: Literal["CUSTOM_CONVERSION"] = "CUSTOM_CONVERSION"
+    # Detailed description of how the number of resulting shares should be determined?
+    # Use legal language from an instrument where possible
+    custom_conversion_description: str
```

### Comparing `pyocf-1.0.1/src/pyocf/primitives/types/conversion_rights/conversionright.py` & `pyocf-1.0b1/src/pyocf/primitives/types/conversion_rights/conversionright.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Abstract type representation of a conversion right from a non-plan security into
-another non-plan security"""
+"""Abstract type representation of a conversion right from a non-plan security into"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/types/conversion_rights/ConversionRight.schema.json
+# ree/main/schema/primitives/types/conversion_rights/ConversionRight.schema.json
 
 from pydantic import BaseModel
 from pydantic import Field
 from pyocf.enums.conversionrighttype import ConversionRightType
 from pyocf.types.conversion_mechanisms.customconversionmechanism import (
     CustomConversionMechanism,
 )
@@ -36,46 +35,28 @@
 
 
 class ConversionRight(BaseModel):
     """Abstract type representation of a conversion right from a non-plan security into
     another non-plan security
     """
 
-    type: Optional[
-        Annotated[
-            ConversionRightType,
-            Field(description="What kind of conversion right is this?"),
-        ]
-    ]
+    # What kind of conversion right is this?
+    type: Optional[ConversionRightType]
+    # What conversion mechanism applies to calculate the number of resulting
+    # securities?
     conversion_mechanism: Annotated[
         Union[
             SAFEConversionMechanism,
             NoteConversionMechanism,
             CustomConversionMechanism,
             PercentCapitalizationConversionMechanism,
             FixedAmountConversionMechanism,
             RatioConversionMechanism,
         ],
-        Field(
-            discriminator="type",
-            description="What conversion mechanism applies to calculate the number of resulting"
-            "securities?",
-        ),
-    ]
-    converts_to_future_round: Optional[
-        Annotated[
-            bool,
-            Field(
-                description="Is this stock class potentially convertible into a future, as-yet undetermined"
-                "stock class (e.g. Founder Preferred)"
-            ),
-        ]
-    ]
-    converts_to_stock_class_id: Optional[
-        Annotated[
-            str,
-            Field(
-                description="The identifier of the existing, known stock class this stock class can convert"
-                "into"
-            ),
-        ]
+        Field(discriminator="type"),
     ]
+    # Is this stock class potentially convertible into a future, as-yet undetermined
+    # stock class (e.g. Founder Preferred)
+    converts_to_future_round: Optional[bool]
+    # The identifier of the existing, known stock class this stock class can convert
+    # into
+    converts_to_stock_class_id: Optional[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/primitives/types/conversion_triggers/conversiontrigger.py` & `pyocf-1.0b1/src/pyocf/primitives/types/conversion_triggers/conversiontrigger.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-"""Abstract type representation of required fields require for conversion rights
-types."""
+"""Abstract type representation of required fields require for conversion rights"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/types/conversion_triggers/ConversionTrigger.schema.
-# json
+# ree/main/schema/primitives/types/conversion_triggers/ConversionTrigger.schema.js
+# on
 
 from pydantic import BaseModel
 from pydantic import Field
 from pyocf.enums.conversiontriggertype import ConversionTriggerType
 from pyocf.types.conversion_rights.convertibleconversionright import (
     ConvertibleConversionRight,
 )
@@ -26,43 +25,26 @@
 
 
 class ConversionTrigger(BaseModel):
     """Abstract type representation of required fields require for conversion rights
     types.
     """
 
-    type: Annotated[
-        ConversionTriggerType,
-        Field(
-            description="When the trigger condition is met, is the conversion automatic, elective or"
-            "automatic with an elective right not to convert"
-        ),
-    ]
-    trigger_id: Annotated[
-        str,
-        Field(
-            description="Id for this conversion trigger, unique within list of ConversionTriggers in"
-            "parent convertible issuance's `conversion_triggers` field."
-        ),
-    ]
-    nickname: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Human-friendly nickname to describe the conversion right"
-            ),
-        ]
-    ]
-    trigger_description: Optional[
-        Annotated[str, Field(description="Long-form description of the trigger")]
-    ]
+    # When the trigger condition is met, is the conversion automatic, elective or
+    # automatic with an elective right not to convert
+    type: ConversionTriggerType
+    # Id for this conversion trigger, unique within list of ConversionTriggers in
+    # parent convertible issuance's `conversion_triggers` field.
+    trigger_id: str
+    # Human-friendly nickname to describe the conversion right
+    nickname: Optional[str]
+    # Long-form description of the trigger
+    trigger_description: Optional[str]
+    # When the conditions of the trigger are met, how does the convertible convert?
     conversion_right: Annotated[
         Union[
             ConvertibleConversionRight,
             WarrantConversionRight,
             StockClassConversionRight,
         ],
-        Field(
-            discriminator="type",
-            description="When the conditions of the trigger are met, how does the convertible convert?",
-        ),
+        Field(discriminator="type"),
     ]
```

### Comparing `pyocf-1.0.1/src/pyocf/primitives/types/vesting/vestingperiod.py` & `pyocf-1.0b1/src/pyocf/primitives/types/vesting/vestingperiod.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,27 @@
-"""Abstract type describing the fields common to all periods of time (e.g. 3
-months, 365 days) for use in Vesting Terms"""
+"""Abstract type describing the fields common to all periods of time (e.g. 3"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/primitives/types/vesting/VestingPeriod.schema.json
+# OCF/tree/main/schema/primitives/types/vesting/VestingPeriod.schema.json
 
 from pydantic import BaseModel
-from pydantic import Field
 from pyocf.enums.periodtype import PeriodType
-from typing import Annotated
 
 
 class VestingPeriod(BaseModel):
     """Abstract type describing the fields common to all periods of time (e.g. 3
     months, 365 days) for use in Vesting Terms
     """
 
-    length: Annotated[
-        int,
-        Field(
-            description="The quantity of `type` units of time; e.g. for 3 months, this would be `3`; for"
-            "30 days, this would be `30`"
-        ),
-    ]
-    type: Annotated[
-        PeriodType,
-        Field(description="The unit of time for the period, e.g. `MONTHS` or `DAYS`"),
-    ]
-    occurrences: Annotated[
-        int,
-        Field(
-            description="The number of times this vesting period triggers. If vesting occurs monthly for"
-            "36 months, for example, this would be `36`"
-        ),
-    ]
+    # The quantity of `type` units of time; e.g. for 3 months, this would be `3`; for
+    # 30 days, this would be `30`
+    length: int
+    # The unit of time for the period, e.g. `MONTHS` or `DAYS`
+    type: PeriodType
+    # The number of times this vesting period triggers. If vesting occurs monthly for
+    # 36 months, for example, this would be `36`
+    occurrences: int
```

### Comparing `pyocf-1.0.1/src/pyocf/simplebase.py` & `pyocf-1.0b1/src/pyocf/simplebase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """A pydantic model for simple types with no attributes"""
 
-# Copyright © 2023 FMR LLC
-
 from pydantic import BaseModel
 
 
 class SimpleBaseModel(BaseModel):
     """A pydantic model for simple types with no attributes
 
     This model allows you to pass the value into object initialization
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyocf-1.0.1/src/pyocf/types/address.py` & `pyocf-1.0b1/src/pyocf/types/address.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,33 @@
 """Type representation of an address"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/Address.schema.json
+# OCF/tree/main/schema/types/Address.schema.json
 
 from pydantic import BaseModel
-from pydantic import Field
 from pyocf.enums.addresstype import AddressType
 from pyocf.types.countrycode import CountryCode
 from pyocf.types.countrysubdivisioncode import CountrySubdivisionCode
-from typing import Annotated
 from typing import Optional
 
 
 class Address(BaseModel):
     """Type representation of an address"""
 
-    address_type: Annotated[
-        AddressType,
-        Field(
-            description="What type of address is this (e.g. legal address, contact address, etc.)"
-        ),
-    ]
-    street_suite: Optional[
-        Annotated[str, Field(description="Street address (multi-line string)")]
-    ]
-    city: Optional[Annotated[str, Field(description="City")]]
-    country_subdivision: Optional[
-        Annotated[
-            CountrySubdivisionCode,
-            Field(
-                description="State, province, or equivalent identifier required for an address in this"
-                "country"
-            ),
-        ]
-    ]
-    country: Annotated[
-        CountryCode,
-        Field(description="Country code for this address (ISO 3166-1 alpha-2)"),
-    ]
-    postal_code: Optional[Annotated[str, Field(description="Address postal code")]]
+    # What type of address is this (e.g. legal address, contact address, etc.)
+    address_type: AddressType
+    # Street address (multi-line string)
+    street_suite: Optional[str]
+    # City
+    city: Optional[str]
+    # State, province, or equivalent identifier required for an address in this
+    # country
+    country_subdivision: Optional[CountrySubdivisionCode]
+    # Country code for this address (ISO 3166-1 alpha-2)
+    country: CountryCode
+    # Address postal code
+    postal_code: Optional[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/types/capitalizationdefinition.py` & `pyocf-1.0b1/src/pyocf/types/capitalizationdefinition.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,33 @@
-"""Type represents a group of securities that constitutes some formally defined
-part of the company (e.g. post-money capitalization vs pre-money for a security)"""
+"""Type represents a group of securities that constitutes some formally defined"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/CapitalizationDefinition.schema.json
+# OCF/tree/main/schema/types/CapitalizationDefinition.schema.json
 
 from pydantic import BaseModel
-from pydantic import Field
-from typing import Annotated
 
 
 class CapitalizationDefinition(BaseModel):
     """Type represents a group of securities that constitutes some formally defined
     part of the company (e.g. post-money capitalization vs pre-money for a security)
     """
 
-    include_stock_class_ids: Annotated[
-        list[str],
-        Field(
-            description="All issuances of stock classes with these ids should be included (unless such an"
-            "issuance is specifically included in `exclude_security_ids`"
-        ),
-    ]
-    include_stock_plans_ids: Annotated[
-        list[str],
-        Field(
-            description="All issuances of plan securities from stock plans with these ids should be"
-            "included (unless such an issuance is specifically excluded in"
-            "`exclude_security_ids`"
-        ),
-    ]
-    include_security_ids: Annotated[
-        list[str],
-        Field(
-            description="Securities (whether Stock, Plan Securities, Convertibles or Warrants) with these"
-            "security ids should be included from this definition of capitalization"
-            "(overrides plan or class-level rules)"
-        ),
-    ]
-    exclude_security_ids: Annotated[
-        list[str],
-        Field(
-            description="Securities (whether Stock, Plan Securities, Convertibles or Warrants) with these"
-            "security ids should be excluded from this definition of capitalization"
-            "(overrides plan or class-level rules)"
-        ),
-    ]
+    # All issuances of stock classes with these ids should be included (unless such an
+    # issuance is specifically included in `exclude_security_ids`
+    include_stock_class_ids: list[str]
+    # All issuances of plan securities from stock plans with these ids should be
+    # included (unless such an issuance is specifically excluded in
+    # `exclude_security_ids`
+    include_stock_plans_ids: list[str]
+    # Securities (whether Stock, Plan Securities, Convertibles or Warrants) with these
+    # security ids should be included from this definition of capitalization
+    # (overrides plan or class-level rules)
+    include_security_ids: list[str]
+    # Securities (whether Stock, Plan Securities, Convertibles or Warrants) with these
+    # security ids should be excluded from this definition of capitalization
+    # (overrides plan or class-level rules)
+    exclude_security_ids: list[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/types/conversion_mechanisms/customconversionmechanism.py` & `pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/safeconversionmechanism.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-"""Sets forth inputs and conversion mechanism of a custom conversion, a conversion
-type that cannot be accurately modelled with any other OCF conversion mechanism
-type"""
+"""Sets forth inputs and conversion mechanism of a SAFE (mirrors the flavors and"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_mechanisms/CustomConversionMechanism.schema.j
-# son
+# ree/main/schema/types/conversion_mechanisms/SAFEConversionMechanism.schema.json
 
-from pydantic import Field
+from pyocf.enums.conversiontimingtype import ConversionTimingType
 from pyocf.primitives.types.conversion_mechanisms.conversionmechanism import (
     ConversionMechanism,
 )
-from typing import Annotated
+from pyocf.types.monetary import Monetary
+from pyocf.types.percentage import Percentage
+from pyocf.types.ratio import Ratio
 from typing import Literal
+from typing import Optional
 
 
-class CustomConversionMechanism(ConversionMechanism):
-    """Sets forth inputs and conversion mechanism of a custom conversion, a conversion
-    type that cannot be accurately modelled with any other OCF conversion mechanism
-    type
+class SAFEConversionMechanism(ConversionMechanism):
+    """Sets forth inputs and conversion mechanism of a SAFE (mirrors the flavors and
+    inputs of the Y Combinator SAFE)
     """
 
-    type: Annotated[
-        Literal["CUSTOM_CONVERSION"], Field(description="")
-    ] = "CUSTOM_CONVERSION"
-    custom_conversion_description: Annotated[
-        str,
-        Field(
-            description="Detailed description of how the number of resulting shares should be determined?"
-            "Use legal language from an instrument where possible"
-        ),
-    ]
+    type: Literal["SAFE_CONVERSION"] = "SAFE_CONVERSION"
+    # What is the percentage discount available upon conversion, if applicable?
+    # (decimal representation - e.g. 0.125 for 12.5%)
+    conversion_discount: Optional[Percentage]
+    # What is the valuation cap (if applicable)?
+    conversion_valuation_cap: Optional[Monetary]
+    # For cash proceeds calculation during a liquidity event.
+    exit_multiple: Optional[Ratio]
+    # Is this an MFN flavored SAFE?
+    conversion_mfn: bool
+    # Should the conversion amount be based on pre or post money capitalization
+    conversion_timing: ConversionTimingType
+    # How is company capitalization defined for purposes of conversion? If possible,
+    # include the legal language from the instrument.
+    capitalization_definition: Optional[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/types/conversion_mechanisms/fixedamountconversionmechanism.py` & `pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/fixedamountconversionmechanism.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 """Describes how a security converts into a fixed amount of a stock class"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_mechanisms/FixedAmountConversionMechanism.sch
-# ema.json
+# ree/main/schema/types/conversion_mechanisms/FixedAmountConversionMechanism.schem
+# a.json
 
-from pydantic import Field
 from pyocf.primitives.types.conversion_mechanisms.conversionmechanism import (
     ConversionMechanism,
 )
 from pyocf.types.numeric import Numeric
-from typing import Annotated
 from typing import Literal
 
 
 class FixedAmountConversionMechanism(ConversionMechanism):
     """Describes how a security converts into a fixed amount of a stock class"""
 
-    type: Annotated[
-        Literal["FIXED_AMOUNT_CONVERSION"], Field(description="")
-    ] = "FIXED_AMOUNT_CONVERSION"
-    converts_to_quantity: Annotated[
-        Numeric,
-        Field(
-            description="How many shares of target Stock Class does this security convert into?"
-        ),
-    ]
+    type: Literal["FIXED_AMOUNT_CONVERSION"] = "FIXED_AMOUNT_CONVERSION"
+    # How many shares of target Stock Class does this security convert into?
+    converts_to_quantity: Numeric
```

### Comparing `pyocf-1.0.1/src/pyocf/types/conversion_mechanisms/noteconversionmechanism.py` & `pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/noteconversionmechanism.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,48 @@
 """Sets forth inputs and conversion mechanism of a convertible note"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_mechanisms/NoteConversionMechanism.schema.jso
-# n
+# ree/main/schema/types/conversion_mechanisms/NoteConversionMechanism.schema.json
 
-from pydantic import Field
 from pyocf.enums.accrualperiodtype import AccrualPeriodType
 from pyocf.enums.compoundingtype import CompoundingType
 from pyocf.enums.daycounttype import DayCountType
 from pyocf.enums.interestpayouttype import InterestPayoutType
 from pyocf.primitives.types.conversion_mechanisms.conversionmechanism import (
     ConversionMechanism,
 )
 from pyocf.types.interestrate import InterestRate
 from pyocf.types.monetary import Monetary
 from pyocf.types.percentage import Percentage
 from pyocf.types.ratio import Ratio
-from typing import Annotated
 from typing import Literal
 from typing import Optional
 
 
 class NoteConversionMechanism(ConversionMechanism):
     """Sets forth inputs and conversion mechanism of a convertible note"""
 
-    type: Annotated[
-        Literal["CONVERTIBLE_NOTE_CONVERSION"], Field(description="")
-    ] = "CONVERTIBLE_NOTE_CONVERSION"
-    interest_rates: Annotated[
-        list[InterestRate],
-        Field(description="Interest rate(s) of the convertible (if applicable)"),
-    ]
-    day_count_convention: Annotated[
-        DayCountType,
-        Field(
-            description="How many days are there is a given period for calculation purposes?"
-        ),
-    ]
-    interest_payout: Annotated[
-        InterestPayoutType,
-        Field(description="How is interest paid out (if at applicable)"),
-    ]
-    interest_accrual_period: Annotated[
-        AccrualPeriodType,
-        Field(description="What is the period over which interest is calculated?"),
-    ]
-    compounding_type: Annotated[
-        CompoundingType, Field(description="What type of interest compounding?")
-    ]
-    conversion_discount: Optional[
-        Annotated[
-            Percentage,
-            Field(
-                description="What is the percentage discount available upon conversion, if applicable?"
-                "(decimal representation - e.g. 0.125 for 12.5%)"
-            ),
-        ]
-    ]
-    conversion_valuation_cap: Optional[
-        Annotated[
-            Monetary, Field(description="What is the valuation cap (if applicable)?")
-        ]
-    ]
-    exit_multiple: Optional[
-        Annotated[
-            Ratio,
-            Field(
-                description="For cash proceeds calculation during a liquidity event."
-            ),
-        ]
-    ]
-    conversion_mfn: Optional[
-        Annotated[
-            bool,
-            Field(
-                description="Is this an MFN (Most Favored Nations) flavored Convertible Note?"
-            ),
-        ]
-    ]
+    type: Literal["CONVERTIBLE_NOTE_CONVERSION"] = "CONVERTIBLE_NOTE_CONVERSION"
+    # Interest rate(s) of the convertible (if applicable)
+    interest_rates: list[InterestRate]
+    # How many days are there is a given period for calculation purposes?
+    day_count_convention: DayCountType
+    # How is interest paid out (if at applicable)
+    interest_payout: InterestPayoutType
+    # What is the period over which interest is calculated?
+    interest_accrual_period: AccrualPeriodType
+    # What type of interest compounding?
+    compounding_type: CompoundingType
+    # What is the percentage discount available upon conversion, if applicable?
+    # (decimal representation - e.g. 0.125 for 12.5%)
+    conversion_discount: Optional[Percentage]
+    # What is the valuation cap (if applicable)?
+    conversion_valuation_cap: Optional[Monetary]
+    # For cash proceeds calculation during a liquidity event.
+    exit_multiple: Optional[Ratio]
+    # Is this an MFN (Most Favored Nations) flavored Convertible Note?
+    conversion_mfn: Optional[bool]
```

### Comparing `pyocf-1.0.1/src/pyocf/types/conversion_mechanisms/percentcapitalizationconversionmechanism.py` & `pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/percentcapitalizationconversionmechanism.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,33 @@
-"""Sets forth inputs and conversion mechanism of percent of capitalization
-conversion (where an instrument purports to grant a percent of company
-capitalization at some point in time)"""
+"""Sets forth inputs and conversion mechanism of percent of capitalization"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_mechanisms/PercentCapitalizationConversionMec
-# hanism.schema.json
+# ree/main/schema/types/conversion_mechanisms/PercentCapitalizationConversionMecha
+# nism.schema.json
 
-from pydantic import Field
 from pyocf.primitives.types.conversion_mechanisms.conversionmechanism import (
     ConversionMechanism,
 )
 from pyocf.types.percentage import Percentage
-from typing import Annotated
 from typing import Literal
 from typing import Optional
 
 
 class PercentCapitalizationConversionMechanism(ConversionMechanism):
     """Sets forth inputs and conversion mechanism of percent of capitalization
     conversion (where an instrument purports to grant a percent of company
     capitalization at some point in time)
     """
 
-    type: Annotated[
-        Literal["FIXED_PERCENT_OF_CAPITALIZATION_CONVERSION"], Field(description="")
+    type: Literal[
+        "FIXED_PERCENT_OF_CAPITALIZATION_CONVERSION"
     ] = "FIXED_PERCENT_OF_CAPITALIZATION_CONVERSION"
-    converts_to_percent: Annotated[
-        Percentage,
-        Field(
-            description="What percentage of the company capitalization does this convert to"
-        ),
-    ]
-    capitalization_definition: Optional[
-        Annotated[
-            str,
-            Field(
-                description="How is company capitalization defined for purposes of conversion? If possible,"
-                "include the legal language from the instrument."
-            ),
-        ]
-    ]
+    # What percentage of the company capitalization does this convert to
+    converts_to_percent: Percentage
+    # How is company capitalization defined for purposes of conversion? If possible,
+    # include the legal language from the instrument.
+    capitalization_definition: Optional[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/types/conversion_mechanisms/ratioconversionmechanism.py` & `pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/ratioconversionmechanism.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,32 @@
-"""Sets forth inputs and conversion mechanism of a ratio conversion (primarily used
-to describe conversion from one stock class (e.g. Preferred) into another (e.g.
-Common)"""
+"""Sets forth inputs and conversion mechanism of a ratio conversion (primarily used"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_mechanisms/RatioConversionMechanism.schema.js
-# on
+# ree/main/schema/types/conversion_mechanisms/RatioConversionMechanism.schema.json
 
-from pydantic import Field
 from pyocf.enums.roundingtype import RoundingType
 from pyocf.primitives.types.conversion_mechanisms.conversionmechanism import (
     ConversionMechanism,
 )
 from pyocf.types.monetary import Monetary
 from pyocf.types.ratio import Ratio
-from typing import Annotated
 from typing import Literal
 
 
 class RatioConversionMechanism(ConversionMechanism):
     """Sets forth inputs and conversion mechanism of a ratio conversion (primarily used
     to describe conversion from one stock class (e.g. Preferred) into another (e.g.
     Common)
     """
 
-    type: Annotated[
-        Literal["RATIO_CONVERSION"], Field(description="")
-    ] = "RATIO_CONVERSION"
-    conversion_price: Annotated[
-        Monetary,
-        Field(
-            description="What is the effective conversion price per share of this stock class?"
-        ),
-    ]
-    ratio: Annotated[
-        Ratio,
-        Field(
-            description="One share of this stock class converts into this many target stock class shares"
-        ),
-    ]
-    rounding_type: Annotated[
-        RoundingType, Field(description="How should fractional shares be rounded?")
-    ]
+    type: Literal["RATIO_CONVERSION"] = "RATIO_CONVERSION"
+    # What is the effective conversion price per share of this stock class?
+    conversion_price: Monetary
+    # One share of this stock class converts into this many target stock class shares
+    ratio: Ratio
+    # How should fractional shares be rounded?
+    rounding_type: RoundingType
```

### Comparing `pyocf-1.0.1/src/pyocf/types/conversion_mechanisms/safeconversionmechanism.py` & `pyocf-1.0b1/src/pyocf/types/conversion_triggers/electiveconversionatwilltrigger.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,50 @@
-"""Sets forth inputs and conversion mechanism of a SAFE (mirrors the flavors and
-inputs of the Y Combinator SAFE)"""
+"""Type representation of elective trigger valid at will (so long as instrument is"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_mechanisms/SAFEConversionMechanism.schema.jso
-# n
+# ree/main/schema/types/conversion_triggers/ElectiveConversionAtWillTrigger.schema
+# .json
 
 from pydantic import Field
-from pyocf.enums.conversiontimingtype import ConversionTimingType
-from pyocf.primitives.types.conversion_mechanisms.conversionmechanism import (
-    ConversionMechanism,
+from pyocf.primitives.types.conversion_triggers.conversiontrigger import (
+    ConversionTrigger,
 )
-from pyocf.types.monetary import Monetary
-from pyocf.types.percentage import Percentage
-from pyocf.types.ratio import Ratio
+from pyocf.types.conversion_rights.convertibleconversionright import (
+    ConvertibleConversionRight,
+)
+from pyocf.types.conversion_rights.stockclassconversionright import (
+    StockClassConversionRight,
+)
+from pyocf.types.conversion_rights.warrantconversionright import WarrantConversionRight
 from typing import Annotated
 from typing import Literal
 from typing import Optional
+from typing import Union
 
 
-class SAFEConversionMechanism(ConversionMechanism):
-    """Sets forth inputs and conversion mechanism of a SAFE (mirrors the flavors and
-    inputs of the Y Combinator SAFE)
+class ElectiveConversionAtWillTrigger(ConversionTrigger):
+    """Type representation of elective trigger valid at will (so long as instrument is
+    valid and outstanding).
     """
 
-    type: Annotated[
-        Literal["SAFE_CONVERSION"], Field(description="")
-    ] = "SAFE_CONVERSION"
-    conversion_discount: Optional[
-        Annotated[
-            Percentage,
-            Field(
-                description="What is the percentage discount available upon conversion, if applicable?"
-                "(decimal representation - e.g. 0.125 for 12.5%)"
-            ),
-        ]
-    ]
-    conversion_valuation_cap: Optional[
-        Annotated[
-            Monetary, Field(description="What is the valuation cap (if applicable)?")
-        ]
-    ]
-    exit_multiple: Optional[
-        Annotated[
-            Ratio,
-            Field(
-                description="For cash proceeds calculation during a liquidity event."
-            ),
-        ]
-    ]
-    conversion_mfn: Annotated[bool, Field(description="Is this an MFN flavored SAFE?")]
-    conversion_timing: Annotated[
-        ConversionTimingType,
-        Field(
-            description="Should the conversion amount be based on pre or post money capitalization"
-        ),
-    ]
-    capitalization_definition: Optional[
-        Annotated[
-            str,
-            Field(
-                description="How is company capitalization defined for purposes of conversion? If possible,"
-                "include the legal language from the instrument."
-            ),
-        ]
+    # Id for this conversion trigger, unique within list of ConversionTriggers in
+    # parent convertible issuance's `conversion_triggers` field.
+    trigger_id: str
+    # Human-friendly nickname to describe the conversion right
+    nickname: Optional[str]
+    # Long-form description of the trigger
+    trigger_description: Optional[str]
+    type: Literal["ELECTIVE_AT_WILL"] = "ELECTIVE_AT_WILL"
+    # When the conditions of the trigger are met, how does the convertible convert?
+    conversion_right: Annotated[
+        Union[
+            ConvertibleConversionRight,
+            WarrantConversionRight,
+            StockClassConversionRight,
+        ],
+        Field(discriminator="type"),
     ]
```

### Comparing `pyocf-1.0.1/src/pyocf/types/conversion_rights/convertibleconversionright.py` & `pyocf-1.0b1/src/pyocf/types/conversion_rights/convertibleconversionright.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Type representation of a conversion right from a convertible into another non-
-plan security"""
+"""Type representation of a conversion right from a convertible into another non-"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_rights/ConvertibleConversionRight.schema.json
+# ree/main/schema/types/conversion_rights/ConvertibleConversionRight.schema.json
 
 from pydantic import Field
 from pyocf.primitives.types.conversion_rights.conversionright import ConversionRight
 from pyocf.types.conversion_mechanisms.customconversionmechanism import (
     CustomConversionMechanism,
 )
 from pyocf.types.conversion_mechanisms.fixedamountconversionmechanism import (
@@ -34,37 +33,25 @@
 
 class ConvertibleConversionRight(ConversionRight):
     """Type representation of a conversion right from a convertible into another non-
     plan security
     """
 
     type: Optional[
-        Annotated[Literal["CONVERTIBLE_CONVERSION_RIGHT"], Field(description="")]
+        Literal["CONVERTIBLE_CONVERSION_RIGHT"]
     ] = "CONVERTIBLE_CONVERSION_RIGHT"
     conversion_mechanism: Annotated[
         Union[
             SAFEConversionMechanism,
             NoteConversionMechanism,
             CustomConversionMechanism,
             PercentCapitalizationConversionMechanism,
             FixedAmountConversionMechanism,
         ],
-        Field(discriminator="type", description=""),
-    ]
-    converts_to_future_round: Optional[
-        Annotated[
-            bool,
-            Field(
-                description="Is this stock class potentially convertible into a future, as-yet undetermined"
-                "stock class (e.g. Founder Preferred)"
-            ),
-        ]
-    ]
-    converts_to_stock_class_id: Optional[
-        Annotated[
-            str,
-            Field(
-                description="The identifier of the existing, known stock class this stock class can convert"
-                "into"
-            ),
-        ]
+        Field(discriminator="type"),
     ]
+    # Is this stock class potentially convertible into a future, as-yet undetermined
+    # stock class (e.g. Founder Preferred)
+    converts_to_future_round: Optional[bool]
+    # The identifier of the existing, known stock class this stock class can convert
+    # into
+    converts_to_stock_class_id: Optional[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/types/conversion_rights/stockclassconversionright.py` & `pyocf-1.0b1/src/pyocf/types/conversion_rights/stockclassconversionright.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,33 @@
-"""Type representation of a conversion right from one Stock Class into another
-Stock Class"""
+"""Type representation of a conversion right from one Stock Class into another"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_rights/StockClassConversionRight.schema.json
+# ree/main/schema/types/conversion_rights/StockClassConversionRight.schema.json
 
-from pydantic import Field
 from pyocf.primitives.types.conversion_rights.conversionright import ConversionRight
 from pyocf.types.conversion_mechanisms.ratioconversionmechanism import (
     RatioConversionMechanism,
 )
-from typing import Annotated
 from typing import Literal
 from typing import Optional
 
 
 class StockClassConversionRight(ConversionRight):
     """Type representation of a conversion right from one Stock Class into another
     Stock Class
     """
 
     type: Optional[
-        Annotated[Literal["STOCK_CLASS_CONVERSION_RIGHT"], Field(description="")]
+        Literal["STOCK_CLASS_CONVERSION_RIGHT"]
     ] = "STOCK_CLASS_CONVERSION_RIGHT"
-    conversion_mechanism: Annotated[RatioConversionMechanism, Field(description="")]
-    converts_to_future_round: Optional[
-        Annotated[
-            bool,
-            Field(
-                description="Is this stock class potentially convertible into a future, as-yet undetermined"
-                "stock class (e.g. Founder Preferred)"
-            ),
-        ]
-    ]
-    converts_to_stock_class_id: Optional[
-        Annotated[
-            str,
-            Field(
-                description="The identifier of the existing, known stock class this stock class can convert"
-                "into"
-            ),
-        ]
-    ]
+    conversion_mechanism: RatioConversionMechanism
+    # Is this stock class potentially convertible into a future, as-yet undetermined
+    # stock class (e.g. Founder Preferred)
+    converts_to_future_round: Optional[bool]
+    # The identifier of the existing, known stock class this stock class can convert
+    # into
+    converts_to_stock_class_id: Optional[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/types/conversion_rights/warrantconversionright.py` & `pyocf-1.0b1/src/pyocf/types/conversion_rights/warrantconversionright.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Type representation of a conversion right from a convertible into another non-
-plan security"""
+"""Type representation of a conversion right from a convertible into another non-"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_rights/WarrantConversionRight.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
+# OCF/tree/main/schema/types/conversion_rights/WarrantConversionRight.schema.json
 
 from pydantic import Field
 from pyocf.primitives.types.conversion_rights.conversionright import ConversionRight
 from pyocf.types.conversion_mechanisms.customconversionmechanism import (
     CustomConversionMechanism,
 )
 from pyocf.types.conversion_mechanisms.fixedamountconversionmechanism import (
@@ -27,40 +26,24 @@
 
 
 class WarrantConversionRight(ConversionRight):
     """Type representation of a conversion right from a convertible into another non-
     plan security
     """
 
-    type: Optional[
-        Annotated[Literal["WARRANT_CONVERSION_RIGHT"], Field(description="")]
-    ] = "WARRANT_CONVERSION_RIGHT"
+    type: Optional[Literal["WARRANT_CONVERSION_RIGHT"]] = "WARRANT_CONVERSION_RIGHT"
+    # What conversion mechanism applies to calculate the number of resulting stock
+    # class shares?
     conversion_mechanism: Annotated[
         Union[
             CustomConversionMechanism,
             PercentCapitalizationConversionMechanism,
             FixedAmountConversionMechanism,
         ],
-        Field(
-            discriminator="type",
-            description="What conversion mechanism applies to calculate the number of resulting stock"
-            "class shares?",
-        ),
-    ]
-    converts_to_future_round: Optional[
-        Annotated[
-            bool,
-            Field(
-                description="Is this stock class potentially convertible into a future, as-yet undetermined"
-                "stock class (e.g. Founder Preferred)"
-            ),
-        ]
-    ]
-    converts_to_stock_class_id: Optional[
-        Annotated[
-            str,
-            Field(
-                description="The identifier of the existing, known stock class this stock class can convert"
-                "into"
-            ),
-        ]
+        Field(discriminator="type"),
     ]
+    # Is this stock class potentially convertible into a future, as-yet undetermined
+    # stock class (e.g. Founder Preferred)
+    converts_to_future_round: Optional[bool]
+    # The identifier of the existing, known stock class this stock class can convert
+    # into
+    converts_to_stock_class_id: Optional[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/types/conversion_triggers/automaticconversiononconditiontrigger.py` & `pyocf-1.0b1/src/pyocf/types/conversion_triggers/automaticconversiononconditiontrigger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Type representation of automatic trigger on a tive or condition."""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_triggers/AutomaticConversionOnConditionTrigge
-# r.schema.json
+# ree/main/schema/types/conversion_triggers/AutomaticConversionOnConditionTrigger.
+# schema.json
 
 from pydantic import Field
 from pyocf.primitives.types.conversion_triggers.conversiontrigger import (
     ConversionTrigger,
 )
 from pyocf.types.conversion_rights.convertibleconversionright import (
     ConvertibleConversionRight,
@@ -25,47 +25,28 @@
 from typing import Optional
 from typing import Union
 
 
 class AutomaticConversionOnConditionTrigger(ConversionTrigger):
     """Type representation of automatic trigger on a tive or condition."""
 
-    trigger_condition: Annotated[
-        str,
-        Field(
-            description="Legal language describing what conditions must be satisfied for the conversion"
-            "to take place (ideally, this should be excerpted from the instrument where"
-            "possible)"
-        ),
-    ]
-    trigger_id: Annotated[
-        str,
-        Field(
-            description="Id for this conversion trigger, unique within list of ConversionTriggers in"
-            "parent convertible issuance's `conversion_triggers` field."
-        ),
-    ]
-    nickname: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Human-friendly nickname to describe the conversion right"
-            ),
-        ]
-    ]
-    trigger_description: Optional[
-        Annotated[str, Field(description="Long-form description of the trigger")]
-    ]
-    type: Annotated[
-        Literal["AUTOMATIC_ON_CONDITION"], Field(description="")
-    ] = "AUTOMATIC_ON_CONDITION"
+    # Legal language describing what conditions must be satisfied for the conversion
+    # to take place (ideally, this should be excerpted from the instrument where
+    # possible)
+    trigger_condition: str
+    # Id for this conversion trigger, unique within list of ConversionTriggers in
+    # parent convertible issuance's `conversion_triggers` field.
+    trigger_id: str
+    # Human-friendly nickname to describe the conversion right
+    nickname: Optional[str]
+    # Long-form description of the trigger
+    trigger_description: Optional[str]
+    type: Literal["AUTOMATIC_ON_CONDITION"] = "AUTOMATIC_ON_CONDITION"
+    # When the conditions of the trigger are met, how does the convertible convert?
     conversion_right: Annotated[
         Union[
             ConvertibleConversionRight,
             WarrantConversionRight,
             StockClassConversionRight,
         ],
-        Field(
-            discriminator="type",
-            description="When the conditions of the trigger are met, how does the convertible convert?",
-        ),
+        Field(discriminator="type"),
     ]
```

### Comparing `pyocf-1.0.1/src/pyocf/types/conversion_triggers/automaticconversionondatetrigger.py` & `pyocf-1.0b1/src/pyocf/types/conversion_triggers/electiveconversionindaterangetrigger.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-"""Type representation of an automatic trigger on a date."""
+"""Type representation of elective trigger valid on or after start_date and until"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_triggers/AutomaticConversionOnDateTrigger.sch
-# ema.json
+# ree/main/schema/types/conversion_triggers/ElectiveConversionInDateRangeTrigger.s
+# chema.json
 
 from pydantic import Field
 from pyocf.primitives.types.conversion_triggers.conversiontrigger import (
     ConversionTrigger,
 )
 from pyocf.types.conversion_rights.convertibleconversionright import (
     ConvertibleConversionRight,
@@ -23,48 +23,33 @@
 from pyocf.types.date import Date
 from typing import Annotated
 from typing import Literal
 from typing import Optional
 from typing import Union
 
 
-class AutomaticConversionOnDateTrigger(ConversionTrigger):
-    """Type representation of an automatic trigger on a date."""
+class ElectiveConversionInDateRangeTrigger(ConversionTrigger):
+    """Type representation of elective trigger valid on or after start_date and until
+    or before end_date.
+    """
 
-    trigger_date: Annotated[
-        Date,
-        Field(
-            description="Date on which trigger occurs automatically (if it hasn't already occured)"
-        ),
-    ]
-    trigger_id: Annotated[
-        str,
-        Field(
-            description="Id for this conversion trigger, unique within list of ConversionTriggers in"
-            "parent convertible issuance's `conversion_triggers` field."
-        ),
-    ]
-    nickname: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Human-friendly nickname to describe the conversion right"
-            ),
-        ]
-    ]
-    trigger_description: Optional[
-        Annotated[str, Field(description="Long-form description of the trigger")]
-    ]
-    type: Annotated[
-        Literal["AUTOMATIC_ON_DATE"], Field(description="")
-    ] = "AUTOMATIC_ON_DATE"
+    # Id for this conversion trigger, unique within list of ConversionTriggers in
+    # parent convertible issuance's `conversion_triggers` field.
+    trigger_id: str
+    type: Literal["ELECTIVE_IN_RANGE"] = "ELECTIVE_IN_RANGE"
+    # Start date of range (inclusive)
+    start_date: Date
+    # End date of range (inclusive)
+    end_date: Date
+    # Human-friendly nickname to describe the conversion right
+    nickname: Optional[str]
+    # Long-form description of the trigger
+    trigger_description: Optional[str]
+    # When the conditions of the trigger are met, how does the convertible convert?
     conversion_right: Annotated[
         Union[
             ConvertibleConversionRight,
             WarrantConversionRight,
             StockClassConversionRight,
         ],
-        Field(
-            discriminator="type",
-            description="When the conditions of the trigger are met, how does the convertible convert?",
-        ),
+        Field(discriminator="type"),
     ]
```

### Comparing `pyocf-1.0.1/src/pyocf/types/conversion_triggers/electiveconversionatwilltrigger.py` & `pyocf-1.0b1/src/pyocf/types/conversion_triggers/unspecifiedconversiontrigger.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-"""Type representation of elective trigger valid at will (so long as instrument is
-valid and outstanding)."""
+"""Use this where no structured data is available regarding what triggers the"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_triggers/ElectiveConversionAtWillTrigger.sche
-# ma.json
+# ree/main/schema/types/conversion_triggers/UnspecifiedConversionTrigger.schema.js
+# on
 
 from pydantic import Field
 from pyocf.primitives.types.conversion_triggers.conversiontrigger import (
     ConversionTrigger,
 )
 from pyocf.types.conversion_rights.convertibleconversionright import (
     ConvertibleConversionRight,
@@ -23,44 +22,29 @@
 from pyocf.types.conversion_rights.warrantconversionright import WarrantConversionRight
 from typing import Annotated
 from typing import Literal
 from typing import Optional
 from typing import Union
 
 
-class ElectiveConversionAtWillTrigger(ConversionTrigger):
-    """Type representation of elective trigger valid at will (so long as instrument is
-    valid and outstanding).
+class UnspecifiedConversionTrigger(ConversionTrigger):
+    """Use this where no structured data is available regarding what triggers the
+    conversion of a given security.
     """
 
-    trigger_id: Annotated[
-        str,
-        Field(
-            description="Id for this conversion trigger, unique within list of ConversionTriggers in"
-            "parent convertible issuance's `conversion_triggers` field."
-        ),
-    ]
-    nickname: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Human-friendly nickname to describe the conversion right"
-            ),
-        ]
-    ]
-    trigger_description: Optional[
-        Annotated[str, Field(description="Long-form description of the trigger")]
-    ]
-    type: Annotated[
-        Literal["ELECTIVE_AT_WILL"], Field(description="")
-    ] = "ELECTIVE_AT_WILL"
+    # Id for this conversion trigger, unique within list of ConversionTriggers in
+    # parent convertible issuance's `conversion_triggers` field.
+    trigger_id: str
+    # Human-friendly nickname to describe the conversion right
+    nickname: Optional[str]
+    # Long-form description of the trigger
+    trigger_description: Optional[str]
+    type: Literal["UNSPECIFIED"] = "UNSPECIFIED"
+    # When the conditions of the trigger are met, how does the convertible convert?
     conversion_right: Annotated[
         Union[
             ConvertibleConversionRight,
             WarrantConversionRight,
             StockClassConversionRight,
         ],
-        Field(
-            discriminator="type",
-            description="When the conditions of the trigger are met, how does the convertible convert?",
-        ),
+        Field(discriminator="type"),
     ]
```

### Comparing `pyocf-1.0.1/src/pyocf/types/conversion_triggers/electiveconversionindaterangetrigger.py` & `pyocf-1.0b1/src/pyocf/types/conversion_triggers/automaticconversionondatetrigger.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-"""Type representation of elective trigger valid on or after start_date and until
-or before end_date."""
+"""Type representation of an automatic trigger on a date."""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_triggers/ElectiveConversionInDateRangeTrigger
-# .schema.json
+# ree/main/schema/types/conversion_triggers/AutomaticConversionOnDateTrigger.schem
+# a.json
 
 from pydantic import Field
 from pyocf.primitives.types.conversion_triggers.conversiontrigger import (
     ConversionTrigger,
 )
 from pyocf.types.conversion_rights.convertibleconversionright import (
     ConvertibleConversionRight,
@@ -24,46 +23,29 @@
 from pyocf.types.date import Date
 from typing import Annotated
 from typing import Literal
 from typing import Optional
 from typing import Union
 
 
-class ElectiveConversionInDateRangeTrigger(ConversionTrigger):
-    """Type representation of elective trigger valid on or after start_date and until
-    or before end_date.
-    """
+class AutomaticConversionOnDateTrigger(ConversionTrigger):
+    """Type representation of an automatic trigger on a date."""
 
-    trigger_id: Annotated[
-        str,
-        Field(
-            description="Id for this conversion trigger, unique within list of ConversionTriggers in"
-            "parent convertible issuance's `conversion_triggers` field."
-        ),
-    ]
-    type: Annotated[
-        Literal["ELECTIVE_IN_RANGE"], Field(description="")
-    ] = "ELECTIVE_IN_RANGE"
-    start_date: Annotated[Date, Field(description="Start date of range (inclusive)")]
-    end_date: Annotated[Date, Field(description="End date of range (inclusive)")]
-    nickname: Optional[
-        Annotated[
-            str,
-            Field(
-                description="Human-friendly nickname to describe the conversion right"
-            ),
-        ]
-    ]
-    trigger_description: Optional[
-        Annotated[str, Field(description="Long-form description of the trigger")]
-    ]
+    # Date on which trigger occurs automatically (if it hasn't already occured)
+    trigger_date: Date
+    # Id for this conversion trigger, unique within list of ConversionTriggers in
+    # parent convertible issuance's `conversion_triggers` field.
+    trigger_id: str
+    # Human-friendly nickname to describe the conversion right
+    nickname: Optional[str]
+    # Long-form description of the trigger
+    trigger_description: Optional[str]
+    type: Literal["AUTOMATIC_ON_DATE"] = "AUTOMATIC_ON_DATE"
+    # When the conditions of the trigger are met, how does the convertible convert?
     conversion_right: Annotated[
         Union[
             ConvertibleConversionRight,
             WarrantConversionRight,
             StockClassConversionRight,
         ],
-        Field(
-            discriminator="type",
-            description="When the conditions of the trigger are met, how does the convertible convert?",
-        ),
+        Field(discriminator="type"),
     ]
```

### Comparing `pyocf-1.0.1/src/pyocf/types/countrycode.py` & `pyocf-1.0b1/src/pyocf/types/countrycode.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Type representation of an ISO 3166-1 alpha 2 country code"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/CountryCode.schema.json
+# OCF/tree/main/schema/types/CountryCode.schema.json
 
 from pydantic import constr
 from pyocf.simplebase import SimpleBaseModel
 
 
 class CountryCode(SimpleBaseModel):
     """Type representation of an ISO 3166-1 alpha 2 country code"""
```

### Comparing `pyocf-1.0.1/src/pyocf/types/countrysubdivisioncode.py` & `pyocf-1.0b1/src/pyocf/types/countrysubdivisioncode.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Type representation of the second part of an ISO 3166-2 country subdivision code"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/CountrySubdivisionCode.schema.json
+# OCF/tree/main/schema/types/CountrySubdivisionCode.schema.json
 
 from pydantic import constr
 from pyocf.simplebase import SimpleBaseModel
 
 
 class CountrySubdivisionCode(SimpleBaseModel):
     """Type representation of the second part of an ISO 3166-2 country subdivision code"""
```

### Comparing `pyocf-1.0.1/src/pyocf/types/currencycode.py` & `pyocf-1.0b1/src/pyocf/types/currencycode.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Type representation of an ISO 4217 currency code"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/CurrencyCode.schema.json
+# OCF/tree/main/schema/types/CurrencyCode.schema.json
 
 from pydantic import constr
 from pyocf.simplebase import SimpleBaseModel
 
 
 class CurrencyCode(SimpleBaseModel):
     """Type representation of an ISO 4217 currency code"""
```

### Comparing `pyocf-1.0.1/src/pyocf/types/email.py` & `pyocf-1.0b1/src/pyocf/types/email.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """Type representation of an email address"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/Email.schema.json
+# OCF/tree/main/schema/types/Email.schema.json
 
 from pydantic import BaseModel
-from pydantic import Field
 from pyocf.enums.emailtype import EmailType
-from typing import Annotated
 
 
 class Email(BaseModel):
     """Type representation of an email address"""
 
-    email_type: Annotated[
-        EmailType,
-        Field(description="Type of e-mail address (e.g. personal or business)"),
-    ]
-    email_address: Annotated[str, Field(description="A valid e-mail address")]
+    # Type of e-mail address (e.g. personal or business)
+    email_type: EmailType
+    # A valid e-mail address
+    email_address: str
```

### Comparing `pyocf-1.0.1/src/pyocf/types/interestrate.py` & `pyocf-1.0b1/src/pyocf/types/interestrate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,28 @@
 """Type representation of an interest rate, including accrual start and end dates"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/InterestRate.schema.json
+# OCF/tree/main/schema/types/InterestRate.schema.json
 
 from pydantic import BaseModel
-from pydantic import Field
 from pyocf.types.date import Date
 from pyocf.types.percentage import Percentage
-from typing import Annotated
 from typing import Optional
 
 
 class InterestRate(BaseModel):
     """Type representation of an interest rate, including accrual start and end dates"""
 
-    rate: Annotated[
-        Percentage,
-        Field(
-            description="Interest rate for the convertible (decimal representation - e.g. 0.125 for"
-            "12.5%)"
-        ),
-    ]
-    accrual_start_date: Annotated[
-        Date,
-        Field(
-            description="Commencement date for interest accruing at the specified rate"
-        ),
-    ]
-    accrual_end_date: Optional[
-        Annotated[
-            Date,
-            Field(
-                description="Optional end date (inclusive) for interest accruing at the specified rate. If"
-                "none specified, interest will accrue indefinitely or until accrual of next"
-                "interest rate commences"
-            ),
-        ]
-    ]
+    # Interest rate for the convertible (decimal representation - e.g. 0.125 for
+    # 12.5%)
+    rate: Percentage
+    # Commencement date for interest accruing at the specified rate
+    accrual_start_date: Date
+    # Optional end date (inclusive) for interest accruing at the specified rate. If
+    # none specified, interest will accrue indefinitely or until accrual of next
+    # interest rate commences
+    accrual_end_date: Optional[Date]
```

### Comparing `pyocf-1.0.1/src/pyocf/types/md5.py` & `pyocf-1.0b1/src/pyocf/types/md5.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""String representation of MD5 hash with basic validation for a string of 32
-characters composed of letters (uppercase or lowercase) and numbers"""
+"""String representation of MD5 hash with basic validation for a string of 32"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/Md5.schema.json
+# OCF/tree/main/schema/types/Md5.schema.json
 
 from pydantic import constr
 from pyocf.simplebase import SimpleBaseModel
 
 
 class Md5(SimpleBaseModel):
     """String representation of MD5 hash with basic validation for a string of 32
```

### Comparing `pyocf-1.0.1/src/pyocf/types/name.py` & `pyocf-1.0b1/src/pyocf/types/name.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 """Type comprising of multiple name components"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/Name.schema.json
+# OCF/tree/main/schema/types/Name.schema.json
 
 from pydantic import BaseModel
-from pydantic import Field
-from typing import Annotated
 from typing import Optional
 
 
 class Name(BaseModel):
     """Type comprising of multiple name components"""
 
-    legal_name: Annotated[
-        str, Field(description="Legal full name for the individual/institution")
-    ]
-    first_name: Optional[
-        Annotated[str, Field(description="First/given name for the individual")]
-    ]
-    last_name: Optional[
-        Annotated[str, Field(description="Last/family name for the individual")]
-    ]
+    # Legal full name for the individual/institution
+    legal_name: str
+    # First/given name for the individual
+    first_name: Optional[str]
+    # Last/family name for the individual
+    last_name: Optional[str]
```

### Comparing `pyocf-1.0.1/src/pyocf/types/numeric.py` & `pyocf-1.0b1/src/pyocf/types/numeric.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Fixed-point string representation of a number (up to 10 decimal places
-supported)"""
+"""Fixed-point string representation of a number (up to 10 decimal places"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/Numeric.schema.json
+# OCF/tree/main/schema/types/Numeric.schema.json
 
 from decimal import Decimal
 from pyocf.simplebase import SimpleBaseModel
 
 
 class Numeric(SimpleBaseModel):
     """Fixed-point string representation of a number (up to 10 decimal places
```

### Comparing `pyocf-1.0.1/src/pyocf/types/ratio.py` & `pyocf-1.0b1/src/pyocf/types/ratio.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,25 @@
-"""Type representation of a ratio as two parts of a quotient, i.e. numerator and
-denominator numeric values"""
+"""Type representation of a ratio as two parts of a quotient, i.e. numerator and"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/Ratio.schema.json
+# OCF/tree/main/schema/types/Ratio.schema.json
 
 from pydantic import BaseModel
-from pydantic import Field
 from pyocf.types.numeric import Numeric
-from typing import Annotated
 
 
 class Ratio(BaseModel):
     """Type representation of a ratio as two parts of a quotient, i.e. numerator and
     denominator numeric values
     """
 
-    numerator: Annotated[
-        Numeric,
-        Field(
-            description="Numerator of the ratio, i.e. the ratio of A to B (A:B) can be expressed as a"
-            "fraction (A/B), where A is the numerator"
-        ),
-    ]
-    denominator: Annotated[
-        Numeric,
-        Field(
-            description="Denominator of the ratio, i.e. the ratio of A to B (A:B) can be expressed as a"
-            "fraction (A/B), where B is the denominator"
-        ),
-    ]
+    # Numerator of the ratio, i.e. the ratio of A to B (A:B) can be expressed as a
+    # fraction (A/B), where A is the numerator
+    numerator: Numeric
+    # Denominator of the ratio, i.e. the ratio of A to B (A:B) can be expressed as a
+    # fraction (A/B), where B is the denominator
+    denominator: Numeric
```

### Comparing `pyocf-1.0.1/src/pyocf/types/securityexemption.py` & `pyocf-1.0b1/src/pyocf/types/securityexemption.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,25 @@
-"""Type representation of a securities issuance exemption that includes an
-unstructured description and a country code for ease of processing and analysis"""
+"""Type representation of a securities issuance exemption that includes an"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/SecurityExemption.schema.json
+# OCF/tree/main/schema/types/SecurityExemption.schema.json
 
 from pydantic import BaseModel
-from pydantic import Field
-from typing import Annotated
 
 
 class SecurityExemption(BaseModel):
     """Type representation of a securities issuance exemption that includes an
     unstructured description and a country code for ease of processing and analysis
     """
 
-    description: Annotated[
-        str,
-        Field(
-            description="Description of an applicable security law exemption governing the issuance"
-        ),
-    ]
-    jurisdiction: Annotated[
-        str,
-        Field(
-            description="Jurisdiction of the applicable law. This is a free-text field as there is no"
-            "known enumeration of all global legal jurisdictions, but please try to use ISO"
-            "3166-1 alpha-2, if appropriate. Otherwise, we rely on implementers to choose an"
-            "appropriate value here."
-        ),
-    ]
+    # Description of an applicable security law exemption governing the issuance
+    description: str
+    # Jurisdiction of the applicable law. This is a free-text field as there is no
+    # known enumeration of all global legal jurisdictions, but please try to use ISO
+    # 3166-1 alpha-2, if appropriate. Otherwise, we rely on implementers to choose an
+    # appropriate value here.
+    jurisdiction: str
```

### Comparing `pyocf-1.0.1/src/pyocf/types/sharenumberrange.py` & `pyocf-1.0b1/src/pyocf/types/sharenumberrange.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,26 @@
-"""Type representation of a range of share numbers associated with an event (such
-as the share numbers associated with an issuance) - for use where shares are not
-fungible and need unique identifiers *per share*"""
+"""Type representation of a range of share numbers associated with an event (such"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/ShareNumberRange.schema.json
+# OCF/tree/main/schema/types/ShareNumberRange.schema.json
 
 from pydantic import BaseModel
-from pydantic import Field
 from pyocf.types.numeric import Numeric
-from typing import Annotated
 
 
 class ShareNumberRange(BaseModel):
     """Type representation of a range of share numbers associated with an event (such
     as the share numbers associated with an issuance) - for use where shares are not
     fungible and need unique identifiers *per share*
     """
 
-    starting_share_number: Annotated[
-        Numeric,
-        Field(
-            description="The starting share number of a range of shares impacted by a particular event"
-            "(**INCLUSIVE** and assuming **share counts start at 1**)"
-        ),
-    ]
-    ending_share_number: Annotated[
-        Numeric,
-        Field(
-            description="The ending share number of a range of shares impacted by a particular event"
-            "(**INCLUSIVE**)"
-        ),
-    ]
+    # The starting share number of a range of shares impacted by a particular event
+    # (**INCLUSIVE** and assuming **share counts start at 1**)
+    starting_share_number: Numeric
+    # The ending share number of a range of shares impacted by a particular event
+    # (**INCLUSIVE**)
+    ending_share_number: Numeric
```

### Comparing `pyocf-1.0.1/src/pyocf/types/stockparent.py` & `pyocf-1.0b1/src/pyocf/types/stockparent.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,25 @@
-"""Type representation of the parent security of a given stock issuance (e.g. if a
-stock issuance came from a plan, such as an RSA, or if a stock came from a
-previous stock entry)"""
+"""Type representation of the parent security of a given stock issuance (e.g. if a"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/StockParent.schema.json
+# OCF/tree/main/schema/types/StockParent.schema.json
 
 from pydantic import BaseModel
-from pydantic import Field
 from pyocf.enums.parentsecuritytype import ParentSecurityType
-from typing import Annotated
 
 
 class StockParent(BaseModel):
     """Type representation of the parent security of a given stock issuance (e.g. if a
     stock issuance came from a plan, such as an RSA, or if a stock came from a
     previous stock entry)
     """
 
-    parent_object_type: Annotated[
-        ParentSecurityType,
-        Field(
-            description="Parent object type for this stock issuance (e.g. a stock plan or warrant)"
-        ),
-    ]
-    parent_object_id: Annotated[
-        str,
-        Field(
-            description="Parent object's ID must be a valid ID pointing to an object of the type"
-            "specified in parent_object_type"
-        ),
-    ]
+    # Parent object type for this stock issuance (e.g. a stock plan or warrant)
+    parent_object_type: ParentSecurityType
+    # Parent object's ID must be a valid ID pointing to an object of the type
+    # specified in parent_object_type
+    parent_object_id: str
```

### Comparing `pyocf-1.0.1/src/pyocf/types/taxid.py` & `pyocf-1.0b1/src/pyocf/types/taxid.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,23 @@
-"""Type representation of a government identifier for tax purposes (e.g. EIN) and
-corresponding country code (ISO-3166)"""
+"""Type representation of a government identifier for tax purposes (e.g. EIN) and"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/TaxID.schema.json
+# OCF/tree/main/schema/types/TaxID.schema.json
 
 from pydantic import BaseModel
-from pydantic import Field
 from pyocf.types.countrycode import CountryCode
-from typing import Annotated
 
 
 class TaxID(BaseModel):
     """Type representation of a government identifier for tax purposes (e.g. EIN) and
     corresponding country code (ISO-3166)
     """
 
-    tax_id: Annotated[str, Field(description="Tax identifier as string")]
-    country: Annotated[
-        CountryCode,
-        Field(
-            description="Issuing country code (ISO 3166-1 alpha-2) for the tax identifier"
-        ),
-    ]
+    # Tax identifier as string
+    tax_id: str
+    # Issuing country code (ISO 3166-1 alpha-2) for the tax identifier
+    country: CountryCode
```

### Comparing `pyocf-1.0.1/src/pyocf/types/vesting/vestingeventtrigger.py` & `pyocf-1.0b1/src/pyocf/types/vesting/vestingstarttrigger.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,22 @@
-"""Describes a vesting condition satisfied when a particular unscheduled event
-occurs"""
+"""Describes a vesting condition satisfied at the security's vesting commencement"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/vesting/VestingEventTrigger.schema.json
+# OCF/tree/main/schema/types/vesting/VestingStartTrigger.schema.json
 
-from pydantic import Field
 from pyocf.primitives.types.vesting.vestingconditiontrigger import (
     VestingConditionTrigger,
 )
-from typing import Annotated
 from typing import Literal
 
 
-class VestingEventTrigger(VestingConditionTrigger):
-    """Describes a vesting condition satisfied when a particular unscheduled event
-    occurs
+class VestingStartTrigger(VestingConditionTrigger):
+    """Describes a vesting condition satisfied at the security's vesting commencement
+    date
     """
 
-    type: Annotated[Literal["VESTING_EVENT"], Field(description="")] = "VESTING_EVENT"
+    type: Literal["VESTING_START_DATE"] = "VESTING_START_DATE"
```

### Comparing `pyocf-1.0.1/src/pyocf/types/vesting/vestingperiodindays.py` & `pyocf-1.0b1/src/pyocf/types/vesting/vestingperiodindays.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,26 @@
-"""Describes a period of time expressed in days (e.g. 365 days) for use in Vesting
-Terms"""
+"""Describes a period of time expressed in days (e.g. 365 days) for use in Vesting"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/vesting/VestingPeriodInDays.schema.json
+# OCF/tree/main/schema/types/vesting/VestingPeriodInDays.schema.json
 
-from pydantic import Field
 from pyocf.primitives.types.vesting.vestingperiod import VestingPeriod
-from typing import Annotated
 from typing import Literal
 
 
 class VestingPeriodInDays(VestingPeriod):
     """Describes a period of time expressed in days (e.g. 365 days) for use in Vesting
     Terms
     """
 
-    length: Annotated[
-        int,
-        Field(
-            description="The quantity of `type` units of time; e.g. for 3 months, this would be `3`; for"
-            "30 days, this would be `30`"
-        ),
-    ]
-    type: Annotated[Literal["DAYS"], Field(description="")] = "DAYS"
-    occurrences: Annotated[
-        int,
-        Field(
-            description="The number of times this vesting period triggers. If vesting occurs monthly for"
-            "36 months, for example, this would be `36`"
-        ),
-    ]
+    # The quantity of `type` units of time; e.g. for 3 months, this would be `3`; for
+    # 30 days, this would be `30`
+    length: int
+    type: Literal["DAYS"] = "DAYS"
+    # The number of times this vesting period triggers. If vesting occurs monthly for
+    # 36 months, for example, this would be `36`
+    occurrences: int
```

### Comparing `pyocf-1.0.1/src/pyocf/types/vesting/vestingperiodinmonths.py` & `pyocf-1.0b1/src/pyocf/types/vesting/vestingperiodinmonths.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,29 @@
-"""Describes a period of time expressed in months (e.g. 3 months) for use in
-Vesting Terms."""
+"""Describes a period of time expressed in months (e.g. 3 months) for use in"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/vesting/VestingPeriodInMonths.schema.json
+# OCF/tree/main/schema/types/vesting/VestingPeriodInMonths.schema.json
 
-from pydantic import Field
 from pyocf.enums.vestingdayofmonth import VestingDayOfMonth
 from pyocf.primitives.types.vesting.vestingperiod import VestingPeriod
-from typing import Annotated
 from typing import Literal
 
 
 class VestingPeriodInMonths(VestingPeriod):
     """Describes a period of time expressed in months (e.g. 3 months) for use in
     Vesting Terms.
     """
 
-    length: Annotated[
-        int,
-        Field(
-            description="The quantity of `type` units of time; e.g. for 3 months, this would be `3`; for"
-            "30 days, this would be `30`"
-        ),
-    ]
-    type: Annotated[Literal["MONTHS"], Field(description="")] = "MONTHS"
-    occurrences: Annotated[
-        int,
-        Field(
-            description="The number of times this vesting period triggers. If vesting occurs monthly for"
-            "36 months, for example, this would be `36`"
-        ),
-    ]
-    day_of_month: Annotated[
-        VestingDayOfMonth,
-        Field(description="The calendar day of a month to award vesting."),
-    ]
+    # The quantity of `type` units of time; e.g. for 3 months, this would be `3`; for
+    # 30 days, this would be `30`
+    length: int
+    type: Literal["MONTHS"] = "MONTHS"
+    # The number of times this vesting period triggers. If vesting occurs monthly for
+    # 36 months, for example, this would be `36`
+    occurrences: int
+    # The calendar day of a month to award vesting.
+    day_of_month: VestingDayOfMonth
```

### Comparing `pyocf-1.0.1/src/pyocf/types/vesting/vestingscheduleabsolutetrigger.py` & `pyocf-1.0b1/src/pyocf/types/vesting/vestingscheduleabsolutetrigger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 """Describes a vesting condition satisfied on an absolute date."""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/vesting/VestingScheduleAbsoluteTrigger.schema.json
+# OCF/tree/main/schema/types/vesting/VestingScheduleAbsoluteTrigger.schema.json
 
-from pydantic import Field
 from pyocf.primitives.types.vesting.vestingconditiontrigger import (
     VestingConditionTrigger,
 )
 from pyocf.types.date import Date
-from typing import Annotated
 from typing import Literal
 
 
 class VestingScheduleAbsoluteTrigger(VestingConditionTrigger):
     """Describes a vesting condition satisfied on an absolute date."""
 
-    type: Annotated[
-        Literal["VESTING_SCHEDULE_ABSOLUTE"], Field(description="")
-    ] = "VESTING_SCHEDULE_ABSOLUTE"
-    date: Annotated[
-        Date, Field(description="The date on which this condition triggers.")
-    ]
+    type: Literal["VESTING_SCHEDULE_ABSOLUTE"] = "VESTING_SCHEDULE_ABSOLUTE"
+    # The date on which this condition triggers.
+    date: Date
```

### Comparing `pyocf-1.0.1/src/pyocf/types/vesting/vestingschedulerelativetrigger.py` & `pyocf-1.0b1/src/pyocf/types/vesting/vestingschedulerelativetrigger.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Describes a vesting condition satisfied when a period of time, relative to
-another vesting condition, has elapsed."""
+"""Describes a vesting condition satisfied when a period of time, relative to"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/vesting/VestingScheduleRelativeTrigger.schema.json
+# OCF/tree/main/schema/types/vesting/VestingScheduleRelativeTrigger.schema.json
 
 from pydantic import Field
 from pyocf.primitives.types.vesting.vestingconditiontrigger import (
     VestingConditionTrigger,
 )
 from pyocf.types.vesting.vestingperiodindays import VestingPeriodInDays
 from pyocf.types.vesting.vestingperiodinmonths import VestingPeriodInMonths
@@ -21,26 +20,17 @@
 
 
 class VestingScheduleRelativeTrigger(VestingConditionTrigger):
     """Describes a vesting condition satisfied when a period of time, relative to
     another vesting condition, has elapsed.
     """
 
-    type: Annotated[
-        Literal["VESTING_SCHEDULE_RELATIVE"], Field(description="")
-    ] = "VESTING_SCHEDULE_RELATIVE"
+    type: Literal["VESTING_SCHEDULE_RELATIVE"] = "VESTING_SCHEDULE_RELATIVE"
+    # The span of time that must have elapsed since the condition
+    # `relative_to_condition_id` occurred for this condition to trigger. For weeks or
+    # "ideal" years (365 days), use `VestingPeriodInDays`. For calendar years use
+    # `VestingPeriodInMonths`.
     period: Annotated[
-        Union[VestingPeriodInDays, VestingPeriodInMonths],
-        Field(
-            discriminator="type",
-            description="The span of time that must have elapsed since the condition"
-            "`relative_to_condition_id` occurred for this condition to trigger. For weeks or"
-            '"ideal" years (365 days), use `VestingPeriodInDays`. For calendar years use'
-            "`VestingPeriodInMonths`.",
-        ),
-    ]
-    relative_to_condition_id: Annotated[
-        str,
-        Field(
-            description="Reference to the vesting condition ID to which the `period` is relative"
-        ),
+        Union[VestingPeriodInDays, VestingPeriodInMonths], Field(discriminator="type")
     ]
+    # Reference to the vesting condition ID to which the `period` is relative
+    relative_to_condition_id: str
```

### Comparing `pyocf-1.0.1/src/pyocf/types/vesting/vestingstarttrigger.py` & `pyocf-1.0b1/src/pyocf/types/vesting/vestingeventtrigger.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-"""Describes a vesting condition satisfied at the security\'s vesting commencement
-date"""
+"""Describes a vesting condition satisfied when a particular unscheduled event"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/vesting/VestingStartTrigger.schema.json
+# OCF/tree/main/schema/types/vesting/VestingEventTrigger.schema.json
 
-from pydantic import Field
 from pyocf.primitives.types.vesting.vestingconditiontrigger import (
     VestingConditionTrigger,
 )
-from typing import Annotated
 from typing import Literal
 
 
-class VestingStartTrigger(VestingConditionTrigger):
-    """Describes a vesting condition satisfied at the security\'s vesting commencement
-    date
+class VestingEventTrigger(VestingConditionTrigger):
+    """Describes a vesting condition satisfied when a particular unscheduled event
+    occurs
     """
 
-    type: Annotated[
-        Literal["VESTING_START_DATE"], Field(description="")
-    ] = "VESTING_START_DATE"
+    type: Literal["VESTING_EVENT"] = "VESTING_EVENT"
```

### Comparing `pyocf-1.0.1/src/pyocf.egg-info/SOURCES.txt` & `pyocf-1.0b1/src/pyocf.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 .pre-commit-config.yaml
-.readthedocs.yaml
 CHANGES.txt
 LICENSE.txt
 MANIFEST.in
 Makefile
 README.rst
 setup.cfg
 setup.py
 src/pyocf/__init__.py
-src/pyocf/api.py
 src/pyocf/captable.py
 src/pyocf/simplebase.py
 src/pyocf.egg-info/PKG-INFO
 src/pyocf.egg-info/SOURCES.txt
 src/pyocf.egg-info/dependency_links.txt
 src/pyocf.egg-info/requires.txt
 src/pyocf.egg-info/top_level.txt
@@ -164,14 +162,15 @@
 src/pyocf/types/interestrate.py
 src/pyocf/types/md5.py
 src/pyocf/types/monetary.py
 src/pyocf/types/name.py
 src/pyocf/types/numeric.py
 src/pyocf/types/percentage.py
 src/pyocf/types/phone.py
+src/pyocf/types/prereleaseomission.py
 src/pyocf/types/ratio.py
 src/pyocf/types/securityexemption.py
 src/pyocf/types/sharenumberrange.py
 src/pyocf/types/stockparent.py
 src/pyocf/types/taxid.py
 src/pyocf/types/terminationwindow.py
 src/pyocf/types/conversion_mechanisms/__init__.py
```

### Comparing `pyocf-1.0.1/tests/samples/Captable.ocf.zip` & `pyocf-1.0b1/tests/samples/Captable.ocf.zip`

 * *Files 15% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
 Zip file size: 12054 bytes, number of entries: 11
--rw-r--r--  3.0 unx     2126 tx defN 23-Jul-06 09:42 Manifest.ocf.json
--rw-r--r--  3.0 unx      544 tx defN 23-Jul-06 09:42 Stakeholders.ocf.json
--rw-r--r--  3.0 unx     1672 tx defN 23-Jul-06 09:42 StockClasses.ocf.json
--rw-r--r--  3.0 unx      667 tx defN 23-Jul-06 09:42 StockLegends.ocf.json
--rw-r--r--  3.0 unx      480 tx defN 23-Jul-06 09:42 StockPlans.ocf.json
--rw-r--r--  3.0 unx    34857 tx defN 23-Jul-06 09:42 Transactions.ocf.json
--rw-r--r--  3.0 unx      505 tx defN 23-Jul-06 09:42 Valuations.ocf.json
--rw-r--r--  3.0 unx    13193 tx defN 23-Jul-06 09:42 VestingTerms.ocf.json
--rw-r--r--  3.0 unx      669 tx defN 23-Jul-06 09:42 VestingTerms.example1.ocf.json
--rw-r--r--  3.0 unx     1988 tx defN 23-Jul-06 09:42 VestingTerms.example2.ocf.json
--rw-r--r--  3.0 unx      440 tx defN 23-Jul-06 09:42 VestingTransactions.examples.ocf.json
+-rw-rw-r--  3.0 unx     2126 tx defN 23-Mar-15 19:30 Manifest.ocf.json
+-rw-rw-r--  3.0 unx      544 tx defN 23-Mar-15 19:30 Stakeholders.ocf.json
+-rw-rw-r--  3.0 unx     1672 tx defN 23-Mar-15 19:30 StockClasses.ocf.json
+-rw-rw-r--  3.0 unx      667 tx defN 23-Mar-15 19:30 StockLegends.ocf.json
+-rw-rw-r--  3.0 unx      480 tx defN 23-Mar-15 19:30 StockPlans.ocf.json
+-rw-rw-r--  3.0 unx    34857 tx defN 23-Mar-15 19:30 Transactions.ocf.json
+-rw-rw-r--  3.0 unx      505 tx defN 23-Mar-15 19:30 Valuations.ocf.json
+-rw-rw-r--  3.0 unx    13193 tx defN 23-Mar-15 19:30 VestingTerms.ocf.json
+-rw-rw-r--  3.0 unx      669 tx defN 23-Mar-15 19:30 VestingTerms.example1.ocf.json
+-rw-rw-r--  3.0 unx     1988 tx defN 23-Mar-15 19:30 VestingTerms.example2.ocf.json
+-rw-rw-r--  3.0 unx      440 tx defN 23-Mar-15 19:30 VestingTransactions.examples.ocf.json
 11 files, 57141 bytes uncompressed, 10110 bytes compressed:  82.3%
```

### Comparing `pyocf-1.0.1/tests/test_load.py` & `pyocf-1.0b1/tests/test_load.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,274 +1,339 @@
-# Copyright © 2023 FMR LLC
-
 import datetime
 import decimal
 import json
 
 from pathlib import Path
-from pyocf import api
+from pyocf.files import (
+    ocfmanifestfile,
+    stakeholdersfile,
+    stockclassesfile,
+    stocklegendtemplatesfile,
+    stockplansfile,
+    transactionsfile,
+    valuationsfile,
+    vestingtermsfile,
+)
 from pyocf.captable import Captable
+from pyocf.objects import (
+    transactions,
+    stockplan,
+    stakeholder,
+    stockclass,
+    stocklegendtemplate,
+    valuation,
+    vestingterms,
+)
+from pyocf.types import (
+    conversion_mechanisms as conv_mechs,
+    conversion_rights as conv_rights,
+    conversion_triggers as conv_trigs,
+    file,
+    interestrate,
+    name,
+    numeric,
+    monetary,
+    vesting,
+)
+from pyocf.enums import (
+    accrualperiodtype,
+    allocationtype,
+    compoundingtype,
+    daycounttype,
+    interestpayouttype,
+    ocfversiontype,
+    stockclasstype,
+    vestingdayofmonth,
+)
+
 
 sample_path = Path(Path(__file__).parent.parent, "Open-Cap-Format-OCF/samples")
 
 
 def test_load_sample_manifest():
     path = Path(Path(__file__).parent, Path(sample_path, "Manifest.ocf.json"))
     with path.open("rt") as infile:
-        obj = api.OCFManifestFile(**json.load(infile))
+        obj = ocfmanifestfile.OCFManifestFile(**json.load(infile))
 
-    assert obj.ocf_version == api.OCFVersionType.ENUM_100
+    assert obj.ocf_version == ocfversiontype.OCFVersionType.ENUM_100
     assert obj.comments == [
         "This is an optional comment",
         """These md5 hashes are just dummy values. They've not been recalculated """
         """in a long time, but we should look into recalculating them dynamically """
         """via an actions or pre-commit hook.""",
     ]
     assert len(obj.stakeholders_files) == 1
-    assert isinstance(obj.stakeholders_files[0], api.File)
+    assert isinstance(obj.stakeholders_files[0], file.File)
 
 
 def test_load_sample_stakeholders():
     path = Path(Path(__file__).parent, Path(sample_path, "Stakeholders.ocf.json"))
     with path.open("rt") as infile:
-        obj = api.StakeholdersFile(**json.load(infile))
+        obj = stakeholdersfile.StakeholdersFile(**json.load(infile))
     assert len(obj.items) == 2
     item = obj.items[0]
-    assert isinstance(item, api.Stakeholder)
+    assert isinstance(item, stakeholder.Stakeholder)
     assert item.object_type == "STAKEHOLDER"
-    assert isinstance(item.name, api.Name)
+    assert isinstance(item.name, name.Name)
 
 
 def test_load_sample_stock_classes():
     path = Path(Path(__file__).parent, Path(sample_path, "StockClasses.ocf.json"))
     with path.open("rt") as infile:
-        obj = api.StockClassesFile(**json.load(infile))
+        obj = stockclassesfile.StockClassesFile(**json.load(infile))
 
     assert len(obj.items) == 2
     item = obj.items[0]
-    assert isinstance(item, api.StockClass)
+    assert isinstance(item, stockclass.StockClass)
     assert item.object_type == "STOCK_CLASS"
     assert item.name == "Common Stock"
-    assert item.class_type == api.StockClassType.ENUM_COMMON
-    assert isinstance(item.par_value, api.Monetary)
+    assert item.class_type == stockclasstype.StockClassType.ENUM_COMMON
+    assert isinstance(item.par_value, monetary.Monetary)
     assert item.par_value.currency == "USD"
     assert item.par_value.amount == decimal.Decimal("0.0001000000")
 
     item = obj.items[1]
-    assert item.class_type == api.StockClassType.ENUM_PREFERRED
+    assert item.class_type == stockclasstype.StockClassType.ENUM_PREFERRED
 
 
 def test_load_sample_stock_legend_templates():
     path = Path(Path(__file__).parent, Path(sample_path, "StockLegends.ocf.json"))
     with path.open("rt") as infile:
-        obj = api.StockLegendTemplatesFile(**json.load(infile))
+        obj = stocklegendtemplatesfile.StockLegendTemplatesFile(**json.load(infile))
 
     assert len(obj.items) == 1
     item = obj.items[0]
-    assert isinstance(item, api.StockLegendTemplate)
+    assert isinstance(item, stocklegendtemplate.StockLegendTemplate)
     item.object_type == "STOCK_LEGEND_TEMPLATE"
     item.name == "1933 Act Legend"
 
 
 def test_load_sample_stock_plans():
     path = Path(Path(__file__).parent, Path(sample_path, "StockPlans.ocf.json"))
     with path.open("rt") as infile:
-        obj = api.StockPlansFile(**json.load(infile))
+        obj = stockplansfile.StockPlansFile(**json.load(infile))
     assert len(obj.items) == 1
     item = obj.items[0]
-    assert isinstance(item, api.StockPlan)
+    assert isinstance(item, stockplan.StockPlan)
     assert item.object_type == "STOCK_PLAN"
     assert item.plan_name == "2021 Stock Incentive Plan"
     assert item.board_approval_date == datetime.date(1983, 12, 31)
     assert item.initial_shares_reserved == decimal.Decimal("10000000")
     assert item.stock_class_id == "8d8371e8-d41d-4a49-9f42-b91758fd155d"
     assert item.comments == [
         "Using new form of SOP released by Firm Y's benefits & comp team on 10/10/2021."
     ]
 
 
 def test_load_sample_transactions():
     path = Path(Path(__file__).parent, Path(sample_path, "Transactions.ocf.json"))
     with path.open("rt") as infile:
-        obj = api.TransactionsFile(**json.load(infile))
+        obj = transactionsfile.TransactionsFile(**json.load(infile))
     item = obj.items[0]
-    assert isinstance(item, api.ConvertibleAcceptance)
+    assert isinstance(
+        item, transactions.acceptance.convertibleacceptance.ConvertibleAcceptance
+    )
     assert item.id == "test-convertible-acceptance-minimal"
     assert item.security_id == "2936wa8yefhdsvcn"
     assert item.object_type == "TX_CONVERTIBLE_ACCEPTANCE"
     assert item.date == datetime.date(2022, 1, 20)
 
     item = obj.items[8]
-    assert isinstance(item, api.ConvertibleIssuance)
+    assert isinstance(
+        item, transactions.issuance.convertibleissuance.ConvertibleIssuance
+    )
     assert item.id == "test-convertible-issuance-minimal"
     assert item.security_id == "con_123456"
     assert item.object_type == "TX_CONVERTIBLE_ISSUANCE"
     assert item.date == datetime.date(1978, 5, 27)
     assert item.comments is None
     trigger = item.conversion_triggers[0]
     assert isinstance(
         trigger,
-        api.AutomaticConversionOnDateTrigger,
+        conv_trigs.automaticconversionondatetrigger.AutomaticConversionOnDateTrigger,
     )
     assert trigger.type == "AUTOMATIC_ON_DATE"
     assert trigger.trigger_id == "CN-1.TRIG.1"
     assert trigger.nickname == "Converts on Maturity"
     assert (
         trigger.trigger_description == "The note shall convert on the date of maturity"
     )
     assert trigger.trigger_date == datetime.date(2022, 1, 1)
 
     cr = trigger.conversion_right
-    assert isinstance(cr, api.ConvertibleConversionRight)
+    assert isinstance(
+        cr, conv_rights.convertibleconversionright.ConvertibleConversionRight
+    )
     assert cr.type == "CONVERTIBLE_CONVERSION_RIGHT"
     cm = cr.conversion_mechanism
-    assert isinstance(cm, api.NoteConversionMechanism)
+    assert isinstance(cm, conv_mechs.noteconversionmechanism.NoteConversionMechanism)
     assert cm.type == "CONVERTIBLE_NOTE_CONVERSION"
-    assert cm.day_count_convention == api.DayCountType.ENUM_ACTUAL_365
-    assert cm.interest_payout == api.InterestPayoutType.ENUM_DEFERRED
-    assert cm.interest_accrual_period == api.AccrualPeriodType.ENUM_MONTHLY
-    assert cm.compounding_type == api.CompoundingType.ENUM_COMPOUNDING
+    assert cm.day_count_convention == daycounttype.DayCountType.ENUM_ACTUAL_365
+    assert cm.interest_payout == interestpayouttype.InterestPayoutType.ENUM_DEFERRED
+    assert (
+        cm.interest_accrual_period == accrualperiodtype.AccrualPeriodType.ENUM_MONTHLY
+    )
+    assert cm.compounding_type == compoundingtype.CompoundingType.ENUM_COMPOUNDING
     assert cm.conversion_discount is None
     assert cm.conversion_valuation_cap is None
     assert cm.exit_multiple is None
     assert cm.conversion_mfn is None
     ir = cm.interest_rates[0]
-    assert isinstance(ir, api.InterestRate)
+    assert isinstance(ir, interestrate.InterestRate)
     assert ir.rate == "0.0899"
     assert ir.accrual_start_date == datetime.date(2021, 1, 1)
     assert ir.accrual_end_date is None
 
     item = obj.items[58]
-    assert isinstance(item, api.WarrantAcceptance)
+    assert isinstance(item, transactions.acceptance.warrantacceptance.WarrantAcceptance)
     assert item.id == "test-warrant-acceptance-full-fields"
     assert item.security_id == "test-security-id"
     assert item.object_type == "TX_WARRANT_ACCEPTANCE"
     assert item.date == datetime.date(2022, 2, 1)
     assert item.comments == ["Here is a comment", "Here is another comment"]
 
     item = obj.items[63]
-    assert isinstance(item, api.WarrantIssuance)
+    assert isinstance(item, transactions.issuance.warrantissuance.WarrantIssuance)
     assert item.id == "test-warrant-issuance-minimal"
     assert item.custom_id == "W-1"
     assert item.object_type == "TX_WARRANT_ISSUANCE"
-    assert isinstance(item.exercise_price, api.Monetary)
+    assert isinstance(item.exercise_price, monetary.Monetary)
     assert item.exercise_price.amount == 1
-    assert isinstance(item.purchase_price, api.Monetary)
+    assert isinstance(item.purchase_price, monetary.Monetary)
     assert item.purchase_price.amount == 1
 
     et = item.exercise_triggers[0]
-    assert isinstance(et, api.AutomaticConversionOnConditionTrigger)
+    accot = conv_trigs.automaticconversiononconditiontrigger
+    assert isinstance(et, accot.AutomaticConversionOnConditionTrigger)
     assert et.type == "AUTOMATIC_ON_CONDITION"
     assert et.trigger_id == "WARRANT-1.TRIG.1"
     assert et.nickname.startswith("Automatic exercise immediately prior to")
 
     cr = et.conversion_right
-    assert isinstance(cr, api.WarrantConversionRight)
+    assert isinstance(cr, conv_rights.warrantconversionright.WarrantConversionRight)
     assert cr.type == "WARRANT_CONVERSION_RIGHT"
     assert cr.converts_to_future_round is None
     assert cr.converts_to_stock_class_id == "stock-class-id"
 
     cm = cr.conversion_mechanism
-    assert isinstance(cm, api.FixedAmountConversionMechanism)
+    assert isinstance(
+        cm, conv_mechs.fixedamountconversionmechanism.FixedAmountConversionMechanism
+    )
     assert cm.type == "FIXED_AMOUNT_CONVERSION"
     assert cm.converts_to_quantity == decimal.Decimal("10000.00")
 
     item = obj.items[67]
-    assert isinstance(item, api.WarrantRetraction)
+    assert isinstance(item, transactions.retraction.warrantretraction.WarrantRetraction)
     assert item.id == "test-warrant-retraction-full-fields"
     assert item.security_id == "test-security-id"
     assert item.object_type == "TX_WARRANT_RETRACTION"
     assert item.reason_text == "Need to retract"
     assert item.date == datetime.date(2022, 2, 1)
     assert item.comments == ["Here is a comment", "Here is another comment"]
 
 
 def test_load_sample_valuations_files():
     path = Path(Path(__file__).parent, Path(sample_path, "Valuations.ocf.json"))
     with path.open("rt") as infile:
-        obj = api.ValuationsFile(**json.load(infile))
+        obj = valuationsfile.ValuationsFile(**json.load(infile))
 
     assert len(obj.items) == 1
     item = obj.items[0]
-    assert isinstance(item, api.Valuation)
+    assert isinstance(item, valuation.Valuation)
     item.object_type == "VALUATION"
     item.valuation_type == "409A",
 
 
 def test_load_sample_vesting_terms():
     path = Path(Path(__file__).parent, Path(sample_path, "VestingTerms.ocf.json"))
     with path.open("rt") as infile:
-        obj = api.VestingTermsFile(**json.load(infile))
+        obj = vestingtermsfile.VestingTermsFile(**json.load(infile))
 
     assert len(obj.items) == 5
     item = obj.items[0]
-    assert isinstance(item, api.VestingTerms)
+    assert isinstance(item, vestingterms.VestingTerms)
     item.object_type == "VESTING_TERMS"
     assert item.name == "Four Year / One Year Cliff"
-    assert item.allocation_type == api.AllocationType.ENUM_CUMULATIVE_ROUNDING
+    assert (
+        item.allocation_type == allocationtype.AllocationType.ENUM_CUMULATIVE_ROUNDING
+    )
 
     assert len(item.vesting_conditions) == 3
-    assert isinstance(item.vesting_conditions[0], api.VestingCondition)
+    assert isinstance(
+        item.vesting_conditions[0], vesting.vestingcondition.VestingCondition
+    )
     assert item.vesting_conditions[0].id == "vesting-start"
     assert item.vesting_conditions[0].next_condition_ids == ["cliff"]
 
     # Vesting conditions can have different trigger types
     condition = item.vesting_conditions[0]
-    assert isinstance(condition.trigger, api.VestingStartTrigger)
+    assert isinstance(
+        condition.trigger, vesting.vestingstarttrigger.VestingStartTrigger
+    )
     assert condition.portion is None
 
     condition = item.vesting_conditions[1]
-    assert isinstance(condition.portion, api.VestingConditionPortion)
+    assert isinstance(
+        condition.portion, vesting.vestingconditionportion.VestingConditionPortion
+    )
     # You can instantiate simple types by just passing in the value
-    assert condition.portion.numerator == api.Numeric("12")
+    assert condition.portion.numerator == numeric.Numeric("12")
     # But pydantic will pass it in with the name "__root__"
-    assert condition.portion.denominator == api.Numeric(__root__="48")
+    assert condition.portion.denominator == numeric.Numeric(__root__="48")
 
     trigger = condition.trigger
-    assert isinstance(trigger, api.VestingScheduleRelativeTrigger)
-    assert isinstance(trigger.period, api.VestingPeriodInMonths)
+    assert isinstance(
+        trigger, vesting.vestingschedulerelativetrigger.VestingScheduleRelativeTrigger
+    )
+    assert isinstance(
+        trigger.period, vesting.vestingperiodinmonths.VestingPeriodInMonths
+    )
     assert trigger.period.length == 12
     assert trigger.period.occurrences == 1
     assert (
         trigger.period.day_of_month
-        == api.VestingDayOfMonth.ENUM_VESTING_START_DAY_OR_LAST_DAY_OF_MONTH
+        == vestingdayofmonth.VestingDayOfMonth.ENUM_VESTING_START_DAY_OR_LAST_DAY_OF_MONTH
     )
 
     condition = item.vesting_conditions[2]
     trigger = condition.trigger
     assert trigger.period.length == 1
     assert trigger.period.occurrences == 36
 
     item = obj.items[1]
-    assert item.allocation_type == api.AllocationType.ENUM_CUMULATIVE_ROUND_DOWN
+    assert (
+        item.allocation_type == allocationtype.AllocationType.ENUM_CUMULATIVE_ROUND_DOWN
+    )
     assert len(item.vesting_conditions) == 8
-    assert isinstance(item.vesting_conditions[0], api.VestingCondition)
+    assert isinstance(
+        item.vesting_conditions[0], vesting.vestingcondition.VestingCondition
+    )
     assert item.vesting_conditions[0].id == "vesting-start"
 
     condition = item.vesting_conditions[1]
     assert condition.portion is None
     assert condition.quantity == 0
 
     condition = item.vesting_conditions[2]
     assert condition.portion.numerator == 1
     assert condition.portion.denominator == 1
 
     trigger = condition.trigger
-    assert isinstance(trigger, api.VestingEventTrigger)
+    assert isinstance(trigger, vesting.vestingeventtrigger.VestingEventTrigger)
     assert trigger.type == "VESTING_EVENT"
 
     item = obj.items[3]
-    assert item.allocation_type == api.AllocationType.ENUM_BACK_LOADED
+    assert item.allocation_type == allocationtype.AllocationType.ENUM_BACK_LOADED
 
     item = obj.items[4]
     condition = item.vesting_conditions[4]
     assert condition.quantity == 0
     assert isinstance(
         condition.trigger,
-        api.VestingScheduleAbsoluteTrigger,
+        vesting.vestingscheduleabsolutetrigger.VestingScheduleAbsoluteTrigger,
     )
     assert condition.trigger.date == datetime.date(2017, 4, 1)
 
 
 def test_load_captable_directory():
     path = Path(Path(__file__).parent, Path(sample_path, "Manifest.ocf.json"))
     # Just check that each type of data is not empty, ie, that it has been loaded.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyocf-1.0.1/tests/test_save.py` & `pyocf-1.0b1/tests/test_save.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,47 @@
-# Copyright © 2023 FMR LLC
-
 import tempfile
 import zipfile
 
 from pathlib import Path
 
 from pyocf.captable import Captable
 
 sample_path = Path(Path(__file__).parent.parent, "Open-Cap-Format-OCF/samples")
 
 
 def test_save_zip():
     path = Path(Path(__file__).parent, "samples/Captable.ocf.zip")
     captable = Captable.load(path)
 
-    try:
-        with tempfile.TemporaryDirectory() as outdir:
-            outpath = Path(outdir, "outfile.zip")
-
-            captable.save(outpath, pretty=True)
-            with zipfile.ZipFile(outpath) as zipped:
-                assert len(zipped.filelist) == 8
-                # Make sure the manifest file is in there
-                assert zipped.filelist[7].filename == "Manifest.ocf.json"
-
-                manifest = zipped.open("Manifest.ocf.json")
-                data = manifest.read()
-
-                # Do some simple checks on the data
-                assert b'"file_type": "OCF_MANIFEST_FILE"' in data
-                assert b'"filepath": "StockLegends.ocf.json",' in data
-
-            outpath.unlink()
-
-    except (PermissionError, NotADirectoryError):
-        # Bugs in windows give permission errors for absolutely no reason
-        # when deleting temporary files. Ignore them.
-        pass
+    with tempfile.NamedTemporaryFile("wb") as outfile:
+        captable.save(outfile, pretty=True)
+
+        zipped = zipfile.ZipFile(outfile.name)
+        assert len(zipped.filelist) == 8
+        # Make sure the manifest file is in there
+        assert zipped.filelist[7].filename == "Manifest.ocf.json"
+
+        manifest = zipped.open("Manifest.ocf.json")
+        data = manifest.read()
+
+        # Do some simple checks on the data
+        assert b'"file_type": "OCF_MANIFEST_FILE"' in data
+        assert b'"filepath": "StockLegends.ocf.json",' in data
 
 
 def test_save_directory():
     path = Path(Path(__file__).parent, "samples/Captable.ocf.zip")
     captable = Captable.load(path)
 
-    try:
-        with tempfile.TemporaryDirectory() as outdir:
-            captable.save(outdir, zip=False, pretty=True)
-
-            path = Path(outdir)
-            files = [x for x in path.iterdir()]
-            assert len(files) == 8
-            # Make sure the manifest file is in there
-            manifest = [x for x in files if x.name == "Manifest.ocf.json"][0]
-            data = manifest.open("rb").read()
-
-            # Do some simple checks on the data
-            assert b'"file_type": "OCF_MANIFEST_FILE"' in data
-            assert b'"filepath": "StockLegends.ocf.json",' in data
-    except (PermissionError, NotADirectoryError):
-        # Bugs in windows give permission errors for absolutely no reason
-        # when deleting temporary files. Ignore them.
-        pass
+    with tempfile.TemporaryDirectory() as outdir:
+        captable.save(outdir, zip=False, pretty=True)
+
+        path = Path(outdir)
+        files = [x for x in path.iterdir()]
+        assert len(files) == 8
+        # Make sure the manifest file is in there
+        manifest = [x for x in files if x.name == "Manifest.ocf.json"][0]
+        data = manifest.open("rb").read()
+
+        # Do some simple checks on the data
+        assert b'"file_type": "OCF_MANIFEST_FILE"' in data
+        assert b'"filepath": "StockLegends.ocf.json",' in data
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyocf-1.0.1/utils/generate.py` & `pyocf-1.0b1/utils/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 
 def multilinewrap(text):
     # Black doesn't wrap comments, so we have to.
     # But that's the easy bit anyway. We let Black handle the code formatting.
     result = []
     for line in text.splitlines():
-        line = line.replace('"', '\\"').replace("'", "\\'")
         result.extend(textwrap.wrap(line, 80))
 
     return result
 
 
 class Reference:
     def __init__(self, refid):
@@ -97,16 +96,15 @@
             # It's a union of one, just return the one.
             return types[0]
 
         return PROPERTY_TYPES_MAP[type_]
 
     @property
     def description(self):
-        desc = "'\n         '".join(multilinewrap(self.json.get("description", "")))
-        return f"{desc}"
+        return multilinewrap(self.json.get("description", ""))
 
     def get_discriminator(self, json):
         if "anyOf" in json:
             # Pick the last one, because the first one can be null
             subschema = json["anyOf"][-1]["$ref"].resolve()
         elif "oneOf" in json:
             # Pick the last one, because the first one can be null
@@ -148,19 +146,16 @@
         if subtype:
             type_ = f"{type_}[{subtype}]"
 
         if type_.startswith("Union["):
             discriminator = self.get_discriminator(self.json)
             if discriminator is not None:
                 type_ = (
-                    f"Annotated[{type_}, "
-                    f"Field(discriminator='{discriminator}', description='{self.description}')]"
+                    f"Annotated[{type_}, " f"Field(discriminator='{discriminator}')]"
                 )
-        else:
-            type_ = f"Annotated[{type_}, " f"Field(description='{self.description}')]"
 
         if not self.required:
             type_ = f"Optional[{type_}]"
 
         type_ = f"{self.name}: {type_}"
 
         if "Literal" in type_:
@@ -339,14 +334,17 @@
             if isinstance(superclass, Schema):
                 imports.add(superclass.import_statement)
             elif superclass == "BaseModel":
                 imports.add("from pydantic import BaseModel")
             elif superclass == "SimpleBaseModel":
                 imports.add("from pyocf.simplebase import SimpleBaseModel")
 
+        if list(self.validators):
+            imports.add("from pydantic import root_validator")
+
         if self.root_constraint:
             if "constr" in self.root_constraint:
                 imports.add("from pydantic import constr")
             if "date" in self.root_constraint:
                 imports.add("from datetime import date")
             if "Decimal" in self.root_constraint:
                 imports.add("from decimal import Decimal")
@@ -360,14 +358,43 @@
         path = ("pyocf",) + self.path.parts[root:]
         pkg = ".".join(path[:-1])
         module = self.filename.split(".")[0]
         imp = f"from {pkg}.{module} import {self.name}"
         return imp
 
     @property
+    def validators(self):
+        """Custom validators, pretty unique per class"""
+        if "anyOf" in self.json:
+            # This currently just supports the case when one property is
+            # required when another property is set to a specific value,
+            # like PlanSecurityIssuance.schema.json
+            assert len(self.json["anyOf"]) == 2
+            for item in self.json["anyOf"]:
+                if "required" in item:
+                    break
+            else:
+                return None
+
+            parameter = list(item["properties"].keys())[0]
+            value = item["properties"][parameter]["const"]
+            required = item["required"][0]
+
+            yield f"""@root_validator(pre=True)
+    def validator_{parameter}(cls, values):
+        if (values.get("{parameter}") == "{value}" and
+            values.get("{required}") is None):
+            raise ValueError(
+                "When {parameter} is '{value}' then {required} is required"
+            )
+
+        return values
+"""
+
+    @property
     def root_constraint(self):
         if "format" in self.json:
             return self.json["format"]
         if self.name == "Numeric":
             return "Decimal"
 
         if "pattern" in self.json:
@@ -391,53 +418,35 @@
         if filepath.name.startswith("_"):
             continue
         if filepath.is_dir():
             make_inits(filepath, types)
         elif not filepath.name.endswith(".py"):
             continue
 
-    with pathlib.Path(path, "__init__.py").open("wt", encoding="utf-8") as initfile:
+    with pathlib.Path(path, "__init__.py").open("wt") as initfile:
         initfile.write(f'"""OCF {path.parts[-1]}"""')
 
 
 def generate_files():
     templdir = pathlib.Path(__file__).parent
     outdir = pathlib.Path(templdir.parent, "src/pyocf")
     types = defaultdict(dict)
     roottypes = defaultdict(dict)
-    all_classes = {}
     for schema in all_schemas.values():
         rootlevel = schema.path.parts.index("schema") + 1
         schema_dir = pathlib.Path(*schema.path.parts[rootlevel:-1])
         object_type = schema.object_type
         if object_type is not None:
             types[pathlib.Path(outdir, schema_dir)][object_type] = schema
             roottypes[object_type] = schema
         tmpl = Template(filename=f"{templdir}/{schema.metatype}.mako")
         path = pathlib.Path(schema_dir, schema.filename + ".py")
         outfile = pathlib.Path(outdir, path)
         outfile.parent.mkdir(parents=True, exist_ok=True)
-        with outfile.open("wt", encoding="utf-8") as outfile:
+        with outfile.open("tw") as outfile:
             outfile.write(tmpl.render(schema=schema))
-        if schema.name in all_classes:
-            raise ValueError(
-                "The schema has changed to include duplicate class names, "
-                "that's new and needs dealing with!"
-            )
-        all_classes[schema.name] = schema.import_statement
-
-    classes_file = pathlib.Path(outdir, "api.py")
-    with classes_file.open("wt", encoding="utf-8") as outfile:
-        outfile.write('"""All PyOCF classes, for easier import"""\n\n')
-        outfile.write("# Autogenerated, do not edit.\n# Copyright © 2023 FMR LLC\n\n")
-
-        for imports in sorted(all_classes.values()):
-            outfile.write(f"{imports}\n")
-
-        outfile.write(f"\n__all__ = [{', '.join(sorted(all_classes))}]")
-
     make_inits(outdir, types)
 
 
 if __name__ == "__main__":
     load_schemas("./Open-Cap-Format-OCF/schema")
     generate_files()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyocf-1.0.1/utils/object.mako` & `pyocf-1.0b1/utils/object.mako`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-"""${schema.description}"""
+"""${schema.description.splitlines()[0]}"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
 % for line in schema.comment.splitlines():
 # ${line}
 % endfor
 
 % if schema.import_statements:
@@ -20,9 +20,16 @@
     """
 
     % if schema.root_constraint:
     __root__: ${schema.root_constraint}
 
     % endif
     % for property in schema.properties:
+    % for line in property.description:
+    # ${line}
+    % endfor
     ${property.definition}
     % endfor
+
+    % for validator in schema.validators:
+    ${validator}
+    % endfor
```

