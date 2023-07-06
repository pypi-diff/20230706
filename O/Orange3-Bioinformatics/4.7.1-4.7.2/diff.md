# Comparing `tmp/Orange3-Bioinformatics-4.7.1.tar.gz` & `tmp/Orange3-Bioinformatics-4.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Orange3-Bioinformatics-4.7.1.tar", last modified: Mon Feb  6 14:56:55 2023, max compression
+gzip compressed data, was "Orange3-Bioinformatics-4.7.2.tar", last modified: Thu Jul  6 19:42:49 2023, max compression
```

## Comparing `Orange3-Bioinformatics-4.7.1.tar` & `Orange3-Bioinformatics-4.7.2.tar`

### file list

```diff
@@ -1,284 +1,285 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.146360 Orange3-Bioinformatics-4.7.1/
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.102359 Orange3-Bioinformatics-4.7.1/.github/
--rw-r--r--   0 runner    (1001) docker     (122)      646 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.102359 Orange3-Bioinformatics-4.7.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      723 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (122)      622 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/.github/ISSUE_TEMPLATE/feature_request.md
--rwxr-xr-x   0 runner    (1001) docker     (122)      217 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.102359 Orange3-Bioinformatics-4.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1838 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)      184 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/.github/workflows/test.yml
--rwxr-xr-x   0 runner    (1001) docker     (122)      755 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      472 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     7593 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     3348 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.102359 Orange3-Bioinformatics-4.7.1/Orange3_Bioinformatics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2084 2023-02-06 14:56:54.000000 Orange3-Bioinformatics-4.7.1/Orange3_Bioinformatics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    10717 2023-02-06 14:56:55.000000 Orange3-Bioinformatics-4.7.1/Orange3_Bioinformatics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-06 14:56:54.000000 Orange3-Bioinformatics-4.7.1/Orange3_Bioinformatics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      223 2023-02-06 14:56:54.000000 Orange3-Bioinformatics-4.7.1/Orange3_Bioinformatics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-02-06 14:56:54.000000 Orange3-Bioinformatics-4.7.1/Orange3_Bioinformatics.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-06 14:56:54.000000 Orange3-Bioinformatics-4.7.1/Orange3_Bioinformatics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      358 2023-02-06 14:56:54.000000 Orange3-Bioinformatics-4.7.1/Orange3_Bioinformatics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-02-06 14:56:54.000000 Orange3-Bioinformatics-4.7.1/Orange3_Bioinformatics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2084 2023-02-06 14:56:55.146360 Orange3-Bioinformatics-4.7.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (122)     2707 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      728 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/README.pypi
--rw-r--r--   0 runner    (1001) docker     (122)      206 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.102359 Orange3-Bioinformatics-4.7.1/doc/
--rw-r--r--   0 runner    (1001) docker     (122)     7464 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.102359 Orange3-Bioinformatics-4.7.1/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/_static/bioinformatics-sidebar-logo.svg
--rw-r--r--   0 runner    (1001) docker     (122)      537 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.102359 Orange3-Bioinformatics-4.7.1/doc/_templates/
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/_templates/about.html
--rw-r--r--   0 runner    (1001) docker     (122)      333 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/_templates/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (122)      495 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/_templates/useful_links.html
--rw-r--r--   0 runner    (1001) docker     (122)    10329 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/contents.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2319 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7009 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (122)      439 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/scripting_reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.106359 Orange3-Bioinformatics-4.7.1/doc/scripting_references/
--rw-r--r--   0 runner    (1001) docker     (122)      309 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/scripting_references/annotation.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.098359 Orange3-Bioinformatics-4.7.1/doc/scripting_references/code/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.106359 Orange3-Bioinformatics-4.7.1/doc/scripting_references/code/geo/
--rw-r--r--   0 runner    (1001) docker     (122)      705 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/scripting_references/code/geo/dataset_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/scripting_references/code/geo/dataset_samples.py
--rw-r--r--   0 runner    (1001) docker     (122)      553 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/scripting_references/code/geo/predict_disease_state.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.106359 Orange3-Bioinformatics-4.7.1/doc/scripting_references/code/go/
--rw-r--r--   0 runner    (1001) docker     (122)      843 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/scripting_references/code/go/enrichment.py
--rw-r--r--   0 runner    (1001) docker     (122)      823 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/scripting_references/code/go/gene_annotations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/scripting_references/dicty_phenotypes.rst
--rw-r--r--   0 runner    (1001) docker     (122)      965 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/scripting_references/geneset.rst
--rw-r--r--   0 runner    (1001) docker     (122)     4033 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/scripting_references/geo.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/scripting_references/go.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/scripting_references/kegg.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/scripting_references/marker_genes.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2660 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/scripting_references/ncbi_gene.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/scripting_references/ncbi_taxonomy.rst
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/scripting_references/resolwe.rst
--rw-r--r--   0 runner    (1001) docker     (122)     3949 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/scripting_references/serverfiles.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.106359 Orange3-Bioinformatics-4.7.1/doc/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)     4768 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/annotate_projection.md
--rw-r--r--   0 runner    (1001) docker     (122)      633 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/cluster_analysis.md
--rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/databases_update.md
--rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/dicty_express.md
--rw-r--r--   0 runner    (1001) docker     (122)     3953 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/differential_expression.md
--rw-r--r--   0 runner    (1001) docker     (122)      535 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/gene_set_enrichment.md
--rw-r--r--   0 runner    (1001) docker     (122)     1564 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/genes.md
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/geo_data_sets.md
--rw-r--r--   0 runner    (1001) docker     (122)     5027 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/go_browser.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.106359 Orange3-Bioinformatics-4.7.1/doc/widgets/icons/
--rw-r--r--   0 runner    (1001) docker     (122)    35120 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/icons/annotator.png
--rw-r--r--   0 runner    (1001) docker     (122)     1638 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/icons/cluster-analysis.png
--rw-r--r--   0 runner    (1001) docker     (122)     1809 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/icons/databases-update.png
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/icons/dicty-express.png
--rw-r--r--   0 runner    (1001) docker     (122)     1639 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/icons/differential-expression.png
--rw-r--r--   0 runner    (1001) docker     (122)     1719 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/icons/gene-set-enrichment.png
--rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/icons/genes.png
--rw-r--r--   0 runner    (1001) docker     (122)     1728 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/icons/geo-data-sets.png
--rw-r--r--   0 runner    (1001) docker     (122)     1943 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/icons/go-browser.png
--rw-r--r--   0 runner    (1001) docker     (122)     1750 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/icons/kegg-pathways.png
--rw-r--r--   0 runner    (1001) docker     (122)    13657 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/icons/volcano-plot.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.098359 Orange3-Bioinformatics-4.7.1/doc/widgets/images/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.110359 Orange3-Bioinformatics-4.7.1/doc/widgets/images/annotate_projection/
--rw-r--r--   0 runner    (1001) docker     (122)   499949 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/images/annotate_projection/annotator-example.png
--rw-r--r--   0 runner    (1001) docker     (122)   220708 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/images/annotate_projection/annotator-example2.png
--rw-r--r--   0 runner    (1001) docker     (122)   291477 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/images/annotate_projection/annotator-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.110359 Orange3-Bioinformatics-4.7.1/doc/widgets/images/cluster_analysis/
--rw-r--r--   0 runner    (1001) docker     (122)    50174 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/images/cluster_analysis/Cluster-Analysis-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.110359 Orange3-Bioinformatics-4.7.1/doc/widgets/images/database_update/
--rw-r--r--   0 runner    (1001) docker     (122)     8208 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/images/database_update/Add-Dataset.png
--rw-r--r--   0 runner    (1001) docker     (122)    18674 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/images/database_update/Databases-Update-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.110359 Orange3-Bioinformatics-4.7.1/doc/widgets/images/dicty_express/
--rw-r--r--   0 runner    (1001) docker     (122)   168071 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/images/dicty_express/dictyExpress-Example.png
--rw-r--r--   0 runner    (1001) docker     (122)    50069 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/images/dicty_express/dictyExpress-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.110359 Orange3-Bioinformatics-4.7.1/doc/widgets/images/differential_expression/
--rw-r--r--   0 runner    (1001) docker     (122)   176490 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/images/differential_expression/Differential-Expression-Example.png
--rw-r--r--   0 runner    (1001) docker     (122)    30207 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/images/differential_expression/Differential-Expression-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.110359 Orange3-Bioinformatics-4.7.1/doc/widgets/images/gene_set_enrichment/
--rw-r--r--   0 runner    (1001) docker     (122)    82620 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/images/gene_set_enrichment/Gene-Set-Enrichment-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.110359 Orange3-Bioinformatics-4.7.1/doc/widgets/images/genes/
--rw-r--r--   0 runner    (1001) docker     (122)   203400 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/images/genes/genes-Example.png
--rw-r--r--   0 runner    (1001) docker     (122)    57611 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/images/genes/genes-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.114359 Orange3-Bioinformatics-4.7.1/doc/widgets/images/geo_data_sets/
--rw-r--r--   0 runner    (1001) docker     (122)   195727 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/images/geo_data_sets/GEO-Data-Sets-Example.png
--rw-r--r--   0 runner    (1001) docker     (122)    36407 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/images/geo_data_sets/GEO-Data-Sets-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.114359 Orange3-Bioinformatics-4.7.1/doc/widgets/images/go_browser/
--rw-r--r--   0 runner    (1001) docker     (122)    24895 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/images/go_browser/Filter-Select.png
--rw-r--r--   0 runner    (1001) docker     (122)   270407 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/images/go_browser/GO-Browser-Example.png
--rw-r--r--   0 runner    (1001) docker     (122)    72500 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/images/go_browser/GO-Browser-stamped.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.114359 Orange3-Bioinformatics-4.7.1/doc/widgets/images/kegg_pathways/
--rw-r--r--   0 runner    (1001) docker     (122)   175266 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/images/kegg_pathways/KEGG-Pathways-Example.png
--rw-r--r--   0 runner    (1001) docker     (122)    51393 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/images/kegg_pathways/KEGG-Pathways-stamped.png
--rw-r--r--   0 runner    (1001) docker     (122)     1911 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/kegg_pathways.md
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/marker_genes.md
--rw-r--r--   0 runner    (1001) docker     (122)      866 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets/volcano_plot.md
--rw-r--r--   0 runner    (1001) docker     (122)     3186 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets.json
--rw-r--r--   0 runner    (1001) docker     (122)      361 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/doc/widgets.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.114359 Orange3-Bioinformatics-4.7.1/orangecontrib/
--rwxr-xr-x   0 runner    (1001) docker     (122)      164 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.114359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/
--rwxr-xr-x   0 runner    (1001) docker     (122)      252 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.114359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/annotation/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23225 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/annotation/annotate_projection.py
--rw-r--r--   0 runner    (1001) docker     (122)     9509 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/annotation/annotate_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.114359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/cluster_analysis/
--rw-r--r--   0 runner    (1001) docker     (122)    13553 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/cluster_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.114359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/dicty/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/dicty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4383 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/dicty/phenotypes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.114359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/geneset/
--rw-r--r--   0 runner    (1001) docker     (122)     1897 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/geneset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8982 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/geneset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.114359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/geo/
--rwxr-xr-x   0 runner    (1001) docker     (122)     4264 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/geo/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.114359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/go/
--rw-r--r--   0 runner    (1001) docker     (122)    27098 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/go/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      360 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/go/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.118359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/
--rw-r--r--   0 runner    (1001) docker     (122)    12217 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21289 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2452 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/brite.py
--rw-r--r--   0 runner    (1001) docker     (122)     8347 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/caching.py
--rw-r--r--   0 runner    (1001) docker     (122)      950 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)    17989 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.118359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/entry/
--rw-r--r--   0 runner    (1001) docker     (122)     5021 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/entry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5564 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/entry/fields.py
--rw-r--r--   0 runner    (1001) docker     (122)     4913 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/entry/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     8795 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/pathway.py
--rw-r--r--   0 runner    (1001) docker     (122)      792 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/service.py
--rw-r--r--   0 runner    (1001) docker     (122)     2912 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.118359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/ncbi/
--rwxr-xr-x   0 runner    (1001) docker     (122)       61 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/ncbi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.118359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/ncbi/gene/
--rwxr-xr-x   0 runner    (1001) docker     (122)    14176 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/ncbi/gene/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1654 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/ncbi/gene/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.118359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/ncbi/homologene/
--rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/ncbi/homologene/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.118359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/ncbi/taxonomy/
--rwxr-xr-x   0 runner    (1001) docker     (122)     4487 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/ncbi/taxonomy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    11321 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/ncbi/taxonomy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.118359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/preprocess/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2314 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/preprocess/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.118359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/resolwe/
--rwxr-xr-x   0 runner    (1001) docker     (122)     1061 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/resolwe/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3335 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/resolwe/genapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     3051 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/resolwe/resapi.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2143 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/resolwe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.118359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.118359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/annotation/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15903 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/annotation/test_annotate_projection.py
--rw-r--r--   0 runner    (1001) docker     (122)    14010 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/annotation/test_annotate_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.122359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/kegg/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/kegg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3065 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/kegg/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     2849 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/kegg/test_databases.py
--rw-r--r--   0 runner    (1001) docker     (122)     1741 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/kegg/test_entry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.122359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/ncbi/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/ncbi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3710 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/ncbi/test_gene.py
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/ncbi/test_homologene.py
--rw-r--r--   0 runner    (1001) docker     (122)     3488 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/ncbi/test_taxonomy.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.122359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/preprocess/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/preprocess/test_normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.122359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/resolwe/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/resolwe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/resolwe/test_genapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     3195 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/test_geneset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/test_geo.py
--rw-r--r--   0 runner    (1001) docker     (122)     4060 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/test_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.122359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1825 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/utils/test_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.122359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.122359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/components/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6181 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/components/test_gene_set_selection.py
--rw-r--r--   0 runner    (1001) docker     (122)     8052 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/components/test_resolwe.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.122359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/data/
--rw-r--r--   0 runner    (1001) docker     (122)     3828 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/data/genes.tab
--rw-r--r--   0 runner    (1001) docker     (122)    12006 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/data/markers-panglao.pkl
--rw-r--r--   0 runner    (1001) docker     (122)    16094 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/test_OWAnnotateProjection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/test_OWDifferentialExpression.py
--rw-r--r--   0 runner    (1001) docker     (122)     2443 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/test_OWGEODatasets.py
--rw-r--r--   0 runner    (1001) docker     (122)     2986 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/test_OWGeneSets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3901 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/test_OWGenes.py
--rw-r--r--   0 runner    (1001) docker     (122)     6113 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/test_OWGenialisExpressions.py
--rw-r--r--   0 runner    (1001) docker     (122)     3033 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/test_OWHomologs.py
--rw-r--r--   0 runner    (1001) docker     (122)    27756 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/test_OWMarkerGenes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.122359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/utils/
--rwxr-xr-x   0 runner    (1001) docker     (122)      542 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1604 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/utils/serverfiles.py
--rw-r--r--   0 runner    (1001) docker     (122)    11389 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/utils/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.126359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)    35390 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWAnnotateProjection.py
--rw-r--r--   0 runner    (1001) docker     (122)    31776 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWClusterAnalysis.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    31402 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWDatabasesUpdate.py
--rw-r--r--   0 runner    (1001) docker     (122)    45948 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWDifferentialExpression.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    19939 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWGEODatasets.py
--rw-r--r--   0 runner    (1001) docker     (122)    39734 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWGOBrowser.py
--rw-r--r--   0 runner    (1001) docker     (122)    20694 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWGeneSetEnrichment.py
--rw-r--r--   0 runner    (1001) docker     (122)    13364 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWGeneSets.py
--rw-r--r--   0 runner    (1001) docker     (122)    23000 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWGenes.py
--rw-r--r--   0 runner    (1001) docker     (122)    25847 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWGenialisExpressions.py
--rw-r--r--   0 runner    (1001) docker     (122)     9003 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWHomologs.py
--rw-r--r--   0 runner    (1001) docker     (122)    30488 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWKEGGPathwayBrowser.py
--rw-r--r--   0 runner    (1001) docker     (122)    41505 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWMarkerGenes.py
--rw-r--r--   0 runner    (1001) docker     (122)     4900 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWSingleSampleScoring.py
--rw-r--r--   0 runner    (1001) docker     (122)     5532 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWVolcanoPlot.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    10659 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWdictyExpress.py
--rw-r--r--   0 runner    (1001) docker     (122)      698 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.126359 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/components/
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10796 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/components/gene_set_selection.py
--rw-r--r--   0 runner    (1001) docker     (122)    17254 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/components/resolwe.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.142360 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/
--rwxr-xr-x   0 runner    (1001) docker     (122)     1302 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/Category-Bioinformatics.svg
--rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWAnnotateProjection.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWClusterAnalysis.svg
--rwxr-xr-x   0 runner    (1001) docker     (122)     2519 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWDatabasesUpdate.svg
--rw-r--r--   0 runner    (1001) docker     (122)      954 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWDifferentialExpression.svg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1960 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWGEODatasets.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1659 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWGOBrowser.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWGeneInfo.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1971 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWGeneSetEnrichment.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWGeneSets.svg
--rw-r--r--   0 runner    (1001) docker     (122)     2486 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWGenialisExpressions.svg
--rw-r--r--   0 runner    (1001) docker     (122)      829 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWHomologs.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1980 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWKEGGPathwayBrowser.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWMarkerGenes.svg
--rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWSingleSampleScoring.svg
--rw-r--r--   0 runner    (1001) docker     (122)     2154 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWVolcanoPlot.svg
--rwxr-xr-x   0 runner    (1001) docker     (122) 12157657 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWdictyExpress.png
--rw-r--r--   0 runner    (1001) docker     (122)     2864 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWdictyExpress.svg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.146360 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1217 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/concurrent.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4121 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-06 14:56:55.146360 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/gui/
--rw-r--r--   0 runner    (1001) docker     (122)     4961 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3474 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/gui/gene_scoring.py
--rw-r--r--   0 runner    (1001) docker     (122)     7267 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/gui/gene_sets.py
--rw-r--r--   0 runner    (1001) docker     (122)    13406 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/gui/label_selection.py
--rw-r--r--   0 runner    (1001) docker     (122)     5722 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/gui/list_completer.py
--rw-r--r--   0 runner    (1001) docker     (122)      567 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/itemdelegates.py
--rw-r--r--   0 runner    (1001) docker     (122)     2862 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/itemmodels.py
--rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)      710 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      235 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2244 2023-02-06 14:56:55.146360 Orange3-Bioinformatics-4.7.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     1236 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-02-06 14:56:42.000000 Orange3-Bioinformatics-4.7.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.046179 Orange3-Bioinformatics-4.7.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:48.986179 Orange3-Bioinformatics-4.7.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:48.986179 Orange3-Bioinformatics-4.7.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)      723 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rwxr-xr-x   0 runner    (1001) docker     (122)      217 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:48.986179 Orange3-Bioinformatics-4.7.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/.github/workflows/rebase.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1838 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      184 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/.github/workflows/test.yml
+-rwxr-xr-x   0 runner    (1001) docker     (122)      755 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     7749 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3348 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:48.986179 Orange3-Bioinformatics-4.7.2/Orange3_Bioinformatics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2084 2023-07-06 19:42:48.000000 Orange3-Bioinformatics-4.7.2/Orange3_Bioinformatics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10746 2023-07-06 19:42:48.000000 Orange3-Bioinformatics-4.7.2/Orange3_Bioinformatics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 19:42:48.000000 Orange3-Bioinformatics-4.7.2/Orange3_Bioinformatics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      223 2023-07-06 19:42:48.000000 Orange3-Bioinformatics-4.7.2/Orange3_Bioinformatics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-07-06 19:42:48.000000 Orange3-Bioinformatics-4.7.2/Orange3_Bioinformatics.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-06 19:42:48.000000 Orange3-Bioinformatics-4.7.2/Orange3_Bioinformatics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      358 2023-07-06 19:42:48.000000 Orange3-Bioinformatics-4.7.2/Orange3_Bioinformatics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-07-06 19:42:48.000000 Orange3-Bioinformatics-4.7.2/Orange3_Bioinformatics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2084 2023-07-06 19:42:49.046179 Orange3-Bioinformatics-4.7.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2707 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      728 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/README.pypi
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:48.990179 Orange3-Bioinformatics-4.7.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (122)     7464 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:48.990179 Orange3-Bioinformatics-4.7.2/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)     1302 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/_static/bioinformatics-sidebar-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:48.990179 Orange3-Bioinformatics-4.7.2/doc/_templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/_templates/about.html
+-rw-r--r--   0 runner    (1001) docker     (122)      333 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/_templates/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/_templates/useful_links.html
+-rw-r--r--   0 runner    (1001) docker     (122)    10329 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/contents.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2319 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7009 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)      439 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/scripting_reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:48.990179 Orange3-Bioinformatics-4.7.2/doc/scripting_references/
+-rw-r--r--   0 runner    (1001) docker     (122)      309 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/scripting_references/annotation.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:48.978179 Orange3-Bioinformatics-4.7.2/doc/scripting_references/code/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:48.994179 Orange3-Bioinformatics-4.7.2/doc/scripting_references/code/geo/
+-rw-r--r--   0 runner    (1001) docker     (122)      705 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/scripting_references/code/geo/dataset_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/scripting_references/code/geo/dataset_samples.py
+-rw-r--r--   0 runner    (1001) docker     (122)      553 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/scripting_references/code/geo/predict_disease_state.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:48.994179 Orange3-Bioinformatics-4.7.2/doc/scripting_references/code/go/
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/scripting_references/code/go/enrichment.py
+-rw-r--r--   0 runner    (1001) docker     (122)      823 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/scripting_references/code/go/gene_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/scripting_references/dicty_phenotypes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      965 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/scripting_references/geneset.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4033 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/scripting_references/geo.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2086 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/scripting_references/go.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/scripting_references/kegg.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/scripting_references/marker_genes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2660 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/scripting_references/ncbi_gene.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2180 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/scripting_references/ncbi_taxonomy.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/scripting_references/resolwe.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3949 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/scripting_references/serverfiles.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:48.994179 Orange3-Bioinformatics-4.7.2/doc/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)     4768 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/annotate_projection.md
+-rw-r--r--   0 runner    (1001) docker     (122)      633 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/cluster_analysis.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1399 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/databases_update.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/dicty_express.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3953 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/differential_expression.md
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/gene_set_enrichment.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1564 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/genes.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/geo_data_sets.md
+-rw-r--r--   0 runner    (1001) docker     (122)     5027 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/go_browser.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:48.998179 Orange3-Bioinformatics-4.7.2/doc/widgets/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)    35120 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/icons/annotator.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1638 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/icons/cluster-analysis.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1809 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/icons/databases-update.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/icons/dicty-express.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1639 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/icons/differential-expression.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1719 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/icons/gene-set-enrichment.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1640 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/icons/genes.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1728 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/icons/geo-data-sets.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1943 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/icons/go-browser.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1750 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/icons/kegg-pathways.png
+-rw-r--r--   0 runner    (1001) docker     (122)    13657 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/icons/volcano-plot.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:48.978179 Orange3-Bioinformatics-4.7.2/doc/widgets/images/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:48.998179 Orange3-Bioinformatics-4.7.2/doc/widgets/images/annotate_projection/
+-rw-r--r--   0 runner    (1001) docker     (122)   499949 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/images/annotate_projection/annotator-example.png
+-rw-r--r--   0 runner    (1001) docker     (122)   220708 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/images/annotate_projection/annotator-example2.png
+-rw-r--r--   0 runner    (1001) docker     (122)   291477 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/images/annotate_projection/annotator-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:48.998179 Orange3-Bioinformatics-4.7.2/doc/widgets/images/cluster_analysis/
+-rw-r--r--   0 runner    (1001) docker     (122)    50174 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/images/cluster_analysis/Cluster-Analysis-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:48.998179 Orange3-Bioinformatics-4.7.2/doc/widgets/images/database_update/
+-rw-r--r--   0 runner    (1001) docker     (122)     8208 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/images/database_update/Add-Dataset.png
+-rw-r--r--   0 runner    (1001) docker     (122)    18674 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/images/database_update/Databases-Update-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.002179 Orange3-Bioinformatics-4.7.2/doc/widgets/images/dicty_express/
+-rw-r--r--   0 runner    (1001) docker     (122)   168071 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/images/dicty_express/dictyExpress-Example.png
+-rw-r--r--   0 runner    (1001) docker     (122)    50069 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/images/dicty_express/dictyExpress-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.002179 Orange3-Bioinformatics-4.7.2/doc/widgets/images/differential_expression/
+-rw-r--r--   0 runner    (1001) docker     (122)   176490 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/images/differential_expression/Differential-Expression-Example.png
+-rw-r--r--   0 runner    (1001) docker     (122)    30207 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/images/differential_expression/Differential-Expression-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.002179 Orange3-Bioinformatics-4.7.2/doc/widgets/images/gene_set_enrichment/
+-rw-r--r--   0 runner    (1001) docker     (122)    82620 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/images/gene_set_enrichment/Gene-Set-Enrichment-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.002179 Orange3-Bioinformatics-4.7.2/doc/widgets/images/genes/
+-rw-r--r--   0 runner    (1001) docker     (122)   203400 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/images/genes/genes-Example.png
+-rw-r--r--   0 runner    (1001) docker     (122)    57611 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/images/genes/genes-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.002179 Orange3-Bioinformatics-4.7.2/doc/widgets/images/geo_data_sets/
+-rw-r--r--   0 runner    (1001) docker     (122)   195727 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/images/geo_data_sets/GEO-Data-Sets-Example.png
+-rw-r--r--   0 runner    (1001) docker     (122)    36407 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/images/geo_data_sets/GEO-Data-Sets-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.002179 Orange3-Bioinformatics-4.7.2/doc/widgets/images/go_browser/
+-rw-r--r--   0 runner    (1001) docker     (122)    24895 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/images/go_browser/Filter-Select.png
+-rw-r--r--   0 runner    (1001) docker     (122)   270407 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/images/go_browser/GO-Browser-Example.png
+-rw-r--r--   0 runner    (1001) docker     (122)    72500 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/images/go_browser/GO-Browser-stamped.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.006179 Orange3-Bioinformatics-4.7.2/doc/widgets/images/kegg_pathways/
+-rw-r--r--   0 runner    (1001) docker     (122)   175266 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/images/kegg_pathways/KEGG-Pathways-Example.png
+-rw-r--r--   0 runner    (1001) docker     (122)    51393 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/images/kegg_pathways/KEGG-Pathways-stamped.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1911 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/kegg_pathways.md
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/marker_genes.md
+-rw-r--r--   0 runner    (1001) docker     (122)      866 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets/volcano_plot.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3186 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets.json
+-rw-r--r--   0 runner    (1001) docker     (122)      361 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/doc/widgets.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.006179 Orange3-Bioinformatics-4.7.2/orangecontrib/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      164 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.006179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      252 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.006179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/annotation/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23225 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/annotation/annotate_projection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9509 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/annotation/annotate_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.006179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/cluster_analysis/
+-rw-r--r--   0 runner    (1001) docker     (122)    13553 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/cluster_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.006179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/dicty/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/dicty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4383 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/dicty/phenotypes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.006179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/geneset/
+-rw-r--r--   0 runner    (1001) docker     (122)     1897 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/geneset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8982 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/geneset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.006179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/geo/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4264 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1664 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/geo/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.006179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/go/
+-rw-r--r--   0 runner    (1001) docker     (122)    27098 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/go/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/go/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.010179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/
+-rw-r--r--   0 runner    (1001) docker     (122)    12217 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21289 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2452 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/brite.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8347 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/caching.py
+-rw-r--r--   0 runner    (1001) docker     (122)      950 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17989 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.010179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/entry/
+-rw-r--r--   0 runner    (1001) docker     (122)     5021 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/entry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5564 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/entry/fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4913 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/entry/parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8795 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/pathway.py
+-rw-r--r--   0 runner    (1001) docker     (122)      792 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/service.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2912 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.010179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/ncbi/
+-rwxr-xr-x   0 runner    (1001) docker     (122)       61 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/ncbi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.010179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/ncbi/gene/
+-rwxr-xr-x   0 runner    (1001) docker     (122)    14176 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/ncbi/gene/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1654 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/ncbi/gene/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.010179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/ncbi/homologene/
+-rw-r--r--   0 runner    (1001) docker     (122)     2093 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/ncbi/homologene/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.010179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/ncbi/taxonomy/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4487 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/ncbi/taxonomy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    11321 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/ncbi/taxonomy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.010179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2314 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/preprocess/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.014179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/resolwe/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1061 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/resolwe/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3335 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/resolwe/genapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3051 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/resolwe/resapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2134 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/resolwe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.014179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.014179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/annotation/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15903 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/annotation/test_annotate_projection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14010 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/annotation/test_annotate_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.014179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/kegg/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/kegg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3065 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/kegg/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2849 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/kegg/test_databases.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1741 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/kegg/test_entry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.018179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/ncbi/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/ncbi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3710 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/ncbi/test_gene.py
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/ncbi/test_homologene.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3488 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/ncbi/test_taxonomy.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.018179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1626 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/preprocess/test_normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.018179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/resolwe/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/resolwe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/resolwe/test_genapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3195 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/test_geneset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/test_geo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4060 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/test_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.018179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1825 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/utils/test_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.018179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.018179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/components/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6181 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/components/test_gene_set_selection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8052 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/components/test_resolwe.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.022179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/data/
+-rw-r--r--   0 runner    (1001) docker     (122)     3828 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/data/genes.tab
+-rw-r--r--   0 runner    (1001) docker     (122)    12006 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/data/markers-panglao.pkl
+-rw-r--r--   0 runner    (1001) docker     (122)    16094 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/test_OWAnnotateProjection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/test_OWDifferentialExpression.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2443 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/test_OWGEODatasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2986 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/test_OWGeneSets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3901 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/test_OWGenes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6113 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/test_OWGenialisExpressions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3033 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/test_OWHomologs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27756 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/test_OWMarkerGenes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.022179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      542 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1604 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/utils/serverfiles.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11389 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/utils/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.026179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)    35390 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWAnnotateProjection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31776 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWClusterAnalysis.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    31402 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWDatabasesUpdate.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45948 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWDifferentialExpression.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    19939 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWGEODatasets.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39734 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWGOBrowser.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20694 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWGeneSetEnrichment.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13364 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWGeneSets.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23000 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWGenes.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25847 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWGenialisExpressions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9003 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWHomologs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30488 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWKEGGPathwayBrowser.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41505 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWMarkerGenes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4900 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWSingleSampleScoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5532 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWVolcanoPlot.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10659 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWdictyExpress.py
+-rw-r--r--   0 runner    (1001) docker     (122)      698 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.026179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/components/
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10796 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/components/gene_set_selection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17254 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/components/resolwe.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.046179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1302 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/Category-Bioinformatics.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     4230 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWAnnotateProjection.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWClusterAnalysis.svg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2519 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWDatabasesUpdate.svg
+-rw-r--r--   0 runner    (1001) docker     (122)      954 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWDifferentialExpression.svg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1960 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWGEODatasets.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1659 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWGOBrowser.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1147 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWGeneInfo.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1971 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWGeneSetEnrichment.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1189 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWGeneSets.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     2486 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWGenialisExpressions.svg
+-rw-r--r--   0 runner    (1001) docker     (122)      829 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWHomologs.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1980 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWKEGGPathwayBrowser.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWMarkerGenes.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     1023 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWSingleSampleScoring.svg
+-rw-r--r--   0 runner    (1001) docker     (122)     2154 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWVolcanoPlot.svg
+-rwxr-xr-x   0 runner    (1001) docker     (122) 12157657 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWdictyExpress.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2864 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWdictyExpress.svg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.046179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1217 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/concurrent.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     4121 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-06 19:42:49.046179 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/gui/
+-rw-r--r--   0 runner    (1001) docker     (122)     4961 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3474 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/gui/gene_scoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7267 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/gui/gene_sets.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13406 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/gui/label_selection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5722 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/gui/list_completer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      567 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/itemdelegates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2862 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/itemmodels.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      710 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      235 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2244 2023-07-06 19:42:49.046179 Orange3-Bioinformatics-4.7.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1236 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1704 2023-07-06 19:42:35.000000 Orange3-Bioinformatics-4.7.2/tox.ini
```

### Comparing `Orange3-Bioinformatics-4.7.1/.github/FUNDING.yml` & `Orange3-Bioinformatics-4.7.2/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/.github/ISSUE_TEMPLATE/bug_report.md` & `Orange3-Bioinformatics-4.7.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/.github/ISSUE_TEMPLATE/feature_request.md` & `Orange3-Bioinformatics-4.7.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/.github/workflows/lint.yml` & `Orange3-Bioinformatics-4.7.2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/.github/workflows/release.yml` & `Orange3-Bioinformatics-4.7.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/.gitignore` & `Orange3-Bioinformatics-4.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/CHANGELOG.md` & `Orange3-Bioinformatics-4.7.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [4.7.2] - 2023-07-06
+### Changed
+- [#335](https://github.com/biolab/orange3-bioinformatics/pull/335):  Time is now column name for Dicty express data
+- 
 ## [4.7.1] - 2023-02-06
 
 ## [4.7.0] - 2023-02-06
 
 ## [4.6.0] - 2022-11-24
 ### Changed
 - [#311](https://github.com/biolab/orange3-bioinformatics/pull/311):  Add QC data to Genialis Expression widget
```

### Comparing `Orange3-Bioinformatics-4.7.1/CODE_OF_CONDUCT.md` & `Orange3-Bioinformatics-4.7.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/LICENSE` & `Orange3-Bioinformatics-4.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/Orange3_Bioinformatics.egg-info/PKG-INFO` & `Orange3-Bioinformatics-4.7.2/Orange3_Bioinformatics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orange3-Bioinformatics
-Version: 4.7.1
+Version: 4.7.2
 Summary: Orange Bioinformatics add-on for Orange data mining software package.
 Home-page: https://github.com/biolab/orange3-bioinformatics
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: info@biolab.si
 Maintainer: Jaka Kokosar
 License: GPL3+
 Project-URL: Bug Tracker, https://github.com/biolab/orange3-bioinformatics/issues
```

### Comparing `Orange3-Bioinformatics-4.7.1/Orange3_Bioinformatics.egg-info/SOURCES.txt` & `Orange3-Bioinformatics-4.7.2/Orange3_Bioinformatics.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 setup.py
 tox.ini
 .github/FUNDING.yml
 .github/PULL_REQUEST_TEMPLATE.md
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/lint.yml
+.github/workflows/rebase.yml
 .github/workflows/release.yml
 .github/workflows/test.yml
 Orange3_Bioinformatics.egg-info/PKG-INFO
 Orange3_Bioinformatics.egg-info/SOURCES.txt
 Orange3_Bioinformatics.egg-info/dependency_links.txt
 Orange3_Bioinformatics.egg-info/entry_points.txt
 Orange3_Bioinformatics.egg-info/namespace_packages.txt
```

### Comparing `Orange3-Bioinformatics-4.7.1/PKG-INFO` & `Orange3-Bioinformatics-4.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Orange3-Bioinformatics
-Version: 4.7.1
+Version: 4.7.2
 Summary: Orange Bioinformatics add-on for Orange data mining software package.
 Home-page: https://github.com/biolab/orange3-bioinformatics
 Author: Bioinformatics Laboratory, FRI UL
 Author-email: info@biolab.si
 Maintainer: Jaka Kokosar
 License: GPL3+
 Project-URL: Bug Tracker, https://github.com/biolab/orange3-bioinformatics/issues
```

### Comparing `Orange3-Bioinformatics-4.7.1/README.md` & `Orange3-Bioinformatics-4.7.2/README.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/README.pypi` & `Orange3-Bioinformatics-4.7.2/README.pypi`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/Makefile` & `Orange3-Bioinformatics-4.7.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/_static/bioinformatics-sidebar-logo.svg` & `Orange3-Bioinformatics-4.7.2/doc/_static/bioinformatics-sidebar-logo.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/_static/custom.css` & `Orange3-Bioinformatics-4.7.2/doc/_static/custom.css`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/conf.py` & `Orange3-Bioinformatics-4.7.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/index.rst` & `Orange3-Bioinformatics-4.7.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/make.bat` & `Orange3-Bioinformatics-4.7.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/scripting_references/code/geo/dataset_info.py` & `Orange3-Bioinformatics-4.7.2/doc/scripting_references/code/geo/dataset_info.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/scripting_references/code/geo/dataset_samples.py` & `Orange3-Bioinformatics-4.7.2/doc/scripting_references/code/geo/dataset_samples.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/scripting_references/code/geo/predict_disease_state.py` & `Orange3-Bioinformatics-4.7.2/doc/scripting_references/code/geo/predict_disease_state.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/scripting_references/code/go/enrichment.py` & `Orange3-Bioinformatics-4.7.2/doc/scripting_references/code/go/enrichment.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/scripting_references/code/go/gene_annotations.py` & `Orange3-Bioinformatics-4.7.2/doc/scripting_references/code/go/gene_annotations.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/scripting_references/dicty_phenotypes.rst` & `Orange3-Bioinformatics-4.7.2/doc/scripting_references/dicty_phenotypes.rst`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/scripting_references/geneset.rst` & `Orange3-Bioinformatics-4.7.2/doc/scripting_references/geneset.rst`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/scripting_references/geo.rst` & `Orange3-Bioinformatics-4.7.2/doc/scripting_references/geo.rst`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/scripting_references/go.rst` & `Orange3-Bioinformatics-4.7.2/doc/scripting_references/go.rst`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/scripting_references/kegg.rst` & `Orange3-Bioinformatics-4.7.2/doc/scripting_references/kegg.rst`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/scripting_references/marker_genes.rst` & `Orange3-Bioinformatics-4.7.2/doc/scripting_references/marker_genes.rst`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/scripting_references/ncbi_gene.rst` & `Orange3-Bioinformatics-4.7.2/doc/scripting_references/ncbi_gene.rst`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/scripting_references/ncbi_taxonomy.rst` & `Orange3-Bioinformatics-4.7.2/doc/scripting_references/ncbi_taxonomy.rst`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/scripting_references/serverfiles.rst` & `Orange3-Bioinformatics-4.7.2/doc/scripting_references/serverfiles.rst`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/annotate_projection.md` & `Orange3-Bioinformatics-4.7.2/doc/widgets/annotate_projection.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/cluster_analysis.md` & `Orange3-Bioinformatics-4.7.2/doc/widgets/cluster_analysis.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/databases_update.md` & `Orange3-Bioinformatics-4.7.2/doc/widgets/databases_update.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/dicty_express.md` & `Orange3-Bioinformatics-4.7.2/doc/widgets/dicty_express.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/differential_expression.md` & `Orange3-Bioinformatics-4.7.2/doc/widgets/differential_expression.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/gene_set_enrichment.md` & `Orange3-Bioinformatics-4.7.2/doc/widgets/gene_set_enrichment.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/genes.md` & `Orange3-Bioinformatics-4.7.2/doc/widgets/genes.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/geo_data_sets.md` & `Orange3-Bioinformatics-4.7.2/doc/widgets/geo_data_sets.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/go_browser.md` & `Orange3-Bioinformatics-4.7.2/doc/widgets/go_browser.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/icons/annotator.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/icons/annotator.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/icons/cluster-analysis.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/icons/cluster-analysis.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/icons/databases-update.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/icons/databases-update.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/icons/dicty-express.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/icons/dicty-express.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/icons/differential-expression.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/icons/differential-expression.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/icons/gene-set-enrichment.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/icons/gene-set-enrichment.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/icons/genes.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/icons/genes.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/icons/geo-data-sets.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/icons/geo-data-sets.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/icons/go-browser.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/icons/go-browser.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/icons/kegg-pathways.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/icons/kegg-pathways.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/icons/volcano-plot.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/icons/volcano-plot.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/images/annotate_projection/annotator-example.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/images/annotate_projection/annotator-example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/images/annotate_projection/annotator-example2.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/images/annotate_projection/annotator-example2.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/images/annotate_projection/annotator-stamped.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/images/annotate_projection/annotator-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/images/cluster_analysis/Cluster-Analysis-stamped.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/images/cluster_analysis/Cluster-Analysis-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/images/database_update/Add-Dataset.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/images/database_update/Add-Dataset.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/images/database_update/Databases-Update-stamped.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/images/database_update/Databases-Update-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/images/dicty_express/dictyExpress-Example.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/images/dicty_express/dictyExpress-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/images/dicty_express/dictyExpress-stamped.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/images/dicty_express/dictyExpress-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/images/differential_expression/Differential-Expression-Example.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/images/differential_expression/Differential-Expression-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/images/differential_expression/Differential-Expression-stamped.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/images/differential_expression/Differential-Expression-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/images/gene_set_enrichment/Gene-Set-Enrichment-stamped.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/images/gene_set_enrichment/Gene-Set-Enrichment-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/images/genes/genes-Example.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/images/genes/genes-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/images/genes/genes-stamped.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/images/genes/genes-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/images/geo_data_sets/GEO-Data-Sets-Example.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/images/geo_data_sets/GEO-Data-Sets-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/images/geo_data_sets/GEO-Data-Sets-stamped.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/images/geo_data_sets/GEO-Data-Sets-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/images/go_browser/Filter-Select.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/images/go_browser/Filter-Select.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/images/go_browser/GO-Browser-Example.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/images/go_browser/GO-Browser-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/images/go_browser/GO-Browser-stamped.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/images/go_browser/GO-Browser-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/images/kegg_pathways/KEGG-Pathways-Example.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/images/kegg_pathways/KEGG-Pathways-Example.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/images/kegg_pathways/KEGG-Pathways-stamped.png` & `Orange3-Bioinformatics-4.7.2/doc/widgets/images/kegg_pathways/KEGG-Pathways-stamped.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/kegg_pathways.md` & `Orange3-Bioinformatics-4.7.2/doc/widgets/kegg_pathways.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/marker_genes.md` & `Orange3-Bioinformatics-4.7.2/doc/widgets/marker_genes.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets/volcano_plot.md` & `Orange3-Bioinformatics-4.7.2/doc/widgets/volcano_plot.md`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/doc/widgets.json` & `Orange3-Bioinformatics-4.7.2/doc/widgets.json`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/annotation/annotate_projection.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/annotation/annotate_projection.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/annotation/annotate_samples.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/annotation/annotate_samples.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/cluster_analysis/__init__.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/cluster_analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/dicty/phenotypes.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/dicty/phenotypes.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/geneset/__init__.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/geneset/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/geneset/utils.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/geneset/utils.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/geo/__init__.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/geo/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/geo/dataset.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/geo/dataset.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/go/__init__.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/go/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/__init__.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/api.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/api.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/brite.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/brite.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/caching.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/caching.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/conf.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/conf.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/databases.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/databases.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/entry/__init__.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/entry/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/entry/fields.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/entry/fields.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/entry/parser.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/entry/parser.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/pathway.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/pathway.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/service.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/service.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/kegg/types.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/kegg/types.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/ncbi/gene/__init__.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/ncbi/gene/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/ncbi/gene/config.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/ncbi/gene/config.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/ncbi/homologene/__init__.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/ncbi/homologene/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/ncbi/taxonomy/__init__.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/ncbi/taxonomy/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/ncbi/taxonomy/utils.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/ncbi/taxonomy/utils.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/preprocess/normalize.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/preprocess/normalize.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/resolwe/__init__.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/resolwe/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/resolwe/genapi.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/resolwe/genapi.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/resolwe/resapi.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/resolwe/resapi.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/resolwe/utils.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/resolwe/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     Returns:
         :obj:`Orange.data.Table`
     """
 
     variables = []
     time_point = 1
     for time in etc_json['etc']['timePoints']:
-        var = ContinuousVariable('TP ' + str(time_point))
-        var.attributes['Time'] = str(time)
+        var = ContinuousVariable(str(time))
+        var.attributes['Time point'] = str(time_point)
         variables.append(var)
         time_point += 1
 
     meta_attr = StringVariable.make('Gene')
     domain = Domain(variables, metas=[meta_attr])
 
     table = []
@@ -50,15 +50,15 @@
         table.append(gene_expression)
 
     orange_table = Table.from_list(domain, table)
     if transpose:
         orange_table = Table.transpose(
             orange_table,
             feature_names_column=meta_attr.name,
-            meta_attr_name='Time Points',
+            meta_attr_name='Time',
             remove_redundant_inst=True,
         )
 
     return orange_table
 
 
 def response_to_json(response):
```

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/annotation/test_annotate_projection.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/annotation/test_annotate_projection.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/annotation/test_annotate_samples.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/annotation/test_annotate_samples.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/kegg/test_api.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/kegg/test_api.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/kegg/test_databases.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/kegg/test_databases.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/kegg/test_entry.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/kegg/test_entry.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/ncbi/test_gene.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/ncbi/test_gene.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/ncbi/test_homologene.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/ncbi/test_homologene.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/ncbi/test_taxonomy.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/ncbi/test_taxonomy.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/preprocess/test_normalize.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/preprocess/test_normalize.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/resolwe/test_genapi.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/resolwe/test_genapi.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/test_geneset.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/test_geneset.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/test_geo.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/test_geo.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/test_statistics.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/utils/test_gui.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/utils/test_gui.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/components/test_gene_set_selection.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/components/test_gene_set_selection.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/components/test_resolwe.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/components/test_resolwe.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/data/genes.tab` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/data/genes.tab`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/data/markers-panglao.pkl` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/data/markers-panglao.pkl`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/test_OWAnnotateProjection.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/test_OWAnnotateProjection.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/test_OWDifferentialExpression.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/test_OWDifferentialExpression.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/test_OWGEODatasets.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/test_OWGEODatasets.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/test_OWGeneSets.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/test_OWGeneSets.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/test_OWGenes.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/test_OWGenes.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/test_OWGenialisExpressions.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/test_OWGenialisExpressions.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/test_OWHomologs.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/test_OWHomologs.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/tests/widgets/test_OWMarkerGenes.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/tests/widgets/test_OWMarkerGenes.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/utils/__init__.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/utils/serverfiles.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/utils/serverfiles.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/utils/statistics.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWAnnotateProjection.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWAnnotateProjection.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWClusterAnalysis.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWClusterAnalysis.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWDatabasesUpdate.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWDatabasesUpdate.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWDifferentialExpression.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWDifferentialExpression.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWGEODatasets.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWGEODatasets.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWGOBrowser.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWGOBrowser.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWGeneSetEnrichment.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWGeneSetEnrichment.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWGeneSets.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWGeneSets.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWGenes.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWGenes.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWGenialisExpressions.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWGenialisExpressions.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWHomologs.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWHomologs.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWKEGGPathwayBrowser.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWKEGGPathwayBrowser.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWMarkerGenes.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWMarkerGenes.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWSingleSampleScoring.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWSingleSampleScoring.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWVolcanoPlot.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWVolcanoPlot.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/OWdictyExpress.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/OWdictyExpress.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/__init__.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/components/gene_set_selection.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/components/gene_set_selection.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/components/resolwe.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/components/resolwe.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/Category-Bioinformatics.svg` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/Category-Bioinformatics.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWAnnotateProjection.svg` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWAnnotateProjection.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWClusterAnalysis.svg` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWClusterAnalysis.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWDatabasesUpdate.svg` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWDatabasesUpdate.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWDifferentialExpression.svg` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWDifferentialExpression.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWGEODatasets.svg` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWGEODatasets.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWGOBrowser.svg` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWGOBrowser.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWGeneInfo.svg` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWGeneInfo.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWGeneSetEnrichment.svg` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWGeneSetEnrichment.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWGeneSets.svg` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWGeneSets.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWGenialisExpressions.svg` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWGenialisExpressions.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWHomologs.svg` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWHomologs.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWKEGGPathwayBrowser.svg` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWKEGGPathwayBrowser.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWMarkerGenes.svg` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWMarkerGenes.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWSingleSampleScoring.svg` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWSingleSampleScoring.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWVolcanoPlot.svg` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWVolcanoPlot.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWdictyExpress.png` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWdictyExpress.png`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/icons/OWdictyExpress.svg` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/icons/OWdictyExpress.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/__init__.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/concurrent.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/data.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/data.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/gui/__init__.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/gui/gene_scoring.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/gui/gene_scoring.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/gui/gene_sets.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/gui/gene_sets.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/gui/label_selection.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/gui/label_selection.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/gui/list_completer.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/gui/list_completer.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/itemdelegates.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/itemdelegates.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/itemmodels.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/itemmodels.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/orangecontrib/bioinformatics/widgets/utils/settings.py` & `Orange3-Bioinformatics-4.7.2/orangecontrib/bioinformatics/widgets/utils/settings.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/pyproject.toml` & `Orange3-Bioinformatics-4.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/setup.cfg` & `Orange3-Bioinformatics-4.7.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/setup.py` & `Orange3-Bioinformatics-4.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `Orange3-Bioinformatics-4.7.1/tox.ini` & `Orange3-Bioinformatics-4.7.2/tox.ini`

 * *Files identical despite different names*

