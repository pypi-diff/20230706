# Comparing `tmp/tosca-parser-2.8.0.tar.gz` & `tmp/tosca-parser-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tosca-parser-2.8.0.tar", last modified: Mon Feb 13 16:03:26 2023, max compression
+gzip compressed data, was "tosca-parser-2.9.0.tar", last modified: Thu Jul  6 09:03:37 2023, max compression
```

## Comparing `tosca-parser-2.8.0.tar` & `tosca-parser-2.9.0.tar`

### file list

```diff
@@ -1,422 +1,422 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.875359 tosca-parser-2.8.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4056 2023-02-13 16:03:26.000000 tosca-parser-2.8.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      624 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24310 2023-02-13 16:03:26.000000 tosca-parser-2.8.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3564 2023-02-13 16:03:26.875359 tosca-parser-2.8.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2097 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.807359 tosca-parser-2.8.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.811359 tosca-parser-2.8.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2423 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/doc/source/contributing.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.811359 tosca-parser-2.8.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1886 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1436 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      989 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/doc/source/usage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1306 2023-02-13 16:03:26.875359 tosca-parser-2.8.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.811359 tosca-parser-2.8.0/tosca_parser.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3564 2023-02-13 16:03:26.000000 tosca-parser-2.8.0/tosca_parser.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18884 2023-02-13 16:03:26.000000 tosca-parser-2.8.0/tosca_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-13 16:03:26.000000 tosca-parser-2.8.0/tosca_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2023-02-13 16:03:26.000000 tosca-parser-2.8.0/tosca_parser.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-13 16:03:26.000000 tosca-parser-2.8.0/tosca_parser.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-13 16:03:26.000000 tosca-parser-2.8.0/tosca_parser.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-02-13 16:03:26.000000 tosca-parser-2.8.0/tosca_parser.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-02-13 16:03:26.000000 tosca-parser-2.8.0/tosca_parser.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1154 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/tosca_parser.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.819359 tosca-parser-2.8.0/toscaparser/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      643 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1842 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/capabilities.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.819359 tosca-parser-2.8.0/toscaparser/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7566 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/common/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8188 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/dataentity.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.819359 tosca-parser-2.8.0/toscaparser/elements/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31479 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/elements/TOSCA_definition_1_0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/elements/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2050 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/elements/artifacttype.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/elements/attribute_definition.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4154 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/elements/capabilitytype.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22660 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/elements/constraints.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2208 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/elements/datatype.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6188 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/elements/entity_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3794 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/elements/grouptype.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3951 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/elements/interfaces.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9458 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/elements/nodetype.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5335 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/elements/policytype.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3797 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/elements/portspectype.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4042 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/elements/property_definition.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2673 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/elements/relationshiptype.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4788 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/elements/scalarunit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4045 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/elements/statefulentitytype.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2789 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/elements/tosca_type_validation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14802 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/entity_template.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.823359 tosca-parser-2.8.0/toscaparser/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/extensions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2537 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/extensions/exttools.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.823359 tosca-parser-2.8.0/toscaparser/extensions/mec/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5831 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/extensions/mec/TOSCA_mec_definition_1_0_0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/extensions/mec/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/extensions/mec/tosca_simple_profile_for_mec_1_0_0.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.823359 tosca-parser-2.8.0/toscaparser/extensions/nfv/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8415 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/extensions/nfv/TOSCA_nfv_definition_1_0_0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/extensions/nfv/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.799359 tosca-parser-2.8.0/toscaparser/extensions/nfv/tests/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.823359 tosca-parser-2.8.0/toscaparser/extensions/nfv/tests/data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      670 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/extensions/nfv/tests/data/tosca_helloworld_nfv.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      795 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/extensions/nfv/tosca_simple_profile_for_nfv_1_0_0.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38374 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/functions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2108 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13927 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/imports.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14498 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/nodetemplate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4271 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/parameters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3406 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/policy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.823359 tosca-parser-2.8.0/toscaparser/prereq/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/prereq/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17198 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/prereq/csar.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2442 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3189 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/relationship_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2347 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/repositories.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/reservation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3874 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10153 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/substitution_mappings.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.827359 tosca-parser-2.8.0/toscaparser/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.799359 tosca-parser-2.8.0/toscaparser/tests/artifacts/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.827359 tosca-parser-2.8.0/toscaparser/tests/artifacts/collectd/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      992 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/collectd/config.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      107 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/collectd/create.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      110 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/collectd/start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.827359 tosca-parser-2.8.0/toscaparser/tests/artifacts/elasticsearch/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      432 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/elasticsearch/create.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      125 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/elasticsearch/start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.827359 tosca-parser-2.8.0/toscaparser/tests/artifacts/kibana/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      362 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/kibana/config.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      464 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/kibana/create.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      106 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/kibana/start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.827359 tosca-parser-2.8.0/toscaparser/tests/artifacts/logstash/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1113 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/logstash/configure_collectd.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1000 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/logstash/configure_elasticsearch.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      905 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/logstash/configure_rsyslog.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      603 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/logstash/create.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)       93 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/logstash/start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.831359 tosca-parser-2.8.0/toscaparser/tests/artifacts/mongodb/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/mongodb/config.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/mongodb/create.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/mongodb/create_database.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/mongodb/start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.831359 tosca-parser-2.8.0/toscaparser/tests/artifacts/mysql/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      209 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/mysql/mysql_database_configure.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      183 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/mysql/mysql_dbms_configure.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      308 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/mysql/mysql_dbms_install.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)       33 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/mysql/mysql_dbms_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.831359 tosca-parser-2.8.0/toscaparser/tests/artifacts/nodejs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/nodejs/config.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/nodejs/create.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/nodejs/start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.831359 tosca-parser-2.8.0/toscaparser/tests/artifacts/rsyslog/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/rsyslog/config.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      124 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/rsyslog/create.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      108 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/rsyslog/start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.831359 tosca-parser-2.8.0/toscaparser/tests/artifacts/webserver/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)       92 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/webserver/webserver_install.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)       31 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/webserver/webserver_start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.831359 tosca-parser-2.8.0/toscaparser/tests/artifacts/wordpress/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      231 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/wordpress/wordpress_configure.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)       86 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/artifacts/wordpress/wordpress_install.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2353 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.839359 tosca-parser-2.8.0/toscaparser/tests/data/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.843359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17490 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_elk.csar
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17490 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_elk.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_hello_world.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_invalid_entry_def.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2300 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_invalid_multilevel_imports_validation.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_metadata_not_yaml.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_missing_metadata.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22194 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_multiple_deployment_flavour.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_no_metadata_file.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_not_zip.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17127 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_relative_path_import_check.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_root_level_yaml.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1662 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_root_level_yaml_and_tosca_metadata.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      478 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_root_yaml_with_tosca_definition1_0.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1004 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_two_root_level_yaml.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2239 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_valid_multilevel_imports_validation.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5967 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wordpress.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5985 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_artifact.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6265 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_artifact_multi.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5978 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_import_path.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6043 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_import_url.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5969 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_script_path.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6043 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_script_url.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5977 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wordpress_valid_artifact.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6260 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wordpress_valid_artifact_multi.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6046 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wordpress_with_url_import_and_script.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wrong_metadata_file.zip
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/multi_level_imports_response.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/root_level_file.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.843359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.847359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/collectd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/elasticsearch.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      567 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/kibana.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      877 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/logstash.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/paypalpizzastore_nodejs_app.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/rsyslog.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7103 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/tosca_elk.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.799359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Python/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.847359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Python/collectd/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      992 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Python/collectd/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.847359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Python/logstash/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1113 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Python/logstash/configure_collectd.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1000 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Python/logstash/configure_elasticsearch.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      905 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Python/logstash/configure_rsyslog.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1126 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/README.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.803359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.847359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/collectd/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      107 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/collectd/create.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      110 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/collectd/start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.847359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/elasticsearch/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      432 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/elasticsearch/create.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      125 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/elasticsearch/start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.847359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/kibana/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      362 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/kibana/config.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      464 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/kibana/create.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      106 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/kibana/start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.847359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/logstash/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      603 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/logstash/create.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)       93 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/logstash/start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.847359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/mongodb/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/mongodb/config.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/mongodb/create.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/mongodb/create_database.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/mongodb/start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.851359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/nodejs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      743 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/nodejs/config.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/nodejs/create.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/nodejs/start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.851359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/rsyslog/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/rsyslog/config.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      124 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/rsyslog/create.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      108 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/rsyslog/start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.851359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/TOSCA-Metadata/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/TOSCA-Metadata/TOSCA.meta
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_meta_file.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.851359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.851359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Definitions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3209 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Definitions/tosca_single_instance_wordpress.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Definitions/wordpress.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1147 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/README.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.803359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.851359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/MYSQLDBMS/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/MYSQLDBMS/configure.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/MYSQLDBMS/install.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/MYSQLDBMS/start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.851359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/MYSQLDatabase/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/MYSQLDatabase/configure.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.851359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/WebServer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/WebServer/install.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/WebServer/start.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.851359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/WordPress/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/WordPress/configure.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/WordPress/install.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.851359 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/TOSCA-Metadata/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/TOSCA-Metadata/TOSCA.meta
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.851359 tosca-parser-2.8.0/toscaparser/tests/data/containers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/containers/test_container_docker_mysql.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.859359 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/collectd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/compute_with_attribute_list.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      524 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/compute_with_nested_atributes.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/compute_with_prop.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      878 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/container_cap_child.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/custom_cap.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/custom_cap_with_datatype.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/custom_caps_def.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      424 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/custom_data_type.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/custom_interface.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      597 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/custom_nested_data_types.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/custom_policy.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/custom_relationship_type_defs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/db_with_list_param.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/elasticsearch.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/imported_sample.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/invalid_template_version.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      565 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/kibana.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      878 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/logstash.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/nested_rsyslog.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/nested_test_kibana.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      976 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/nested_test_wordpress.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/node_with_cap.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/paypalpizzastore_nodejs_app.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/rsyslog.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/template_metadata.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/wordpress.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/custom_types/wordpress.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.859359 tosca-parser-2.8.0/toscaparser/tests/data/datatypes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1188 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/datatypes/custom_datatype_def.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1666 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/datatypes/test_custom_datatypes_in_current_template.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/datatypes/test_custom_datatypes_nested_datatype_error.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      647 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/datatypes/test_custom_datatypes_positive.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/datatypes/test_custom_datatypes_value_error.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/datatypes/test_datatype_portspec_add_req.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.859359 tosca-parser-2.8.0/toscaparser/tests/data/dsl_definitions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/dsl_definitions/test_nested_dsl_def.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.863359 tosca-parser-2.8.0/toscaparser/tests/data/functions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_capabilties_inheritance.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_concat.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_concat_invalid.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      625 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_container_cap_child.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_attribute_custom_data_type.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      837 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_attribute_host_keyword.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_attribute_host_not_found.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_attribute_illegal_host_in_outputs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      887 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_attribute_nested_data_types.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_attribute_source_target_keywords.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_attribute_unknown_attribute_name.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_attribute_unknown_node_template_name.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_attribute_with_index.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_attribute_with_index_error.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      579 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_attribute_with_nested_params.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_implicit_attribute.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      787 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_prop_cap_bool.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_prop_cap_host.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_property_source_target_keywords.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1624 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_property_with_host.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_invalid_function_signature.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_token.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_token_invalid.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_unknown_capability_property.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_unknown_input_in_interface.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/test_unknown_input_in_property.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/functions/tosca_nested_property_names_indexes.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.863359 tosca-parser-2.8.0/toscaparser/tests/data/groups/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/groups/definitions.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1356 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/groups/tosca_group_template.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.863359 tosca-parser-2.8.0/toscaparser/tests/data/interfaces/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      622 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/interfaces/test_custom_interface_in_template.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/interfaces/test_custom_interface_invalid_operation.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.863359 tosca-parser-2.8.0/toscaparser/tests/data/load_balancer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2027 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/load_balancer/tosca_load_balancer.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.867359 tosca-parser-2.8.0/toscaparser/tests/data/node_filter/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/node_filter/test_node_filter.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.867359 tosca-parser-2.8.0/toscaparser/tests/data/policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/policies/custom_definitions.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4922 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/policies/tacker_defs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5741 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/policies/tacker_nfv_defs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2469 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/policies/test_policies_without_required_property.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2468 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/policies/test_tosca_nfv_multiple_policies.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1163 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/policies/tosca_custom_policy_template.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3251 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/policies/tosca_policy_template.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.867359 tosca-parser-2.8.0/toscaparser/tests/data/relationship/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1304 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/relationship/test_custom_relationship.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.867359 tosca-parser-2.8.0/toscaparser/tests/data/repositories/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/repositories/test_repositories_definition.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      879 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/repositories/tosca_repositories_test_definition.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.867359 tosca-parser-2.8.0/toscaparser/tests/data/requirements/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1905 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/requirements/test_requirements.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_attributes_inheritance.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_available_rel_tpls.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1004 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_capability_without_properties.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1759 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_credential_datatype.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_custom_capabilty.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_custom_caps_def.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_custom_caps_with_datatype.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_endpoint_on_compute.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_import_invalid_template_version.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_import_metadata.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_instance_nested_imports.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_invalid_input_defaults.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_invalid_section_names.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_invalid_template_version.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      647 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_long_rel.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3680 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_multiple_validation_errors.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_no_inputs_in_template.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_no_outputs_in_template.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_nodetype_without_relationship.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1070 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_normative_type_properties_override.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_scalar_unit_without_unit.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_tosca_custom_rel.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      528 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_tosca_custom_rel_with_script.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_tosca_normative_type_by_shortname.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_tosca_top_level_error1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/test_tosca_top_level_error2.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.867359 tosca-parser-2.8.0/toscaparser/tests/data/topology_template/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1893 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/topology_template/databasesubsystem.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1956 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/topology_template/definitions.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1874 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/topology_template/definitions_1_2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/topology_template/queuingsubsystem.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1888 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/topology_template/system.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2258 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/topology_template/transactionsubsystem.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.871359 tosca-parser-2.8.0/toscaparser/tests/data/topology_template/validate/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2424 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/topology_template/validate/queuingsubsystem_invalid_input.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/topology_template/validate/system_invalid_input.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1737 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/topology_template/validate/test_example_app_substitution_mappings.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/topology_template/validate/test_substitution_mappings_invalid_output.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/topology_template/validate/test_substitution_mappings_valid_output.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6895 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/tosca_elk.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/tosca_helloworld.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1440 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/tosca_imports_validation.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3507 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/tosca_single_instance_wordpress.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3385 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/tosca_single_instance_wordpress_with_local_abspath_import.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3316 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/tosca_single_instance_wordpress_with_url_import.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/data/tosca_test_get_operation_output.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.803359 tosca-parser-2.8.0/toscaparser/tests/extensions/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.871359 tosca-parser-2.8.0/toscaparser/tests/extensions/nfv/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/extensions/nfv/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1050 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/extensions/nfv/test_tosca_nfv_tpl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.803359 tosca-parser-2.8.0/toscaparser/tests/spec_samples/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.871359 tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.871359 tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      984 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/network/tosca_one_server_one_network.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1391 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/network/tosca_one_server_three_networks.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/network/tosca_server_on_existing_network.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1870 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/network/tosca_two_servers_one_network.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.871359 tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1759 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_blockstorage_with_attachment.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2526 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_blockstorage_with_attachment_notation1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2815 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_blockstorage_with_attachment_notation2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1908 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_blockstorage_with_custom_relationship_type.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1677 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_blockstorage_with_relationship_template.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2810 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_multiple_blockstorage_with_attachment.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_single_object_store.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2656 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/tosca_nodejs_mongodb_two_instances.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      976 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/tosca_single_server.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17040 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/test_constraints.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1373 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/test_custom_relationships.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19911 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/test_datatypes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1723 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/test_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18163 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/test_functions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16664 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/test_prereq.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15137 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/test_properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12568 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/test_scalarunit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1861 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16339 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/test_topology_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18708 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/test_toscadef.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45468 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/test_toscatpl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    78141 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/test_toscatplvalidation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2117 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5385 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tests/test_validate_tosca_version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15465 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/topology_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15089 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tosca_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1698 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/tpl_relationship_graph.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3153 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/triggers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2120 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/unsupportedtype.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:03:26.875359 tosca-parser-2.8.0/toscaparser/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/utils/gettextutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2118 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/utils/urlutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7954 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/utils/validateutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2823 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/toscaparser/utils/yamlparser.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1241 2023-02-13 16:02:58.000000 tosca-parser-2.8.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.418744 tosca-parser-2.9.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4131 2023-07-06 09:03:37.000000 tosca-parser-2.9.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      624 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24417 2023-07-06 09:03:37.000000 tosca-parser-2.9.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10142 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3564 2023-07-06 09:03:37.418744 tosca-parser-2.9.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2097 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.382744 tosca-parser-2.9.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.382744 tosca-parser-2.9.0/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2423 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/doc/source/contributing.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.382744 tosca-parser-2.9.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1886 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1436 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      989 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/doc/source/usage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1306 2023-07-06 09:03:37.422744 tosca-parser-2.9.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.382744 tosca-parser-2.9.0/tosca_parser.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3564 2023-07-06 09:03:37.000000 tosca-parser-2.9.0/tosca_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18884 2023-07-06 09:03:37.000000 tosca-parser-2.9.0/tosca_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-06 09:03:37.000000 tosca-parser-2.9.0/tosca_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2023-07-06 09:03:37.000000 tosca-parser-2.9.0/tosca_parser.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-07-06 09:03:37.000000 tosca-parser-2.9.0/tosca_parser.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-07-06 09:03:37.000000 tosca-parser-2.9.0/tosca_parser.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-07-06 09:03:37.000000 tosca-parser-2.9.0/tosca_parser.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2023-07-06 09:03:37.000000 tosca-parser-2.9.0/tosca_parser.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1154 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/tosca_parser.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.386744 tosca-parser-2.9.0/toscaparser/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      643 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1842 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/capabilities.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.386744 tosca-parser-2.9.0/toscaparser/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7566 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/common/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8188 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/dataentity.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.386744 tosca-parser-2.9.0/toscaparser/elements/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31479 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/elements/TOSCA_definition_1_0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/elements/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2050 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/elements/artifacttype.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      780 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/elements/attribute_definition.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4154 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/elements/capabilitytype.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22660 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/elements/constraints.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2208 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/elements/datatype.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6188 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/elements/entity_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3794 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/elements/grouptype.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4085 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/elements/interfaces.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9458 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/elements/nodetype.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5335 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/elements/policytype.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3797 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/elements/portspectype.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4042 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/elements/property_definition.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2673 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/elements/relationshiptype.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4788 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/elements/scalarunit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4045 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/elements/statefulentitytype.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2789 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/elements/tosca_type_validation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14802 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/entity_template.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.386744 tosca-parser-2.9.0/toscaparser/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/extensions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2537 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/extensions/exttools.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.386744 tosca-parser-2.9.0/toscaparser/extensions/mec/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5831 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/extensions/mec/TOSCA_mec_definition_1_0_0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/extensions/mec/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/extensions/mec/tosca_simple_profile_for_mec_1_0_0.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.386744 tosca-parser-2.9.0/toscaparser/extensions/nfv/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8415 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/extensions/nfv/TOSCA_nfv_definition_1_0_0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/extensions/nfv/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.374744 tosca-parser-2.9.0/toscaparser/extensions/nfv/tests/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.386744 tosca-parser-2.9.0/toscaparser/extensions/nfv/tests/data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      670 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/extensions/nfv/tests/data/tosca_helloworld_nfv.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      795 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/extensions/nfv/tosca_simple_profile_for_nfv_1_0_0.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38374 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/functions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2108 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14248 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/imports.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14498 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/nodetemplate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4271 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/parameters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3406 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/policy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.390744 tosca-parser-2.9.0/toscaparser/prereq/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/prereq/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17198 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/prereq/csar.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2442 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3189 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/relationship_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2347 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/repositories.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/reservation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3874 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10153 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/substitution_mappings.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.390744 tosca-parser-2.9.0/toscaparser/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.374744 tosca-parser-2.9.0/toscaparser/tests/artifacts/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.390744 tosca-parser-2.9.0/toscaparser/tests/artifacts/collectd/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      992 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/collectd/config.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      107 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/collectd/create.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      110 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/collectd/start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.390744 tosca-parser-2.9.0/toscaparser/tests/artifacts/elasticsearch/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      432 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/elasticsearch/create.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      125 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/elasticsearch/start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.390744 tosca-parser-2.9.0/toscaparser/tests/artifacts/kibana/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      362 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/kibana/config.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      464 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/kibana/create.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      106 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/kibana/start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.394744 tosca-parser-2.9.0/toscaparser/tests/artifacts/logstash/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1113 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/logstash/configure_collectd.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1000 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/logstash/configure_elasticsearch.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      905 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/logstash/configure_rsyslog.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      603 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/logstash/create.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)       93 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/logstash/start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.394744 tosca-parser-2.9.0/toscaparser/tests/artifacts/mongodb/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/mongodb/config.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/mongodb/create.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/mongodb/create_database.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/mongodb/start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.394744 tosca-parser-2.9.0/toscaparser/tests/artifacts/mysql/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      209 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/mysql/mysql_database_configure.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      183 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/mysql/mysql_dbms_configure.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      308 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/mysql/mysql_dbms_install.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)       33 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/mysql/mysql_dbms_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.394744 tosca-parser-2.9.0/toscaparser/tests/artifacts/nodejs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/nodejs/config.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/nodejs/create.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/nodejs/start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.394744 tosca-parser-2.9.0/toscaparser/tests/artifacts/rsyslog/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/rsyslog/config.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      124 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/rsyslog/create.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      108 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/rsyslog/start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.394744 tosca-parser-2.9.0/toscaparser/tests/artifacts/webserver/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)       92 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/webserver/webserver_install.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)       31 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/webserver/webserver_start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.394744 tosca-parser-2.9.0/toscaparser/tests/artifacts/wordpress/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      231 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/wordpress/wordpress_configure.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)       86 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/artifacts/wordpress/wordpress_install.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2353 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.398744 tosca-parser-2.9.0/toscaparser/tests/data/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.402744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17490 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_elk.csar
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17490 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_elk.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_hello_world.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_invalid_entry_def.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2300 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_invalid_multilevel_imports_validation.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_metadata_not_yaml.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_missing_metadata.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22194 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_multiple_deployment_flavour.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_no_metadata_file.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_not_zip.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17127 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_relative_path_import_check.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_root_level_yaml.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1662 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_root_level_yaml_and_tosca_metadata.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      478 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_root_yaml_with_tosca_definition1_0.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1004 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_two_root_level_yaml.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2239 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_valid_multilevel_imports_validation.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5967 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wordpress.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5985 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_artifact.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6265 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_artifact_multi.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5978 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_import_path.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6043 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_import_url.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5969 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_script_path.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6043 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_script_url.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5977 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wordpress_valid_artifact.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6260 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wordpress_valid_artifact_multi.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6046 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wordpress_with_url_import_and_script.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wrong_metadata_file.zip
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/multi_level_imports_response.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/root_level_file.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.402744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.402744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/collectd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/elasticsearch.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      567 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/kibana.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      877 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/logstash.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/paypalpizzastore_nodejs_app.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/rsyslog.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7103 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/tosca_elk.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.374744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Python/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.402744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Python/collectd/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      992 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Python/collectd/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.402744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Python/logstash/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1113 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Python/logstash/configure_collectd.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1000 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Python/logstash/configure_elasticsearch.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      905 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Python/logstash/configure_rsyslog.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1126 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/README.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.374744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.402744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/collectd/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      107 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/collectd/create.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      110 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/collectd/start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.402744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/elasticsearch/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      432 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/elasticsearch/create.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      125 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/elasticsearch/start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.402744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/kibana/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      362 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/kibana/config.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      464 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/kibana/create.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      106 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/kibana/start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.406744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/logstash/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      603 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/logstash/create.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)       93 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/logstash/start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.406744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/mongodb/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/mongodb/config.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/mongodb/create.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/mongodb/create_database.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/mongodb/start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.406744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/nodejs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      743 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/nodejs/config.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/nodejs/create.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/nodejs/start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.406744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/rsyslog/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/rsyslog/config.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      124 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/rsyslog/create.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      108 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/rsyslog/start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.406744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/TOSCA-Metadata/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/TOSCA-Metadata/TOSCA.meta
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_meta_file.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.406744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.406744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Definitions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3209 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Definitions/tosca_single_instance_wordpress.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Definitions/wordpress.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1147 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/README.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.378744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.406744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/MYSQLDBMS/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/MYSQLDBMS/configure.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/MYSQLDBMS/install.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/MYSQLDBMS/start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.406744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/MYSQLDatabase/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/MYSQLDatabase/configure.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.406744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/WebServer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/WebServer/install.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/WebServer/start.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.406744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/WordPress/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/WordPress/configure.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Scripts/WordPress/install.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.406744 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/TOSCA-Metadata/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/TOSCA-Metadata/TOSCA.meta
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.406744 tosca-parser-2.9.0/toscaparser/tests/data/containers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/containers/test_container_docker_mysql.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.410744 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/collectd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/compute_with_attribute_list.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      524 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/compute_with_nested_atributes.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/compute_with_prop.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      878 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/container_cap_child.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/custom_cap.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/custom_cap_with_datatype.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/custom_caps_def.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      424 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/custom_data_type.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/custom_interface.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      597 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/custom_nested_data_types.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/custom_policy.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/custom_relationship_type_defs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/db_with_list_param.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/elasticsearch.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/imported_sample.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/invalid_template_version.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      565 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/kibana.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      878 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/logstash.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/nested_rsyslog.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/nested_test_kibana.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      976 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/nested_test_wordpress.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/node_with_cap.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/paypalpizzastore_nodejs_app.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/rsyslog.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/template_metadata.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/wordpress.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/custom_types/wordpress.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.410744 tosca-parser-2.9.0/toscaparser/tests/data/datatypes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1188 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/datatypes/custom_datatype_def.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1666 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/datatypes/test_custom_datatypes_in_current_template.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/datatypes/test_custom_datatypes_nested_datatype_error.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      647 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/datatypes/test_custom_datatypes_positive.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/datatypes/test_custom_datatypes_value_error.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/datatypes/test_datatype_portspec_add_req.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.410744 tosca-parser-2.9.0/toscaparser/tests/data/dsl_definitions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/dsl_definitions/test_nested_dsl_def.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.414744 tosca-parser-2.9.0/toscaparser/tests/data/functions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_capabilties_inheritance.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_concat.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_concat_invalid.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      625 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_container_cap_child.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_attribute_custom_data_type.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      837 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_attribute_host_keyword.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_attribute_host_not_found.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_attribute_illegal_host_in_outputs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      887 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_attribute_nested_data_types.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_attribute_source_target_keywords.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_attribute_unknown_attribute_name.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_attribute_unknown_node_template_name.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_attribute_with_index.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_attribute_with_index_error.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      579 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_attribute_with_nested_params.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_implicit_attribute.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      787 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_prop_cap_bool.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_prop_cap_host.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_property_source_target_keywords.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1624 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_property_with_host.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_invalid_function_signature.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_token.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_token_invalid.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      896 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_unknown_capability_property.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_unknown_input_in_interface.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/test_unknown_input_in_property.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/functions/tosca_nested_property_names_indexes.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.414744 tosca-parser-2.9.0/toscaparser/tests/data/groups/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/groups/definitions.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1356 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/groups/tosca_group_template.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.414744 tosca-parser-2.9.0/toscaparser/tests/data/interfaces/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      622 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/interfaces/test_custom_interface_in_template.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/interfaces/test_custom_interface_invalid_operation.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.414744 tosca-parser-2.9.0/toscaparser/tests/data/load_balancer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2027 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/load_balancer/tosca_load_balancer.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.414744 tosca-parser-2.9.0/toscaparser/tests/data/node_filter/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/node_filter/test_node_filter.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.414744 tosca-parser-2.9.0/toscaparser/tests/data/policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/policies/custom_definitions.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4922 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/policies/tacker_defs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5741 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/policies/tacker_nfv_defs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2469 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/policies/test_policies_without_required_property.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2468 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/policies/test_tosca_nfv_multiple_policies.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1163 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/policies/tosca_custom_policy_template.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3251 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/policies/tosca_policy_template.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.414744 tosca-parser-2.9.0/toscaparser/tests/data/relationship/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1304 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/relationship/test_custom_relationship.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.414744 tosca-parser-2.9.0/toscaparser/tests/data/repositories/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/repositories/test_repositories_definition.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      879 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/repositories/tosca_repositories_test_definition.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.414744 tosca-parser-2.9.0/toscaparser/tests/data/requirements/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1905 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/requirements/test_requirements.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_attributes_inheritance.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_available_rel_tpls.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1004 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_capability_without_properties.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1759 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_credential_datatype.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_custom_capabilty.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_custom_caps_def.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_custom_caps_with_datatype.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_endpoint_on_compute.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_import_invalid_template_version.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_import_metadata.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_instance_nested_imports.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_invalid_input_defaults.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      522 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_invalid_section_names.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_invalid_template_version.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      647 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_long_rel.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3680 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_multiple_validation_errors.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_no_inputs_in_template.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_no_outputs_in_template.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_nodetype_without_relationship.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1070 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_normative_type_properties_override.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_scalar_unit_without_unit.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_tosca_custom_rel.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      528 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_tosca_custom_rel_with_script.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_tosca_normative_type_by_shortname.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_tosca_top_level_error1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/test_tosca_top_level_error2.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.418744 tosca-parser-2.9.0/toscaparser/tests/data/topology_template/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1893 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/topology_template/databasesubsystem.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1956 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/topology_template/definitions.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1874 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/topology_template/definitions_1_2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/topology_template/queuingsubsystem.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1888 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/topology_template/system.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2258 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/topology_template/transactionsubsystem.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.418744 tosca-parser-2.9.0/toscaparser/tests/data/topology_template/validate/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2424 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/topology_template/validate/queuingsubsystem_invalid_input.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/topology_template/validate/system_invalid_input.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1737 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/topology_template/validate/test_example_app_substitution_mappings.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/topology_template/validate/test_substitution_mappings_invalid_output.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      909 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/topology_template/validate/test_substitution_mappings_valid_output.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6895 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/tosca_elk.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/tosca_helloworld.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1440 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/tosca_imports_validation.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3507 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/tosca_single_instance_wordpress.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3385 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/tosca_single_instance_wordpress_with_local_abspath_import.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3316 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/tosca_single_instance_wordpress_with_url_import.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/data/tosca_test_get_operation_output.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.378744 tosca-parser-2.9.0/toscaparser/tests/extensions/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.418744 tosca-parser-2.9.0/toscaparser/tests/extensions/nfv/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/extensions/nfv/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1050 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/extensions/nfv/test_tosca_nfv_tpl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.378744 tosca-parser-2.9.0/toscaparser/tests/spec_samples/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.418744 tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.418744 tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      984 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/network/tosca_one_server_one_network.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1391 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/network/tosca_one_server_three_networks.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/network/tosca_server_on_existing_network.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1870 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/network/tosca_two_servers_one_network.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.418744 tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1759 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_blockstorage_with_attachment.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2526 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_blockstorage_with_attachment_notation1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2815 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_blockstorage_with_attachment_notation2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1908 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_blockstorage_with_custom_relationship_type.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1677 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_blockstorage_with_relationship_template.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2810 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_multiple_blockstorage_with_attachment.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_single_object_store.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2656 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/tosca_nodejs_mongodb_two_instances.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      976 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/tosca_single_server.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17040 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/test_constraints.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1373 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/test_custom_relationships.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19911 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/test_datatypes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1723 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/test_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18163 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/test_functions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16664 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/test_prereq.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15137 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/test_properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12568 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/test_scalarunit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1861 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16339 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/test_topology_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18708 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/test_toscadef.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46816 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/test_toscatpl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    79015 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/test_toscatplvalidation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2117 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5385 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tests/test_validate_tosca_version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15465 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/topology_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15191 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tosca_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1698 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/tpl_relationship_graph.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3153 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/triggers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2120 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/unsupportedtype.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:37.418744 tosca-parser-2.9.0/toscaparser/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/utils/gettextutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2118 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/utils/urlutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7954 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/utils/validateutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2823 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/toscaparser/utils/yamlparser.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1230 2023-07-06 09:03:05.000000 tosca-parser-2.9.0/tox.ini
```

### Comparing `tosca-parser-2.8.0/AUTHORS` & `tosca-parser-2.9.0/AUTHORS`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 Bharath Thiruveedula <bharath_ves@hotmail.com>
 Bill Huber <wbhuber@us.ibm.com>
 Bob HADDLETON <bob.haddleton@alcatel-lucent.com>
 Bob Haddleton <bob.haddleton@nokia.com>
 Bob.Haddleton <bob.haddleton@nokia.com>
 Bob.Haddleton <bobh@haddleton.net>
 Brad Topol <btopol@us.ibm.com>
+Brendan Shephard <bshephar@redhat.com>
 Cao Xuan Hoang <hoangcx@vn.fujitsu.com>
 Christian Berendt <berendt@b1-systems.de>
 Corey Bryant <corey.bryant@canonical.com>
 Csaba Fülöp <csaba.fulop@nokia.com>
 Denis Makogon <lildee1991@gmail.com>
 Dharmesh Bhakta <bhakta@us.ibm.com>
 Dimitri Mazmanov <dimitri.mazmanov@ericsson.com>
@@ -48,14 +49,15 @@
 Miguel Caballer <micafer1@upv.es>
 Monty Taylor <mordred@inaugust.com>
 Nandini <nandini.vemula@tcs.com>
 Nguyen Hai <nguyentrihai93@gmail.com>
 Oleksii Chuprykov <ochuprykov@mirantis.com>
 OpenStack Release Bot <infra-root@openstack.org>
 Rohan Shah <ryshah@us.ibm.com>
+Roman Stolyarov <sadimer@ispras.ru>
 Sahdev Zala <spzala@us.ibm.com>
 Saju Madhavan <sajuptpm@gmail.com>
 Santhosh64 <santhoshkumar.kondapalli@tcs.com>
 Serg Melikyan <smelikyan@mirantis.com>
 Sergey Lukjanov <slukjanov@mirantis.com>
 Simeon Monov <sdmonov@us.ibm.com>
 Steve Martinelli <stevemar@ca.ibm.com>
```

