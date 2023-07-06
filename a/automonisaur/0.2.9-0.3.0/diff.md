# Comparing `tmp/automonisaur-0.2.9.tar.gz` & `tmp/automonisaur-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automonisaur-0.2.9.tar", last modified: Fri Feb 25 21:39:47 2022, max compression
+gzip compressed data, was "automonisaur-0.3.0.tar", last modified: Thu Jul  6 11:18:28 2023, max compression
```

## Comparing `automonisaur-0.2.9.tar` & `automonisaur-0.3.0.tar`

### file list

```diff
@@ -1,229 +1,327 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.465043 automonisaur-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (121)     3743 2022-02-25 21:39:47.465043 automonisaur-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2650 2022-02-25 21:39:42.000000 automonisaur-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.449042 automonisaur-0.2.9/automon/
--rwxr-xr-x   0 runner    (1001) docker     (121)       31 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/healthcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/helpers/
--rwxr-xr-x   0 runner    (1001) docker     (121)      112 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1235 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/assertions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/helpers/asyncio/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/asyncio/loop.py
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/asyncio_.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/helpers/cryptography/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/cryptography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/cryptography/hashing.py
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/cryptography/secret.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/dates.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/helpers/grok/
--rw-r--r--   0 runner    (1001) docker     (121)    11247 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/grok/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      357 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/http.py
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/markdown.py
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/helpers/os/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/os/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/os/environ.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1796 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/regex.py
--rw-r--r--   0 runner    (1001) docker     (121)     4412 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/sanitation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/sleeper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/helpers/subprocess/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/subprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2923 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/subprocess/run.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/helpers/threading/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/threading/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1672 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/threading/initialize_threading.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2145 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/helpers/threading/worker_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/integrations/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/integrations/cryptocurrency/
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/cryptocurrency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/cryptocurrency/accounting.py
--rw-r--r--   0 runner    (1001) docker     (121)      934 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/cryptocurrency/coinbase.py
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/cryptocurrency/other.py
--rw-r--r--   0 runner    (1001) docker     (121)     1698 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/cryptocurrency/robinhood.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/integrations/datascience/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/datascience/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/integrations/datascience/pandas/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/datascience/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/datascience/pandas/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (121)     2053 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/datascience/pandas/pandas.py
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/datascience/pandas/series.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/integrations/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (121)      173 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/elasticsearch/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (121)    10770 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/elasticsearch/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3130 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/elasticsearch/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1931 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/elasticsearch/jvm.py
--rw-r--r--   0 runner    (1001) docker     (121)     5000 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/elasticsearch/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     6090 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/elasticsearch/snapshots.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/integrations/flask/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4360 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/flask/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/flask/auth_creds.py
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/flask/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/flask/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/integrations/geoip/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/geoip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/integrations/google/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.453042 automonisaur-0.2.9/automon/integrations/google/gmail/
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/google/gmail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/google/gmail/v1/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/google/gmail/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4030 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/google/gmail/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/google/gmail/v1/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/ldap/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/ldap/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3587 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/ldap/client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/mac/
--rwxr-xr-x   0 runner    (1001) docker     (121)       29 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/mac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/mac/airport/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/mac/airport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6070 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/mac/airport/airport.py
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/mac/airport/scan.py
--rw-r--r--   0 runner    (1001) docker     (121)     2291 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/mac/airport/ssid.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/minio/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/minio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5327 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/minio/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1477 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/minio/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/neo4j/
--rwxr-xr-x   0 runner    (1001) docker     (121)       64 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/neo4j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6470 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/neo4j/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2376 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/neo4j/clientAsync.py
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/neo4j/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    11007 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/neo4j/cypher.py
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/neo4j/results.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/nmap/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/nmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2646 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/nmap/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/nmap/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     4675 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/nmap/output.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/openvpn/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/openvpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7004 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/openvpn/openvpn.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/requests/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4286 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/requests/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/requests/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/selenium/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/selenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      816 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/selenium/actions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3858 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/selenium/browser.py
--rw-r--r--   0 runner    (1001) docker     (121)     5459 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/selenium/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/sentryio/
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/sentryio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3076 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/sentryio/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1838 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/sentryio/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/shodan/
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/shodan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.457043 automonisaur-0.2.9/automon/integrations/slack/
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1293 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/slack/bots.py
--rw-r--r--   0 runner    (1001) docker     (121)     3606 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/slack/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5354 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/slack/clientAsync.py
--rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/slack/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2446 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/slack/error.py
--rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/slack/slack_formatting.py
--rw-r--r--   0 runner    (1001) docker     (121)    10992 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/slack/slack_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.461043 automonisaur-0.2.9/automon/integrations/snmp/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/snmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16009 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/snmp/generate_maps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.461043 automonisaur-0.2.9/automon/integrations/splunk/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3716 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2634 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.461043 automonisaur-0.2.9/automon/integrations/splunk_soar/
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk_soar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk_soar/artifact.py
--rw-r--r--   0 runner    (1001) docker     (121)    10147 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk_soar/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      944 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk_soar/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      964 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk_soar/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      699 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk_soar/container.py
--rw-r--r--   0 runner    (1001) docker     (121)     1740 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk_soar/phantom_unittest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.461043 automonisaur-0.2.9/automon/integrations/splunk_soar/rest/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk_soar/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8879 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk_soar/rest/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     3701 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/splunk_soar/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.461043 automonisaur-0.2.9/automon/integrations/swift/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/swift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17233 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/swift/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2729 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/swift/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/swift/error.py
--rw-r--r--   0 runner    (1001) docker     (121)     3874 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/swift/iterables.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.461043 automonisaur-0.2.9/automon/integrations/vds/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/vds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5614 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/vds/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/integrations/vds/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/liveliness.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.461043 automonisaur-0.2.9/automon/log/
--rwxr-xr-x   0 runner    (1001) docker     (121)       84 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6009 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/log/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.461043 automonisaur-0.2.9/automon/tests/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.461043 automonisaur-0.2.9/automon/tests/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/test_grok.py
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/test_healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (121)      358 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/test_liveliness.py
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/test_networking.py
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     2120 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/test_sanitation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/core/test_sleeper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.465043 automonisaur-0.2.9/automon/tests/integrations/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.465043 automonisaur-0.2.9/automon/tests/integrations/airport/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/airport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/airport/test_airport.py
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/airport/test_airport_neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.465043 automonisaur-0.2.9/automon/tests/integrations/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4898 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/elasticsearch/test_elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/elasticsearch/test_elasticsearch_JvmMonitor.py
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/elasticsearch/test_elasticsearch_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/elasticsearch/test_elasticsearch_common.py
--rw-r--r--   0 runner    (1001) docker     (121)     1502 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/elasticsearch/test_elasticsearch_snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.465043 automonisaur-0.2.9/automon/tests/integrations/minio/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/minio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/minio/test_minio_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/minio/test_minio_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.465043 automonisaur-0.2.9/automon/tests/integrations/neo4j/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/neo4j/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2804 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/neo4j/test_neo4j_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/neo4j/test_neo4j_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/neo4j/test_neo4j_cypher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.465043 automonisaur-0.2.9/automon/tests/integrations/nmap/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/nmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1963 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/nmap/test_nmap_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/nmap/test_nmap_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.465043 automonisaur-0.2.9/automon/tests/integrations/sentryio/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/sentryio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/sentryio/test_sentryio.py
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/sentryio/test_sentryio_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.465043 automonisaur-0.2.9/automon/tests/integrations/splunk_soar/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/splunk_soar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/splunk_soar/test_soar_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/splunk_soar/test_soar_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1241 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)     1606 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_datascience.py
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_flask.py
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_geoip.py
--rw-r--r--   0 runner    (1001) docker     (121)      528 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_selenium.py
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_shodan.py
--rw-r--r--   0 runner    (1001) docker     (121)     2817 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_slack.py
--rw-r--r--   0 runner    (1001) docker     (121)     1925 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_splunk.py
--rw-r--r--   0 runner    (1001) docker     (121)     3418 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_swift.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-25 21:39:42.000000 automonisaur-0.2.9/automon/tests/integrations/test_vds.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-25 21:39:47.465043 automonisaur-0.2.9/automonisaur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3743 2022-02-25 21:39:47.000000 automonisaur-0.2.9/automonisaur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7283 2022-02-25 21:39:47.000000 automonisaur-0.2.9/automonisaur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-25 21:39:47.000000 automonisaur-0.2.9/automonisaur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-02-25 21:39:47.000000 automonisaur-0.2.9/automonisaur.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-25 21:39:47.465043 automonisaur-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-02-25 21:39:42.000000 automonisaur-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.107260 automonisaur-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-06 11:18:22.000000 automonisaur-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-06 11:18:28.107260 automonisaur-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-06 11:18:22.000000 automonisaur-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.087260 automonisaur-0.3.0/automon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/healthcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.087260 automonisaur-0.3.0/automon/helpers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      126 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1235 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/assertions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.087260 automonisaur-0.3.0/automon/helpers/asyncioWrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/asyncioWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/asyncioWrapper/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.087260 automonisaur-0.3.0/automon/helpers/cryptography/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/cryptography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/cryptography/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/cryptography/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/dates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.087260 automonisaur-0.3.0/automon/helpers/grok/
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/grok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/httpWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.091260 automonisaur-0.3.0/automon/helpers/mathWrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/mathWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/mathWrapper/file_size.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.091260 automonisaur-0.3.0/automon/helpers/nest_asyncioWrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/nest_asyncioWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/nest_asyncioWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.091260 automonisaur-0.3.0/automon/helpers/osWrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/osWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/osWrapper/environ.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1796 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/sanitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/sleeper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.091260 automonisaur-0.3.0/automon/helpers/subprocessWrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/subprocessWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/subprocessWrapper/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.091260 automonisaur-0.3.0/automon/helpers/subprocessWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/subprocessWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/subprocessWrapper/tests/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/subprocessWrapper/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/subprocessWrapper/tests/test_sanitize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.091260 automonisaur-0.3.0/automon/helpers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/tests/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/tests/test_grok.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/tests/test_healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/tests/test_liveliness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/tests/test_networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/tests/test_sanitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/tests/test_sleeper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.091260 automonisaur-0.3.0/automon/helpers/threadingWrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/threadingWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/threadingWrapper/initialize_threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/helpers/threadingWrapper/worker_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.091260 automonisaur-0.3.0/automon/integrations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.091260 automonisaur-0.3.0/automon/integrations/cryptocurrency/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/cryptocurrency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/cryptocurrency/accounting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/cryptocurrency/coinbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/cryptocurrency/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/cryptocurrency/robinhood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.091260 automonisaur-0.3.0/automon/integrations/cryptocurrency/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/cryptocurrency/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/cryptocurrency/tests/test_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.091260 automonisaur-0.3.0/automon/integrations/datascience/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/datascience/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.091260 automonisaur-0.3.0/automon/integrations/datascience/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/datascience/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/datascience/pandas/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/datascience/pandas/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/datascience/pandas/series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.091260 automonisaur-0.3.0/automon/integrations/datascience/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/datascience/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/datascience/tests/test_datascience.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.091260 automonisaur-0.3.0/automon/integrations/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/elasticsearch/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/elasticsearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/elasticsearch/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/elasticsearch/jvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/elasticsearch/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/elasticsearch/snapshots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.091260 automonisaur-0.3.0/automon/integrations/elasticsearch/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/elasticsearch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/elasticsearch/tests/test_elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/elasticsearch/tests/test_elasticsearch_JvmMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/elasticsearch/tests/test_elasticsearch_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/elasticsearch/tests/test_elasticsearch_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/elasticsearch/tests/test_elasticsearch_snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.095260 automonisaur-0.3.0/automon/integrations/flaskWrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/flaskWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/flaskWrapper/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/flaskWrapper/auth_creds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/flaskWrapper/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/flaskWrapper/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.095260 automonisaur-0.3.0/automon/integrations/flaskWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/flaskWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/flaskWrapper/tests/test_flask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.095260 automonisaur-0.3.0/automon/integrations/geoip/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/geoip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.095260 automonisaur-0.3.0/automon/integrations/geoip/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/geoip/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/geoip/tests/test_geoip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.095260 automonisaur-0.3.0/automon/integrations/google/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.095260 automonisaur-0.3.0/automon/integrations/google/gmail/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/google/gmail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.095260 automonisaur-0.3.0/automon/integrations/google/gmail/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/google/gmail/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/google/gmail/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/google/gmail/v1/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.095260 automonisaur-0.3.0/automon/integrations/google/people/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/google/people/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/google/people/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/google/people/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10812 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/google/people/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/google/people/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/google/people/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.095260 automonisaur-0.3.0/automon/integrations/google/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/google/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/google/tests/test_google_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/google/tests/test_google_contacts_neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.095260 automonisaur-0.3.0/automon/integrations/instagram/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/instagram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/instagram/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/instagram/client_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/instagram/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/instagram/stories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.095260 automonisaur-0.3.0/automon/integrations/instagram/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/instagram/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/instagram/tests/test_instagram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/instagram/tests/test_instagram_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/instagram/tests/test_instagram_browser_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/instagram/tests/test_instagram_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/instagram/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/instagram/xpaths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.095260 automonisaur-0.3.0/automon/integrations/ldap/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/ldap/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3587 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/ldap/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.095260 automonisaur-0.3.0/automon/integrations/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/mac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.095260 automonisaur-0.3.0/automon/integrations/mac/airport/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/mac/airport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/mac/airport/airport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/mac/airport/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/mac/airport/ssid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.095260 automonisaur-0.3.0/automon/integrations/mac/airport/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/mac/airport/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/mac/airport/tests/test_airport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/mac/airport/tests/test_airport_neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.095260 automonisaur-0.3.0/automon/integrations/minioWrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/minioWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/minioWrapper/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/minioWrapper/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/minioWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/minioWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/minioWrapper/object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.095260 automonisaur-0.3.0/automon/integrations/minioWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/minioWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/minioWrapper/tests/test_minio_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/minioWrapper/tests/test_minio_client_public.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/minioWrapper/tests/test_minio_client_public_clear_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/minioWrapper/tests/test_minio_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.099260 automonisaur-0.3.0/automon/integrations/neo4jWrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/neo4jWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6477 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/neo4jWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/neo4jWrapper/clientAsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/neo4jWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/neo4jWrapper/cypher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/neo4jWrapper/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.099260 automonisaur-0.3.0/automon/integrations/neo4jWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/neo4jWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/neo4jWrapper/tests/test_neo4j_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/neo4jWrapper/tests/test_neo4j_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/neo4jWrapper/tests/test_neo4j_cypher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.099260 automonisaur-0.3.0/automon/integrations/nmap/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/nmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/nmap/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/nmap/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/nmap/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.099260 automonisaur-0.3.0/automon/integrations/nmap/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/nmap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/nmap/tests/test_nmap_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/nmap/tests/test_nmap_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.099260 automonisaur-0.3.0/automon/integrations/openvpn/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/openvpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/openvpn/openvpn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.099260 automonisaur-0.3.0/automon/integrations/requestsWrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/requestsWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/requestsWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/requestsWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/requestsWrapper/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.099260 automonisaur-0.3.0/automon/integrations/requestsWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/requestsWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/requestsWrapper/tests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/requestsWrapper/tests/test_rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/requestsWrapper/tests/test_rest_inherit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.099260 automonisaur-0.3.0/automon/integrations/seleniumWrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/seleniumWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/seleniumWrapper/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/seleniumWrapper/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/seleniumWrapper/browser_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/seleniumWrapper/browser_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/seleniumWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/seleniumWrapper/config_webdriver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/seleniumWrapper/config_webdriver_chrome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/seleniumWrapper/config_window_size.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.099260 automonisaur-0.3.0/automon/integrations/seleniumWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/seleniumWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/seleniumWrapper/tests/test_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/seleniumWrapper/tests/test_browser_headless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/seleniumWrapper/tests/test_browser_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/seleniumWrapper/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/seleniumWrapper/tests/test_new_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/seleniumWrapper/tests/test_user_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/seleniumWrapper/user_agents.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.099260 automonisaur-0.3.0/automon/integrations/sentryio/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/sentryio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/sentryio/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/sentryio/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.099260 automonisaur-0.3.0/automon/integrations/sentryio/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/sentryio/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/sentryio/tests/test_sentryio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/sentryio/tests/test_sentryio_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.099260 automonisaur-0.3.0/automon/integrations/shodan/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/shodan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.099260 automonisaur-0.3.0/automon/integrations/shodan/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/shodan/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/shodan/tests/test_shodan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.103260 automonisaur-0.3.0/automon/integrations/slackWrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/slackWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/slackWrapper/bots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/slackWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/slackWrapper/clientAsync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/slackWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/slackWrapper/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/slackWrapper/slack_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11017 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/slackWrapper/slack_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.103260 automonisaur-0.3.0/automon/integrations/slackWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/slackWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/slackWrapper/tests/test_slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.103260 automonisaur-0.3.0/automon/integrations/snmp/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/snmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16016 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/snmp/generate_maps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.103260 automonisaur-0.3.0/automon/integrations/splunk/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.103260 automonisaur-0.3.0/automon/integrations/splunk/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk/tests/test_splunk_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk/tests/test_splunk_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.103260 automonisaur-0.3.0/automon/integrations/splunk_soar/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/action_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25888 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.103260 automonisaur-0.3.0/automon/integrations/splunk_soar/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.103260 automonisaur-0.3.0/automon/integrations/splunk_soar/integration/servicenow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/integration/servicenow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/integration/servicenow/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/integration/servicenow/ticket.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1731 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/phantom_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.103260 automonisaur-0.3.0/automon/integrations/splunk_soar/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14303 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/rest/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.107260 automonisaur-0.3.0/automon/integrations/splunk_soar/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   899665 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/tests/dino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/tests/test_soar_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/tests/test_soar_client_create_container_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/tests/test_soar_client_filter_vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/tests/test_soar_client_get_action_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run_by_playbook_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/tests/test_soar_client_list_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/tests/test_soar_client_list_vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/tests/test_soar_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/tests/test_soar_uat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/tests/test_soar_uat_run_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/tests/test_soar_uat_update_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/splunk_soar/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.107260 automonisaur-0.3.0/automon/integrations/swift/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/swift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17233 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/swift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/swift/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/swift/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/swift/iterables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.107260 automonisaur-0.3.0/automon/integrations/swift/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/swift/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/swift/tests/test_swift.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.107260 automonisaur-0.3.0/automon/integrations/vds/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/vds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/vds/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/vds/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.107260 automonisaur-0.3.0/automon/integrations/vds/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/vds/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/integrations/vds/tests/test_vds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/liveliness.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.107260 automonisaur-0.3.0/automon/log/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       84 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6254 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/log/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.107260 automonisaur-0.3.0/automon/log/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/log/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-06 11:18:22.000000 automonisaur-0.3.0/automon/log/tests/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 11:18:28.107260 automonisaur-0.3.0/automonisaur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-06 11:18:28.000000 automonisaur-0.3.0/automonisaur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-07-06 11:18:28.000000 automonisaur-0.3.0/automonisaur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 11:18:28.000000 automonisaur-0.3.0/automonisaur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 11:18:28.000000 automonisaur-0.3.0/automonisaur.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 11:18:28.107260 automonisaur-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-06 11:18:22.000000 automonisaur-0.3.0/setup.py
```

### Comparing `automonisaur-0.2.9/PKG-INFO` & `automonisaur-0.3.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,94 +1,83 @@
-Metadata-Version: 2.1
-Name: automonisaur
-Version: 0.2.9
-Summary: Core libraries for automonisaur
-Home-page: https://github.com/TheShellLand/automonisaur
-Author: naisanza
-Author-email: naisanza@gmail.com
-License: UNKNOWN
-Description: ![](https://github.com/TheShellLand/automonisaur/raw/master/docs/images/sauruspark.gif)
-        
-        # Automonisaur: Core Libraries
-        
-        **[about](#about)** |
-        **[integrations](#integrations)** |
-        **[install](#install)** |
-        **[docker](docker)** |
-        **[unittest locally](#unittest-locally)** |
-        **[codecov](https://codecov.io/gh/TheShellLand/automonisaur)** |
-        **[pypi](https://pypi.org/project/automonisaur/)**
-        
-        [![master](https://github.com/TheShellLand/automonisaur/actions/workflows/ci.yml/badge.svg)](https://github.com/TheShellLand/automonisaur/actions/workflows/ci.yml)
-        [![master](https://github.com/TheShellLand/automonisaur/actions/workflows/python39.yml/badge.svg)](https://github.com/TheShellLand/automonisaur/actions/workflows/python39.yml)
-        [![master](https://github.com/TheShellLand/automonisaur/actions/workflows/python38.yml/badge.svg)](https://github.com/TheShellLand/automonisaur/actions/workflows/python38.yml)
-        [![master](https://github.com/TheShellLand/automonisaur/actions/workflows/python37.yml/badge.svg)](https://github.com/TheShellLand/automonisaur/actions/workflows/python37.yml)
-        [![master](https://github.com/TheShellLand/automonisaur/actions/workflows/python36.yml/badge.svg)](https://github.com/TheShellLand/automonisaur/actions/workflows/python36.yml)
-        
-        [![Downloads](https://pepy.tech/badge/automonisaur)](https://pepy.tech/project/automonisaur)
-        [![Downloads](https://pepy.tech/badge/automonisaur/month)](https://pepy.tech/project/automonisaur)
-        [![Downloads](https://pepy.tech/badge/automonisaur/week)](https://pepy.tech/project/automonisaur)
-        
-        [//]: # ([![codecov]&#40;https://codecov.io/gh/TheShellLand/automonisaur/branch/master/graph/badge.svg&#41;]&#40;https://codecov.io/gh/TheShellLand/automonisaur&#41;)
-        
-        ### About
-        
-        This library adds some easier-to-use wrappers around common services for data science and threat intelligence.
-        
-        Provides easier clients and configuration options, as well as any additional helpers to get things up and running.
-        
-        Github issues and feature requests welcomed.
-        
-        ### Integrations
-        
-        - airport
-        - elasticsearch
-        - flask
-        - logging
-        - minio
-        - neo4j
-        - nmap
-        - requests
-        - selenium
-        - sentryio
-        - slack
-        - snmp
-        - splunk
-        - swift
-        
-        #### Requires
-        
-        - python >= 3.7
-        
-        _Note: install requirements.txt to use all integrations_
-        
-        #### install core library
-        
-        ```shell script
-        /bin/bash install.sh
-        ```
-        
-        #### install integration libraries
-        
-        ```shell script
-        # shell script
-        /bin/bash requirements.sh
-        
-        # pip
-        python3 -m pip install -U -r requirements.txt
-        
-        # pip 
-        python3 -m pip install -U -r https://raw.githubusercontent.com/TheShellLand/automonisaur/master/requirements.txt
-        ```
-        
-        #### unittest locally
-        
-        ```shell script
-        /bin/bash unittests.sh
-        ```
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+![](https://github.com/TheShellLand/automonisaur/raw/master/docs/images/sauruspark.gif)
+
+# Automonisaur: Core Libraries
+
+**[about](#about)** |
+**[integrations](#integrations)** |
+**[install](#install)** |
+**[docker](docker)** |
+**[unittest locally](#unittest-locally)** |
+**[codecov](https://codecov.io/gh/TheShellLand/automonisaur)** |
+**[pypi](https://pypi.org/project/automonisaur/)**
+
+[![master](https://github.com/TheShellLand/automonisaur/actions/workflows/ci.yml/badge.svg)](https://github.com/TheShellLand/automonisaur/actions/workflows/ci.yml)
+[![master](https://github.com/TheShellLand/automonisaur/actions/workflows/python311.yml/badge.svg)](https://github.com/TheShellLand/automonisaur/actions/workflows/python311.yml)
+[![master](https://github.com/TheShellLand/automonisaur/actions/workflows/python310.yml/badge.svg)](https://github.com/TheShellLand/automonisaur/actions/workflows/python310.yml)
+[![master](https://github.com/TheShellLand/automonisaur/actions/workflows/python39.yml/badge.svg)](https://github.com/TheShellLand/automonisaur/actions/workflows/python39.yml)
+[![master](https://github.com/TheShellLand/automonisaur/actions/workflows/python38.yml/badge.svg)](https://github.com/TheShellLand/automonisaur/actions/workflows/python38.yml)
+[![master](https://github.com/TheShellLand/automonisaur/actions/workflows/python37.yml/badge.svg)](https://github.com/TheShellLand/automonisaur/actions/workflows/python37.yml)
+[![master](https://github.com/TheShellLand/automonisaur/actions/workflows/python36.yml/badge.svg)](https://github.com/TheShellLand/automonisaur/actions/workflows/python36.yml)
+
+[![Downloads](https://pepy.tech/badge/automonisaur)](https://pepy.tech/project/automonisaur)
+[![Downloads](https://pepy.tech/badge/automonisaur/month)](https://pepy.tech/project/automonisaur)
+[![Downloads](https://pepy.tech/badge/automonisaur/week)](https://pepy.tech/project/automonisaur)
+
+[//]: # ([![codecov]&#40;https://codecov.io/gh/TheShellLand/automonisaur/branch/master/graph/badge.svg&#41;]&#40;https://codecov.io/gh/TheShellLand/automonisaur&#41;)
+
+### About
+
+This library adds some easier-to-use wrappers around common services for data science and threat intelligence.
+
+Provides easier clients and configuration options, as well as any additional helpers to get things up and running.
+
+Github issues and feature requests welcomed.
+
+### Integrations
+
+- airport
+- elasticsearch
+- flask
+- google people api
+- instagram
+- logging
+- minio
+- neo4j
+- nmap
+- requests
+- selenium
+- sentryio
+- slack
+- snmp
+- splunk
+- swift
+
+#### Requires
+
+- python >= 3.6
+
+_Note: install requirements.txt to use all integrations_
+
+#### install core library
+
+```shell script
+/bin/bash install.sh
+```
+
+#### install integration libraries
+
+```shell script
+# shell script
+/bin/bash install-requirements.sh
+
+# pip
+python3 -m pip install -U -r requirements.txt
+
+# pip 
+python3 -m pip install -U -r https://raw.githubusercontent.com/TheShellLand/automonisaur/master/requirements.txt
+```
+
+#### unittest locally
+
+```shell script
+/bin/bash unittests.sh
+```
```

### Comparing `automonisaur-0.2.9/README.md` & `automonisaur-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,38 @@
+Metadata-Version: 2.1
+Name: automonisaur
+Version: 0.3.0
+Summary: Core libraries for automonisaur
+Home-page: https://github.com/TheShellLand/automonisaur
+Author: naisanza
+Author-email: naisanza@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![](https://github.com/TheShellLand/automonisaur/raw/master/docs/images/sauruspark.gif)
 
 # Automonisaur: Core Libraries
 
 **[about](#about)** |
 **[integrations](#integrations)** |
 **[install](#install)** |
 **[docker](docker)** |
 **[unittest locally](#unittest-locally)** |
 **[codecov](https://codecov.io/gh/TheShellLand/automonisaur)** |
 **[pypi](https://pypi.org/project/automonisaur/)**
 
 [![master](https://github.com/TheShellLand/automonisaur/actions/workflows/ci.yml/badge.svg)](https://github.com/TheShellLand/automonisaur/actions/workflows/ci.yml)
+[![master](https://github.com/TheShellLand/automonisaur/actions/workflows/python311.yml/badge.svg)](https://github.com/TheShellLand/automonisaur/actions/workflows/python311.yml)
+[![master](https://github.com/TheShellLand/automonisaur/actions/workflows/python310.yml/badge.svg)](https://github.com/TheShellLand/automonisaur/actions/workflows/python310.yml)
 [![master](https://github.com/TheShellLand/automonisaur/actions/workflows/python39.yml/badge.svg)](https://github.com/TheShellLand/automonisaur/actions/workflows/python39.yml)
 [![master](https://github.com/TheShellLand/automonisaur/actions/workflows/python38.yml/badge.svg)](https://github.com/TheShellLand/automonisaur/actions/workflows/python38.yml)
 [![master](https://github.com/TheShellLand/automonisaur/actions/workflows/python37.yml/badge.svg)](https://github.com/TheShellLand/automonisaur/actions/workflows/python37.yml)
 [![master](https://github.com/TheShellLand/automonisaur/actions/workflows/python36.yml/badge.svg)](https://github.com/TheShellLand/automonisaur/actions/workflows/python36.yml)
 
 [![Downloads](https://pepy.tech/badge/automonisaur)](https://pepy.tech/project/automonisaur)
 [![Downloads](https://pepy.tech/badge/automonisaur/month)](https://pepy.tech/project/automonisaur)
@@ -31,49 +49,53 @@
 Github issues and feature requests welcomed.
 
 ### Integrations
 
 - airport
 - elasticsearch
 - flask
+- google people api
+- instagram
 - logging
 - minio
 - neo4j
 - nmap
 - requests
 - selenium
 - sentryio
 - slack
 - snmp
 - splunk
 - swift
 
 #### Requires
 
-- python >= 3.7
+- python >= 3.6
 
 _Note: install requirements.txt to use all integrations_
 
 #### install core library
 
 ```shell script
 /bin/bash install.sh
 ```
 
 #### install integration libraries
 
 ```shell script
 # shell script
-/bin/bash requirements.sh
+/bin/bash install-requirements.sh
 
 # pip
 python3 -m pip install -U -r requirements.txt
 
 # pip 
 python3 -m pip install -U -r https://raw.githubusercontent.com/TheShellLand/automonisaur/master/requirements.txt
 ```
 
 #### unittest locally
 
 ```shell script
 /bin/bash unittests.sh
 ```
+
+
```

### Comparing `automonisaur-0.2.9/automon/helpers/assertions.py` & `automonisaur-0.3.0/automon/helpers/assertions.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/helpers/asyncio_.py` & `automonisaur-0.3.0/automon/helpers/nest_asyncioWrapper/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,30 +16,30 @@
         self.maxqueue = 1000
         self.queue = asyncio.Queue(maxsize=self.maxqueue)
         self._nest = nest_asyncio.apply()
         asyncio.run(self._coro())
 
         self._finished = None
 
-    async def _coro(self) -> asyncio.coroutine:
+    async def _coro(self) -> asyncio:
         await asyncio.sleep(0)
 
     def run_until_complete(self):
         while True:
             if self.queue.qsize():
                 asyncio.run(asyncio.sleep(0))
             else:
                 self._finished = True
                 break
 
     @staticmethod
     def sleep(seconds: int):
         asyncio.run(asyncio.sleep(seconds))
 
-    def run(self) -> asyncio.run:
+    def run(self) -> asyncio:
         asyncio.run(self._coro())
 
     def start(self) -> run:
         return self.run()
 
     def create_task(self, task):
         return self.event_loop.create_task(task)
```

### Comparing `automonisaur-0.2.9/automon/helpers/grok/__init__.py` & `automonisaur-0.3.0/automon/helpers/grok/__init__.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/helpers/markdown.py` & `automonisaur-0.3.0/automon/helpers/markdown.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/helpers/networking.py` & `automonisaur-0.3.0/automon/helpers/networking.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,13 +22,13 @@
             s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             s.settimeout(timeout)
             s.connect((host, port))
             s.close()
             log.debug(f'SUCCESS {url}')
             return True
         except Exception as e:
-            log.error(f'FAILED {url} {e}', enable_traceback=False)
+            log.error(f'{url} {e}', enable_traceback=False)
             return False
 
     @staticmethod
     def urlparse(url):
         return urlparse(url)
```

### Comparing `automonisaur-0.2.9/automon/helpers/regex.py` & `automonisaur-0.3.0/automon/helpers/regex.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/helpers/sanitation.py` & `automonisaur-0.3.0/automon/helpers/sanitation.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/helpers/sleeper.py` & `automonisaur-0.3.0/automon/helpers/sleeper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,97 @@
 import time
 import random
 
 from automon.log import Logging
 
-log = Logging(__name__, level=Logging.INFO)
+log = Logging('Sleeper', level=Logging.INFO)
 
 
 class Sleeper:
 
     @staticmethod
     def seconds(caller: object or str, seconds: int) -> time.sleep:
         """Sleep for this many seconds"""
 
         sleep = seconds
-        log.info(f'[{Sleeper.seconds.__name__}] [{caller}] sleeping for {sleep} seconds')
+        if sleep < 2:
+            log.info(f'[{Sleeper.seconds.__name__}] '
+                     f'[{caller}] sleeping for {sleep} second')
+        else:
+            log.info(f'[{Sleeper.seconds.__name__}] '
+                     f'[{caller}] sleeping for {sleep} seconds')
         return time.sleep(sleep)
 
     @staticmethod
     def minute(caller: object or str, sleep: int = 60) -> time.sleep:
         """Sleep for a minute"""
 
-        log.info(f'[{Sleeper.minute.__name__}] [{caller}] sleeping for {sleep} seconds')
+        log.info(f'[{Sleeper.minute.__name__}] '
+                 f'[{caller}] sleeping for {sleep} seconds')
         return time.sleep(sleep)
 
     @staticmethod
     def within_a_minute(caller, sleep: int = None):
         """Sleep for a random minute"""
 
-        sleep = sleep if isinstance(sleep, int) else random.choice(range(1, 1 * 60))
-        log.info(f'[{Sleeper.within_a_minute.__name__}] [{caller}] sleeping for {sleep} seconds')
+        sleep = sleep if isinstance(sleep, int) else \
+            random.choice(range(1, 1 * 60))
+        log.info(f'[{Sleeper.within_a_minute.__name__}] '
+                 f'[{caller}] sleeping for {sleep} seconds')
         return time.sleep(sleep)
 
     @staticmethod
     def minutes(caller, minutes: int):
         """Sleep for this many minutes"""
 
         sleep = minutes * 60
-        log.info(f'[{Sleeper.minutes.__name__}] [{caller}] sleeping for {sleep} minutes')
+        log.info(f'[{Sleeper.minutes.__name__}] '
+                 f'[{caller}] sleeping for {sleep} minutes')
         return time.sleep(sleep)
 
     @staticmethod
     def hour(caller, hour: int = 1):
         """At some time within an hour, this will run"""
 
         sleep = hour if not hour else random.choice(
             range(1, hour * 60 * 60))
-        log.info(f'[{Sleeper.hour.__name__}] [{caller}] sleeping for {sleep} seconds')
+        log.info(f'[{Sleeper.hour.__name__}] '
+                 f'[{caller}] sleeping for {sleep} seconds')
         return time.sleep(sleep)
 
     @staticmethod
     def hours(caller, hours):
         """Sleep for this many hours"""
 
         sleep = hours * 60 * 60
-        log.info(f'[{Sleeper.hours.__name__}] [{caller}] sleeping for {hours} hours')
+        log.info(f'[{Sleeper.hours.__name__}] '
+                 f'[{caller}] sleeping for {hours} hours')
         return time.sleep(sleep)
 
     @staticmethod
     def day(caller, hours: int = 24):
         """At some time within 24 hours, this will run"""
 
         sleep = hours if not hours else random.choice(
             range(1, hours * 60 * 60))
-        log.info(f'[{Sleeper.day.__name__}] [{caller}] sleeping for {sleep} seconds')
+        log.info(f'[{Sleeper.day.__name__}] '
+                 f'[{caller}] sleeping for {sleep} seconds')
         return time.sleep(sleep)
 
     @staticmethod
     def daily(caller, hours: int = 24):
         """Sleep for one day"""
 
         sleep = hours if not hours else hours * 60 * 60
-        log.info(f'[{Sleeper.daily.__name__}] [{caller}] sleeping for {sleep} seconds')
+        log.info(f'[{Sleeper.daily.__name__}] '
+                 f'[{caller}] sleeping for {sleep} seconds')
         return time.sleep(sleep)
 
     @staticmethod
     def time_range(caller, seconds: int):
         """Sleep for a random range
         """
         sleep = seconds if not seconds else random.choice(
             range(1, seconds))
-        log.info(f'[{Sleeper.time_range.__name__}] [{caller}] sleeping for {sleep} seconds')
+        log.info(f'[{Sleeper.time_range.__name__}] '
+                 f'[{caller}] sleeping for {sleep} seconds')
         return time.sleep(sleep)
```

### Comparing `automonisaur-0.2.9/automon/helpers/threading/initialize_threading.py` & `automonisaur-0.3.0/automon/helpers/threadingWrapper/initialize_threading.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/helpers/threading/worker_thread.py` & `automonisaur-0.3.0/automon/helpers/threadingWrapper/worker_thread.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/cryptocurrency/accounting.py` & `automonisaur-0.3.0/automon/integrations/cryptocurrency/accounting.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/cryptocurrency/coinbase.py` & `automonisaur-0.3.0/automon/integrations/cryptocurrency/coinbase.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/cryptocurrency/other.py` & `automonisaur-0.3.0/automon/integrations/cryptocurrency/other.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/cryptocurrency/robinhood.py` & `automonisaur-0.3.0/automon/integrations/cryptocurrency/robinhood.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/datascience/pandas/pandas.py` & `automonisaur-0.3.0/automon/integrations/datascience/pandas/pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import pandas
 
 from io import StringIO
 from time import time as epoch_time
 
-from automon import Logging
+from automon.log import Logging
 
 from .series import Series
 from .dataframe import DataFrame
 
 
 class Pandas:
```

### Comparing `automonisaur-0.2.9/automon/integrations/elasticsearch/client.py` & `automonisaur-0.3.0/automon/integrations/elasticsearch/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,22 +57,21 @@
         try:
             client = Elasticsearch(
                 hosts=self.config.ELASTICSEARCH_HOST,
                 cloud_id=self.config.ELASTICSEARCH_CLOUD_ID,
                 api_key=self.config.ELASTICSEARCH_API_KEY,
                 request_timeout=self.config.ELASTICSEARCH_REQUEST_TIMEOUT,
                 http_auth=self.config.http_auth,
-                use_ssl=self.config.use_ssl,
-                verify_certs=self.config.verify_certs,
-                connection_class=self.config.connection_class)
+                verify_certs=self.config.verify_certs
+            )
             self._log.info(f'Connected to elasticsearch: {client}')
             return client
 
         except Exception as e:
-            self._log.error(f'Cannot connect to elasticsearch: {self.config.ELASTICSEARCH_HOST}, {e}')
+            self._log.error(f'Cannot connect to elasticsearch: {self.config.ELASTICSEARCH_HOST}, {e}', enable_traceback=False)
 
         return False
 
     def connected(self):
         """Check if connected"""
         if self.client:
             try:
```

### Comparing `automonisaur-0.2.9/automon/integrations/elasticsearch/config.py` & `automonisaur-0.3.0/automon/integrations/elasticsearch/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,15 @@
                  user: str = '',
                  password: str = '',
                  api_key: tuple = None,
                  api_key_id: str = None,
                  api_key_secret: str = None,
                  request_timeout: int = 1,
                  http_auth: tuple = None,
-                 use_ssl: bool = True,
                  verify_certs: bool = True,
-                 connection_class: object = None,
                  proxy=None):
         """elasticsearch config"""
 
         self._log = Logging(ElasticsearchConfig.__name__, Logging.DEBUG)
 
         # hosts
         self.ELASTICSEARCH_HOST = host or os.getenv('ELASTICSEARCH_HOSTS')
@@ -42,17 +40,15 @@
                 and not self.ELASTICSEARCH_API_KEY:
             self.ELASTICSEARCH_API_KEY = (self.ELASTICSEARCH_API_KEY_ID, self.ELASTICSEARCH_API_KEY_SECRET)
 
         # options
         self.ELASTICSEARCH_PROXY = proxy or os.getenv('ELASTICSEARCH_PROXY')
         self.ELASTICSEARCH_REQUEST_TIMEOUT = request_timeout or os.getenv('ELASTICSEARCH_REQUEST_TIMEOUT')
         self.request_timeout = self.ELASTICSEARCH_REQUEST_TIMEOUT
-        self.use_ssl = use_ssl
         self.verify_certs = verify_certs
-        self.connection_class = connection_class
 
         if self.ELASTICSEARCH_USER and self.ELASTICSEARCH_PASSWORD:
             self.http_auth = (self.ELASTICSEARCH_USER, self.ELASTICSEARCH_PASSWORD)
         else:
             self.http_auth = http_auth
 
     def __repr__(self):
```

### Comparing `automonisaur-0.2.9/automon/integrations/elasticsearch/jvm.py` & `automonisaur-0.3.0/automon/integrations/elasticsearch/jvm.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/elasticsearch/metrics.py` & `automonisaur-0.3.0/automon/integrations/elasticsearch/metrics.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/elasticsearch/snapshots.py` & `automonisaur-0.3.0/automon/integrations/elasticsearch/snapshots.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/flask/auth.py` & `automonisaur-0.3.0/automon/integrations/flaskWrapper/auth.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/flask/config.py` & `automonisaur-0.3.0/automon/integrations/flaskWrapper/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import os
 import hashlib
 
-from flask import Flask
 
-
-class FlaskConfig(Flask):
+class FlaskConfig(object):
 
     @staticmethod
     def javascript_compatibility(app):
         """Javascript expression compatibility
 
         Required to work with passing args to a flask page
         """
```

### Comparing `automonisaur-0.2.9/automon/integrations/google/gmail/v1/client.py` & `automonisaur-0.3.0/automon/integrations/google/gmail/v1/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from automon.integrations.requests import RequestsClient
+from automon.integrations.requestsWrapper import RequestsClient
 
 from .config import GmailConfig
 
 
 class GmailClient:
 
     def __init__(self, api_key: str = None, user: str = None, password: str = None, config: GmailConfig = None):
```

### Comparing `automonisaur-0.2.9/automon/integrations/google/gmail/v1/config.py` & `automonisaur-0.3.0/automon/integrations/google/gmail/v1/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from os import getenv
 
-from automon import Logging
+from automon.log import Logging
 
 log = Logging(name='GmailConfig', level=Logging.DEBUG)
 
 
 class GmailConfig:
     def __init__(self, endpoint: str = None,
                  api_key: str = None,
```

### Comparing `automonisaur-0.2.9/automon/integrations/ldap/client.py` & `automonisaur-0.3.0/automon/integrations/ldap/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/mac/airport/airport.py` & `automonisaur-0.3.0/automon/integrations/mac/airport/airport.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 
 from bs4 import BeautifulSoup
 
-from automon import Logging
+from automon.log import Logging
 from automon.helpers import Run
 from automon.helpers import Dates
 
 from .ssid import Ssid
 from .scan import ScanXml
 
 flags = {
```

### Comparing `automonisaur-0.2.9/automon/integrations/mac/airport/scan.py` & `automonisaur-0.3.0/automon/integrations/mac/airport/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from bs4 import BeautifulSoup
 
-from automon import Logging
+from automon.log import Logging
 
 from .ssid import Ssid
 
 log = Logging(name='ScanXml', level=Logging.DEBUG)
 
 
 class ScanXml:
```

### Comparing `automonisaur-0.2.9/automon/integrations/mac/airport/ssid.py` & `automonisaur-0.3.0/automon/integrations/mac/airport/ssid.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/neo4j/client.py` & `automonisaur-0.3.0/automon/integrations/neo4jWrapper/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import neo4j
 import logging
 
 from neo4j import GraphDatabase
 from queue import Queue
 
 from automon.log import Logging
-from automon.integrations.neo4j.cypher import Cypher
+from automon.integrations.neo4jWrapper.cypher import Cypher
 
 from .config import Neo4jConfig
 from .results import Results
 
 logging.getLogger('neo4j').setLevel(logging.ERROR)
 log = Logging('Neo4jClient', Logging.DEBUG)
```

### Comparing `automonisaur-0.2.9/automon/integrations/neo4j/clientAsync.py` & `automonisaur-0.3.0/automon/integrations/neo4jWrapper/clientAsync.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import asyncio
 
 from neo4j import GraphDatabase
 from queue import Queue
 
 from automon.log import Logging
 from automon.log.logger import logging
-from automon.integrations.neo4j.cypher import Cypher
+from automon.integrations.neo4jWrapper.cypher import Cypher
 
 from .config import Neo4jConfig
 from .results import Results
 
 logging.getLogger('neo4j').setLevel(logging.ERROR)
 log = Logging(__name__, Logging.DEBUG)
```

### Comparing `automonisaur-0.2.9/automon/integrations/neo4j/config.py` & `automonisaur-0.3.0/automon/integrations/vds/config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 import os
 
 from automon.log import Logging
-from automon.helpers.sanitation import Sanitation as S
 
-log = Logging(name='Neo4jConfig', level=Logging.DEBUG)
 
-
-class Neo4jConfig:
-    def __init__(self, user: str = None,
+class VdsConfig(object):
+    ldap_port = 636
+    rest_port = 8090
+
+    rest_path = 'adap'
+
+    def __init__(self, protocol: str = None,
+                 server: str = None,
+                 port: int = None,
+                 path: str = None,
+                 user: str = None,
                  password: str = None,
-                 hosts: str = None,
-                 encrypted: bool = None,
-                 trust: bool = None):
-        """Neo4j config
-        """
-
-        self.NEO4J_USER = user or os.getenv('NEO4J_USER') or ''
-        self.NEO4J_PASSWORD = password or os.getenv('NEO4J_PASSWORD') or ''
-        self.NEO4J_HOST = hosts or os.getenv('NEO4J_HOST') or ''
-
-        self.encrypted = encrypted
-        self.trust = trust
-
-        if not self.NEO4J_USER: log.warn(f'missing NEO4J_USER')
-        if not self.NEO4J_PASSWORD: log.warn(f'missing NEO4J_PASSWORD')
-        if not self.NEO4J_HOST: log.warn(f'missing NEO4J_HOST')
+                 basedn: str = None):
+        """VDS configuration"""
+
+        self.prot = protocol or 'https'
+        self.server = server or os.getenv('VDS_SERVER')
+        self.port = port or os.getenv('VDS_PORT') or self.rest_port
+        self.path = path or self.rest_path
+
+        self.user = user or os.getenv('VDS_BIND_USER')
+        self.bind_user = self.user
+        self.password = password or os.getenv('VDS_PASSWORD')
+        self.basedn = basedn or os.getenv('VDS_BASE_DN')
+
+        self.uri = f'{self.prot}://{self.server}:{self.port}/{self.path}'
+
+        self._log = Logging(name=VdsConfig.__name__, level=Logging.ERROR)
+
+        [self._log.debug(f'config: {x}') for x in self.__dict__.items()]
 
     def __repr__(self):
-        return f'{self.__dict__}'
+        return f'{self.prot}://{self.server}:{self.port} ({self.bind_user}) ({self.basedn})'
```

### Comparing `automonisaur-0.2.9/automon/integrations/neo4j/cypher.py` & `automonisaur-0.3.0/automon/integrations/neo4jWrapper/cypher.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/neo4j/results.py` & `automonisaur-0.3.0/automon/integrations/neo4jWrapper/results.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import re
 
-from neo4j.work.result import Result
+from neo4j.work.summary import ResultSummary
 
 from automon.log import Logging
 
-log = Logging(name='Results', level=Logging.DEBUG)
+log = Logging(name='ResultSummary', level=Logging.DEBUG)
 
 
-class Results(Result):
+class Results(ResultSummary):
     def __init__(self, results):
         self._results = results
         self.summary = results._summary
 
         if self.summary:
             self.counters = self.summary.counters
             self.notifications = self.summary.notifications
```

### Comparing `automonisaur-0.2.9/automon/integrations/nmap/client.py` & `automonisaur-0.3.0/automon/integrations/nmap/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 from automon.log import Logging
-from automon.helpers.subprocess import Run
+from automon.helpers import Run
 from automon.helpers.dates import Dates
 
 from .config import NmapConfig
 from .output import NmapResult
 
 
 class Nmap(object):
```

### Comparing `automonisaur-0.2.9/automon/integrations/nmap/config.py` & `automonisaur-0.3.0/automon/integrations/nmap/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from automon.log import Logging
-from automon.helpers.subprocess import Run
+from automon.helpers import Run
 
 
 class NmapConfig(object):
     def __init__(self, **kwargs):
         self._log = Logging(name=NmapConfig.__name__, level=Logging.ERROR)
 
         self.nmap = None
```

### Comparing `automonisaur-0.2.9/automon/integrations/nmap/output.py` & `automonisaur-0.3.0/automon/integrations/nmap/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import mmap
 import xmltodict
 import pandas as pd
 
 from automon.log import Logging
 from pandas import DataFrame
-from automon.helpers.subprocess import Run
+from automon.helpers import Run
 from automon.integrations.datascience import Pandas
 
 
 class NmapResult(object):
     def __init__(self, file: str = None, run: Run = None, **kwargs):
         self._log = Logging(name=NmapResult.__name__, level=Logging.INFO)
```

### Comparing `automonisaur-0.2.9/automon/integrations/openvpn/openvpn.py` & `automonisaur-0.3.0/automon/integrations/openvpn/openvpn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import io
 
-from automon.integrations.minio import MinioClient, MinioConfig
+from automon.integrations.minioWrapper import MinioClient, MinioConfig
 from automon.log import Logging
 from automon.helpers.sleeper import Sleeper
 
 log = Logging(name='openvpn', level='info')
 
 
 class ClientConfig:
```

### Comparing `automonisaur-0.2.9/automon/integrations/requests/client.py` & `automonisaur-0.3.0/automon/integrations/requestsWrapper/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,33 +12,36 @@
                  config: RequestsConfig = None):
         """Wrapper for requests library"""
 
         self.config = config or RequestsConfig()
 
         self.url = url
         self.data = data
+        self.errors = None
         self.headers = headers
         self.results = None
         self.requests = requests
 
         if url:
             self.url = url
             self.get(url=self.url, data=self.data, headers=self.headers)
 
     def __repr__(self):
         return f'{self.__dict__}'
 
     def _log_result(self):
         if self.results.status_code == 200:
             msg = f'{self.results.status_code} ' \
+                  f'{self.results.request.method} ' \
                   f'{self.results.url} ' \
                   f'{round(len(self.results.content) / 1024, 2)} KB'
             return log.debug(msg)
 
         msg = f'{self.results.status_code} ' \
+              f'{self.results.request.method} ' \
               f'{self.results.url} ' \
               f'{round(len(self.results.content) / 1024, 2)} KB ' \
               f'{self.results.content}'
         return log.error(msg, raise_exception=False)
 
     def _params(self, url, data, headers):
         if url is None:
@@ -46,14 +49,17 @@
 
         if data is None:
             data = self.data
 
         if headers is None:
             headers = self.headers
 
+        self.url = url
+        self.data = data
+        self.headers = headers
         return url, data, headers
 
     @property
     def content(self):
         if self.results is not None:
             return self.results.content
 
@@ -66,14 +72,15 @@
         url, data, headers = self._params(url, data, headers)
 
         try:
             self.results = requests.delete(url=url, data=data, headers=headers, **kwargs)
             self._log_result()
             return True
         except Exception as e:
+            self.errors = e
             log.error(f'delete failed. {e}', enable_traceback=False)
         return False
 
     def get(self,
             url: str = None,
             data: dict = None,
             headers: dict = None, **kwargs) -> bool:
@@ -82,14 +89,15 @@
         url, data, headers = self._params(url, data, headers)
 
         try:
             self.results = requests.get(url=url, data=data, headers=headers, **kwargs)
             self._log_result()
             return True
         except Exception as e:
+            self.errors = e
             log.error(f'get failed. {e}', enable_traceback=False)
         return False
 
     def patch(self,
               url: str = None,
               data: dict = None,
               headers: dict = None, **kwargs) -> bool:
@@ -98,14 +106,15 @@
         url, data, headers = self._params(url, data, headers)
 
         try:
             self.results = requests.patch(url=url, data=data, headers=headers, **kwargs)
             self._log_result()
             return True
         except Exception as e:
+            self.errors = e
             log.error(f'patch failed. {e}', enable_traceback=False)
         return False
 
     def post(self,
              url: str = None,
              data: dict = None,
              headers: dict = None, **kwargs) -> bool:
@@ -114,14 +123,15 @@
         url, data, headers = self._params(url, data, headers)
 
         try:
             self.results = requests.post(url=url, data=data, headers=headers, **kwargs)
             self._log_result()
             return True
         except Exception as e:
+            self.errors = e
             log.error(f'post failed. {e}', enable_traceback=False)
         return False
 
     def put(self,
             url: str = None,
             data: dict = None,
             headers: dict = None, **kwargs) -> bool:
@@ -130,14 +140,15 @@
         url, data, headers = self._params(url, data, headers)
 
         try:
             self.results = requests.put(url=url, data=data, headers=headers, **kwargs)
             self._log_result()
             return True
         except Exception as e:
+            self.errors = e
             log.error(f'put failed. {e}', enable_traceback=False)
         return False
 
     def to_dict(self):
         if self.results is not None:
             return json.loads(self.results.content)
```

### Comparing `automonisaur-0.2.9/automon/integrations/selenium/actions.py` & `automonisaur-0.3.0/automon/integrations/seleniumWrapper/actions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from selenium.webdriver.common.action_chains import ActionChains
 
 from automon.log import Logging
 
-log = Logging(name='selenium', level=Logging.INFO)
+log = Logging(name='SeleniumActions', level=Logging.INFO)
 
 
 class SeleniumActions:
     @staticmethod
     def click(browser, xpath):
         """Given an xpath, it will click it
```

### Comparing `automonisaur-0.2.9/automon/integrations/sentryio/client.py` & `automonisaur-0.3.0/automon/integrations/sentryio/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/sentryio/config.py` & `automonisaur-0.3.0/automon/integrations/sentryio/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sentry_sdk import set_level
 
-from automon.helpers.os import environ
+from automon.helpers.osWrapper import environ
 
 
 class SentryConfig(object):
     def __init__(self, dsn: str = None,
                  environment: str = None,
                  release: str = None,
                  debug: bool = False,
```

### Comparing `automonisaur-0.2.9/automon/integrations/shodan/__init__.py` & `automonisaur-0.3.0/automon/integrations/shodan/__init__.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/slack/bots.py` & `automonisaur-0.3.0/automon/integrations/slackWrapper/bots.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/slack/client.py` & `automonisaur-0.3.0/automon/integrations/slackWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/slack/clientAsync.py` & `automonisaur-0.3.0/automon/integrations/slackWrapper/clientAsync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import slack
 import random
 import asyncio
 
 from automon.log import Logging
-from automon.helpers.asyncio_ import AsyncStarter
+from automon.helpers.nest_asyncioWrapper import AsyncStarter
 
 from .config import ConfigSlack
 from .bots import BotInfo
 from .error import SlackError
 
 
 class SlackAsyncClient(ConfigSlack):
```

### Comparing `automonisaur-0.2.9/automon/integrations/slack/config.py` & `automonisaur-0.3.0/automon/integrations/slackWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/slack/error.py` & `automonisaur-0.3.0/automon/integrations/slackWrapper/error.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/slack/slack_formatting.py` & `automonisaur-0.3.0/automon/integrations/slackWrapper/slack_formatting.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/slack/slack_logger.py` & `automonisaur-0.3.0/automon/integrations/slackWrapper/slack_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import asyncio
 import traceback
 
 from json import dumps
 from asyncio import sleep
 
-from automon.helpers.asyncio_ import AsyncStarter
-from automon.integrations.slack.client import SlackClient
+from automon.helpers.nest_asyncioWrapper import AsyncStarter
+from automon.integrations.slackWrapper.client import SlackClient
 
-from automon.integrations.slack.slack_formatting import Emoji, Chat, Format
+from automon.integrations.slackWrapper.slack_formatting import Emoji, Chat, Format
 from automon.log import Logging, INFO, ERROR, WARN, CRITICAL, DEBUG
 
 
 class AsyncSlackLogging(SlackClient):
 
     def __init__(self, slack: SlackClient = None,
                  username: str = '',
```

### Comparing `automonisaur-0.2.9/automon/integrations/snmp/generate_maps.py` & `automonisaur-0.3.0/automon/integrations/snmp/generate_maps.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 import re
 import yaml
 import xmltodict
 import subprocess
 
-from automon.integrations.slack.slack_formatting import Chat
+from automon.integrations.slackWrapper.slack_formatting import Chat
 from automon.log import Logging
 
 log = Logging(__name__, level=Logging.INFO)
 
 
 class SmidumpFormat:
     """smidump output formats"""
```

### Comparing `automonisaur-0.2.9/automon/integrations/splunk/client.py` & `automonisaur-0.3.0/automon/integrations/splunk/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,79 @@
+import functools
 from queue import Queue
 
 import splunklib.results
-import splunklib.client as client
+import splunklib.client
 
 from automon.log import Logging
 from automon.integrations.splunk.config import SplunkConfig
 from automon.integrations.splunk.helpers import Job, Application
 
-log = Logging(name=__name__, level=Logging.DEBUG)
+log = Logging(name='SplunkClient', level=Logging.DEBUG)
 
 
 class SplunkRestClient:
 
     def __int__(self, config: SplunkConfig = SplunkConfig()):
-        self._log = Logging(SplunkRestClient.__name__, level=Logging.DEBUG)
         self.config = config
 
 
 class SplunkClient(object):
 
     def __init__(self, config: SplunkConfig = None):
-        self._log = Logging(SplunkClient.__name__, level=Logging.DEBUG)
+        """Splunk client"""
+
         self.config = config or SplunkConfig()
+        self.queue = Queue()
 
-        try:
-            self.client = client.connect(
-                host=self.config.host,
-                port=self.config.port,
-                username=self.config.username,
-                password=self.config.password,
-                verify=self.config.verify,
-                scheme=self.config.scheme,
-                app=self.config.app,
-                owner=self.config.owner,
-                token=self.config.token,
-                cookie=self.config.cookie,
-                handler=self.config.handler
-            )
-
-            # referred to as a service in docs
-            self.service = self.client
-            self.connected = True
-            assert isinstance(self.service, client.Service)
-
-        except Exception as e:
-            self.connected = False
-            self._log.error(f'{e}\t{self.config.host}:{self.config.port}', enable_traceback=False)
+    def __str__(self):
+        if self.is_connected():
+            return f'connected to {self.config}'
+        return f'not connected to {self.config}'
 
-        self.queue = Queue()
+    @property
+    def client(self) -> splunklib.client.connect:
+        return splunklib.client.connect(
+            host=self.config.host,
+            port=self.config.port,
+            username=self.config.username,
+            password=self.config.password,
+            verify=self.config.verify,
+            scheme=self.config.scheme,
+            app=self.config.app,
+            owner=self.config.owner,
+            token=self.config.token,
+            cookie=self.config.cookie,
+            handler=self.config.handler
+        )
+
+    @property
+    def service(self) -> splunklib.client.connect:
+        return self.client()
+
+    def _is_connected(func):
+        @functools.wraps(func)
+        def wrapped(self, *args, **kwargs):
+            try:
+                self.client
+                return func(self, *args, **kwargs)
+            except Exception as e:
+                log.error(f'not connected. {e}', enable_traceback=False)
+            return False
+
+        return wrapped
+
+    @_is_connected
+    def is_connected(self) -> bool:
+        return True
 
     def info(self):
         return f'{self}'
 
-    def search(self, query):
+    def search(self, query) -> list:
         """create normal search query"""
         kwargs_normalsearch = {"exec_mode": "normal"}
         job = self.create_job(query, **kwargs_normalsearch)
         # job = self.create_job(query)
         return self.results(job)
 
     def oneshot(self, query, earliest_time: str = '-15m', latest_time: str = 'now'):
@@ -82,41 +99,36 @@
         return self.service.jobs
 
     def create_job(self, query, **kwargs):
         """create search job"""
         return self.service.jobs.create(query, **kwargs)
 
     @staticmethod
-    def results(job: client.Job):
+    def results(job: splunklib.client.Job) -> list:
         """io blocking waiting for job results"""
         j = Job(job)
         while True:
             while not j.is_ready():
                 pass
             if j.isDone == '1':
                 break
 
         results = [x for x in splunklib.results.ResultsReader(j.results())]
         return results
 
     def job_summary(self):
         return f'There are {len(self.jobs())} jobs available to the current user'
 
-    def get_apps(self):
+    def get_apps(self) -> [Application]:
         return [Application(x) for x in self.service.apps]
 
     def create_app(self, app_name):
         return self.service.apps.create(app_name)
 
     def get_app(self, app_name):
         return self.service.apps[app_name]
 
     def delete_app(self, app_name):
         return self.service.apps.delete(app_name)
 
     def app_info(self, app_name):
         return f'{self.service.apps[app_name]}'
-
-    def __str__(self):
-        if self.connected:
-            return f'connected to {self.config}'
-        return f'not connected to {self.config}'
```

### Comparing `automonisaur-0.2.9/automon/integrations/splunk/config.py` & `automonisaur-0.3.0/automon/integrations/splunk/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,40 @@
-import os
-
 import splunklib.binding as binding
 
 from automon.log import Logging
+from automon.helpers import environ
+
+log = Logging(name='SplunkConfig', level=Logging.DEBUG)
 
 
 class SplunkConfig:
-    def __init__(self, host: str = None, port: int = None, username: str = None,
-                 password: str = None, verify: str = True, scheme: str = 'https',
-                 app: NotImplemented = None, owner: NotImplemented = None,
-                 token: str = None, cookie: str = None, timeout: int = 1):
-        self._log = Logging(name=SplunkConfig.__name__, level=Logging.DEBUG)
-
-        self.host = host or os.getenv('SPLUNK_HOST') or 'splunkcloud.com'
-        self.port = port or os.getenv('SPLUNK_PORT') or 8090
-        self.username = username or os.getenv('SPLUNK_USERNAME') or 'admin'
-        self.password = password or os.getenv('SPLUNK_PASSWORD') or 'changeme'
+    def __init__(self,
+                 host: str = None,
+                 port: int = None,
+                 username: str = None,
+                 password: str = None,
+                 verify: str = True,
+                 scheme: str = 'https',
+                 app: NotImplemented = None,
+                 owner: NotImplemented = None,
+                 token: str = None,
+                 cookie: str = None,
+                 timeout: int = 1):
+        """Splunk config"""
+
+        self.host = host or environ('SPLUNK_HOST', 'splunkcloud.com')
+        self.port = port or environ('SPLUNK_PORT', 8089)
+        self.username = username or environ('SPLUNK_USERNAME', 'admin')
+        self.password = password or environ('SPLUNK_PASSWORD', 'changeme')
         self.verify = verify
         self.scheme = scheme or 'https'
         self.app = app
         self.owner = owner
         self.token = token
         self.cookie = cookie
         self.handler = binding.handler(timeout=timeout)
 
     def info(self):
         return f'{self}'
 
     def __str__(self):
-        return f'{self.username}@{self.scheme}://{self.host}:{self.port}'
+        return f'{self.__dict__}'
```

### Comparing `automonisaur-0.2.9/automon/integrations/splunk/helpers.py` & `automonisaur-0.3.0/automon/integrations/splunk/helpers.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/splunk_soar/common.py` & `automonisaur-0.3.0/automon/integrations/splunk_soar/datatypes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 import datetime
 
 from dateutil import parser
 
-from automon import Logging
+from automon.log import Logging
 
-log = Logging('Scaffolding', level=Logging.DEBUG)
+log = Logging('AbstractDataType', level=Logging.DEBUG)
 
 
-class Scaffolding:
+class AbstractDataType:
     def __init__(self, data: dict):
         self.__dict__.update(data)
 
     def __repr__(self):
         return self.to_json()
 
     def __len__(self):
```

### Comparing `automonisaur-0.2.9/automon/integrations/splunk_soar/config.py` & `automonisaur-0.3.0/automon/integrations/splunk_soar/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from automon import Logging
-from automon.helpers.os import environ
+from automon.log import Logging
+from automon.helpers.osWrapper import environ
 
 log = Logging(name='SplunkSoarConfig', level=Logging.DEBUG)
 
 
 class SplunkSoarConfig:
     def __init__(self, host: str = None,
                  user: str = None,
@@ -21,12 +21,13 @@
 
         if not self.host:
             log.warn(f'missing SPLUNK_SOAR_HOST')
 
     def __repr__(self):
         return f'{self.__dict__}'
 
-    def isReady(self):
+    @property
+    def is_ready(self) -> bool:
         if self.host:
             return True
         log.warn(f'bad config')
         return False
```

### Comparing `automonisaur-0.2.9/automon/integrations/splunk_soar/phantom_unittest.py` & `automonisaur-0.3.0/automon/integrations/splunk_soar/phantom_unittest.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         'artifact_id'
     ]
 
 
 def artifact(id_value: int = 0, source_data_identifier_value: str = '', results_item_1: list = results()):
     return {
             'container_id': id_value,
-            'name': "Marriott User Validation",
+            'name': "User Validation",
             'contains': "{}",
             'source_data_identifier': source_data_identifier_value,
             'label': "enrich",
             'cef_value': "",
             'dedup_is_success': True,
             'run_automation': False,
             'cef_name': "",
```

### Comparing `automonisaur-0.2.9/automon/integrations/splunk_soar/rules.py` & `automonisaur-0.3.0/automon/integrations/splunk_soar/rules.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/swift/client.py` & `automonisaur-0.3.0/automon/integrations/swift/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/swift/config.py` & `automonisaur-0.3.0/automon/integrations/swift/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/swift/error.py` & `automonisaur-0.3.0/automon/integrations/swift/error.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/swift/iterables.py` & `automonisaur-0.3.0/automon/integrations/swift/iterables.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/integrations/vds/client.py` & `automonisaur-0.3.0/automon/integrations/vds/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/log/logger.py` & `automonisaur-0.3.0/automon/log/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,30 +82,32 @@
         return self.logs
 
 
 class Logging(object):
     """Standard logging
     """
 
-    TEST = 5
-    DEBUG = DEBUG
-    INFO = INFO
-    WARN = WARN
-    ERROR = ERROR
-    CRITICAL = CRITICAL
-    NOTSET = NOTSET
+    TEST: int = 5
+    DEBUG: int = DEBUG
+    INFO: int = INFO
+    WARN: int = WARN
+    ERROR: int = ERROR
+    CRITICAL: int = CRITICAL
+    NOTSET: int = NOTSET
 
     def __init__(self, name: str = __name__,
                  level: int = INFO,
                  file: str = None,
                  encoding: str = 'utf-8',
                  filemode: str = 'a',
                  log_stream: LogStream = False,
+                 log_format: str = None,
                  callbacks: list = None,
-                 timestamp: bool = True, *args, **kwargs):
+                 timestamp: bool = True,
+                 *args, **kwargs):
 
         self.started = Dates.now()
 
         self.logging = logging.getLogger(name)
         self.logging.setLevel(level)
 
         self.callbacks = callbacks or []
@@ -119,18 +121,22 @@
         filename = '%(filename)s'
         pathname = '%(pathname)s'
         func = '%(funcName)s'
         line = '%(lineno)d'
         module = '%(module)s'
         message = '%(message)s'
 
-        # self.log_format = f'{levelname}\t[{logger}]\t{message}'
-        self.log_format = f'{levelname}\t[{logger}]\t[{filename} {func}:L{line}]\t{message}'
-        # self.log_format = '%(levelname)s\t%(message)s\t%(name)s'
-        # self.log_format = '%(levelname)s\t%(name)s\t%(module)s\t%(message)s'
+        if log_format:
+            self.log_format = log_format
+        else:
+            # self.log_format = f'{levelname}\t{message}'
+            self.log_format = f'{levelname}\t[{logger}]\t{message}'
+            # self.log_format = f'{levelname}\t[{logger}]\t[{filename} {func}:L{line}]\t{message}'
+            # self.log_format = '%(levelname)s\t%(message)s\t%(name)s'
+            # self.log_format = '%(levelname)s\t%(name)s\t%(module)s\t%(message)s'
 
         if timestamp:
             self.log_format = f'{time}\t{self.log_format}'
 
         logging.basicConfig(level=level, format=self.log_format, **kwargs)
 
         if file:
```

### Comparing `automonisaur-0.2.9/automon/tests/core/test_assertions.py` & `automonisaur-0.3.0/automon/helpers/tests/test_assertions.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/tests/core/test_logger.py` & `automonisaur-0.3.0/automon/log/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/tests/core/test_networking.py` & `automonisaur-0.3.0/automon/helpers/tests/test_networking.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/tests/core/test_runner.py` & `automonisaur-0.3.0/automon/helpers/tests/test_runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from automon.helpers.subprocess import Run
+from automon.helpers import Run
 
 
 class RunTest(unittest.TestCase):
     r = Run()
 
     def test_Run(self):
         self.assertTrue(Run)
```

### Comparing `automonisaur-0.2.9/automon/tests/core/test_sanitation.py` & `automonisaur-0.3.0/automon/helpers/tests/test_sanitation.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/tests/core/test_sleeper.py` & `automonisaur-0.3.0/automon/helpers/tests/test_sleeper.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/tests/integrations/airport/test_airport.py` & `automonisaur-0.3.0/automon/integrations/mac/airport/tests/test_airport.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,17 @@
     def test_summary(self):
         if self.a.isReady():
             self.assertTrue(self.a.scan_summary())
             self.assertTrue(self.a.scan_summary(0))
 
     def test_xml(self):
         if self.a.isReady():
-            self.assertTrue(self.a.scan_xml())
+            scan = self.a.scan_xml()
+            if scan:
+                self.assertTrue(scan)
             self.assertFalse(self.a.scan_xml(0))
 
     def test_set_channel(self):
         if self.a.isReady():
             pass
             # self.assertTrue(self.a.set_channel(10))
```

### Comparing `automonisaur-0.2.9/automon/tests/integrations/airport/test_airport_neo4j.py` & `automonisaur-0.3.0/automon/integrations/mac/airport/tests/test_airport_neo4j.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import sys
 import unittest
 
 from automon.integrations.mac.airport import Airport
 
-from automon.integrations.neo4j import Neo4jClient
+from automon.integrations.neo4jWrapper import Neo4jClient
 
 
 class AirportToNeo4jTest(unittest.TestCase):
     a = Airport()
     n = Neo4jClient()
 
     def test_scan_xml(self):
         if self.a.isReady():
-            self.assertTrue(self.a.scan_xml())
+            test = self.a.scan_xml()
+            if test:
+                self.assertTrue(test)
 
         if self.n.isConnected():
             # self.n.delete_all()
             for bssid in self.a.ssids:
                 flatten = bssid._ssid
                 flatten.update(bssid.__dict__)
                 flatten.pop('_ssid')
```

### Comparing `automonisaur-0.2.9/automon/tests/integrations/elasticsearch/test_elasticsearch.py` & `automonisaur-0.3.0/automon/integrations/elasticsearch/tests/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/tests/integrations/elasticsearch/test_elasticsearch_JvmMonitor.py` & `automonisaur-0.3.0/automon/integrations/elasticsearch/tests/test_elasticsearch_JvmMonitor.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/tests/integrations/elasticsearch/test_elasticsearch_snapshot.py` & `automonisaur-0.3.0/automon/integrations/elasticsearch/tests/test_elasticsearch_snapshot.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/tests/integrations/minio/test_minio_client.py` & `automonisaur-0.3.0/automon/integrations/minioWrapper/tests/test_minio_client_public.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 import unittest
 import hashlib
 
-from automon.integrations.minio.client import MinioClient
+from automon.integrations.minioWrapper import MinioClient
+from automon.integrations.minioWrapper.bucket import Bucket
 
+MINIO_ENDPOINT = 'play.minio.io:9000'
+MINIO_ACCESS_KEY = 'Q3AM3UQ867SPQQA43P2F'
+MINIO_SECRET_KEY = 'zuf+tfteSlswRu7BJ86wekitnifILbZam1KYY3TG'
 
-class Client(unittest.TestCase):
+client = MinioClient(endpoint=MINIO_ENDPOINT, access_key=MINIO_ACCESS_KEY, secret_key=MINIO_SECRET_KEY)
+bucket = hashlib.md5(f'{MINIO_ENDPOINT}'.encode()).hexdigest()
 
-    def test_MinioClient(self):
-        self.assertTrue(MinioClient())
-        self.assertTrue(MinioClient)
 
-    def test_publicServer(self):
-        MINIO_ENDPOINT = 'play.minio.io:9000'
-        MINIO_ACCESS_KEY = 'Q3AM3UQ867SPQQA43P2F'
-        MINIO_SECRET_KEY = 'zuf+tfteSlswRu7BJ86wekitnifILbZam1KYY3TG'
+class ClientTest(unittest.TestCase):
 
-        m = MinioClient(endpoint=MINIO_ENDPOINT, access_key=MINIO_ACCESS_KEY, secret_key=MINIO_SECRET_KEY)
-        bucket = hashlib.md5(f'{MINIO_ENDPOINT}'.encode()).hexdigest()
+    def test_list_buckets(self):
+        if client.is_connected():
+            self.assertTrue(client.list_buckets())
+            self.assertEqual(type(client.list_buckets()), list)
 
-        if m.isConnected():
+    def test_get_bucket(self):
+        if client.is_connected():
+            test = client.make_bucket(bucket)
 
-            self.assertTrue(len(m.list_buckets()) >= 0)   # this might fail if no buckets
-            self.assertTrue(type(m.list_buckets()), list)
-            self.assertTrue(type(m.list_buckets(bucket)), list)
-
-            if m.list_buckets(bucket):
-                self.assertTrue(m.remove_bucket(bucket))
-            else:
-                self.assertTrue(m.make_bucket(bucket))
+            self.assertTrue(client.get_bucket(test))
+            self.assertTrue(type(client.get_bucket(test)), Bucket)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `automonisaur-0.2.9/automon/tests/integrations/neo4j/test_neo4j_client.py` & `automonisaur-0.3.0/automon/integrations/neo4jWrapper/tests/test_neo4j_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 
-from automon.integrations.neo4j.client import Neo4jClient
-from automon.integrations.neo4j.cypher import Cypher
+from automon.integrations.neo4jWrapper.client import Neo4jClient
+from automon.integrations.neo4jWrapper.cypher import Cypher
 
 
 class Neo4jTest(unittest.TestCase):
     client = Neo4jClient()
 
     def test_build_cypher(self):
         c = Neo4jClient()
```

### Comparing `automonisaur-0.2.9/automon/tests/integrations/neo4j/test_neo4j_config.py` & `automonisaur-0.3.0/automon/integrations/neo4jWrapper/tests/test_neo4j_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from automon.integrations.neo4j.config import Neo4jConfig
+from automon.integrations.neo4jWrapper.config import Neo4jConfig
 
 
 class ConfigTest(unittest.TestCase):
     c = Neo4jConfig()
 
     def test_config(self):
         self.assertTrue(Neo4jConfig)
```

### Comparing `automonisaur-0.2.9/automon/tests/integrations/neo4j/test_neo4j_cypher.py` & `automonisaur-0.3.0/automon/integrations/neo4jWrapper/tests/test_neo4j_cypher.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from automon.integrations.neo4j.client import Neo4jClient
+from automon.integrations.neo4jWrapper.client import Neo4jClient
 
 
 class Neo4jTest(unittest.TestCase):
     client = Neo4jClient()
 
     def test_cypher(self):
         if self.client.isConnected():
```

### Comparing `automonisaur-0.2.9/automon/tests/integrations/nmap/test_nmap_client.py` & `automonisaur-0.3.0/automon/integrations/nmap/tests/test_nmap_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/tests/integrations/sentryio/test_sentryio.py` & `automonisaur-0.3.0/automon/integrations/sentryio/tests/test_sentryio.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/tests/integrations/sentryio/test_sentryio_callback.py` & `automonisaur-0.3.0/automon/integrations/sentryio/tests/test_sentryio_callback.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from automon import Logging
+from automon.log import Logging
 from automon.integrations.sentryio.client import SentryClient
 
 
 class CallbackTest(unittest.TestCase):
     sentry = SentryClient()
     log = Logging(name=__name__, level=Logging.DEBUG)
     log.callbacks.append(sentry)
```

### Comparing `automonisaur-0.2.9/automon/tests/integrations/splunk_soar/test_soar_client.py` & `automonisaur-0.3.0/automon/integrations/splunk_soar/tests/test_soar_client.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,49 +2,46 @@
 
 from automon.integrations.splunk_soar import SplunkSoarClient
 
 c = SplunkSoarClient()
 
 
 class TestClient(unittest.TestCase):
-
-    def test_isConnected(self):
-        if c.isConnected():
-            self.assertTrue(c.isConnected())
-        else:
-            self.assertFalse(c.isConnected())
-
-    def test_create_artifact(self):
-        if c.isConnected():
+    if c.is_connected():
+        def test_create_artifact(self):
             id = c.create_container(label='testing', name='testing').id
             self.assertTrue(c.create_artifact(container_id=id))
-        else:
-            self.assertFalse(c.create_artifact(container_id=0))
 
-    def test_create_container(self):
-        if c.isConnected():
+        def test_create_container(self):
             self.assertTrue(c.create_container(label='testing', name='testing'))
-        else:
-            self.assertFalse(c.create_container(label='testing', name='testing'))
 
-    def test_delete_containers(self):
-        if c.isConnected():
-            id = c.create_container(label='testing', name='testing').id
-            self.assertTrue(c.delete_container(container_id=id))
-        else:
-            self.assertFalse(c.delete_container(container_id=0))
+        def test_delete_containers(self):
+            container = c.create_container(label='testing', name='testing')
+            self.assertTrue(c.delete_container(container_id=container.id))
+
+        def test_get_container(self):
+            container = c.create_container(label='testing', name='testing')
+            self.assertTrue(c.get_container(container_id=container.id))
+
+        def test_get_vault(self):
+            container = c.create_container(label='testing', name='testing')
+
+            list_vault = c.list_vault()
+            vault = list_vault.get_one()
+            if vault:
+                self.assertTrue(c.get_vault(vault_id=vault.id))
 
-    def test_list_artifact(self):
-        if c.isConnected():
+        def test_isConnected(self):
+            self.assertTrue(c.is_connected())
+
+        def test_list_artifact(self):
             self.assertTrue(c.list_artifact())
-        else:
-            self.assertFalse(c.list_artifact())
 
-    def test_list_containers(self):
-        if c.isConnected():
+        def test_list_containers(self):
             self.assertTrue(c.list_containers())
-        else:
-            self.assertFalse(c.list_containers())
+
+        def test_list_vault(self):
+            self.assertTrue(c.list_vault())
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `automonisaur-0.2.9/automon/tests/integrations/test_crypto.py` & `automonisaur-0.3.0/automon/integrations/cryptocurrency/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/tests/integrations/test_datascience.py` & `automonisaur-0.3.0/automon/integrations/datascience/tests/test_datascience.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/automon/tests/integrations/test_flask.py` & `automonisaur-0.3.0/automon/integrations/flaskWrapper/tests/test_flask.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 
 from flask import Flask
 
-from automon.integrations.flask.boilerplate import FlaskBoilerplate
-from automon.integrations.flask.config import FlaskConfig
+from automon.integrations.flaskWrapper.boilerplate import FlaskBoilerplate
+from automon.integrations.flaskWrapper.config import FlaskConfig
 
 
 class FlaskTest(unittest.TestCase):
     app = Flask(__name__)
 
     def test_FlaskBoilerplate(self):
         self.assertTrue(FlaskBoilerplate)
```

### Comparing `automonisaur-0.2.9/automon/tests/integrations/test_slack.py` & `automonisaur-0.3.0/automon/integrations/slackWrapper/tests/test_slack.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 
-from automon.integrations.slack.client import SlackClient
-from automon.integrations.slack.error import SlackError
-from automon.integrations.slack.bots import BotInfo
-from automon.integrations.slack.config import SlackConfig
-from automon.integrations.slack.slack_formatting import Format, Chat, Emoji
+from automon.integrations.slackWrapper.client import SlackClient
+from automon.integrations.slackWrapper.error import SlackError
+from automon.integrations.slackWrapper.bots import BotInfo
+from automon.integrations.slackWrapper.config import SlackConfig
+from automon.integrations.slackWrapper.slack_formatting import Format, Chat, Emoji
 
 
 class ConfigTest(unittest.TestCase):
     def test_SlackConfig(self):
         self.assertTrue(SlackConfig())
```

### Comparing `automonisaur-0.2.9/automon/tests/integrations/test_swift.py` & `automonisaur-0.3.0/automon/integrations/swift/tests/test_swift.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.2.9/setup.py` & `automonisaur-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="automonisaur",
-    version="0.2.9",
+    version="0.3.0",
     author="naisanza",
     author_email="naisanza@gmail.com",
     description="Core libraries for automonisaur",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TheShellLand/automonisaur",
     packages=setuptools.find_packages(),
+    tests_require=["pytest"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.6',
     install_requires=[]
 )
```

