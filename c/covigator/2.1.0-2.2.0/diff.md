# Comparing `tmp/covigator-2.1.0.tar.gz` & `tmp/covigator-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covigator-2.1.0.tar", last modified: Mon Feb 13 14:28:03 2023, max compression
+gzip compressed data, was "covigator-2.2.0.tar", last modified: Thu Jul  6 08:20:31 2023, max compression
```

## Comparing `covigator-2.1.0.tar` & `covigator-2.2.0.tar`

### file list

```diff
@@ -1,164 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 14:28:03.951282 covigator-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1066 2023-02-13 14:27:55.000000 covigator-2.1.0/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (122)      178 2023-02-13 14:27:55.000000 covigator-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5457 2023-02-13 14:28:03.951282 covigator-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4871 2023-02-13 14:27:55.000000 covigator-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 14:28:03.931282 covigator-2.1.0/covigator/
--rw-r--r--   0 runner    (1001) docker     (122)      468 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 14:28:03.931282 covigator-2.1.0/covigator/accessor/
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/accessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/accessor/abstract_accessor.py
--rw-r--r--   0 runner    (1001) docker     (122)    17131 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/accessor/covid19_portal_accessor.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    10084 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/accessor/ena_accessor.py
--rw-r--r--   0 runner    (1001) docker     (122)     6735 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/command_line.py
--rw-r--r--   0 runner    (1001) docker     (122)     8414 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 14:28:03.931282 covigator-2.1.0/covigator/dashboard/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 14:28:03.935282 covigator-2.1.0/covigator/dashboard/assets/
--rw-r--r--   0 runner    (1001) docker     (122)    19683 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/2021_twitter_logo_blue.png
--rw-r--r--   0 runner    (1001) docker     (122)    40495 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/CV19DP_logo_oneliner2.svg
--rw-r--r--   0 runner    (1001) docker     (122)    31369 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/CoVigator_ico.png
--rw-r--r--   0 runner    (1001) docker     (122)   106477 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/CoVigator_logo.png
--rw-r--r--   0 runner    (1001) docker     (122)  1013129 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/CoVigator_logo_ENA.png
--rw-r--r--   0 runner    (1001) docker     (122)    43957 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/CoVigator_logo_txt.png
--rw-r--r--   0 runner    (1001) docker     (122)    46264 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/CoVigator_logo_txt_nobg.png
--rw-r--r--   0 runner    (1001) docker     (122)    47880 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/CoVigator_logo_txt_reg.png
--rw-r--r--   0 runner    (1001) docker     (122)    55075 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg.png
--rw-r--r--   0 runner    (1001) docker     (122)    75513 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_covid19_portal.png
--rw-r--r--   0 runner    (1001) docker     (122)   189872 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_covid19_portal.xcf
--rw-r--r--   0 runner    (1001) docker     (122)   165548 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_ena.xcf
--rw-r--r--   0 runner    (1001) docker     (122)    49347 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/ENA_logo_2021.png
--rw-r--r--   0 runner    (1001) docker     (122)    40828 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/ENA_logo_2021_wo_text.png
--rw-r--r--   0 runner    (1001) docker     (122)    31369 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)    23354 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/favicon___.ico
--rw-r--r--   0 runner    (1001) docker     (122)      326 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/resizing_script.js
--rw-r--r--   0 runner    (1001) docker     (122)    13254 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/s1.css
--rw-r--r--   0 runner    (1001) docker     (122)     1928 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/styles.css
--rwxr-xr-x   0 runner    (1001) docker     (122)    12110 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/tron_logo.png
--rw-r--r--   0 runner    (1001) docker     (122)    14215 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/tron_logo_no_bg.png
--rwxr-xr-x   0 runner    (1001) docker     (122)    61168 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/tron_logo_without_text.png
--rw-r--r--   0 runner    (1001) docker     (122)   344224 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/assets/wordcloud.png
--rw-r--r--   0 runner    (1001) docker     (122)    17319 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 14:28:03.935282 covigator-2.1.0/covigator/dashboard/figures/
--rw-r--r--   0 runner    (1001) docker     (122)      278 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/figures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      713 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/figures/figures.py
--rw-r--r--   0 runner    (1001) docker     (122)    15948 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/figures/intrahost_mutations.py
--rw-r--r--   0 runner    (1001) docker     (122)     9891 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/figures/lineages.py
--rw-r--r--   0 runner    (1001) docker     (122)     7227 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/figures/mutation_stats.py
--rw-r--r--   0 runner    (1001) docker     (122)    42513 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/figures/recurrent_mutations.py
--rw-r--r--   0 runner    (1001) docker     (122)     4599 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/figures/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 14:28:03.939282 covigator-2.1.0/covigator/dashboard/tabs/
--rw-r--r--   0 runner    (1001) docker     (122)      551 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5499 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/tabs/acknowledgements.py
--rw-r--r--   0 runner    (1001) docker     (122)     7286 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/tabs/dataset_covid19_portal.py
--rw-r--r--   0 runner    (1001) docker     (122)    13453 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/tabs/dataset_ena.py
--rw-r--r--   0 runner    (1001) docker     (122)     3202 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/tabs/download.py
--rw-r--r--   0 runner    (1001) docker     (122)     3036 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/tabs/footer.py
--rw-r--r--   0 runner    (1001) docker     (122)    11086 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/tabs/intrahost_mutations.py
--rw-r--r--   0 runner    (1001) docker     (122)    10235 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/tabs/lineages.py
--rw-r--r--   0 runner    (1001) docker     (122)     6746 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/tabs/mutation_stats.py
--rw-r--r--   0 runner    (1001) docker     (122)     8570 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/tabs/overview.py
--rw-r--r--   0 runner    (1001) docker     (122)    14909 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/tabs/recurrent_mutations.py
--rw-r--r--   0 runner    (1001) docker     (122)     7267 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/dashboard/tabs/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 14:28:03.939282 covigator-2.1.0/covigator/database/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3841 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/database/database.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    41065 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/database/model.py
--rw-r--r--   0 runner    (1001) docker     (122)    37100 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/database/queries.py
--rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 14:28:03.939282 covigator-2.1.0/covigator/misc/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2175 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/misc/backoff_retrier.py
--rw-r--r--   0 runner    (1001) docker     (122)      249 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/misc/compression.py
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/misc/country_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 14:28:03.939282 covigator-2.1.0/covigator/pipeline/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3712 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/pipeline/covid19_portal_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (122)     2703 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/pipeline/downloader.py
--rw-r--r--   0 runner    (1001) docker     (122)     6261 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/pipeline/ena_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (122)      883 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/pipeline/runner.py
--rw-r--r--   0 runner    (1001) docker     (122)    13976 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/pipeline/vcf_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 14:28:03.939282 covigator-2.1.0/covigator/precomputations/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/precomputations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5594 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/precomputations/load_cooccurrences.py
--rw-r--r--   0 runner    (1001) docker     (122)     5636 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/precomputations/load_ns_s_counts.py
--rw-r--r--   0 runner    (1001) docker     (122)     5544 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/precomputations/load_top_occurrences.py
--rw-r--r--   0 runner    (1001) docker     (122)     3461 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/precomputations/load_variants_per_lineage.py
--rw-r--r--   0 runner    (1001) docker     (122)    17560 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/precomputations/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 14:28:03.939282 covigator-2.1.0/covigator/processor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10544 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/processor/abstract_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)     3081 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/processor/covid19portal_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/processor/ena_downloader.py
--rw-r--r--   0 runner    (1001) docker     (122)     5762 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/processor/ena_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 14:28:03.943282 covigator-2.1.0/covigator/references/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/references/conservation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2965 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/references/domains_NS_S.csv
--rw-r--r--   0 runner    (1001) docker     (122)     3699 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/references/gene_annotations.py
--rw-r--r--   0 runner    (1001) docker     (122)      577 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/references/genes_NS_S.csv
--rw-r--r--   0 runner    (1001) docker     (122)   601324 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/references/sars_cov_2.json
--rw-r--r--   0 runner    (1001) docker     (122)   934358 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/references/wuhCor1.mutDepletionConsHMM.bed
--rw-r--r--   0 runner    (1001) docker     (122)   932961 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/references/wuhCor1.mutDepletionSarbecovirusConsHMM.bed
--rw-r--r--   0 runner    (1001) docker     (122)   931439 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/references/wuhCor1.mutDepletionVertebrateCoVConsHMM.bed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 14:28:03.943282 covigator-2.1.0/covigator/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 14:28:03.943282 covigator-2.1.0/covigator/tests/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/integration_tests/integration_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/integration_tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (122)      281 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/integration_tests/test_gene_annotations.py
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/integration_tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (122)      773 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/integration_tests/test_vcf_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 14:28:03.947282 covigator-2.1.0/covigator/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (122)    30427 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/MN908947.3.fa
--rw-r--r--   0 runner    (1001) docker     (122)    18016 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/Sars_cov_2.ASM985889v3.pep.all.fa
--rw-r--r--   0 runner    (1001) docker     (122)  1231182 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/Sars_cov_2.all_variants.snpeff.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/Sars_cov_2.all_variants.snpeff.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (122)     4422 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/domains_NS_S.csv
--rw-r--r--   0 runner    (1001) docker     (122)      577 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/genes_NS_S.csv
--rw-r--r--   0 runner    (1001) docker     (122)    13972 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/gisaid_allprot0526.fasta
--rw-r--r--   0 runner    (1001) docker     (122)    27733 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/gisaid_allprot1208.fasta
--rw-r--r--   0 runner    (1001) docker     (122)    27784 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/gisaid_allprot1208.with_mutations.fasta
--rw-r--r--   0 runner    (1001) docker     (122)   601324 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/sars_cov_2.json
--rw-r--r--   0 runner    (1001) docker     (122)      765 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/sars_cov_2_dn_ds.json
--rw-r--r--   0 runner    (1001) docker     (122)     7041 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/snpeff.vcf
--rw-r--r--   0 runner    (1001) docker     (122)     4041 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/snpeff_with_deletion.vcf
--rw-r--r--   0 runner    (1001) docker     (122)     4041 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/snpeff_with_insertion.vcf
--rw-r--r--   0 runner    (1001) docker     (122)     3877 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/snpeff_without_annotation.vcf
--rw-r--r--   0 runner    (1001) docker     (122)     4023 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/snpeff_without_dp4.vcf
--rw-r--r--   0 runner    (1001) docker     (122)      910 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/test.another_pangolin.csv
--rw-r--r--   0 runner    (1001) docker     (122)     2148 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/test.assembly.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/test.assembly.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/test.coverage.tsv
--rw-r--r--   0 runner    (1001) docker     (122)     3483 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/test.deduplication_metrics.txt
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/test.lofreq.pangolin.csv
--rw-r--r--   0 runner    (1001) docker     (122)      398 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/test.lofreq.pangolin.with_none.csv
--rw-r--r--   0 runner    (1001) docker     (122)     3357 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/test.lofreq.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (122)      126 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/test.lofreq.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (122)    30247 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/resources/test_data.fasta
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 14:28:03.951282 covigator-2.1.0/covigator/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/unit_tests/abstract_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     3928 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/unit_tests/faked_objects.py
--rw-r--r--   0 runner    (1001) docker     (122)     9533 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/unit_tests/mocked.py
--rw-r--r--   0 runner    (1001) docker     (122)      413 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/unit_tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/unit_tests/test_country_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     3321 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/unit_tests/test_database_initialisation.py
--rw-r--r--   0 runner    (1001) docker     (122)     3117 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/unit_tests/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (122)    27682 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/unit_tests/test_ena_accessor.py
--rw-r--r--   0 runner    (1001) docker     (122)     7491 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/unit_tests/test_figures.py
--rw-r--r--   0 runner    (1001) docker     (122)    10466 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/unit_tests/test_precomputer.py
--rw-r--r--   0 runner    (1001) docker     (122)     8107 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/unit_tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)    11852 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/unit_tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (122)    13056 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/tests/unit_tests/test_vcf_loader.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-02-13 14:27:55.000000 covigator-2.1.0/covigator/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-13 14:28:03.931282 covigator-2.1.0/covigator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5457 2023-02-13 14:28:03.000000 covigator-2.1.0/covigator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6170 2023-02-13 14:28:03.000000 covigator-2.1.0/covigator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-13 14:28:03.000000 covigator-2.1.0/covigator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      524 2023-02-13 14:28:03.000000 covigator-2.1.0/covigator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      466 2023-02-13 14:28:03.000000 covigator-2.1.0/covigator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-02-13 14:28:03.000000 covigator-2.1.0/covigator.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (122)       79 2023-02-13 14:28:03.951282 covigator-2.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1862 2023-02-13 14:27:55.000000 covigator-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.661650 covigator-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1066 2023-07-06 08:20:19.000000 covigator-2.2.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (122)      338 2023-07-06 08:20:19.000000 covigator-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6059 2023-07-06 08:20:31.661650 covigator-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5473 2023-07-06 08:20:19.000000 covigator-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.641650 covigator-2.2.0/covigator/
+-rw-r--r--   0 runner    (1001) docker     (122)     1440 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.641650 covigator-2.2.0/covigator/accessor/
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/accessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1803 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/accessor/abstract_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17131 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/accessor/covid19_portal_accessor.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10084 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/accessor/ena_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6726 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8414 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.641650 covigator-2.2.0/covigator/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.645650 covigator-2.2.0/covigator/dashboard/assets/
+-rw-r--r--   0 runner    (1001) docker     (122)    19683 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/2021_twitter_logo_blue.png
+-rw-r--r--   0 runner    (1001) docker     (122)    40495 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CV19DP_logo_oneliner2.svg
+-rw-r--r--   0 runner    (1001) docker     (122)    31369 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CoVigator_ico.png
+-rw-r--r--   0 runner    (1001) docker     (122)   106477 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)  1013129 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_ENA.png
+-rw-r--r--   0 runner    (1001) docker     (122)    43957 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt.png
+-rw-r--r--   0 runner    (1001) docker     (122)    46264 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_nobg.png
+-rw-r--r--   0 runner    (1001) docker     (122)    47880 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_reg.png
+-rw-r--r--   0 runner    (1001) docker     (122)    55075 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg.png
+-rw-r--r--   0 runner    (1001) docker     (122)    75513 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_covid19_portal.png
+-rw-r--r--   0 runner    (1001) docker     (122)   189872 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_covid19_portal.xcf
+-rw-r--r--   0 runner    (1001) docker     (122)   165548 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_ena.xcf
+-rw-r--r--   0 runner    (1001) docker     (122)    49347 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/ENA_logo_2021.png
+-rw-r--r--   0 runner    (1001) docker     (122)    40828 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/ENA_logo_2021_wo_text.png
+-rw-r--r--   0 runner    (1001) docker     (122)    31369 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)    23354 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/favicon___.ico
+-rw-r--r--   0 runner    (1001) docker     (122)      326 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/resizing_script.js
+-rw-r--r--   0 runner    (1001) docker     (122)    13254 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/s1.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1928 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/styles.css
+-rwxr-xr-x   0 runner    (1001) docker     (122)    12110 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/tron_logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)    14215 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/tron_logo_no_bg.png
+-rwxr-xr-x   0 runner    (1001) docker     (122)    61168 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/tron_logo_without_text.png
+-rw-r--r--   0 runner    (1001) docker     (122)   344224 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/assets/wordcloud.png
+-rw-r--r--   0 runner    (1001) docker     (122)    17319 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.645650 covigator-2.2.0/covigator/dashboard/figures/
+-rw-r--r--   0 runner    (1001) docker     (122)      278 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/figures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/figures/figures.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16413 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/figures/intrahost_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10781 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/figures/lineages.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7227 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/figures/mutation_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42807 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/figures/recurrent_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4599 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/figures/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.649650 covigator-2.2.0/covigator/dashboard/tabs/
+-rw-r--r--   0 runner    (1001) docker     (122)      551 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6156 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/acknowledgements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7286 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/dataset_covid19_portal.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13437 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/dataset_ena.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3202 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/download.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3036 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/footer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11070 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/intrahost_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10590 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/lineages.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6746 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/mutation_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8570 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/overview.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15016 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/recurrent_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7496 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/dashboard/tabs/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.649650 covigator-2.2.0/covigator/database/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4035 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/database/database.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    44182 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/database/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42544 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/database/queries.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1738 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.649650 covigator-2.2.0/covigator/misc/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2175 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/misc/backoff_retrier.py
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/misc/compression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/misc/country_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.649650 covigator-2.2.0/covigator/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3712 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/pipeline/covid19_portal_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2703 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/pipeline/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6261 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/pipeline/ena_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)      883 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/pipeline/runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13976 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/pipeline/vcf_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.649650 covigator-2.2.0/covigator/precomputations/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/precomputations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5594 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/precomputations/load_cooccurrences.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5632 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/precomputations/load_ns_s_counts.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5544 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/precomputations/load_top_occurrences.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3453 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/precomputations/load_variants_per_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17548 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/precomputations/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.649650 covigator-2.2.0/covigator/processor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10544 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/processor/abstract_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3081 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/processor/covid19portal_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/processor/ena_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5762 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/processor/ena_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.653650 covigator-2.2.0/covigator/references/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2503 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/references/conservation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2965 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/references/domains_NS_S.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     3699 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/references/gene_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      577 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/references/genes_NS_S.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    37762 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/references/lineage_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (122)   601324 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/references/sars_cov_2.json
+-rw-r--r--   0 runner    (1001) docker     (122)   934358 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/references/wuhCor1.mutDepletionConsHMM.bed
+-rw-r--r--   0 runner    (1001) docker     (122)   932961 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/references/wuhCor1.mutDepletionSarbecovirusConsHMM.bed
+-rw-r--r--   0 runner    (1001) docker     (122)   931439 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/references/wuhCor1.mutDepletionVertebrateCoVConsHMM.bed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.653650 covigator-2.2.0/covigator/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.657650 covigator-2.2.0/covigator/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1330 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/integration_tests/integration_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/integration_tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/integration_tests/test_gene_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (122)      827 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/integration_tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/integration_tests/test_vcf_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.661650 covigator-2.2.0/covigator/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)    30427 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/MN908947.3.fa
+-rw-r--r--   0 runner    (1001) docker     (122)    18016 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/Sars_cov_2.ASM985889v3.pep.all.fa
+-rw-r--r--   0 runner    (1001) docker     (122)  1231182 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/Sars_cov_2.all_variants.snpeff.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/Sars_cov_2.all_variants.snpeff.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (122)     4422 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/domains_NS_S.csv
+-rw-r--r--   0 runner    (1001) docker     (122)      577 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/genes_NS_S.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    13972 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/gisaid_allprot0526.fasta
+-rw-r--r--   0 runner    (1001) docker     (122)    27733 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/gisaid_allprot1208.fasta
+-rw-r--r--   0 runner    (1001) docker     (122)    27784 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/gisaid_allprot1208.with_mutations.fasta
+-rw-r--r--   0 runner    (1001) docker     (122)   601324 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/sars_cov_2.json
+-rw-r--r--   0 runner    (1001) docker     (122)      765 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/sars_cov_2_dn_ds.json
+-rw-r--r--   0 runner    (1001) docker     (122)     7041 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/snpeff.vcf
+-rw-r--r--   0 runner    (1001) docker     (122)     4041 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/snpeff_with_deletion.vcf
+-rw-r--r--   0 runner    (1001) docker     (122)     4041 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/snpeff_with_insertion.vcf
+-rw-r--r--   0 runner    (1001) docker     (122)     3877 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/snpeff_without_annotation.vcf
+-rw-r--r--   0 runner    (1001) docker     (122)     4023 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/snpeff_without_dp4.vcf
+-rw-r--r--   0 runner    (1001) docker     (122)      910 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/test.another_pangolin.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     2148 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/test.assembly.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/test.assembly.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/test.coverage.tsv
+-rw-r--r--   0 runner    (1001) docker     (122)     3483 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/test.deduplication_metrics.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/test.lofreq.pangolin.csv
+-rw-r--r--   0 runner    (1001) docker     (122)      398 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/test.lofreq.pangolin.with_none.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     3357 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/test.lofreq.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/test.lofreq.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (122)    30247 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/resources/test_data.fasta
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.661650 covigator-2.2.0/covigator/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3419 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/abstract_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3928 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/faked_objects.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9533 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/mocked.py
+-rw-r--r--   0 runner    (1001) docker     (122)      413 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1308 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_country_parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8228 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_database_initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3117 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27682 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_ena_accessor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7491 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_figures.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10320 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_lineage_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10466 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_precomputer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8107 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14924 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13056 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/tests/unit_tests/test_vcf_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-06 08:20:19.000000 covigator-2.2.0/covigator/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 08:20:31.641650 covigator-2.2.0/covigator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6059 2023-07-06 08:20:31.000000 covigator-2.2.0/covigator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6267 2023-07-06 08:20:31.000000 covigator-2.2.0/covigator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 08:20:31.000000 covigator-2.2.0/covigator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      524 2023-07-06 08:20:31.000000 covigator-2.2.0/covigator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      480 2023-07-06 08:20:31.000000 covigator-2.2.0/covigator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-06 08:20:31.000000 covigator-2.2.0/covigator.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)       79 2023-07-06 08:20:31.661650 covigator-2.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1862 2023-07-06 08:20:19.000000 covigator-2.2.0/setup.py
```

### Comparing `covigator-2.1.0/LICENSE` & `covigator-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/PKG-INFO` & `covigator-2.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covigator
-Version: 2.1.0
+Version: 2.2.0
 Home-page: 
 Author: TRON - Translational Oncology at the University Medical Center of the Johannes Gutenberg University Mainz - Computational Medicine group
 Author-email: patrick.sorn@tron-mainz.de
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
@@ -69,23 +69,30 @@
 mutations. Importantly, we only process the Illumina samples from ENA. 
 This means excluding all of the Oxford Nanopore samples and hence having a partial view of all the available data.
 
 The dashboard is implemented in the visualization framework [Dash](https://dash.plotly.com/). 
 The computation is distributed through our cluster with a library of similar name [Dask](https://dask.org/).
 The analysis pipeline is implemented in the [Nextflow](https://www.nextflow.io/) framework.
 
-![CoVigator system](docs/source/_static/figures/system_design.drawio.png)
+![CoVigator system](docs/source/_static/figures/system_design_manuscript.png)
 
 <p align = "center">
 <b>Figure 3: System design</b>
 </p>
 
 The CoVigator project was developed at the Biomarker Development Center at 
 [TRON (Translational Oncology at the University Medical Center of the Johannes Gutenberg University gGmbH)](https://tron-mainz.de/). 
 The project was kindly supported by 
 [Intel´s Pandemic Response Technology Initiative](https://newsroom.intel.com/tag/pandemic-response-technology-initiative).
 
 ## How to cite
 
-* Schrörs, B., Riesgo-Ferreiro, P., Sorn, P., Gudimella, R., Bukur, T., Rösler, T., Löwer, M., & Sahin, U. (2021). 
+*   Bukur T., Riesgo-Ferreiro P., Sorn P, Gudimella R., Hausmann J., Rösler T., Löwer M., Schrörs B., & Sahin U. 
+CoVigator — A Knowledge Base for Navigating SARS-CoV-2 Genomic Variants. Viruses. 2023; 15(6):1391. [10.3390/v15061391](https://doi.org/10.3390/v15061391)
+
+*   Schrörs, B., Riesgo-Ferreiro, P., Sorn, P., Gudimella, R., Bukur, T., Rösler, T., Löwer, M., & Sahin, U. (2021). 
 Large-scale analysis of SARS-CoV-2 spike-glycoprotein mutants demonstrates the need for continuous screening of virus 
 isolates. PLOS ONE, 16(9), e0249254. [10.1371/journal.pone.0249254](https://doi.org/10.1371/journal.pone.0249254)
+
+### Acknowledgements
+
+The lineage annotation in the covigator dashboard package uses "the description of constellations of mutations for the SARS-CoV-2 virus" by [cov-lineages](https://github.com/cov-lineages/constellations) provided and licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)
```

### Comparing `covigator-2.1.0/README.md` & `covigator-2.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -55,23 +55,30 @@
 mutations. Importantly, we only process the Illumina samples from ENA. 
 This means excluding all of the Oxford Nanopore samples and hence having a partial view of all the available data.
 
 The dashboard is implemented in the visualization framework [Dash](https://dash.plotly.com/). 
 The computation is distributed through our cluster with a library of similar name [Dask](https://dask.org/).
 The analysis pipeline is implemented in the [Nextflow](https://www.nextflow.io/) framework.
 
-![CoVigator system](docs/source/_static/figures/system_design.drawio.png)
+![CoVigator system](docs/source/_static/figures/system_design_manuscript.png)
 
 <p align = "center">
 <b>Figure 3: System design</b>
 </p>
 
 The CoVigator project was developed at the Biomarker Development Center at 
 [TRON (Translational Oncology at the University Medical Center of the Johannes Gutenberg University gGmbH)](https://tron-mainz.de/). 
 The project was kindly supported by 
 [Intel´s Pandemic Response Technology Initiative](https://newsroom.intel.com/tag/pandemic-response-technology-initiative).
 
 ## How to cite
 
-* Schrörs, B., Riesgo-Ferreiro, P., Sorn, P., Gudimella, R., Bukur, T., Rösler, T., Löwer, M., & Sahin, U. (2021). 
+*   Bukur T., Riesgo-Ferreiro P., Sorn P, Gudimella R., Hausmann J., Rösler T., Löwer M., Schrörs B., & Sahin U. 
+CoVigator — A Knowledge Base for Navigating SARS-CoV-2 Genomic Variants. Viruses. 2023; 15(6):1391. [10.3390/v15061391](https://doi.org/10.3390/v15061391)
+
+*   Schrörs, B., Riesgo-Ferreiro, P., Sorn, P., Gudimella, R., Bukur, T., Rösler, T., Löwer, M., & Sahin, U. (2021). 
 Large-scale analysis of SARS-CoV-2 spike-glycoprotein mutants demonstrates the need for continuous screening of virus 
 isolates. PLOS ONE, 16(9), e0249254. [10.1371/journal.pone.0249254](https://doi.org/10.1371/journal.pone.0249254)
+
+### Acknowledgements
+
+The lineage annotation in the covigator dashboard package uses "the description of constellations of mutations for the SARS-CoV-2 virus" by [cov-lineages](https://github.com/cov-lineages/constellations) provided and licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)
```

### Comparing `covigator-2.1.0/covigator/accessor/abstract_accessor.py` & `covigator-2.2.0/covigator/accessor/abstract_accessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,12 @@
         sample.country_raw = sample.country
         sample.country = parsed_country.country
         sample.country_alpha_2 = parsed_country.country_alpha_2
         sample.country_alpha_3 = parsed_country.country_alpha_3
         sample.continent_alpha_2 = parsed_country.continent_alpha_2
         sample.continent = parsed_country.continent
 
-
-    @staticmethod
-    def _parse_dates(sample: Union[SampleEna, SampleCovid19]):
+    def _parse_dates(self, sample: Union[SampleEna, SampleCovid19]):
         sample.collection_date = _parse_abstract(sample.collection_date, date.fromisoformat)
         sample.first_created = _parse_abstract(sample.first_created, date.fromisoformat)
         if sample.collection_date is not None and sample.collection_date < MINIMUM_DATE:
             raise CovigatorExcludedSampleTooEarlyDateException
```

### Comparing `covigator-2.1.0/covigator/accessor/covid19_portal_accessor.py` & `covigator-2.2.0/covigator/accessor/covid19_portal_accessor.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/accessor/ena_accessor.py` & `covigator-2.2.0/covigator/accessor/ena_accessor.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/command_line.py` & `covigator-2.2.0/covigator/command_line.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
                 walltime='72:00:00',  # hard codes maximum time to 72 hours
                 scheduler_options={"dashboard_address": ':{}'.format(config.dask_port)}) as cluster:
             cluster.scale(jobs=int(args.num_jobs))
             _start_dask_processor(args, config, cluster=cluster)
 
 
 def ena_downloader():
-    parser = ArgumentParser(
+    ArgumentParser(
         description="Covigator {} ENA downloader".format(covigator.VERSION))
 
     config = Configuration(verbose=True)
     covigator.configuration.initialise_logs(config.logfile_accesor)
     EnaDownloader(database=Database(config=config, initialize=True), config=config).process()
```

### Comparing `covigator-2.1.0/covigator/configuration.py` & `covigator-2.2.0/covigator/configuration.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/2021_twitter_logo_blue.png` & `covigator-2.2.0/covigator/dashboard/assets/2021_twitter_logo_blue.png`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/CV19DP_logo_oneliner2.svg` & `covigator-2.2.0/covigator/dashboard/assets/CV19DP_logo_oneliner2.svg`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/CoVigator_ico.png` & `covigator-2.2.0/covigator/dashboard/assets/CoVigator_ico.png`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/CoVigator_logo.png` & `covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo.png`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/CoVigator_logo_ENA.png` & `covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_ENA.png`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/CoVigator_logo_txt.png` & `covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt.png`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/CoVigator_logo_txt_nobg.png` & `covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_nobg.png`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/CoVigator_logo_txt_reg.png` & `covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_reg.png`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg.png` & `covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg.png`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_covid19_portal.png` & `covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_covid19_portal.png`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_covid19_portal.xcf` & `covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_covid19_portal.xcf`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_ena.xcf` & `covigator-2.2.0/covigator/dashboard/assets/CoVigator_logo_txt_reg_no_bg_ena.xcf`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/ENA_logo_2021.png` & `covigator-2.2.0/covigator/dashboard/assets/ENA_logo_2021.png`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/ENA_logo_2021_wo_text.png` & `covigator-2.2.0/covigator/dashboard/assets/ENA_logo_2021_wo_text.png`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/favicon.ico` & `covigator-2.2.0/covigator/dashboard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/favicon___.ico` & `covigator-2.2.0/covigator/dashboard/assets/favicon___.ico`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/s1.css` & `covigator-2.2.0/covigator/dashboard/assets/s1.css`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/styles.css` & `covigator-2.2.0/covigator/dashboard/assets/styles.css`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/tron_logo.png` & `covigator-2.2.0/covigator/dashboard/assets/tron_logo.png`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/tron_logo_no_bg.png` & `covigator-2.2.0/covigator/dashboard/assets/tron_logo_no_bg.png`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/tron_logo_without_text.png` & `covigator-2.2.0/covigator/dashboard/assets/tron_logo_without_text.png`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/assets/wordcloud.png` & `covigator-2.2.0/covigator/dashboard/assets/wordcloud.png`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/dashboard.py` & `covigator-2.2.0/covigator/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/figures/figures.py` & `covigator-2.2.0/covigator/dashboard/figures/figures.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,15 +16,16 @@
             }]
 STYLE_HEADER = {
     'backgroundColor': 'white',
     'fontWeight': 'bold'
 }
 STYLE_CELL = {
     'padding': '5px',
-    'maxWidth': '100px'
+    'maxWidth': '100px',
+    'whiteSpace': 'normal'
 }
 
 
 class Figures:
 
     def __init__(self, queries: Queries):
         self.queries = queries
```

### Comparing `covigator-2.1.0/covigator/dashboard/figures/intrahost_mutations.py` & `covigator-2.2.0/covigator/dashboard/figures/intrahost_mutations.py`

 * *Files 8% similar despite different names*

```diff
@@ -176,14 +176,15 @@
             unique_subclonal_variants = data.groupby('variant_id').agg({
                 'gene_name': 'first',
                 'pfam_description': 'first',
                 'hgvs_p': 'first',
                 'annotation_highest_impact': 'first',
                 'cons_hmm_sars_cov_2': 'first',
             })
+
             # this fills empty conservation values
             unique_subclonal_variants["cons_hmm_sars_cov_2"].fillna(0.0, inplace=True)
             unique_subclonal_variants["cons_hmm_sars_cov_2"] = unique_subclonal_variants["cons_hmm_sars_cov_2"].transform(lambda x: round(x, 3))
             unique_subclonal_variants["median_vaf"] = data[["variant_id", "vaf"]]\
                 .groupby('variant_id')["vaf"].agg(lambda x: round(float(np.median(x)), 3))
             unique_subclonal_variants["iqr_vaf"] = data[["variant_id", "vaf"]]\
                 .groupby('variant_id')["vaf"].agg(lambda x: round(np.percentile(x, 0.75) - np.percentile(x, 0.25),  3))
@@ -194,14 +195,17 @@
             unique_subclonal_variants["count_observations"] = data[["variant_id", "date"]] \
                 .groupby('variant_id')["date"].agg('count')
             unique_subclonal_variants["score"] = unique_subclonal_variants[["count_observations", "cons_hmm_sars_cov_2"]]\
                 .apply(lambda x: round(np.log(x[0]) * x[1], 3), axis=1)
 
             unique_subclonal_variants.reset_index(inplace=True)
 
+            # Merge with llineage defining mutations
+            unique_subclonal_variants = self.queries._merge_with_lineage_defining_variants(unique_subclonal_variants)
+
             if order_by == "score":
                 ordered_data = unique_subclonal_variants.sort_values("score", ascending=True)
             elif order_by == "count":
                 ordered_data = unique_subclonal_variants.sort_values("count_observations", ascending=False)
             elif order_by == "conservation":
                 ordered_data = unique_subclonal_variants.sort_values("cons_hmm_sars_cov_2", ascending=True)
             elif order_by == "vaf":
@@ -213,15 +217,15 @@
                 id='top-occurring-subclonal-variants-table',
                 data=ordered_data.to_dict('records'),
                 columns=[
                             {"name": ["Gene"], "id": "gene_name"},
                             {"name": ["Pfam Domain"], "id": "pfam_description"},
                             {"name": ["DNA mutation"], "id": "variant_id"},
                             {"name": ["Protein mutation"], "id": "hgvs_p"},
-                            {"name": ["Effect"], "id": "annotation_highest_impact"},
+                            {"name": ["Pangolin lineage"], "id": "pangolin_hover"},
                             {"name": ["First observation"], "id": "first_observation"},
                             {"name": ["Last observation"], "id": "last_observation"},
                             {"name": ["Count"], "id": "count_observations"},
                             {"name": ["ConsHMM"], "id": "cons_hmm_sars_cov_2"},
                             {"name": ["Median VAF"], "id": "median_vaf"},
                             {"name": ["IQR VAF"], "id": "iqr_vaf"},
                             {"name": ["Score"], "id": "score"},
@@ -231,14 +235,20 @@
                 style_header=STYLE_HEADER,
                 row_selectable='single',
                 css=[{'selector': '.dash-cell div.dash-cell-value',
                       'rule': 'display: inline; white-space: inherit; overflow: inherit; text-overflow: inherit;'}],
                 style_table={'overflowX': 'auto'},
                 style_data={'whiteSpace': 'normal', 'height': 'auto'},
                 style_cell={'maxWidth': '100px'},
+                tooltip_data=[
+                        {
+                            'pangolin_hover': {'value': row['pangolin_lineage'], 'type': 'markdown'}
+                        } for row in ordered_data.to_dict('records')
+                    ],
+                    tooltip_duration=None,
             )
 
         return [
             fig,
             html.Br(),
             html.Div(children=[
                 html.Button("Download CSV", id="btn_csv3"),
```

### Comparing `covigator-2.1.0/covigator/dashboard/figures/lineages.py` & `covigator-2.2.0/covigator/dashboard/figures/lineages.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,18 +53,27 @@
     return styles
 
 
 class LineageFigures(Figures):
 
     def get_lineages_plot(self, data_source: str, date_start, date_end, countries=None, lineages=None, time_period=14, prevalence=0):
         logger.debug("Getting data on samples by country...")
+        who_label = self.queries.get_lineages_who_label()
         data = self.queries.get_accumulated_lineages_by_country(
             data_source=data_source, countries=countries, lineages=lineages)
         graph = dcc.Markdown("""**No data for the current selection**""")
         if data is not None and data.shape[0] > 0:
+            # Generate a dictionary mapping pangolin lineage ids in the dataframe to the WHO labels in the database
+            # Use combo label of pangolin ids + WHO labels separated by a hyphen in the legend of the lineages plot
+            label_names = data.merge(who_label, how="left", left_on="lineage", right_on="pangolin_lineage")[["lineage","who_label"]]
+            label_names["label_value"] = label_names.apply(lambda x: f"{x.lineage} - {x.who_label}"
+                if not pd.isnull(x.who_label) else f"{x.lineage}", axis=1)
+            label_names = label_names.set_index("lineage").to_dict()["label_value"]
+            # Append others to label dict in case of prevalence grouping
+            label_names["others"] = "others"
             # Filter data based on start and end range
             data = data.loc[(data.date >= date_start) & (data.date <= date_end)]
             logger.debug("Prepare plot on samples by lineage...")
             lineages = list(data.sort_values("cumsum", ascending=False).lineage.unique())
             if prevalence > 0:
                 # Calculate cumulative sum for each lineage in selected time interval
                 cumsum_for_range = data.groupby('lineage')[['count_y']].sum()
@@ -131,20 +140,21 @@
                     'range': [0, 1],
                     'title': '% samples'
                 },
                 height=700,
                 hovermode="x unified"
             )
             fig.update_xaxes(showspikes=True)
+            fig.for_each_trace(lambda x: x.update(name=label_names[x.name]))
 
             top_lineages = lineages[0: min(5, len(lineages))]
             top_lineages_and_cumsum = data[data.lineage.isin(top_lineages)][["lineage", "cumsum"]] \
                 .groupby("lineage").max().reset_index().sort_values("cumsum", ascending=False)
             top_lineages_tooltip = list(
-                top_lineages_and_cumsum.apply(lambda x: "{} ({})".format(x[0], int(x[1])), axis=1))
+                top_lineages_and_cumsum.apply(lambda x: "{} ({})".format(label_names[x[0]], int(x[1])), axis=1))
 
             graph = [
                 dcc.Graph(figure=fig, config=PLOTLY_CONFIG),
                 dcc.Markdown("""
                 **Samples by lineages**
                 
                 Top {} lineages: {}.
```

### Comparing `covigator-2.1.0/covigator/dashboard/figures/mutation_stats.py` & `covigator-2.2.0/covigator/dashboard/figures/mutation_stats.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/figures/recurrent_mutations.py` & `covigator-2.2.0/covigator/dashboard/figures/recurrent_mutations.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,25 +271,31 @@
                     id="top-occurring-variants-table",
                     data=data.to_dict('records'),
                     sort_action='native',
                     columns=[
                                 {"name": ["Variant", "Gene"], "id": "gene_name"},
                                 {"name": ["", "DNA mutation"], "id": "dna_mutation"},
                                 {"name": ["", "Protein mutation"], "id": "hgvs_p"},
-                                {"name": ["", "Effect"], "id": "annotation"},
+                                {"name": ["", "Pangolin lineage"], "id": "pangolin_hover"},
                                 {"name": ["", "Frequency"], "id": "frequency"},
                                 {"name": ["", "Count"], "id": "total"},
                             ] + month_columns,
                     style_data_conditional=STYLES_STRIPPED + styles_counts + styles_frequency + styles_total_count,
                     style_table={'overflowX': 'auto'},
                     style_as_list_view=True,
                     style_header=STYLE_HEADER,
                     style_cell=STYLE_CELL,
                     sort_by=[{"column_id": "frequency", "direction": "desc"}],
-                    row_selectable='multi'
+                    row_selectable='multi',
+                    tooltip_data=[
+                        {
+                            'pangolin_hover': {'value': row['pangolin_lineage'], 'type': 'markdown'}
+                        } for row in data.to_dict('records')
+                    ],
+                    tooltip_duration=None
                 ),
                 html.Br(),
                 html.Div(children=[
                     html.Button("Download CSV", id="btn_csv2"),
                     dcc.Download(id="download-dataframe-csv2"),
                     dcc.Store(id="memory2", data=data.to_dict('records'))]),
                 html.Br(),
@@ -555,15 +561,15 @@
                            ))]
 
     def get_variants_plot(self, gene_name, domain_name, selected_variants, bin_size, source):
 
         # reads gene annotations
         logger.debug("Getting genes and domains...")
         assert gene_name is not None or domain_name is not None, "Either gene or domain need to be provided"
-        
+
         if domain_name is None:
             gene = self.queries.get_gene(gene_name)
             domains = self.queries.get_domains_by_gene(gene_name)
             start = gene.start
             end = gene.end
         else:
             domain = self.queries.get_domain(domain_name=domain_name)
@@ -768,15 +774,15 @@
                     sort_by=[{"column_id": "variant_id", "direction": "asc"}],
                 ))
                 tables.append(html.Br())
             tables.append(html.Div(children=[
                 html.Button("Download CSV", id="btn_csv"),
                 dcc.Download(id="download-dataframe-csv"),
                 dcc.Store(id="memory", data=data.to_dict('records'))]))
-            tables.append(html.Br()),
+            tables.append(html.Br())
             tables.append(dcc.Markdown("""
             ***Co-occurrence clustering*** *shows the resulting clusters from the
             co-occurrence matrix with the Jaccard index corrected with the Cohen's kappa coefficient. 
             The co-occurrence matrix is built taking into account only mutations with at least {} pairwise 
             co-occurrences and if a gene is provided only mutations within that gene.  
             Clustering is performed on the co-occurrence matrix using OPTICS. 
             The mimimum number of neighbours to call
```

### Comparing `covigator-2.1.0/covigator/dashboard/figures/samples.py` & `covigator-2.2.0/covigator/dashboard/figures/samples.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/tabs/__init__.py` & `covigator-2.2.0/covigator/dashboard/tabs/__init__.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/tabs/acknowledgements.py` & `covigator-2.2.0/covigator/dashboard/tabs/acknowledgements.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,25 @@
                 **The CoVigator project** was developed at the Biomarker Development Center at TRON (Translational 
                 Oncology at the University Medical Center of the Johannes Gutenberg University) gGmbH. 
                 The project was kindly supported by Intel´s Pandemic Response Technology Initiative.
                 """),
                 html.Br(),
                 html.P("If you want to cite us:"),
                 html.P([
+                    "Bukur, T., Riesgo-Ferreiro, P., Sorn, P., Gudimella, R., Hausmann, J., Rösler, T., "
+                    "Löwer, M., Schrörs, B., & Sahin, U. CoVigator — A Knowledge Base for Navigating SARS-CoV-2 Genomic Variants. "
+                    "Viruses. 2023; 15(6):1391.",
+                ],
+                    style={"font-style": "italic", "margin-left": "50px"}),
+                html.P(
+                    html.A("https://doi.org/10.3390/v15061391",
+                           href="https://doi.org/10.3390/v15061391", target="_blank"),
+                    style={"text-indent": "50px"}
+                ),
+                html.P([
                     "Schrörs, B., Riesgo-Ferreiro, P., Sorn, P., Gudimella, R., Bukur, T., Rösler, T., "
                     "Löwer, M., & Sahin, U. (2021). Large-scale analysis of SARS-CoV-2 spike-glycoprotein mutants "
                     "demonstrates the need for continuous screening of virus isolates. PLOS ONE, 16(9), e0249254.",
                 ],
                     style={"font-style": "italic", "margin-left": "50px"}),
                 html.P(
                     html.A("https://doi.org/10.1371/journal.pone.0249254",
```

### Comparing `covigator-2.1.0/covigator/dashboard/tabs/dataset_covid19_portal.py` & `covigator-2.2.0/covigator/dashboard/tabs/dataset_covid19_portal.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/tabs/dataset_ena.py` & `covigator-2.2.0/covigator/dashboard/tabs/dataset_ena.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     date_of_most_recent_sample = queries.get_date_of_most_recent_sample(source=DataSource.ENA)
 
     return html.Div(
         className="two columns",
         children=[
             html.Div([
                 html.Div(dbc.Button(
-                    "Distribution of samples by library strategy",
+                    "Samples by library strategy",
                     color="secondary",
                     className="me-1",
                     style={'font-size': '100%'}
                 )),
                 html.Br(),
                 html.Div(dbc.Button(
                     "Read trimming",
```

### Comparing `covigator-2.1.0/covigator/dashboard/tabs/download.py` & `covigator-2.2.0/covigator/dashboard/tabs/download.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/tabs/footer.py` & `covigator-2.2.0/covigator/dashboard/tabs/footer.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/tabs/intrahost_mutations.py` & `covigator-2.2.0/covigator/dashboard/tabs/intrahost_mutations.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 "Top intrahost mutations",
                 color="secondary",
                 className="me-1",
                 style={'font-size': '100%'}
             )),
             html.Br(),
             html.Div(dbc.Button(
-                "Distribution of selected intrahost mutation",
+                "Selected intrahost mutation",
                 color="secondary",
                 className="me-1",
                 style={'font-size': '100%'})),
             html.Br(),
             html.Div(dbc.Button(
                 "Co-occurrent clonal mutations",
                 color="secondary",
```

### Comparing `covigator-2.1.0/covigator/dashboard/tabs/lineages.py` & `covigator-2.2.0/covigator/dashboard/tabs/lineages.py`

 * *Files 15% similar despite different names*

```diff
@@ -45,21 +45,23 @@
             html.Br(),
             html.Div(id=ID_LINEAGES_TABLE),
         ])
 
 
 def get_lineages_tab_left_bar(queries: Queries, data_source: DataSource):
 
-    lineages = queries.get_lineages(source=data_source.name)
     # Get all available months from collection_date column in sample table
+    lineages = queries.get_combined_labels(data_source.name)
     months = queries.get_sample_months(MONTH_PATTERN, data_source=data_source.name)
-    today = datetime.now()
-    today_formatted = today.strftime(MONTH_PATTERN)
-    oneyearago = today - timedelta(days=356)
-    oneyearago_formatted = oneyearago.strftime(MONTH_PATTERN)
+
+    last_update = queries.get_last_update(data_source.name)
+    last_update_formatted = last_update.strftime(MONTH_PATTERN)
+
+    one_year_before_update = last_update - timedelta(days=365)
+    one_year_before_update_formatted = one_year_before_update.strftime(MONTH_PATTERN)
 
     return html.Div(
         className="two columns",
         children=[
             html.Div([
                 html.Div(dbc.Button(
                     "Lineages accumulation",
@@ -102,15 +104,15 @@
                 value=None,
                 multi=True
             ),
             html.Br(),
             dcc.Markdown("""Select one or more lineages"""),
             dcc.Dropdown(
                 id=ID_DROPDOWN_LINEAGE,
-                options=[{'label': c, 'value': c} for c in queries.get_lineages(data_source.name)],
+                options=[{'label': c, 'value': v} for c, v in zip(lineages.combined_label, lineages.pangolin_lineage)],
                 value=None,
                 multi=True
             ),
             html.Br(),
             dcc.Markdown("""Select time period for smoothing"""),
             dcc.Dropdown(
                 id=ID_DROPDOWN_PERIOD,
@@ -120,24 +122,24 @@
             ),
             html.Br(),
             dcc.Markdown("""Select a start and end date"""),
             html.Div(children=[
                 dcc.Dropdown(
                     id=ID_DROPDOWN_LINEAGE_DATE_RANGE_START,
                     options=[{'label': c, 'value': c} for c in months],
-                    value=oneyearago_formatted,
+                    value=one_year_before_update_formatted,
                     multi=False,
                     clearable=False
                 ),
                 html.Div(
                     id=ID_DROPDOWN_LINEAGE_DATE_RANGE_END_DIV,
                     children=dcc.Dropdown(
                         id=ID_DROPDOWN_LINEAGE_DATE_RANGE_END,
                         options=[{'label': c, 'value': c} for c in months],
-                        value=today_formatted,
+                        value=last_update_formatted,
                         multi=False,
                         clearable=False
                     ))]),
             html.Br(),
             dcc.Markdown("""Minimum prevalence of lineage in the time interval to be plotted"""),
             dcc.Slider(
                 id=ID_SLIDER_PREVALENCE,
@@ -157,16 +159,17 @@
 def set_callbacks_lineages_tab(app, session: Session):
 
     queries = Queries(session=session)
     figures = LineageFigures(queries)
 
     countries_ena = queries.get_countries(DataSource.ENA.name)
     countries_covid19_portal = queries.get_countries(DataSource.COVID19_PORTAL.name)
-    lineages_ena = queries.get_lineages(DataSource.ENA.name)
-    lineages_covid19_portal = queries.get_lineages(DataSource.COVID19_PORTAL.name)
+
+    lineages_ena = queries.get_combined_labels(DataSource.ENA.name)
+    lineages_covid19_portal = queries.get_combined_labels(DataSource.COVID19_PORTAL.name)
 
     # Get months from ENA/Covid19 table
     months_from_db_ena = queries.get_sample_months(MONTH_PATTERN, data_source=DataSource.ENA.name)
     months_from_db_covid19_portal = queries.get_sample_months(MONTH_PATTERN, data_source=DataSource.COVID19_PORTAL.name)
 
     @app.callback(
         Output(ID_DROPDOWN_COUNTRY, 'options'),
@@ -187,25 +190,28 @@
         Input(ID_DROPDOWN_DATA_SOURCE, 'value'))
     def set_lineages(source):
         """
         Updates the country drop down list when the data source is changed
         """
         lineages = []
         if source == DataSource.ENA.name:
-            lineages = [{'label': c, 'value': c} for c in lineages_ena]
+            lineages = [{'label': c, 'value': v} for c, v in zip(lineages_ena.combined_label, lineages_ena.pangolin_lineage)]
         elif source == DataSource.COVID19_PORTAL.name:
-            lineages = [{'label': c, 'value': c} for c in lineages_covid19_portal]
+            lineages = [{'label': c, 'value': v} for c, v in zip(lineages_covid19_portal.combined_label, lineages_covid19_portal.pangolin_lineage)]
         return lineages
 
     @app.callback(
         Output(ID_DROPDOWN_LINEAGE_DATE_RANGE_END_DIV, 'children'),
         Input(ID_DROPDOWN_LINEAGE_DATE_RANGE_START, 'value'),
         Input(ID_DROPDOWN_DATA_SOURCE, 'value')
     )
     def update_dropdown_end_date(start_date, data_source):
+        """
+        Updates the date selection slider when data source is changed
+        """
         today = datetime.now()
         today_formatted = today.strftime(MONTH_PATTERN)
         months = []
         if data_source == DataSource.ENA.name:
             months = [m for m in months_from_db_ena if m >= start_date]
         elif data_source == DataSource.COVID19_PORTAL.name:
             months = [m for m in months_from_db_covid19_portal if m >= start_date]
```

### Comparing `covigator-2.1.0/covigator/dashboard/tabs/mutation_stats.py` & `covigator-2.2.0/covigator/dashboard/tabs/mutation_stats.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/tabs/overview.py` & `covigator-2.2.0/covigator/dashboard/tabs/overview.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/dashboard/tabs/recurrent_mutations.py` & `covigator-2.2.0/covigator/dashboard/tabs/recurrent_mutations.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,18 +61,20 @@
 
 
 def get_variants_tab_left_bar(queries: Queries, data_source: DataSource):
 
     # removes repeated gene names (ie: ORF1ab)
     genes = sorted({c.name for c in queries.get_genes()})
     months = queries.get_sample_months(MONTH_PATTERN, data_source=data_source.name)
-    today = datetime.now()
-    today_formatted = today.strftime(MONTH_PATTERN)
-    oneyearago = today - timedelta(days=356)
-    oneyearago_formatted = oneyearago.strftime(MONTH_PATTERN)
+
+    last_update = queries.get_last_update(data_source.name)
+    last_update_formatted = last_update.strftime(MONTH_PATTERN)
+
+    one_year_before_update = last_update - timedelta(days=365)
+    one_year_before_update_formatted = one_year_before_update.strftime(MONTH_PATTERN)
 
     if data_source == DataSource.ENA:
         teaser = html.Div([html.Div(
             dbc.Button("Top recurrent mutations", color="secondary", className="me-1", style={'font-size': '100%'})),
                         html.Br(), html.Div(
                 dbc.Button("Genome/gene view", color="secondary", className="me-1", style={'font-size': '100%'})),
                         html.Br(), html.Div(
@@ -137,24 +139,24 @@
         ),
         html.Br(),
         dcc.Markdown("""Select a start and end date"""),
         html.Div(children=[
             dcc.Dropdown(
                 id=ID_DROPDOWN_DATE_RANGE_START,
                 options=[{'label': c, 'value': c} for c in months],
-                value=oneyearago_formatted,
+                value=one_year_before_update_formatted,
                 multi=False,
                 clearable=False
             ),
             html.Div(
                 id=ID_DROPDOWN_DATE_RANGE_END_DIV,
                 children=dcc.Dropdown(
                     id=ID_DROPDOWN_DATE_RANGE_END,
                     options=[{'label': c, 'value': c} for c in months],
-                    value=today_formatted,
+                    value=last_update_formatted,
                     multi=False,
                     clearable=False
                 ))]),
         html.Br(),
         dcc.Markdown("""**Genome view**
         
 Bin size"""),
```

### Comparing `covigator-2.1.0/covigator/dashboard/tabs/samples.py` & `covigator-2.2.0/covigator/dashboard/tabs/samples.py`

 * *Files 15% similar despite different names*

```diff
@@ -39,14 +39,16 @@
             html.Hr(),
             html.Br(),
             html.Div(id=ID_DN_DS_GRAPH),
         ])
 
 
 def get_samples_tab_left_bar(queries: Queries, data_source: DataSource):
+
+    lineages = queries.get_combined_labels(data_source.name)
     return html.Div(
         className="two columns",
         children=[
             html.Div([
                 html.Div(dbc.Button(
                     "Samples accumulation",
                     color="secondary",
@@ -77,15 +79,15 @@
                 value=None,
                 multi=True
             ),
             html.Br(),
             dcc.Markdown("""Select one or more lineages"""),
             dcc.Dropdown(
                 id=ID_DROPDOWN_LINEAGE,
-                options=[{'label': c, 'value': c} for c in queries.get_lineages(data_source.name)],
+                options=[{'label': c, 'value': v} for c, v in zip(lineages.combined_label, lineages.pangolin_lineage)],
                 value=None,
                 multi=True
             ),
             html.Br(),
             dcc.Markdown("""Minimum number of samples per country"""),
             dcc.Slider(
                 id=ID_SLIDER_MIN_SAMPLES,
@@ -113,16 +115,16 @@
 def set_callbacks_samples_tab(app, session: Session):
 
     queries = Queries(session=session)
     figures = SampleFigures(queries)
 
     countries_ena = queries.get_countries(DataSource.ENA.name)
     countries_covid19_portal = queries.get_countries(DataSource.COVID19_PORTAL.name)
-    lineages_ena = queries.get_lineages(DataSource.ENA.name)
-    lineages_covid19_portal = queries.get_lineages(DataSource.COVID19_PORTAL.name)
+    lineages_ena = queries.get_combined_labels(source=DataSource.ENA.name)
+    lineages_covid19_portal = queries.get_combined_labels(source=DataSource.COVID19_PORTAL.name)
 
     @app.callback(
         Output(ID_DROPDOWN_COUNTRY, 'options'),
         Input(ID_DROPDOWN_DATA_SOURCE, 'value'))
     def set_countries(source):
         """
         Updates the country drop down list when the data source is changed
@@ -139,17 +141,17 @@
         Input(ID_DROPDOWN_DATA_SOURCE, 'value'))
     def set_lineages(source):
         """
         Updates the country drop down list when the data source is changed
         """
         lineages = []
         if source == DataSource.ENA.name:
-            lineages = [{'label': c, 'value': c} for c in lineages_ena]
+            lineages = [{'label': c, 'value': v} for c, v in zip(lineages_ena.combined_label, lineages_ena.pangolin_lineage)]
         elif source == DataSource.COVID19_PORTAL.name:
-            lineages = [{'label': c, 'value': c} for c in lineages_covid19_portal]
+            lineages = [{'label': c, 'value': v} for c, v in zip(lineages_covid19_portal.combined_label, lineages_covid19_portal.pangolin_lineage)]
         return lineages
 
     @app.callback(
         Output(ID_SLIDER_MIN_SAMPLES, 'disabled'),
         Input(ID_DROPDOWN_COUNTRY, 'value'),
         Input(ID_DROPDOWN_LINEAGE, 'value')
     )
```

### Comparing `covigator-2.1.0/covigator/database/database.py` & `covigator-2.2.0/covigator/database/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import tenacity
 from logzero import logger
 from sqlalchemy import create_engine, text
 from sqlalchemy.engine import Engine
 from sqlalchemy.orm import sessionmaker, Session
 from tenacity import wait_exponential, stop_after_attempt
 from covigator.configuration import Configuration
-from covigator.database.model import Base, Gene, Conservation
+from covigator.database.model import Base, Gene, Conservation, Lineages
 from covigator.exceptions import CovigatorDatabaseConnectionException
 from covigator.references.conservation import ConservationLoader
 from covigator.references.gene_annotations import GeneAnnotationsLoader
+from covigator.references.lineage_annotation import LineageAnnotationsLoader
 
 
 class Database:
 
     def __init__(self, config: Configuration = None, test=False, verbose=False, initialize=False):
         if test:
             # connects to the test postgres in the CI environment
@@ -41,14 +42,16 @@
     def initialise_database(self):
         session = self.get_database_session()
         # loads reference genome if not set
         if session.query(Gene).count() == 0:
             GeneAnnotationsLoader(session).load_data()
         if session.query(Conservation).count() == 0:
             ConservationLoader(session).load_data()
+        if session.query(Lineages).count() == 0:
+            LineageAnnotationsLoader(session).load_data()
 
     def get_database_session(self) -> Session:
         return self.Session()
 
 
 @contextmanager
 def session_scope(config: Configuration = None, database: Database = None, initialize=False, test=False) -> Session:
```

### Comparing `covigator-2.1.0/covigator/database/model.py` & `covigator-2.2.0/covigator/database/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from datetime import datetime
 from typing import List
 from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import relationship
 from sqlalchemy import Column, String, Float, Enum, DateTime, Integer, Boolean, Date, ForeignKey, \
     ForeignKeyConstraint, BigInteger, JSON, Index
 import enum
 from covigator.configuration import Configuration
 
 
 def get_table_versioned_name(basename, config: Configuration):
@@ -43,14 +44,18 @@
 PRECOMPUTED_VARIANT_ABUNDANCE_HIST_TABLE_NAME = get_table_versioned_name('precomputed_variant_abundance_histogram', config=config)
 PRECOMPUTED_VARIANTS_PER_LINEAGE_TABLE_NAME = get_table_versioned_name('precomputed_variants_per_lineage', config=config)
 JOB_STATUS_CONSTRAINT_NAME = get_table_versioned_name('job_status', config=config)
 DATA_SOURCE_CONSTRAINT_NAME = get_table_versioned_name('data_source', config=config)
 COVIGATOR_MODULE_CONSTRAINT_NAME = get_table_versioned_name('covigator_module', config=config)
 REGION_TYPE_CONSTRAINT_NAME = get_table_versioned_name('region_type', config=config)
 VARIANT_TYPE_CONSTRAINT_NAME = get_table_versioned_name('variant_type', config=config)
+LINEAGE_TABLE_NAME = get_table_versioned_name('lineage', config=config)
+CONSTELLATION_SITES_TABLE_NAME = get_table_versioned_name('lineage_defining_variant', config=config)
+LINEAGE_SITES_JUNCTION_TABLE_NAME = get_table_versioned_name('lineage_variant', config=config)
+VARIANT_LEVEL_CONSTRAINT_NAME = get_table_versioned_name('variant_level', config=config)
 SEPARATOR = ";"
 
 Base = declarative_base()
 
 
 class Gene(Base):
     """
@@ -354,15 +359,14 @@
 
     def get_sample_folder(self, base_folder: str):
         return os.path.join(
             base_folder,
             self.collection_date.strftime("%Y%m%d") if self.collection_date is not None else "nodate",
             self.run_accession)
 
-
 class Variant(Base):
     """
     A variant with its specific annotations. THis does not contain any sample specific annotations.
     """
     __tablename__ = VARIANT_TABLE_NAME
 
     variant_id = Column(String, primary_key=True)
@@ -527,14 +531,15 @@
     pfam_description = Column(String)
 
     def get_variant_id(self):
         return "{}:{}>{}".format(self.position, self.reference, self.alternate)
 
 
 class LowFrequencyVariant(Base):
+
     __tablename__ = LOW_FREQUENCY_VARIANT_TABLE_NAME
 
     variant_id = Column(String, primary_key=True)
     chromosome = Column(String)
     position = Column(Integer, index=True)
     reference = Column(String)
     alternate = Column(String)
@@ -1072,15 +1077,15 @@
 
 class RegionType(enum.Enum):
 
     __constraint_name__ = REGION_TYPE_CONSTRAINT_NAME
 
     GENE = 1
     DOMAIN = 2
-    CODING_REGION=3
+    CODING_REGION = 3
 
 
 class PrecomputedSynonymousNonSynonymousCounts(Base):
 
     __tablename__ = PRECOMPUTED_NS_S_COUNTS_TABLE_NAME
 
     id = Column(Integer, primary_key=True, autoincrement=True)
@@ -1124,7 +1129,82 @@
 
     id = Column(Integer, primary_key=True, autoincrement=True)
     lineage = Column(String)
     variant_id = Column(String)
     country = Column(String)
     count_observations = Column(Integer)
     source = Column(Enum(DataSource, name=DataSource.__constraint_name__))
+
+
+class Lineages(Base):
+    """
+    Annotate pangolin lineage identifiers with WHO designation, VOC/VUI, parent name
+    """
+    __tablename__ = LINEAGE_TABLE_NAME
+
+    pango_lineage_id = Column(String, primary_key=True)
+    # Constellation label used by scorpio for assignment
+    constellation_id = Column(String)
+    who_label = Column(String)
+    # VOC/VUI/V information
+    phe_label = Column(String)
+    voc_date = Column(Date)
+    vui_date = Column(Date)
+    variant_of_concern = Column(Boolean, default=False)
+    variant_under_investigation = Column(Boolean, default=False)
+    parent_lineage_id = Column(String)
+    tags = Column(String)
+
+    variants = relationship(
+        "LineageDefiningVariants",
+        secondary=LINEAGE_SITES_JUNCTION_TABLE_NAME,
+        back_populates='constellations',
+    )
+
+
+class VariantLevel(enum.Enum):
+    __constraint_name__ = VARIANT_LEVEL_CONSTRAINT_NAME
+
+    PROTEOMIC = 1
+    GENOMIC = 2
+
+
+class LineageDefiningVariants(Base):
+    """
+    Store lineage defining mutations as defined in the scorpio constellation files. Mutations can be in nucleotide
+    (intergenic) or proteomic space. The columns variant_id, position, reference and alternate therefore have different
+    meanings and formatting
+
+    Variant_id: position_in_genome:[reference_bases]>[alternate_nuc] (genomic level)
+                canonical_protein_name:[reference_aa]position_in_protein[alternate_aa] (proteomic level)
+    position: position_in_genome (genomic level) or position_in_protein (proteomic level)
+    reference: reference_bases (genomic level) or reference_aa (proteomic level)
+    alternate: alternate_bases (genomic level) or alternate_aa (proteomic level)
+    """
+    __tablename__ = CONSTELLATION_SITES_TABLE_NAME
+
+    variant_id = Column(String, primary_key=True)
+    variant_type = Column(Enum(VariantType, name=VariantType.__constraint_name__))
+    protein = Column(String)
+    position = Column(Integer, index=True)
+    reference = Column(String)
+    alternate = Column(String)
+    ambiguous_alternate = Column(Boolean, default=False)
+    annotation = Column(String)
+    hgvs = Column(String)
+    variant_level = Column(Enum(VariantLevel, name=VariantLevel.__constraint_name__))
+
+    constellations = relationship(
+        "Lineages",
+        secondary=LINEAGE_SITES_JUNCTION_TABLE_NAME,
+        back_populates="variants")
+
+
+class LineageVariant(Base):
+    """
+    Junction table that maps constellation sites to their respective lineage
+    """
+    __tablename__ = LINEAGE_SITES_JUNCTION_TABLE_NAME
+
+    pango_lineage_id = Column(ForeignKey(Lineages.pango_lineage_id), primary_key=True)
+    variant_id = Column(ForeignKey(LineageDefiningVariants.variant_id), primary_key=True)
+
```

### Comparing `covigator-2.1.0/covigator/database/queries.py` & `covigator-2.2.0/covigator/database/queries.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from datetime import date, datetime
 from typing import List, Union, Tuple
+
 import pandas as pd
 from logzero import logger
 import sqlalchemy
 from sqlalchemy import and_, desc, asc, func, String, DateTime, text
 from sqlalchemy.engine.default import DefaultDialect
 from sqlalchemy.orm import Session, aliased
 from sqlalchemy.sql.sqltypes import NullType
 from covigator import SYNONYMOUS_VARIANT
 from covigator.database.model import DataSource, SampleEna, JobStatus, \
     VariantObservation, Gene, Variant, VariantCooccurrence, Conservation, \
     SubclonalVariantObservation, PrecomputedVariantsPerSample, PrecomputedSubstitutionsCounts, PrecomputedIndelLength, \
     VariantType, PrecomputedAnnotation, PrecomputedOccurrence, PrecomputedTableCounts, \
     PrecomputedVariantAbundanceHistogram, PrecomputedSynonymousNonSynonymousCounts, RegionType, Domain, \
-    LastUpdate, SampleCovid19Portal, VariantObservationCovid19Portal, VariantCovid19Portal
+    LastUpdate, SampleCovid19Portal, VariantObservationCovid19Portal, VariantCovid19Portal, Lineages, LineageVariant, \
+    LineageDefiningVariants
 from covigator.exceptions import CovigatorQueryException, CovigatorDashboardMissingPrecomputedData
 
 
 class Queries:
 
     def __init__(self, session: Session):
         self.session = session
@@ -103,14 +105,101 @@
 
     def get_lineages(self, source: str) -> List[str]:
         klass = self.get_sample_klass(source=source)
         return [c for c, in self.session.query(klass.pangolin_lineage).filter(
             and_(klass.status == JobStatus.FINISHED.name, klass.pangolin_lineage != None)).distinct().order_by(
                 klass.pangolin_lineage.asc()).all()]
 
+    def find_parent_who_label(self, lineage, parent_mapping) -> str:
+        """
+        In some instances a constellation does not include a WHO label. Nevertheless, these sublineages also belong to
+        this VOC and should also be grouped with this label. Returns a string containing the WHO label of the topmost
+        parent in the tree if present, otherwise just the label.
+
+        Examples are local lineage variations such as AY.4.2 and AY.4 --> Delta
+        """
+        lineage = parent_mapping.query("pangolin_lineage == @lineage").get(["pangolin_lineage", "who_label",
+                                                                            "parent_lineage_id"])
+        # No or last parent in tree --> return WHO label
+        parent = lineage.get("parent_lineage_id").item()
+        if pd.isnull(parent):
+            return lineage.get("who_label").item()
+        else:
+            return self.find_parent_who_label(parent, parent_mapping)
+
+    def get_lineages_who_label(self) -> pd.DataFrame:
+        """
+        Query database for lineage WHO label annotation. Returns a DataFrame with columns: pangolin_lineage, who_label
+        """
+        query = self.session.query(Lineages.pango_lineage_id.label("pangolin_lineage"), Lineages.who_label)
+        lineages = pd.read_sql(query.statement, self.session.bind)
+        lineages = lineages[["pangolin_lineage", "who_label"]]
+        return lineages
+
+    def get_combined_labels(self, source: str) -> pd.DataFrame:
+        """
+        Create a mapping from pangolin IDs in the data source to WHO identifiers and create a combined
+        label to be used in the dashboard
+        """
+        who_labels = self.get_lineages_who_label()
+        lineages = self.get_lineages(source)
+        if not lineages:
+            return None
+        lineages = pd.DataFrame(lineages, columns=["pangolin_lineage"])
+        lineages = lineages.merge(who_labels, how="left")
+        lineages["combined_label"] = lineages.apply(lambda x: f"{x.pangolin_lineage} - {x.who_label}"
+            if not pd.isnull(x.who_label) else f"{x.pangolin_lineage}", axis=1)
+        return lineages
+
+    def get_lineage_defining_variants(self) -> pd.DataFrame:
+        """
+        Query database for lineage defining variants. Returns a dataframe with columns: pangolin_lineage, variant
+        """
+        query = self.session.query(LineageVariant.pango_lineage_id.label("pangolin_lineage"), LineageVariant.variant_id,
+                                   LineageDefiningVariants.hgvs).join(LineageDefiningVariants)
+        lineage_variants = pd.read_sql(query.statement, self.session.bind)
+        # Rename columns to match columns used in recurrent/intrahost mutations tab
+        lineage_variants["dna_mutation"] = lineage_variants.apply(lambda x: x.variant_id if pd.isnull(x.hgvs)
+                                                                  else None, axis=1)
+        lineage_variants = lineage_variants.rename(columns={"hgvs":"hgvs_p"})
+        aa_level_mutations = lineage_variants[~pd.isnull(lineage_variants.hgvs_p)].loc[:, ['pangolin_lineage','hgvs_p']]
+        aa_level_mutations = aa_level_mutations.sort_values(['hgvs_p', 'pangolin_lineage']).groupby('hgvs_p')['pangolin_lineage'].agg(','.join)
+        aa_level_mutations = aa_level_mutations.reset_index()
+
+        nucleotide_level_mutations = lineage_variants[~pd.isnull(lineage_variants.dna_mutation)].loc[:, ['pangolin_lineage','dna_mutation']]
+        nucleotide_level_mutations = nucleotide_level_mutations.sort_values(['dna_mutation', 'pangolin_lineage']).groupby('dna_mutation')['pangolin_lineage'].agg(','.join)
+        nucleotide_level_mutations = nucleotide_level_mutations.reset_index()
+
+        return aa_level_mutations, nucleotide_level_mutations
+
+    def _merge_with_lineage_defining_variants(self, data: pd.DataFrame):
+        """
+        Merge tables from recurrent and intrahost mutations tab with lineage defining mutations
+        """
+
+        assert "variant_id" in data.columns, "Column variant_id is missing..."
+        assert "hgvs_p" in data.columns, "Column hgvs_p is missing..."
+        lineage_mutation_aa, lineage_mutation_nuc = self.get_lineage_defining_variants()
+        lineage_mutation_nuc.rename(columns={'dna_mutation': 'variant_id'}, inplace=True)
+
+        # Merge data with lineage defining variants on different levels
+        data = data.merge(lineage_mutation_aa, how="left", left_on="hgvs_p", right_on="hgvs_p")
+        data = data.merge(lineage_mutation_nuc, how="left", left_on="variant_id", right_on="variant_id")
+
+        data["pangolin_lineage_x"].fillna(data["pangolin_lineage_y"], inplace=True)
+        data.drop(columns=["pangolin_lineage_y"], inplace=True)
+        # formats the lineage column
+        data.rename(columns={"pangolin_lineage_x": "pangolin_lineage"}, inplace=True)
+        data["no_of_lineages"] = data.fillna({"pangolin_lineage": ""}).apply(
+                lambda x: len(x.pangolin_lineage.split(",")), axis=1)
+        data['pangolin_hover'] = data.apply(
+                lambda x: "{} lineages".format(x.no_of_lineages) if x.no_of_lineages > 3 else x.pangolin_lineage,
+                    axis=1)
+        return data
+
     def get_variants_per_sample(self, data_source: str, genes: List[str], variant_types: List[str]):
         """
         Returns a DataFrame with columns: number_mutations, count, type
         where type: SNV, insertion or deletion
         """
         self._assert_data_source(data_source)
         query = self.session.query(PrecomputedVariantsPerSample)\
@@ -549,22 +638,24 @@
             query = query.filter(PrecomputedOccurrence.gene_name == gene_name)
         if metric == "count":
             query = query.order_by(PrecomputedOccurrence.count.desc())
         elif metric == "frequency_by_month":
             query = query.order_by(PrecomputedOccurrence.frequency.desc())
         else:
             raise CovigatorQueryException("Not supported metric for top occurring variants")
-
+        
         top_occurring_variants = pd.read_sql(query.statement, self.session.bind)
-
+        # Merge with lineage defining variants
+        top_occurring_variants = self._merge_with_lineage_defining_variants(top_occurring_variants)
         # formats the DNA mutation
-        top_occurring_variants.rename(columns={'variant_id': 'dna_mutation'}, inplace=True)
+        top_occurring_variants.rename(columns={"variant_id": "dna_mutation"}, inplace=True)
+
         # pivots the table over months
         top_occurring_variants = pd.pivot_table(
-            top_occurring_variants, index=['gene_name', 'dna_mutation', 'hgvs_p', 'annotation', "frequency", "total"],
+            top_occurring_variants, index=['gene_name', 'dna_mutation', 'hgvs_p', 'annotation', "frequency", "total", "pangolin_lineage", "pangolin_hover"],
             columns=["month"], values=[metric], fill_value=0).droplevel(0, axis=1).reset_index()
 
         return top_occurring_variants.sort_values(by="frequency", ascending=False).head(top)
 
     def get_variant_abundance_histogram(self, source: str, bin_size=50, cache=True) -> pd.DataFrame:
         histogram = None
         if cache:
```

### Comparing `covigator-2.1.0/covigator/exceptions.py` & `covigator-2.2.0/covigator/exceptions.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/misc/backoff_retrier.py` & `covigator-2.2.0/covigator/misc/backoff_retrier.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/misc/country_parser.py` & `covigator-2.2.0/covigator/misc/country_parser.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/pipeline/covid19_portal_pipeline.py` & `covigator-2.2.0/covigator/pipeline/covid19_portal_pipeline.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/pipeline/downloader.py` & `covigator-2.2.0/covigator/pipeline/downloader.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/pipeline/ena_pipeline.py` & `covigator-2.2.0/covigator/pipeline/ena_pipeline.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/pipeline/runner.py` & `covigator-2.2.0/covigator/pipeline/runner.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/pipeline/vcf_loader.py` & `covigator-2.2.0/covigator/pipeline/vcf_loader.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/precomputations/load_cooccurrences.py` & `covigator-2.2.0/covigator/precomputations/load_cooccurrences.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/precomputations/load_ns_s_counts.py` & `covigator-2.2.0/covigator/precomputations/load_ns_s_counts.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                 data=data_portal, source=DataSource.GISAID, region=region))
 
         return database_rows
 
     def _dataframe_to_model(self, data, source: DataSource, region: RegionType):
 
         database_rows = []
-        for index, row in data.iterrows():
+        for _, row in data.iterrows():
             database_rows.append(self._row_to_model(row, source, region))
 
         if region == RegionType.GENE:
             # if we are processing genes then we calculate also for the coding region overall
             coding_region_ns = {}
             coding_region_s = {}
             for index, row in data.iterrows():
```

### Comparing `covigator-2.1.0/covigator/precomputations/load_top_occurrences.py` & `covigator-2.2.0/covigator/precomputations/load_top_occurrences.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/precomputations/load_variants_per_lineage.py` & `covigator-2.2.0/covigator/precomputations/load_variants_per_lineage.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,19 +48,19 @@
         try:
             variants_per_lineage_portal = self.get_variants_per_lineage(source=DataSource.COVID19_PORTAL.name)
         except ValueError:
             logger.error("No top occurrences for Covid19 Portal data")
         database_rows = []
         # stores the precomputed data
         if variants_per_lineage_ena is not None:
-            for index, row in variants_per_lineage_ena.iterrows():
+            for _, row in variants_per_lineage_ena.iterrows():
                 # add entries per gene
                 database_rows.append(_row_to_variants_per_lineage(row, source=DataSource.ENA))
         if variants_per_lineage_portal is not None:
-            for index, row in variants_per_lineage_portal.iterrows():
+            for _, row in variants_per_lineage_portal.iterrows():
                 # add entries per gene
                 database_rows.append(_row_to_variants_per_lineage(row, source=DataSource.COVID19_PORTAL))
         return database_rows
 
     def get_variants_per_lineage(self, source: str):
         klass_variant_observation = self.queries.get_variant_observation_klass(source)
         klass_sample = self.queries.get_sample_klass(source)
```

### Comparing `covigator-2.1.0/covigator/precomputations/loader.py` & `covigator-2.2.0/covigator/precomputations/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,23 +74,23 @@
             select count(*) as number_mutations, variant_type, sample from {table_name}
             group by variant_type, sample)
             as counts group by counts.number_mutations, counts.variant_type;
             """.format(table_name=table_name)
         data_without_gene = pd.read_sql_query(sql_query, self.session.bind)
 
         database_rows = []
-        for index, row in data.iterrows():
+        for _, row in data.iterrows():
             database_rows.append(PrecomputedVariantsPerSample(
                 count=row["count"],
                 number_mutations=row["number_mutations"],
                 source=data_source.name,
                 variant_type=row["variant_type"],
                 gene_name=row["gene_name"] if row["gene_name"] is not None else "intergenic"
             ))
-        for index, row in data_without_gene.iterrows():
+        for _, row in data_without_gene.iterrows():
             database_rows.append(PrecomputedVariantsPerSample(
                 count=row["count"],
                 number_mutations=row["number_mutations"],
                 source=data_source.name,
                 variant_type=row["variant_type"]
             ))
         return database_rows
@@ -343,15 +343,15 @@
                 bin_size=bin_size, source=DataSource.COVID19_PORTAL.name, cache=False)
             if histogram is not None:
                 histogram["bin_size"] = bin_size
                 histogram["source"] = DataSource.COVID19_PORTAL
                 histograms.append(histogram)
         database_rows = []
         if len(histograms) > 0:
-            for index, row in pd.concat(histograms).iterrows():
+            for _, row in pd.concat(histograms).iterrows():
                 # add entries per gene
                 database_rows.append(PrecomputedVariantAbundanceHistogram(
                     position_bin=row["position_bin"],
                     count_unique_variants=row["count_unique_variants"],
                     count_variant_observations=row["count_variant_observations"],
                     bin_size=row["bin_size"],
                     source=row["source"],
```

### Comparing `covigator-2.1.0/covigator/processor/abstract_processor.py` & `covigator-2.2.0/covigator/processor/abstract_processor.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/processor/covid19portal_processor.py` & `covigator-2.2.0/covigator/processor/covid19portal_processor.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/processor/ena_downloader.py` & `covigator-2.2.0/covigator/processor/ena_downloader.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/processor/ena_processor.py` & `covigator-2.2.0/covigator/processor/ena_processor.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/references/conservation.py` & `covigator-2.2.0/covigator/references/conservation.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/references/domains_NS_S.csv` & `covigator-2.2.0/covigator/references/domains_NS_S.csv`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/references/gene_annotations.py` & `covigator-2.2.0/covigator/references/gene_annotations.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/references/genes_NS_S.csv` & `covigator-2.2.0/covigator/references/genes_NS_S.csv`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/references/sars_cov_2.json` & `covigator-2.2.0/covigator/references/sars_cov_2.json`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/references/wuhCor1.mutDepletionConsHMM.bed` & `covigator-2.2.0/covigator/references/wuhCor1.mutDepletionConsHMM.bed`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/references/wuhCor1.mutDepletionSarbecovirusConsHMM.bed` & `covigator-2.2.0/covigator/references/wuhCor1.mutDepletionSarbecovirusConsHMM.bed`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/references/wuhCor1.mutDepletionVertebrateCoVConsHMM.bed` & `covigator-2.2.0/covigator/references/wuhCor1.mutDepletionVertebrateCoVConsHMM.bed`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/integration_tests/integration_tests.py` & `covigator-2.2.0/covigator/tests/integration_tests/integration_tests.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/integration_tests/test_downloader.py` & `covigator-2.2.0/covigator/tests/integration_tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/integration_tests/test_pipeline.py` & `covigator-2.2.0/covigator/tests/integration_tests/test_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 class PipelineTest(unittest.TestCase):
 
     def test_pipeline_run(self):
         fastq1 = "SRR11140748_R1.fastq.gz"
         fastq2 = "SRR11140748_R2.fastq.gz"
         vcf_file = "expected_snpeff.vcf"
         p = Pipeline(config=Configuration())
-    
+
         # TODO: Implement Unit Test here
-        # Maybe do diff as assertion?    
+        # Maybe do diff as assertion?
         #self.assertEqual(p.run(fastq1=fastq1, fastq2=fastq2), vcf_file)
         #with self.assertRaises(CovigatorPipelineError):
             #vcf_file = p.run(fastq1=fastq1, fastq2=fastq2)
         vcf, _ = p.run(run_accession="test", fastq1=fastq1, fastq2=fastq2)
         self.assertEqual(open(vcf).read(), open(vcf_file).read())
```

### Comparing `covigator-2.1.0/covigator/tests/integration_tests/test_vcf_loader.py` & `covigator-2.2.0/covigator/tests/integration_tests/test_vcf_loader.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/resources/MN908947.3.fa` & `covigator-2.2.0/covigator/tests/resources/MN908947.3.fa`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/resources/Sars_cov_2.ASM985889v3.pep.all.fa` & `covigator-2.2.0/covigator/tests/resources/Sars_cov_2.ASM985889v3.pep.all.fa`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/resources/Sars_cov_2.all_variants.snpeff.vcf.gz` & `covigator-2.2.0/covigator/tests/resources/Sars_cov_2.all_variants.snpeff.vcf.gz`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/resources/domains_NS_S.csv` & `covigator-2.2.0/covigator/tests/resources/domains_NS_S.csv`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/resources/genes_NS_S.csv` & `covigator-2.2.0/covigator/tests/resources/genes_NS_S.csv`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/resources/gisaid_allprot0526.fasta` & `covigator-2.2.0/covigator/tests/resources/gisaid_allprot0526.fasta`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/resources/gisaid_allprot1208.fasta` & `covigator-2.2.0/covigator/tests/resources/gisaid_allprot1208.fasta`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/resources/gisaid_allprot1208.with_mutations.fasta` & `covigator-2.2.0/covigator/tests/resources/gisaid_allprot1208.with_mutations.fasta`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/resources/sars_cov_2.json` & `covigator-2.2.0/covigator/tests/resources/sars_cov_2.json`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/resources/sars_cov_2_dn_ds.json` & `covigator-2.2.0/covigator/tests/resources/sars_cov_2_dn_ds.json`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/resources/snpeff.vcf` & `covigator-2.2.0/covigator/tests/resources/snpeff.vcf`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/resources/snpeff_with_deletion.vcf` & `covigator-2.2.0/covigator/tests/resources/snpeff_with_deletion.vcf`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/resources/snpeff_with_insertion.vcf` & `covigator-2.2.0/covigator/tests/resources/snpeff_with_insertion.vcf`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/resources/snpeff_without_annotation.vcf` & `covigator-2.2.0/covigator/tests/resources/snpeff_without_annotation.vcf`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/resources/snpeff_without_dp4.vcf` & `covigator-2.2.0/covigator/tests/resources/snpeff_without_dp4.vcf`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/resources/test.another_pangolin.csv` & `covigator-2.2.0/covigator/tests/resources/test.another_pangolin.csv`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/resources/test.assembly.vcf.gz` & `covigator-2.2.0/covigator/tests/resources/test.assembly.vcf.gz`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/resources/test.deduplication_metrics.txt` & `covigator-2.2.0/covigator/tests/resources/test.deduplication_metrics.txt`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/resources/test.lofreq.vcf.gz` & `covigator-2.2.0/covigator/tests/resources/test.lofreq.vcf.gz`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/resources/test_data.fasta` & `covigator-2.2.0/covigator/tests/resources/test_data.fasta`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/unit_tests/abstract_test.py` & `covigator-2.2.0/covigator/tests/unit_tests/abstract_test.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/unit_tests/faked_objects.py` & `covigator-2.2.0/covigator/tests/unit_tests/faked_objects.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/unit_tests/mocked.py` & `covigator-2.2.0/covigator/tests/unit_tests/mocked.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/unit_tests/test_country_parser.py` & `covigator-2.2.0/covigator/tests/unit_tests/test_country_parser.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/unit_tests/test_downloader.py` & `covigator-2.2.0/covigator/tests/unit_tests/test_downloader.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/unit_tests/test_ena_accessor.py` & `covigator-2.2.0/covigator/tests/unit_tests/test_ena_accessor.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/unit_tests/test_figures.py` & `covigator-2.2.0/covigator/tests/unit_tests/test_figures.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/unit_tests/test_precomputer.py` & `covigator-2.2.0/covigator/tests/unit_tests/test_precomputer.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/unit_tests/test_processor.py` & `covigator-2.2.0/covigator/tests/unit_tests/test_processor.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator/tests/unit_tests/test_queries.py` & `covigator-2.2.0/covigator/tests/unit_tests/test_queries.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import unittest
 
 from parameterized import parameterized
 
 from covigator import SYNONYMOUS_VARIANT
 from covigator.precomputations.loader import PrecomputationsLoader
 from covigator.precomputations.load_ns_s_counts import NsSCountsLoader
-from covigator.database.model import JobStatus, DataSource, Gene, RegionType, Domain
+from covigator.database.model import JobStatus, DataSource, Gene, RegionType, Domain, Lineages
 from covigator.database.queries import Queries
 from covigator.tests.unit_tests.abstract_test import AbstractTest
 from covigator.tests.unit_tests.mocked import get_mocked_variant, \
     get_mocked_variant_observation, mock_samples, mock_cooccurrence_matrix, mock_samples_and_variants, MOCKED_DOMAINS, \
     get_mocked_sample
 
-
 class QueriesTests(AbstractTest):
 
     def setUp(self) -> None:
         self.queries = Queries(session=self.session)
 
     def test_get_date_of_first_ena_sample(self):
         first_sample_date = None
@@ -90,15 +89,15 @@
         self.assertGreaterEqual(data[data["frequency"] > 0].shape[0], len(variants))
         self.assertGreaterEqual(data[data["jaccard"] > 0].shape[0], len(variants))
 
     @unittest.skip
     def test_get_mds(self):
         mock_cooccurrence_matrix(faker=self.faker, session=self.session)
 
-        mds_fit, mds_coords = self.queries.get_mds(gene_name="S")
+        mds_fit, _ = self.queries.get_mds(gene_name="S")
         self.assertIsNotNone(mds_fit)
 
     @parameterized.expand([(DataSource.ENA, )])
     def test_get_variant_abundance_histogram(self, source):
 
         # gets an empty histogram
         histogram = self.queries.get_variant_abundance_histogram(cache=False, source=source.name)
@@ -195,14 +194,74 @@
         self.assertIsNotNone(domains)
         self.assertGreater(len(domains), 0)
         for d in domains:
             self.assertIsInstance(d, Domain)
             self.assertIsNotNone(d.name)
             self.assertEqual(d.gene_name, "S")
 
+    def test_get_lineages_who_label(self):
+        who_labels = self.queries.get_lineages_who_label()
+        self.assertIsNotNone(who_labels)
+        self.assertGreater(who_labels.shape[0], 0)
+        self.assertGreater(who_labels[~who_labels.who_label.isna()].shape[0], 0) # no emtpy who labels
+
+    def test_find_parent_who_label(self):
+        import pandas as pd
+        query = self.session.query(Lineages.pango_lineage_id.label("pangolin_lineage"), Lineages.who_label,
+                                   Lineages.parent_lineage_id)
+        data = pd.read_sql(query.statement, self.session.bind)
+        who_label = self.queries.find_parent_who_label("AY.4.2", data)
+        self.assertEqual(who_label, "Delta")
+        who_label = self.queries.find_parent_who_label("AY.4", data)
+        self.assertEqual(who_label, "Delta")
+        who_label = self.queries.find_parent_who_label("XE-parent2", data)
+        self.assertEqual(who_label, "Omicron")
+
+
+    @parameterized.expand([(DataSource.ENA, )])
+    def test_get_combined_labels(self, source):
+        # Mock some ENA samples
+        labels = self.queries.get_combined_labels(source.name)
+        self.assertIsNone(labels)
+
+        test_samples = [get_mocked_sample(faker=self.faker, source=source) for _ in range(10)]
+        self.session.add_all(test_samples)
+        self.session.commit()
+
+        labels = self.queries.get_combined_labels(source.name)
+        self.assertIsNotNone(labels)
+        self.assertGreater(labels.shape[0], 0)
+        self.assertEqual(labels[labels.combined_label.isna()].shape[0], 0)
+
+    def test_get_lineage_defining_variants(self):
+        lineage_mutation_aa, lineage_mutation_nuc = self.queries.get_lineage_defining_variants()
+        self.assertIsNotNone(lineage_mutation_aa)
+        self.assertIsNotNone(lineage_mutation_nuc)
+        self.assertGreater(lineage_mutation_aa.shape[0], 0)
+        self.assertGreater(lineage_mutation_nuc.shape[0], 0)
+
+        # Make sure that mutations on different levels have different columns for merging
+        self.assertTrue("dna_mutation" in lineage_mutation_nuc.columns)
+        self.assertTrue("hgvs_p" in lineage_mutation_aa.columns)
+
+    def test_merge_with_lineage_defining_variants(self):
+        import pandas as pd
+        data = {"variant_id": ["23403:A>G", "10029:C>T", "22995:C>A", "11201:A>G"], "hgvs_p": ["p.D614G", "p.T3255I", "p.T478K", "p.T3646A"]}
+        df = pd.DataFrame(data=data)
+        merged_table = self.queries._merge_with_lineage_defining_variants(df)
+        self.assertIsNotNone(merged_table)
+        self.assertGreater(merged_table.shape[0], 0)
+        # All mutations overlap with lineage mutations
+        self.assertEqual(merged_table[merged_table.no_of_lineages.isna()].shape[0], 0)
+        # Correct lineage numbers returned
+        self.assertTrue(merged_table.no_of_lineages.values.tolist() == [21, 19, 20, 2])
+        # Check that hover label is created correctly
+        self.assertTrue(merged_table.pangolin_hover.values.tolist() == ["21 lineages", "19 lineages", "20 lineages", "AY.4,AY.4.2"])
+
+
     def test_count_jobs_in_queue(self):
         mock_samples(faker=self.faker, session=self.session, job_status=JobStatus.QUEUED, num_samples=50)
         mock_samples(faker=self.faker, session=self.session, job_status=JobStatus.FINISHED, num_samples=50)
 
         count_jobs_in_queue_ena = self.queries.count_jobs_in_queue(DataSource.ENA)
         self.assertEqual(count_jobs_in_queue_ena, 50)
```

### Comparing `covigator-2.1.0/covigator/tests/unit_tests/test_vcf_loader.py` & `covigator-2.2.0/covigator/tests/unit_tests/test_vcf_loader.py`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/covigator.egg-info/PKG-INFO` & `covigator-2.2.0/covigator.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covigator
-Version: 2.1.0
+Version: 2.2.0
 Home-page: 
 Author: TRON - Translational Oncology at the University Medical Center of the Johannes Gutenberg University Mainz - Computational Medicine group
 Author-email: patrick.sorn@tron-mainz.de
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
@@ -69,23 +69,30 @@
 mutations. Importantly, we only process the Illumina samples from ENA. 
 This means excluding all of the Oxford Nanopore samples and hence having a partial view of all the available data.
 
 The dashboard is implemented in the visualization framework [Dash](https://dash.plotly.com/). 
 The computation is distributed through our cluster with a library of similar name [Dask](https://dask.org/).
 The analysis pipeline is implemented in the [Nextflow](https://www.nextflow.io/) framework.
 
-![CoVigator system](docs/source/_static/figures/system_design.drawio.png)
+![CoVigator system](docs/source/_static/figures/system_design_manuscript.png)
 
 <p align = "center">
 <b>Figure 3: System design</b>
 </p>
 
 The CoVigator project was developed at the Biomarker Development Center at 
 [TRON (Translational Oncology at the University Medical Center of the Johannes Gutenberg University gGmbH)](https://tron-mainz.de/). 
 The project was kindly supported by 
 [Intel´s Pandemic Response Technology Initiative](https://newsroom.intel.com/tag/pandemic-response-technology-initiative).
 
 ## How to cite
 
-* Schrörs, B., Riesgo-Ferreiro, P., Sorn, P., Gudimella, R., Bukur, T., Rösler, T., Löwer, M., & Sahin, U. (2021). 
+*   Bukur T., Riesgo-Ferreiro P., Sorn P, Gudimella R., Hausmann J., Rösler T., Löwer M., Schrörs B., & Sahin U. 
+CoVigator — A Knowledge Base for Navigating SARS-CoV-2 Genomic Variants. Viruses. 2023; 15(6):1391. [10.3390/v15061391](https://doi.org/10.3390/v15061391)
+
+*   Schrörs, B., Riesgo-Ferreiro, P., Sorn, P., Gudimella, R., Bukur, T., Rösler, T., Löwer, M., & Sahin, U. (2021). 
 Large-scale analysis of SARS-CoV-2 spike-glycoprotein mutants demonstrates the need for continuous screening of virus 
 isolates. PLOS ONE, 16(9), e0249254. [10.1371/journal.pone.0249254](https://doi.org/10.1371/journal.pone.0249254)
+
+### Acknowledgements
+
+The lineage annotation in the covigator dashboard package uses "the description of constellations of mutations for the SARS-CoV-2 virus" by [cov-lineages](https://github.com/cov-lineages/constellations) provided and licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)
```

### Comparing `covigator-2.1.0/covigator.egg-info/SOURCES.txt` & `covigator-2.2.0/covigator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 covigator/processor/ena_downloader.py
 covigator/processor/ena_processor.py
 covigator/references/__init__.py
 covigator/references/conservation.py
 covigator/references/domains_NS_S.csv
 covigator/references/gene_annotations.py
 covigator/references/genes_NS_S.csv
+covigator/references/lineage_annotation.py
 covigator/references/sars_cov_2.json
 covigator/references/wuhCor1.mutDepletionConsHMM.bed
 covigator/references/wuhCor1.mutDepletionSarbecovirusConsHMM.bed
 covigator/references/wuhCor1.mutDepletionVertebrateCoVConsHMM.bed
 covigator/tests/__init__.py
 covigator/tests/integration_tests/__init__.py
 covigator/tests/integration_tests/integration_tests.py
@@ -135,11 +136,12 @@
 covigator/tests/unit_tests/mocked.py
 covigator/tests/unit_tests/test_compression.py
 covigator/tests/unit_tests/test_country_parser.py
 covigator/tests/unit_tests/test_database_initialisation.py
 covigator/tests/unit_tests/test_downloader.py
 covigator/tests/unit_tests/test_ena_accessor.py
 covigator/tests/unit_tests/test_figures.py
+covigator/tests/unit_tests/test_lineage_annotation.py
 covigator/tests/unit_tests/test_precomputer.py
 covigator/tests/unit_tests/test_processor.py
 covigator/tests/unit_tests/test_queries.py
 covigator/tests/unit_tests/test_vcf_loader.py
```

### Comparing `covigator-2.1.0/covigator.egg-info/entry_points.txt` & `covigator-2.2.0/covigator.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `covigator-2.1.0/setup.py` & `covigator-2.2.0/setup.py`

 * *Files identical despite different names*