### Comparing `tosca-parser-2.8.0/CONTRIBUTING.rst` & `tosca-parser-2.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/ChangeLog` & `tosca-parser-2.9.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+2.9.0
+-----
+
+* Support importing def from local instead of url
+* Interface outputs
+* Fix passenv for tox4
+
 2.8.0
 -----
 
 * Update python classifier for python 3.10
 
 2.7.0
 -----
```

### Comparing `tosca-parser-2.8.0/LICENSE` & `tosca-parser-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/PKG-INFO` & `tosca-parser-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: tosca-parser
-Version: 2.8.0
+Version: 2.9.0
 Summary: Parser for TOSCA Simple Profile in YAML.
 Home-page: https://docs.openstack.org/tosca-parser/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `tosca-parser-2.8.0/README.rst` & `tosca-parser-2.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/doc/source/conf.py` & `tosca-parser-2.9.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/doc/source/contributor/contributing.rst` & `tosca-parser-2.9.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/doc/source/index.rst` & `tosca-parser-2.9.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/doc/source/installation.rst` & `tosca-parser-2.9.0/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/doc/source/usage.rst` & `tosca-parser-2.9.0/doc/source/usage.rst`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/requirements.txt` & `tosca-parser-2.9.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/setup.cfg` & `tosca-parser-2.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/setup.py` & `tosca-parser-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/tosca_parser.egg-info/PKG-INFO` & `tosca-parser-2.9.0/tosca_parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: tosca-parser
-Version: 2.8.0
+Version: 2.9.0
 Summary: Parser for TOSCA Simple Profile in YAML.
 Home-page: https://docs.openstack.org/tosca-parser/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `tosca-parser-2.8.0/tosca_parser.egg-info/SOURCES.txt` & `tosca-parser-2.9.0/tosca_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/tosca_parser.py` & `tosca-parser-2.9.0/tosca_parser.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/__init__.py` & `tosca-parser-2.9.0/toscaparser/__init__.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/capabilities.py` & `tosca-parser-2.9.0/toscaparser/capabilities.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/common/exception.py` & `tosca-parser-2.9.0/toscaparser/common/exception.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/dataentity.py` & `tosca-parser-2.9.0/toscaparser/dataentity.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/elements/TOSCA_definition_1_0.yaml` & `tosca-parser-2.9.0/toscaparser/elements/TOSCA_definition_1_0.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/elements/artifacttype.py` & `tosca-parser-2.9.0/toscaparser/elements/artifacttype.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/elements/attribute_definition.py` & `tosca-parser-2.9.0/toscaparser/elements/attribute_definition.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/elements/capabilitytype.py` & `tosca-parser-2.9.0/toscaparser/elements/capabilitytype.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/elements/constraints.py` & `tosca-parser-2.9.0/toscaparser/elements/constraints.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/elements/datatype.py` & `tosca-parser-2.9.0/toscaparser/elements/datatype.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/elements/entity_type.py` & `tosca-parser-2.9.0/toscaparser/elements/entity_type.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/elements/grouptype.py` & `tosca-parser-2.9.0/toscaparser/elements/grouptype.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/elements/interfaces.py` & `tosca-parser-2.9.0/toscaparser/elements/interfaces.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 
 SECTIONS = (LIFECYCLE, CONFIGURE, LIFECYCLE_SHORTNAME,
             CONFIGURE_SHORTNAME) = \
            ('tosca.interfaces.node.lifecycle.Standard',
             'tosca.interfaces.relationship.Configure',
             'Standard', 'Configure')
 
-INTERFACEVALUE = (IMPLEMENTATION, INPUTS) = ('implementation', 'inputs')
+INTERFACEVALUE = (IMPLEMENTATION, INPUTS, OUTPUTS) = \
+    ('implementation', 'inputs', 'outputs')
 
 INTERFACE_DEF_RESERVED_WORDS = ['type', 'inputs', 'derived_from', 'version',
                                 'description']
 
 
 class InterfacesDef(StatefulEntityType):
     '''TOSCA built-in interfaces type.'''
@@ -35,14 +36,15 @@
         self.node_template = node_template
         self.type = interfacename
         self.interfacename = interfacename
         self.name = name
         self.value = value
         self.implementation = None
         self.inputs = None
+        self.outputs = None
         self.defs = {}
         if interfacename == LIFECYCLE_SHORTNAME:
             self.interfacetype = LIFECYCLE
         elif interfacename == CONFIGURE_SHORTNAME:
             self.interfacetype = CONFIGURE
         elif hasattr(self.ntype, 'interfaces') \
                 and self.ntype.interfaces \
@@ -67,14 +69,16 @@
         if value:
             if isinstance(self.value, dict):
                 for i, j in self.value.items():
                     if i == IMPLEMENTATION:
                         self.implementation = j
                     elif i == INPUTS:
                         self.inputs = j
+                    elif i == OUTPUTS:
+                        self.outputs = j
                     else:
                         what = ('"interfaces" of template "%s"' %
                                 self.node_template.name)
                         ExceptionCollector.appendException(
                             UnknownFieldError(what=what, field=i))
             else:
                 self.implementation = value
```

### Comparing `tosca-parser-2.8.0/toscaparser/elements/nodetype.py` & `tosca-parser-2.9.0/toscaparser/elements/nodetype.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/elements/policytype.py` & `tosca-parser-2.9.0/toscaparser/elements/policytype.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/elements/portspectype.py` & `tosca-parser-2.9.0/toscaparser/elements/portspectype.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/elements/property_definition.py` & `tosca-parser-2.9.0/toscaparser/elements/property_definition.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/elements/relationshiptype.py` & `tosca-parser-2.9.0/toscaparser/elements/relationshiptype.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/elements/scalarunit.py` & `tosca-parser-2.9.0/toscaparser/elements/scalarunit.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/elements/statefulentitytype.py` & `tosca-parser-2.9.0/toscaparser/elements/statefulentitytype.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/elements/tosca_type_validation.py` & `tosca-parser-2.9.0/toscaparser/elements/tosca_type_validation.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/entity_template.py` & `tosca-parser-2.9.0/toscaparser/entity_template.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/extensions/exttools.py` & `tosca-parser-2.9.0/toscaparser/extensions/exttools.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/extensions/mec/TOSCA_mec_definition_1_0_0.yaml` & `tosca-parser-2.9.0/toscaparser/extensions/mec/TOSCA_mec_definition_1_0_0.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/extensions/mec/tosca_simple_profile_for_mec_1_0_0.py` & `tosca-parser-2.9.0/toscaparser/extensions/mec/tosca_simple_profile_for_mec_1_0_0.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/extensions/nfv/TOSCA_nfv_definition_1_0_0.yaml` & `tosca-parser-2.9.0/toscaparser/extensions/nfv/TOSCA_nfv_definition_1_0_0.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/extensions/nfv/tests/data/tosca_helloworld_nfv.yaml` & `tosca-parser-2.9.0/toscaparser/extensions/nfv/tests/data/tosca_helloworld_nfv.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/extensions/nfv/tosca_simple_profile_for_nfv_1_0_0.py` & `tosca-parser-2.9.0/toscaparser/extensions/nfv/tosca_simple_profile_for_nfv_1_0_0.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/functions.py` & `tosca-parser-2.9.0/toscaparser/functions.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/groups.py` & `tosca-parser-2.9.0/toscaparser/groups.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/imports.py` & `tosca-parser-2.9.0/toscaparser/imports.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,19 +30,20 @@
 class ImportsLoader(object):
 
     IMPORTS_SECTION = (FILE, REPOSITORY, NAMESPACE_URI, NAMESPACE_PREFIX) = \
                       ('file', 'repository', 'namespace_uri',
                        'namespace_prefix')
 
     def __init__(self, importslist, path, type_definition_list=None,
-                 tpl=None):
+                 tpl=None, local_defs=None):
         self.importslist = importslist
         self.custom_defs = {}
         self.nested_tosca_tpls = []
         self.nested_imports = {}
+        self.local_defs = local_defs
         if not path and not tpl:
             msg = _('Input tosca template is not provided.')
             log.warning(msg)
             ExceptionCollector.appendException(ValidationError(message=msg))
         self.path = path
         self.repositories = {}
         if tpl and tpl.get('repositories'):
@@ -193,15 +194,22 @@
                      'definition "%(import_name)s".')
                    % {'import_name': import_name})
             log.error(msg)
             ExceptionCollector.appendException(ValidationError(message=msg))
             return None, None
 
         if toscaparser.utils.urlutils.UrlUtils.validate_url(file_name):
-            return file_name, YAML_LOADER(file_name, False)
+            has_file = False
+            if self.local_defs is not None:
+                for k in self.local_defs.keys():
+                    if k == file_name:
+                        file_name = self.local_defs[k]
+                        has_file = True
+
+            return file_name, YAML_LOADER(file_name, a_file=has_file)
         elif not repository:
             import_template = None
             if self.path:
                 if toscaparser.utils.urlutils.UrlUtils.validate_url(self.path):
                     if os.path.isabs(file_name):
                         msg = (_('Absolute file name "%(name)s" cannot be '
                                  'used in a URL-based input template '
```

### Comparing `tosca-parser-2.8.0/toscaparser/nodetemplate.py` & `tosca-parser-2.9.0/toscaparser/nodetemplate.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/parameters.py` & `tosca-parser-2.9.0/toscaparser/parameters.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/policy.py` & `tosca-parser-2.9.0/toscaparser/policy.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/prereq/csar.py` & `tosca-parser-2.9.0/toscaparser/prereq/csar.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/properties.py` & `tosca-parser-2.9.0/toscaparser/properties.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/relationship_template.py` & `tosca-parser-2.9.0/toscaparser/relationship_template.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/repositories.py` & `tosca-parser-2.9.0/toscaparser/repositories.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/reservation.py` & `tosca-parser-2.9.0/toscaparser/reservation.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/shell.py` & `tosca-parser-2.9.0/toscaparser/shell.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/substitution_mappings.py` & `tosca-parser-2.9.0/toscaparser/substitution_mappings.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/artifacts/collectd/config.py` & `tosca-parser-2.9.0/toscaparser/tests/artifacts/collectd/config.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/artifacts/logstash/configure_collectd.py` & `tosca-parser-2.9.0/toscaparser/tests/artifacts/logstash/configure_collectd.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/artifacts/logstash/configure_elasticsearch.py` & `tosca-parser-2.9.0/toscaparser/tests/artifacts/logstash/configure_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/artifacts/logstash/configure_rsyslog.py` & `tosca-parser-2.9.0/toscaparser/tests/artifacts/logstash/configure_rsyslog.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/artifacts/logstash/create.sh` & `tosca-parser-2.9.0/toscaparser/tests/artifacts/logstash/create.sh`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/artifacts/nodejs/config.sh` & `tosca-parser-2.9.0/toscaparser/tests/artifacts/nodejs/config.sh`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/artifacts/rsyslog/config.sh` & `tosca-parser-2.9.0/toscaparser/tests/artifacts/rsyslog/config.sh`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/base.py` & `tosca-parser-2.9.0/toscaparser/tests/base.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_elk.csar` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_elk.csar`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_elk.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_elk.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_hello_world.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_hello_world.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_invalid_entry_def.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_invalid_entry_def.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_invalid_multilevel_imports_validation.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_invalid_multilevel_imports_validation.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_metadata_not_yaml.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_metadata_not_yaml.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_missing_metadata.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_missing_metadata.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_multiple_deployment_flavour.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_multiple_deployment_flavour.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_relative_path_import_check.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_relative_path_import_check.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_root_level_yaml.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_root_level_yaml.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_root_level_yaml_and_tosca_metadata.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_root_level_yaml_and_tosca_metadata.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_two_root_level_yaml.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_two_root_level_yaml.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_valid_multilevel_imports_validation.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_valid_multilevel_imports_validation.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wordpress.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wordpress.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_artifact.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_artifact.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_artifact_multi.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_artifact_multi.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_import_path.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_import_path.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_import_url.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_import_url.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_script_path.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_script_path.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_script_url.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wordpress_invalid_script_url.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wordpress_valid_artifact.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wordpress_valid_artifact.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wordpress_valid_artifact_multi.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wordpress_valid_artifact_multi.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wordpress_with_url_import_and_script.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wordpress_with_url_import_and_script.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/csar_wrong_metadata_file.zip` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/csar_wrong_metadata_file.zip`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/multi_level_imports_response.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/multi_level_imports_response.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/root_level_file.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/root_level_file.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/kibana.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/kibana.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/logstash.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/logstash.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/paypalpizzastore_nodejs_app.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/paypalpizzastore_nodejs_app.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/tosca_elk.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Definitions/tosca_elk.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Python/collectd/config.py` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Python/collectd/config.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Python/logstash/configure_collectd.py` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Python/logstash/configure_collectd.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Python/logstash/configure_elasticsearch.py` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Python/logstash/configure_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Python/logstash/configure_rsyslog.py` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Python/logstash/configure_rsyslog.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/README.txt` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/README.txt`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/logstash/create.sh` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/logstash/create.sh`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/nodejs/config.sh` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/nodejs/config.sh`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/rsyslog/config.sh` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_elk/Scripts/rsyslog/config.sh`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_meta_file.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_meta_file.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Definitions/tosca_single_instance_wordpress.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Definitions/tosca_single_instance_wordpress.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Definitions/wordpress.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/Definitions/wordpress.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/README.txt` & `tosca-parser-2.9.0/toscaparser/tests/data/CSAR/tosca_single_instance_wordpress/README.txt`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/containers/test_container_docker_mysql.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/containers/test_container_docker_mysql.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/custom_types/compute_with_nested_atributes.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/custom_types/compute_with_nested_atributes.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/custom_types/container_cap_child.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/custom_types/container_cap_child.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/custom_types/custom_cap.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/custom_types/custom_cap.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/custom_types/custom_cap_with_datatype.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/custom_types/custom_cap_with_datatype.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/custom_types/custom_nested_data_types.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/custom_types/custom_nested_data_types.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/custom_types/custom_relationship_type_defs.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/custom_types/custom_relationship_type_defs.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/custom_types/imported_sample.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/custom_types/imported_sample.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/custom_types/kibana.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/custom_types/kibana.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/custom_types/logstash.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/custom_types/logstash.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/custom_types/nested_test_wordpress.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/custom_types/nested_test_wordpress.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/custom_types/node_with_cap.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/custom_types/node_with_cap.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/custom_types/paypalpizzastore_nodejs_app.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/custom_types/paypalpizzastore_nodejs_app.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/custom_types/wordpress.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/custom_types/wordpress.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/custom_types/wordpress.yml` & `tosca-parser-2.9.0/toscaparser/tests/data/custom_types/wordpress.yml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/datatypes/custom_datatype_def.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/datatypes/custom_datatype_def.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/datatypes/test_custom_datatypes_in_current_template.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/datatypes/test_custom_datatypes_in_current_template.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/datatypes/test_custom_datatypes_nested_datatype_error.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/datatypes/test_custom_datatypes_nested_datatype_error.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/datatypes/test_custom_datatypes_positive.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/datatypes/test_custom_datatypes_positive.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/datatypes/test_datatype_portspec_add_req.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/datatypes/test_datatype_portspec_add_req.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/functions/test_capabilties_inheritance.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/functions/test_capabilties_inheritance.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/functions/test_concat.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/functions/test_concat.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/functions/test_container_cap_child.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/functions/test_container_cap_child.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_attribute_custom_data_type.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_attribute_custom_data_type.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_attribute_host_keyword.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_attribute_host_keyword.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_attribute_nested_data_types.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_attribute_nested_data_types.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_attribute_source_target_keywords.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_attribute_source_target_keywords.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_attribute_unknown_attribute_name.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_attribute_unknown_attribute_name.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_attribute_unknown_node_template_name.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_attribute_unknown_node_template_name.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_attribute_with_nested_params.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_attribute_with_nested_params.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_implicit_attribute.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_implicit_attribute.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_prop_cap_bool.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_prop_cap_bool.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_property_source_target_keywords.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_property_source_target_keywords.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/functions/test_get_property_with_host.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/functions/test_get_property_with_host.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/functions/test_invalid_function_signature.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/functions/test_invalid_function_signature.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/functions/test_token_invalid.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/functions/test_token_invalid.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/functions/test_unknown_capability_property.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/functions/test_unknown_capability_property.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/functions/tosca_nested_property_names_indexes.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/functions/tosca_nested_property_names_indexes.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/groups/tosca_group_template.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/groups/tosca_group_template.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/interfaces/test_custom_interface_in_template.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/interfaces/test_custom_interface_in_template.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/load_balancer/tosca_load_balancer.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/load_balancer/tosca_load_balancer.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/policies/tacker_defs.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/policies/tacker_defs.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/policies/tacker_nfv_defs.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/policies/tacker_nfv_defs.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/policies/test_policies_without_required_property.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/policies/test_policies_without_required_property.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/policies/test_tosca_nfv_multiple_policies.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/policies/test_tosca_nfv_multiple_policies.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/policies/tosca_custom_policy_template.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/policies/tosca_custom_policy_template.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/policies/tosca_policy_template.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/policies/tosca_policy_template.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/relationship/test_custom_relationship.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/relationship/test_custom_relationship.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/repositories/test_repositories_definition.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/repositories/test_repositories_definition.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/repositories/tosca_repositories_test_definition.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/repositories/tosca_repositories_test_definition.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/requirements/test_requirements.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/requirements/test_requirements.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/test_attributes_inheritance.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/test_attributes_inheritance.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/test_capability_without_properties.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/test_capability_without_properties.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/test_credential_datatype.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/test_credential_datatype.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/test_instance_nested_imports.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/test_instance_nested_imports.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/test_invalid_section_names.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/test_invalid_section_names.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/test_long_rel.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/test_long_rel.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/test_multiple_validation_errors.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/test_multiple_validation_errors.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/test_nodetype_without_relationship.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/test_nodetype_without_relationship.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/test_normative_type_properties_override.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/test_normative_type_properties_override.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/test_tosca_custom_rel.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/test_tosca_custom_rel.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/test_tosca_custom_rel_with_script.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/test_tosca_custom_rel_with_script.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/test_tosca_normative_type_by_shortname.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/test_tosca_normative_type_by_shortname.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/topology_template/databasesubsystem.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/topology_template/databasesubsystem.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/topology_template/definitions.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/topology_template/definitions.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/topology_template/definitions_1_2.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/topology_template/definitions_1_2.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/topology_template/queuingsubsystem.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/topology_template/queuingsubsystem.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/topology_template/system.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/topology_template/system.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/topology_template/transactionsubsystem.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/topology_template/transactionsubsystem.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/topology_template/validate/queuingsubsystem_invalid_input.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/topology_template/validate/queuingsubsystem_invalid_input.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/topology_template/validate/system_invalid_input.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/topology_template/validate/system_invalid_input.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/topology_template/validate/test_example_app_substitution_mappings.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/topology_template/validate/test_example_app_substitution_mappings.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/topology_template/validate/test_substitution_mappings_invalid_output.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/topology_template/validate/test_substitution_mappings_invalid_output.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/topology_template/validate/test_substitution_mappings_valid_output.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/topology_template/validate/test_substitution_mappings_valid_output.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/tosca_elk.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/tosca_elk.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/tosca_helloworld.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/tosca_helloworld.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/tosca_imports_validation.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/tosca_imports_validation.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/tosca_single_instance_wordpress.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/tosca_single_instance_wordpress.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/tosca_single_instance_wordpress_with_local_abspath_import.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/tosca_single_instance_wordpress_with_local_abspath_import.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/data/tosca_single_instance_wordpress_with_url_import.yaml` & `tosca-parser-2.9.0/toscaparser/tests/data/tosca_single_instance_wordpress_with_url_import.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/extensions/nfv/test_tosca_nfv_tpl.py` & `tosca-parser-2.9.0/toscaparser/tests/extensions/nfv/test_tosca_nfv_tpl.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/network/tosca_one_server_one_network.yaml` & `tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/network/tosca_one_server_one_network.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/network/tosca_one_server_three_networks.yaml` & `tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/network/tosca_one_server_three_networks.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/network/tosca_server_on_existing_network.yaml` & `tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/network/tosca_server_on_existing_network.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/network/tosca_two_servers_one_network.yaml` & `tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/network/tosca_two_servers_one_network.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_blockstorage_with_attachment.yaml` & `tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_blockstorage_with_attachment.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_blockstorage_with_attachment_notation1.yaml` & `tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_blockstorage_with_attachment_notation1.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_blockstorage_with_attachment_notation2.yaml` & `tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_blockstorage_with_attachment_notation2.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_blockstorage_with_custom_relationship_type.yaml` & `tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_blockstorage_with_custom_relationship_type.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_blockstorage_with_relationship_template.yaml` & `tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_blockstorage_with_relationship_template.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_multiple_blockstorage_with_attachment.yaml` & `tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/storage/tosca_multiple_blockstorage_with_attachment.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/tosca_nodejs_mongodb_two_instances.yaml` & `tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/tosca_nodejs_mongodb_two_instances.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/spec_samples/v1.0/tosca_single_server.yaml` & `tosca-parser-2.9.0/toscaparser/tests/spec_samples/v1.0/tosca_single_server.yaml`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/test_constraints.py` & `tosca-parser-2.9.0/toscaparser/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/test_custom_relationships.py` & `tosca-parser-2.9.0/toscaparser/tests/test_custom_relationships.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/test_datatypes.py` & `tosca-parser-2.9.0/toscaparser/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/test_exception.py` & `tosca-parser-2.9.0/toscaparser/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/test_functions.py` & `tosca-parser-2.9.0/toscaparser/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/test_prereq.py` & `tosca-parser-2.9.0/toscaparser/tests/test_prereq.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/test_properties.py` & `tosca-parser-2.9.0/toscaparser/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/test_scalarunit.py` & `tosca-parser-2.9.0/toscaparser/tests/test_scalarunit.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/test_shell.py` & `tosca-parser-2.9.0/toscaparser/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/test_topology_template.py` & `tosca-parser-2.9.0/toscaparser/tests/test_topology_template.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/test_toscadef.py` & `tosca-parser-2.9.0/toscaparser/tests/test_toscadef.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/test_toscatpl.py` & `tosca-parser-2.9.0/toscaparser/tests/test_toscatpl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1009,7 +1009,37 @@
 
     def test_policies_without_required_property(self):
         tosca_tpl = os.path.join(
             os.path.dirname(os.path.abspath(__file__)),
             "data/policies/test_policies_without_required_property.yaml")
         self.assertRaises(exception.ValidationError, ToscaTemplate,
                           tosca_tpl, None)
+
+    def test_local_custom_defs(self):
+        """Compare if custom defs on local and remote the same."""
+
+        tosca_tpl = os.path.join(
+            os.path.dirname(os.path.abspath(__file__)),
+            "data/tosca_single_instance_wordpress_with_url_import.yaml")
+
+        local_def = os.path.join(
+            os.path.dirname(os.path.abspath(__file__)),
+            "data/custom_types/wordpress.yaml")
+        remote_def = (
+            "https://raw.githubusercontent.com/openstack/"
+            "tosca-parser/master/toscaparser/tests/data/custom_types/"
+            "wordpress.yaml")
+
+        local_defs = {remote_def: local_def}
+        params = {'db_name': 'my_wordpress', 'db_user': 'my_db_user',
+                  'db_root_pwd': '12345678'}
+        tosca = ToscaTemplate(tosca_tpl, parsed_params=params)
+        tosca_local = ToscaTemplate(tosca_tpl, parsed_params=params,
+                                    local_defs=local_defs)
+
+        # Compare the name of input params defined in the custom defs
+        expected = ["wp_db_name", "wp_db_user", "wp_db_password"]
+        for t in [tosca, tosca_local]:
+            actual = list(
+                (t.tpl["topology_template"]["node_templates"]["wordpress"]
+                    ["interfaces"]["Standard"]["configure"]["inputs"]).keys())
+            self.assertEqual(expected, actual)
```

### Comparing `tosca-parser-2.8.0/toscaparser/tests/test_toscatplvalidation.py` & `tosca-parser-2.9.0/toscaparser/tests/test_toscatplvalidation.py`

 * *Files 1% similar despite different names*

```diff
@@ -445,14 +445,36 @@
         path = 'toscaparser/tests/data/tosca_elk.yaml'
         custom_defs = self._imports_content_test(tpl_snippet,
                                                  path,
                                                  "node_types")
         self.assertTrue(custom_defs.get("mycompany.tosca.nodes."
                                         "WebApplication.WordPress"))
 
+    def test_imports_with_local_defs(self):
+        """Compare custom types on local and remote."""
+
+        ctypes = {
+            "remote": ("https://raw.githubusercontent.com/openstack/"
+                       "heat-translator/master/translator/tests/data/"
+                       "custom_types/wordpress.yaml"),
+            "local": "../data/wordpress.yaml"}
+
+        tpl_snippet = '''
+        imports:
+        - {}
+        '''.format(ctypes["remote"])
+        local_defs = {ctypes["remote"]: ctypes["local"]}
+
+        path = 'toscaparser/tests/data/tosca_elk.yaml'
+        imports = (toscaparser.utils.yamlparser.
+                   simple_parse(tpl_snippet)['imports'])
+        ld1 = ImportsLoader(imports, path, "node_types")
+        ld2 = ImportsLoader(imports, path, "node_types", local_defs)
+        self.assertEqual(ld1.get_custom_defs(), ld2.get_custom_defs())
+
     def test_imports_file_with_suffix_yml(self):
         tpl_snippet = '''
         imports:
         - custom_types/wordpress.yml
         '''
         path = 'toscaparser/tests/data/tosca_elk.yaml'
         custom_defs = self._imports_content_test(tpl_snippet,
```

### Comparing `tosca-parser-2.8.0/toscaparser/tests/test_utils.py` & `tosca-parser-2.9.0/toscaparser/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tests/test_validate_tosca_version.py` & `tosca-parser-2.9.0/toscaparser/tests/test_validate_tosca_version.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/topology_template.py` & `tosca-parser-2.9.0/toscaparser/topology_template.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/tosca_template.py` & `tosca-parser-2.9.0/toscaparser/tosca_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,23 +63,25 @@
     ADDITIONAL_SECTIONS = {'tosca_simple_yaml_1_0': SPECIAL_SECTIONS,
                            'tosca_simple_yaml_1_2': SPECIAL_SECTIONS}
 
     ADDITIONAL_SECTIONS.update(exttools.get_sections())
 
     '''Load the template data.'''
     def __init__(self, path=None, parsed_params=None, a_file=True,
-                 yaml_dict_tpl=None):
+                 yaml_dict_tpl=None, local_defs=None):
 
         ExceptionCollector.start()
         self.a_file = a_file
         self.input_path = None
         self.path = None
         self.tpl = None
         self.nested_tosca_tpls_with_topology = {}
         self.nested_tosca_templates_with_topology = []
+        self.local_defs = local_defs
+
         if path:
             self.input_path = path
             self.path = self._get_path(path)
             if self.path:
                 self.tpl = YAML_LOADER(self.path, self.a_file)
             if yaml_dict_tpl:
                 msg = (_('Both path and yaml_dict_tpl arguments were '
@@ -205,15 +207,16 @@
         if not imports:
             imports = self._tpl_imports()
         if not path:
             path = self.path
 
         if imports:
             custom_service = toscaparser.imports.\
-                ImportsLoader(imports, path, type_defs, self.tpl)
+                ImportsLoader(imports, path, type_defs, self.tpl,
+                              self.local_defs)
 
             nested_tosca_tpls = custom_service.get_nested_tosca_tpls()
             self._update_nested_tosca_tpls_with_topology(nested_tosca_tpls)
 
             nested_imports = custom_service.get_nested_imports()
             custom_defs = custom_service.get_custom_defs()
             if not custom_defs:
```

### Comparing `tosca-parser-2.8.0/toscaparser/tpl_relationship_graph.py` & `tosca-parser-2.9.0/toscaparser/tpl_relationship_graph.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/triggers.py` & `tosca-parser-2.9.0/toscaparser/triggers.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/unsupportedtype.py` & `tosca-parser-2.9.0/toscaparser/unsupportedtype.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/utils/gettextutils.py` & `tosca-parser-2.9.0/toscaparser/utils/gettextutils.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/utils/urlutils.py` & `tosca-parser-2.9.0/toscaparser/utils/urlutils.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/utils/validateutils.py` & `tosca-parser-2.9.0/toscaparser/utils/validateutils.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/toscaparser/utils/yamlparser.py` & `tosca-parser-2.9.0/toscaparser/utils/yamlparser.py`

 * *Files identical despite different names*

### Comparing `tosca-parser-2.8.0/tox.ini` & `tosca-parser-2.9.0/tox.ini`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 [tox]
 minversion = 3.1.0
 envlist = py3,pep8
 ignore_basepython_conflict = True
-skipsdist = True
 
 [testenv]
 basepython = python3
 usedevelop = True
 setenv =
    VIRTUAL_ENV={envdir}
    PYTHONWARNINGS=default::DeprecationWarning
-passenv = http_proxy HTTP_PROXY https_proxy HTTPS_PROXY no_proxy NO_PROXY
+passenv =
+	http_proxy
+	HTTP_PROXY
+	https_proxy
+	HTTPS_PROXY
+	no_proxy
+	NO_PROXY
 deps =
        -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
        -r{toxinidir}/requirements.txt
        -r{toxinidir}/test-requirements.txt
 commands = stestr run --slowest '{posargs}'
 
 [testenv:pep8]
```

