# Comparing `tmp/vbcore-2.1.0rc0.tar.gz` & `tmp/vbcore-2.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbcore-2.1.0rc0.tar", last modified: Mon Jul  3 22:48:18 2023, max compression
+gzip compressed data, was "vbcore-2.2.0rc0.tar", last modified: Wed Jul  5 22:55:40 2023, max compression
```

## Comparing `vbcore-2.1.0rc0.tar` & `vbcore-2.2.0rc0.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.827467 vbcore-2.1.0rc0/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      402 2023-07-03 22:48:18.827467 vbcore-2.1.0rc0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.806467 vbcore-2.1.0rc0/requirements/
--rw-rw-rw-   0 root         (0) root         (0)      222 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-all.in
--rw-rw-rw-   0 root         (0) root         (0)     5202 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-all.txt
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-build.in
--rw-rw-rw-   0 root         (0) root         (0)     2093 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-build.txt
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-crypto.in
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-crypto.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-db.in
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-db.txt
--rw-rw-rw-   0 root         (0) root         (0)      384 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-dev.in
--rw-rw-rw-   0 root         (0) root         (0)     5233 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-extra.in
--rw-rw-rw-   0 root         (0) root         (0)     1303 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-extra.txt
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-http.in
--rw-rw-rw-   0 root         (0) root         (0)     1142 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-http.txt
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-net.in
--rw-rw-rw-   0 root         (0) root         (0)      945 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-net.txt
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-scheduler.in
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-scheduler.txt
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-test.in
--rw-rw-rw-   0 root         (0) root         (0)     1755 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)      790 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/requirements/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 22:48:18.827467 vbcore-2.1.0rc0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     4745 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.809467 vbcore-2.1.0rc0/vbcore/
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     1686 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/aio.py
--rw-rw-rw-   0 root         (0) root         (0)     4716 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/base.py
--rw-rw-rw-   0 root         (0) root         (0)     7460 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/batch.py
--rw-rw-rw-   0 root         (0) root         (0)     1396 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/configurator.py
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.811467 vbcore-2.1.0rc0/vbcore/crypto/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/crypto/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1266 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/crypto/argon.py
--rw-rw-rw-   0 root         (0) root         (0)      942 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/crypto/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1093 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/crypto/bcrypt.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/crypto/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1193 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/crypto/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1213 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/crypto/hashes.py
--rw-rw-rw-   0 root         (0) root         (0)     4635 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/csvfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.811467 vbcore-2.1.0rc0/vbcore/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.812467 vbcore-2.1.0rc0/vbcore/data/transformations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/transformations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.813467 vbcore-2.1.0rc0/vbcore/data/transformations/builders/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/transformations/builders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/transformations/builders/base.py
--rw-rw-rw-   0 root         (0) root         (0)     2026 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/transformations/builders/csv.py
--rw-rw-rw-   0 root         (0) root         (0)     5586 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/transformations/builders/dicttoxml.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/transformations/builders/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     5880 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/transformations/builders/html.py
--rw-rw-rw-   0 root         (0) root         (0)     1908 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/transformations/builders/json.py
--rw-rw-rw-   0 root         (0) root         (0)     2230 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/transformations/builders/xml.py
--rw-rw-rw-   0 root         (0) root         (0)     1593 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/data/transformations/builders/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.814467 vbcore-2.1.0rc0/vbcore/datastruct/
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/datastruct/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/datastruct/buffer.py
--rw-rw-rw-   0 root         (0) root         (0)     6158 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/datastruct/cache.py
--rw-rw-rw-   0 root         (0) root         (0)     2904 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/datastruct/dictionaries.py
--rw-rw-rw-   0 root         (0) root         (0)     2772 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/datastruct/lazy.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/datastruct/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/datastruct/orderer_set.py
--rw-rw-rw-   0 root         (0) root         (0)     4400 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/date_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.815467 vbcore-2.1.0rc0/vbcore/db/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15840 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/db/events.py
--rw-rw-rw-   0 root         (0) root         (0)     4935 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/db/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/db/listener.py
--rw-rw-rw-   0 root         (0) root         (0)     2997 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/db/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     6775 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/db/mysql_dumper.py
--rw-rw-rw-   0 root         (0) root         (0)     1826 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/db/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     4942 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/db/sqla.py
--rw-rw-rw-   0 root         (0) root         (0)     5600 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/db/support.py
--rw-rw-rw-   0 root         (0) root         (0)     2318 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/db/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.816467 vbcore-2.1.0rc0/vbcore/dictutils/
--rw-rw-rw-   0 root         (0) root         (0)      210 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/dictutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15745 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/dictutils/flatter_dict.py
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/dictutils/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     1032 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2350 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     1010 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3883 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3901 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/files.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.817467 vbcore-2.1.0rc0/vbcore/http/
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2938 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/batch.py
--rw-rw-rw-   0 root         (0) root         (0)     8181 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/client.py
--rw-rw-rw-   0 root         (0) root         (0)     3880 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/gql.py
--rw-rw-rw-   0 root         (0) root         (0)     3367 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/headers.py
--rw-rw-rw-   0 root         (0) root         (0)     2632 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/httpcode.py
--rw-rw-rw-   0 root         (0) root         (0)     4012 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/httpdumper.py
--rw-rw-rw-   0 root         (0) root         (0)      445 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/methods.py
--rw-rw-rw-   0 root         (0) root         (0)     6063 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/proxy.py
--rw-rw-rw-   0 root         (0) root         (0)     1894 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/rpc.py
--rw-rw-rw-   0 root         (0) root         (0)     2128 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/http/useragent.py
--rw-rw-rw-   0 root         (0) root         (0)     4631 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/importer.py
--rw-rw-rw-   0 root         (0) root         (0)     5279 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/json.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.817467 vbcore-2.1.0rc0/vbcore/jsonschema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/jsonschema/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.818467 vbcore-2.1.0rc0/vbcore/jsonschema/schemas/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/jsonschema/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2118 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/jsonschema/schemas/jsonrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7052 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/jsonschema/support.py
--rw-rw-rw-   0 root         (0) root         (0)     2533 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/lambdas.py
--rw-rw-rw-   0 root         (0) root         (0)     5111 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/loggers.py
--rw-rw-rw-   0 root         (0) root         (0)     5173 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/misc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.818467 vbcore-2.1.0rc0/vbcore/net/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/net/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/net/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     5747 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/net/sendmail.py
--rw-rw-rw-   0 root         (0) root         (0)     5984 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/net/sftp.py
--rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/net/socks_smtp.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.819467 vbcore-2.1.0rc0/vbcore/rule_engine/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/rule_engine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/rule_engine/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3171 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/rule_engine/engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.819467 vbcore-2.1.0rc0/vbcore/standalone/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/standalone/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3310 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/standalone/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)     8327 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/standalone/wsgi_gunicorn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.819467 vbcore-2.1.0rc0/vbcore/stringutils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/stringutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1226 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/stringutils/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     2158 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/stringutils/notations.py
--rw-rw-rw-   0 root         (0) root         (0)     4449 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/system.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.820467 vbcore-2.1.0rc0/vbcore/tester/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tester/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16074 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tester/asserter.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tester/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tester/fetchmail.py
--rw-rw-rw-   0 root         (0) root         (0)     1963 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tester/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     7405 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tester/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.821467 vbcore-2.1.0rc0/vbcore/tester/plugins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tester/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      163 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tester/plugins/fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tester/plugins/startup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.822467 vbcore-2.1.0rc0/vbcore/tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6170 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      948 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/crypto.py
--rw-rw-rw-   0 root         (0) root         (0)     2111 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/database.py
--rw-rw-rw-   0 root         (0) root         (0)     1017 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.822467 vbcore-2.1.0rc0/vbcore/tools/initializer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1080 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.824467 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.bumpversion.cfg
--rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.dockerignore
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.editorconfig
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.flake8
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.824467 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.git-hooks/
--rwxrwxrwx   0 root         (0) root         (0)      179 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.git-hooks/pre-commit
--rwxrwxrwx   0 root         (0) root         (0)       30 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.git-hooks/pre-push
--rw-rw-rw-   0 root         (0) root         (0)     2205 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)    16254 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     4464 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.825466 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/devops/
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/devops/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)     2091 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/devops/gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.825466 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/devops/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/devops/scripts/build.sh
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/devops/scripts/dist-publish.sh
--rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/devops/scripts/fresh-install.sh
--rw-rw-rw-   0 root         (0) root         (0)      233 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/devops/scripts/test-builds.sh
--rw-rw-rw-   0 root         (0) root         (0)      801 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/liccheck.ini
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.826467 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       65 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/requirements/requirements-build.in
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/requirements/requirements-dev.in
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/requirements/requirements-test.in
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/requirements/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)     3738 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.826467 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/skel/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/skel/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.826467 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/skel/entrypoints/
--rw-rw-rw-   0 root         (0) root         (0)      419 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/skel/entrypoints/main.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/skel/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/skel/version.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/tox.ini
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)     1520 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/sendmail.py
--rw-rw-rw-   0 root         (0) root         (0)     2745 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/sftp.py
--rw-rw-rw-   0 root         (0) root         (0)     1561 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/tools/wsgi_gunicorn.py
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/types.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/version.py
--rw-rw-rw-   0 root         (0) root         (0)     2877 2023-07-03 22:48:07.000000 vbcore-2.1.0rc0/vbcore/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 22:48:18.810467 vbcore-2.1.0rc0/vbcore.egg-info/
--rw-r--r--   0 root         (0) root         (0)      402 2023-07-03 22:48:18.000000 vbcore-2.1.0rc0/vbcore.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5458 2023-07-03 22:48:18.000000 vbcore-2.1.0rc0/vbcore.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 22:48:18.000000 vbcore-2.1.0rc0/vbcore.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-07-03 22:48:18.000000 vbcore-2.1.0rc0/vbcore.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 22:48:18.000000 vbcore-2.1.0rc0/vbcore.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      590 2023-07-03 22:48:18.000000 vbcore-2.1.0rc0/vbcore.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-03 22:48:18.000000 vbcore-2.1.0rc0/vbcore.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:40.000091 vbcore-2.2.0rc0/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      402 2023-07-05 22:55:40.000091 vbcore-2.2.0rc0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.974091 vbcore-2.2.0rc0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)      222 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements-all.in
+-rw-rw-rw-   0 root         (0) root         (0)     5007 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements-all.txt
+-rw-rw-rw-   0 root         (0) root         (0)      245 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements-build.in
+-rw-rw-rw-   0 root         (0) root         (0)     2093 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements-build.txt
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements-crypto.in
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements-crypto.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements-db.in
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements-db.txt
+-rw-rw-rw-   0 root         (0) root         (0)      384 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements-dev.in
+-rw-rw-rw-   0 root         (0) root         (0)     5233 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements-extra.in
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements-extra.txt
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements-http.in
+-rw-rw-rw-   0 root         (0) root         (0)     1142 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements-http.txt
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements-net.in
+-rw-rw-rw-   0 root         (0) root         (0)      736 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements-net.txt
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements-scheduler.in
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements-scheduler.txt
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements-test.in
+-rw-rw-rw-   0 root         (0) root         (0)     1755 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)      790 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/requirements/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 22:55:40.000091 vbcore-2.2.0rc0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     4745 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.978091 vbcore-2.2.0rc0/vbcore/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7746 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/configurator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.981091 vbcore-2.2.0rc0/vbcore/crypto/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/crypto/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1266 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/crypto/argon.py
+-rw-rw-rw-   0 root         (0) root         (0)      942 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/crypto/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/crypto/bcrypt.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/crypto/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/crypto/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1213 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/crypto/hashes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4635 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/csvfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.981091 vbcore-2.2.0rc0/vbcore/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.981091 vbcore-2.2.0rc0/vbcore/data/transformations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/data/transformations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.983091 vbcore-2.2.0rc0/vbcore/data/transformations/builders/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/data/transformations/builders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/data/transformations/builders/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2026 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/data/transformations/builders/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)     5586 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/data/transformations/builders/dicttoxml.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/data/transformations/builders/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     5880 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/data/transformations/builders/html.py
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/data/transformations/builders/json.py
+-rw-rw-rw-   0 root         (0) root         (0)     2230 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/data/transformations/builders/xml.py
+-rw-rw-rw-   0 root         (0) root         (0)     1593 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/data/transformations/builders/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.984091 vbcore-2.2.0rc0/vbcore/datastruct/
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/datastruct/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/datastruct/buffer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6158 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/datastruct/cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     2904 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/datastruct/dictionaries.py
+-rw-rw-rw-   0 root         (0) root         (0)     2772 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/datastruct/lazy.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/datastruct/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1156 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/datastruct/orderer_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     4354 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/date_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.986091 vbcore-2.2.0rc0/vbcore/db/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15840 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/db/events.py
+-rw-rw-rw-   0 root         (0) root         (0)     4935 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/db/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/db/listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     2997 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/db/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     6774 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/db/mysql_dumper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1905 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/db/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4942 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/db/sqla.py
+-rw-rw-rw-   0 root         (0) root         (0)     5600 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/db/support.py
+-rw-rw-rw-   0 root         (0) root         (0)     2318 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/db/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.987091 vbcore-2.2.0rc0/vbcore/dictutils/
+-rw-rw-rw-   0 root         (0) root         (0)      210 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/dictutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15787 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/dictutils/flatter_dict.py
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/dictutils/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2350 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3883 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3901 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/files.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.989091 vbcore-2.2.0rc0/vbcore/http/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/http/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2863 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/http/batch.py
+-rw-rw-rw-   0 root         (0) root         (0)     8112 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/http/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     3880 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/http/gql.py
+-rw-rw-rw-   0 root         (0) root         (0)     3367 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/http/headers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2632 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/http/httpcode.py
+-rw-rw-rw-   0 root         (0) root         (0)     4012 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/http/httpdumper.py
+-rw-rw-rw-   0 root         (0) root         (0)      445 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/http/methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     6063 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/http/proxy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1894 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/http/rpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2143 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/http/useragent.py
+-rw-rw-rw-   0 root         (0) root         (0)     4590 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/importer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5279 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.989091 vbcore-2.2.0rc0/vbcore/jsonschema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/jsonschema/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.989091 vbcore-2.2.0rc0/vbcore/jsonschema/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/jsonschema/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2118 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/jsonschema/schemas/jsonrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7052 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/jsonschema/support.py
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/lambdas.py
+-rw-rw-rw-   0 root         (0) root         (0)     6516 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/loggers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5173 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/misc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.990091 vbcore-2.2.0rc0/vbcore/net/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/net/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7973 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/net/ftpclient.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/net/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5363 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/net/sendmail.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/net/socks_smtp.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.991091 vbcore-2.2.0rc0/vbcore/rule_engine/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/rule_engine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/rule_engine/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3171 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/rule_engine/engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.991091 vbcore-2.2.0rc0/vbcore/standalone/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/standalone/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3309 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/standalone/scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)     8327 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/standalone/wsgi_gunicorn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.992091 vbcore-2.2.0rc0/vbcore/stringutils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/stringutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1226 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/stringutils/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2158 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/stringutils/notations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4449 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/system.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.993091 vbcore-2.2.0rc0/vbcore/tester/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tester/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16074 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tester/asserter.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tester/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tester/fetchmail.py
+-rw-rw-rw-   0 root         (0) root         (0)     1963 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tester/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     7405 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tester/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.993091 vbcore-2.2.0rc0/vbcore/tester/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tester/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tester/plugins/fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tester/plugins/startup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.995091 vbcore-2.2.0rc0/vbcore/tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6170 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      948 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/crypto.py
+-rw-rw-rw-   0 root         (0) root         (0)     2111 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/entrypoint.py
+-rw-rw-rw-   0 root         (0) root         (0)     3542 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/ftpclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.995091 vbcore-2.2.0rc0/vbcore/tools/initializer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.997091 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/.bumpversion.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      360 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/.editorconfig
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/.flake8
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.998091 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/.git-hooks/
+-rwxrwxrwx   0 root         (0) root         (0)      179 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/.git-hooks/pre-commit
+-rwxrwxrwx   0 root         (0) root         (0)       30 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/.git-hooks/pre-push
+-rw-rw-rw-   0 root         (0) root         (0)     2205 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)    16254 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     4464 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.998091 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/devops/
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/devops/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)     2091 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/devops/gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.999091 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/devops/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/devops/scripts/build.sh
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/devops/scripts/dist-publish.sh
+-rw-rw-rw-   0 root         (0) root         (0)       71 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/devops/scripts/fresh-install.sh
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/devops/scripts/test-builds.sh
+-rw-rw-rw-   0 root         (0) root         (0)      801 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/liccheck.ini
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.999091 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/requirements/requirements-build.in
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/requirements/requirements-dev.in
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/requirements/requirements-test.in
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/requirements/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)     3738 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:40.000091 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/skel/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/skel/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:40.000091 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/skel/entrypoints/
+-rw-rw-rw-   0 root         (0) root         (0)      419 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/skel/entrypoints/main.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/skel/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/skel/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/tox.ini
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1520 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/sendmail.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/tools/wsgi_gunicorn.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/types.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2853 2023-07-05 22:55:28.000000 vbcore-2.2.0rc0/vbcore/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 22:55:39.979091 vbcore-2.2.0rc0/vbcore.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      402 2023-07-05 22:55:39.000000 vbcore-2.2.0rc0/vbcore.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5468 2023-07-05 22:55:39.000000 vbcore-2.2.0rc0/vbcore.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 22:55:39.000000 vbcore-2.2.0rc0/vbcore.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-05 22:55:39.000000 vbcore-2.2.0rc0/vbcore.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 22:55:39.000000 vbcore-2.2.0rc0/vbcore.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      558 2023-07-05 22:55:39.000000 vbcore-2.2.0rc0/vbcore.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-05 22:55:39.000000 vbcore-2.2.0rc0/vbcore.egg-info/top_level.txt
```

### Comparing `vbcore-2.1.0rc0/requirements/requirements-all.txt` & `vbcore-2.2.0rc0/requirements/requirements-all.txt`

 * *Files 2% similar despite different names*

```diff
@@ -61,20 +61,14 @@
     # via -r requirements/requirements.txt
 cryptography==41.0.1
     # via
     #   -r requirements/requirements-net.txt
     #   paramiko
 defusedxml==0.7.1
     # via -r requirements/requirements-extra.txt
-dnspython==2.3.0
-    # via
-    #   -r requirements/requirements-net.txt
-    #   email-validator
-email-validator==2.0.0.post2
-    # via -r requirements/requirements-net.txt
 frozenlist==1.3.3
     # via
     #   -r requirements/requirements-http.txt
     #   aiohttp
     #   aiosignal
 gql==3.4.1
     # via -r requirements/requirements-extra.txt
@@ -87,16 +81,15 @@
     #   -r requirements/requirements-db.txt
     #   sqlalchemy
 gunicorn==20.1.0
     # via -r requirements/requirements-extra.txt
 idna==3.4
     # via
     #   -r requirements/requirements-extra.txt
-    #   -r requirements/requirements-net.txt
-    #   email-validator
+    #   -r requirements/requirements-http.txt
     #   requests
     #   yarl
 jsonschema==4.17.3
     # via -r requirements/requirements-extra.txt
 multidict==6.0.4
     # via
     #   -r requirements/requirements-extra.txt
```

### Comparing `vbcore-2.1.0rc0/requirements/requirements-build.txt` & `vbcore-2.2.0rc0/requirements/requirements-build.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/requirements/requirements-crypto.txt` & `vbcore-2.2.0rc0/requirements/requirements-crypto.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/requirements/requirements-db.txt` & `vbcore-2.2.0rc0/requirements/requirements-db.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/requirements/requirements-dev.txt` & `vbcore-2.2.0rc0/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/requirements/requirements-extra.txt` & `vbcore-2.2.0rc0/requirements/requirements-extra.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/requirements/requirements-http.txt` & `vbcore-2.2.0rc0/requirements/requirements-http.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/requirements/requirements-net.txt` & `vbcore-2.2.0rc0/requirements/requirements-net.txt`

 * *Files 11% similar despite different names*

```diff
@@ -11,22 +11,14 @@
     #   -c requirements/requirements-build.txt
     #   cryptography
     #   pynacl
 cryptography==41.0.1
     # via
     #   -c requirements/requirements-build.txt
     #   paramiko
-dnspython==2.3.0
-    # via email-validator
-email-validator==2.0.0.post2
-    # via -r requirements/requirements-net.in
-idna==3.4
-    # via
-    #   -c requirements/requirements-build.txt
-    #   email-validator
 paramiko==3.2.0
     # via -r requirements/requirements-net.in
 pycparser==2.21
     # via
     #   -c requirements/requirements-build.txt
     #   cffi
 pynacl==1.5.0
```

### Comparing `vbcore-2.1.0rc0/requirements/requirements-scheduler.txt` & `vbcore-2.2.0rc0/requirements/requirements-scheduler.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/requirements/requirements-test.txt` & `vbcore-2.2.0rc0/requirements/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/requirements/requirements.txt` & `vbcore-2.2.0rc0/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/setup.py` & `vbcore-2.2.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/aio.py` & `vbcore-2.2.0rc0/vbcore/aio.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/batch.py` & `vbcore-2.2.0rc0/vbcore/batch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import abc
 import dataclasses
-import logging
 import threading
 import typing as t
 from contextlib import contextmanager
 from enum import auto
 from queue import Queue
 
 from vbcore import aio
 from vbcore.enums import StrEnum
+from vbcore.loggers import VBLoggerMixin
+from vbcore.types import OptDict
 
 
 class BatchExecutor:
     def __init__(self, tasks: t.Optional[list] = None, **__):
         self._tasks = tasks or []
 
     @staticmethod
@@ -56,15 +57,15 @@
 
 
 class Thread(threading.Thread):
     def __init__(
         self,
         runnable: t.Callable,
         *args,
-        params: t.Optional[dict] = None,
+        params: OptDict = None,
         daemon: bool = False,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self._runnable = runnable
         self._args = args
         self._params = params or {}
@@ -135,15 +136,14 @@
     worker_type: WorkersType = WorkersType.PRODUCER
 
 
 class PCTask(abc.ABC):
     def __init__(self, *args, **kwargs):
         self._args = args
         self._kwargs = kwargs
-        self._log = logging.getLogger(self.__module__)
 
     @abc.abstractmethod
     def perform(self, item):
         raise NotImplementedError
 
 
 class IProducerConsumerBatchExecutor(abc.ABC):
@@ -153,15 +153,14 @@
         consumer: PCTask,
         *_,
         **__,
     ):
         self._producer = producer
         self._consumer = consumer
         self.is_running: bool = False
-        self._log = logging.getLogger(self.__module__)
 
     @contextmanager
     def runner(self):
         if not self.is_running:
             self.startup()
         yield self
         self.barrier()
@@ -198,15 +197,15 @@
         """No producer required"""
 
     def load(self, item):
         product = self._producer.perform(item)
         self._consumer.perform(product)
 
 
-class ProducerConsumerBatchExecutor(IProducerConsumerBatchExecutor):
+class ProducerConsumerBatchExecutor(IProducerConsumerBatchExecutor, VBLoggerMixin):
     def __init__(
         self,
         producer: PCTask,
         consumer: PCTask,
         *args,
         batch_size: t.Optional[BatchSize] = None,
         thread_class: t.Type[Thread] = Thread,
@@ -234,39 +233,44 @@
 
     def start_threads(
         self,
         single: t.Tuple[t.Callable, WorkersType],
         workers: t.Tuple[t.Callable, WorkersType],
     ):
         self._thread_class(single[0], daemon=True, name=single[1]).start()
+        self.log.debug("started thread %s with %s", single[1], single[0])
         for num in range(0, self.size.pool_workers):
             name = f"{workers[1]}-{num+1}"
             self._thread_class(workers[0], daemon=True, name=name).start()
+            self.log.debug("started thread %s with %s", name, workers[0])
 
     def consumer(self):
         while True:
             item = self._consumer_queue.get()
+            self.log.debug("get item from consumer queue: %s", item)
             try:
                 self._consumer.perform(item)
             except Exception as exc:  # pylint: disable=broad-except
-                self._log.exception(exc)
+                self.log.exception(exc)
             finally:
                 self._consumer_queue.task_done()
 
     def producer(self):
         while True:
             item = self._producer_queue.get()
+            self.log.debug("get item from producer queue: %s", item)
             try:
                 item = self._producer.perform(item)
                 self._consumer_queue.put(item)
             except Exception as exc:  # pylint: disable=broad-except
-                self._log.exception(exc)
+                self.log.exception(exc)
             finally:
                 self._producer_queue.task_done()
 
     def barrier(self):
+        self.log.debug("lock barrier reached")
         self._producer_queue.join()
         self._consumer_queue.join()
         super().barrier()
 
     def load(self, item):
         self._producer_queue.put(item)
```

### Comparing `vbcore-2.1.0rc0/vbcore/configurator.py` & `vbcore-2.2.0rc0/vbcore/configurator.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import typing as t
 from collections import OrderedDict
 from functools import partial
 
 import decouple
 from dotenv import load_dotenv as base_load_dotenv
 
+from vbcore.types import OptAny
+
 _conf_search_path = os.environ.get("ENV_PATH")
 _conf_file_name = os.environ.get("ENV_FILE")
 _conf_file_encoding = os.environ.get("ENV_FILE_ENCODING") or "UTF-8"
 
 
 class AutoConfig(decouple.AutoConfig):
     encoding: str = _conf_file_encoding
@@ -21,18 +23,18 @@
         ]
     )
 
     @classmethod
     def from_environ(
         cls,
         key: str,
-        default=None,
-        required=True,
+        default: OptAny = None,
+        required: bool = True,
         cast: t.Callable[[str], t.Any] = str,
-    ):
+    ) -> t.Any:
         env_var = os.environ.get(key)
         if env_var:
             try:
                 return cast(env_var)
             except Exception as exc:
                 raise ValueError(
                     f"unable to cast config key '{key}' to type: {cast}"
```

### Comparing `vbcore-2.1.0rc0/vbcore/context.py` & `vbcore-2.2.0rc0/vbcore/context.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/crypto/argon.py` & `vbcore-2.2.0rc0/vbcore/crypto/argon.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/crypto/base.py` & `vbcore-2.2.0rc0/vbcore/crypto/base.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/crypto/bcrypt.py` & `vbcore-2.2.0rc0/vbcore/crypto/bcrypt.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/crypto/factory.py` & `vbcore-2.2.0rc0/vbcore/crypto/factory.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/crypto/hashes.py` & `vbcore-2.2.0rc0/vbcore/crypto/hashes.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/csvfile.py` & `vbcore-2.2.0rc0/vbcore/csvfile.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/data/transformations/builders/base.py` & `vbcore-2.2.0rc0/vbcore/data/transformations/builders/base.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/data/transformations/builders/csv.py` & `vbcore-2.2.0rc0/vbcore/data/transformations/builders/csv.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/data/transformations/builders/dicttoxml.py` & `vbcore-2.2.0rc0/vbcore/data/transformations/builders/dicttoxml.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/data/transformations/builders/factory.py` & `vbcore-2.2.0rc0/vbcore/data/transformations/builders/factory.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/data/transformations/builders/html.py` & `vbcore-2.2.0rc0/vbcore/data/transformations/builders/html.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/data/transformations/builders/json.py` & `vbcore-2.2.0rc0/vbcore/data/transformations/builders/json.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/data/transformations/builders/xml.py` & `vbcore-2.2.0rc0/vbcore/data/transformations/builders/xml.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/data/transformations/builders/yaml.py` & `vbcore-2.2.0rc0/vbcore/data/transformations/builders/yaml.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/datastruct/buffer.py` & `vbcore-2.2.0rc0/vbcore/datastruct/buffer.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/datastruct/cache.py` & `vbcore-2.2.0rc0/vbcore/datastruct/cache.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/datastruct/dictionaries.py` & `vbcore-2.2.0rc0/vbcore/datastruct/dictionaries.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/datastruct/lazy.py` & `vbcore-2.2.0rc0/vbcore/datastruct/lazy.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/datastruct/orderer_set.py` & `vbcore-2.2.0rc0/vbcore/datastruct/orderer_set.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/date_helper.py` & `vbcore-2.2.0rc0/vbcore/date_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import typing as t
 from datetime import datetime
 
 from dateutil.parser import parse as date_parse
 
 from vbcore.base import Static
-from vbcore.types import AnyDateType, DateType
+from vbcore.types import AnyDateType, DateType, OptStr
 
 
 class Millis(metaclass=Static):
     seconds: t.ClassVar[int] = 1000
     minute: t.ClassVar[int] = seconds * 60
     hour: t.ClassVar[int] = minute * 60
     day: t.ClassVar[int] = hour * 24
@@ -60,17 +60,17 @@
         return curr_date.weekday() > 4
 
     @classmethod
     def change_format(
         cls,
         str_date: str,
         out_fmt: str,
-        in_fmt: t.Optional[str] = None,
+        in_fmt: OptStr = None,
         raise_exc: bool = True,
-    ) -> t.Optional[str]:
+    ) -> OptStr:
         """
 
         :param str_date: input string date
         :param out_fmt: format output date
         :param in_fmt: format input date (optional: could be detected from string)
         :param raise_exc: raise or not exception (default True)
         :return: return formatted date
@@ -83,32 +83,32 @@
             return date_time.strftime(out_fmt)
         except (ValueError, TypeError):
             if raise_exc is True:
                 raise  # pragma: no cover
         return None
 
     @classmethod
-    def str_now(cls, is_utc: bool = True, tz=None, fmt: t.Optional[str] = None) -> str:
+    def str_now(cls, is_utc: bool = True, tz=None, fmt: OptStr = None) -> str:
         """
 
         :param is_utc:
         :param tz:
         :param fmt:
         :return:
         """
         now = datetime.utcnow() if is_utc else datetime.now(tz)
         return cls.date_to_str(now, fmt)
 
     @classmethod
-    def date_to_str(cls, date: DateType, fmt: t.Optional[str] = None) -> str:
+    def date_to_str(cls, date: DateType, fmt: OptStr = None) -> str:
         return date.strftime(fmt or DateTimeFmt.ISO)
 
     @classmethod
     def str_to_date(
-        cls, date: str, fmt: t.Optional[str] = None, is_iso: bool = False, **kwargs
+        cls, date: str, fmt: OptStr = None, is_iso: bool = False, **kwargs
     ) -> datetime:
         """
 
         :param date: input string date
         :param fmt: format input date (optional: could be detected from string)
         :param is_iso: flag for implicit iso format
         :param kwargs: passed to date_parse
@@ -136,12 +136,12 @@
     ) -> t.Optional[str]:
         return DateHelper.change_format(
             str_date, in_fmt=DateTimeFmt.ISO, out_fmt=fmt, raise_exc=exc
         )
 
     @classmethod
     def to_iso_format(
-        cls, str_date: str, fmt: t.Optional[str] = None, exc: bool = True
+        cls, str_date: str, fmt: OptStr = None, exc: bool = True
     ) -> t.Optional[str]:
         return DateHelper.change_format(
             str_date, in_fmt=fmt, out_fmt=DateTimeFmt.ISO, raise_exc=exc
         )
```

### Comparing `vbcore-2.1.0rc0/vbcore/db/events.py` & `vbcore-2.2.0rc0/vbcore/db/events.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/db/exceptions.py` & `vbcore-2.2.0rc0/vbcore/db/exceptions.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/db/listener.py` & `vbcore-2.2.0rc0/vbcore/db/listener.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/db/mixins.py` & `vbcore-2.2.0rc0/vbcore/db/mixins.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/db/mysql_dumper.py` & `vbcore-2.2.0rc0/vbcore/db/mysql_dumper.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import tarfile
 import typing as t
 from dataclasses import dataclass
 from datetime import datetime
 from itertools import groupby
 from subprocess import CompletedProcess, PIPE, run as run_subprocess  # nosec
 
-from vbcore.base import BaseLoggerMixin
 from vbcore.date_helper import DateTimeFmt
+from vbcore.loggers import VBLoggerMixin
 from vbcore.net.helpers import Url
 from vbcore.types import CoupleStr, OptInt, OptStr, StrList, StrTuple
 
 CmdLine = StrList
 
 
 @dataclass(frozen=True)
@@ -109,15 +109,15 @@
 
     def dump_table(self, database: str, table: str) -> MySQLDump:
         cmdline = self.mysqldump_cmdline(database=database, table=table)
         result = self.execute_binary(cmdline)
         return MySQLDump(database=database, table=table, dump=result.stdout)
 
 
-class MysqlBackup(BaseLoggerMixin):
+class MysqlBackup(VBLoggerMixin):
     def __init__(
         self,
         dumper: MySQLDumper,
         folder: str = ".",
         add_datetime: bool = True,
         datetime_format: OptStr = None,
     ):
```

### Comparing `vbcore-2.1.0rc0/vbcore/db/schema.py` & `vbcore-2.2.0rc0/vbcore/db/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from sqlalchemy import create_mock_engine, MetaData  # type: ignore
 from sqlalchemy.engine import Engine
 from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.orm import class_mapper
 from sqlalchemy_schemadisplay import create_schema_graph, create_uml_graph
 
+from vbcore.loggers import Log
 from vbcore.types import OptStr
 
 
 def model_to_uml(
     module: str,
     show_operations: bool = False,
     show_attributes: bool = True,
@@ -23,16 +24,16 @@
 
     for attr in dir(models):
         if attr[0] == "_":
             continue
         try:
             cls = getattr(models, attr)
             mappers.append(class_mapper(cls))
-        except SQLAlchemyError:
-            pass
+        except SQLAlchemyError as exc:
+            Log.get(__name__).warning(exc, exc_info=True)
 
     return create_uml_graph(
         mappers,
         show_operations=show_operations,
         show_attributes=show_attributes,
         show_inherited=show_inherited,
         show_datatypes=show_datatypes,
```

### Comparing `vbcore-2.1.0rc0/vbcore/db/sqla.py` & `vbcore-2.2.0rc0/vbcore/db/sqla.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/db/support.py` & `vbcore-2.2.0rc0/vbcore/db/support.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/db/views.py` & `vbcore-2.2.0rc0/vbcore/db/views.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/dictutils/flatter_dict.py` & `vbcore-2.2.0rc0/vbcore/dictutils/flatter_dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,15 +304,15 @@
         """
         if key not in self and default != NO_DEFAULT:
             return default
         value = self[key]
         self.__delitem__(key)  # pylint: disable=unnecessary-dunder-call
         return value
 
-    def setdefault(self, key, default):
+    def setdefault(self, key, default=None):
         """
         If key is in the flat dictionary, return its value. If not,
         insert key with a value of default and return default.
         default defaults to ``None``.
 
         :param mixed key: The key name
         :param mixed default: The default value
@@ -335,27 +335,27 @@
             if delimiter in key:
                 raise ValueError(f"Key {key} collides with delimiter {delimiter}")
         self._delimiter = delimiter
         for key in self._values.keys():
             if isinstance(self._values[key], FlatDict):
                 self._values[key].set_delimiter(delimiter)
 
-    def update(self, other, **kwargs):
+    def update(self, __m=None, **kwargs):  # pylint: disable=arguments-differ
         """
         Update the flat dictionary with the key/value pairs from other,
         overwriting existing keys.
 
         ``update()`` accepts either another flat dictionary object or an
         iterable of key/value pairs (as tuples or other iterables of length
         two). If keyword arguments are specified, the flat dictionary is then
         updated with those key/value pairs: ``d.update(red=1, blue=2)``.
 
         :rtype: None
         """
-        for k, v in dict(other or kwargs).items():
+        for k, v in dict(__m or kwargs).items():
             self[k] = v
 
     def values(self):
         """
         Return a copy of the flat dictionary's list of values. See the note
         for :meth:`flatdict.FlatDict.items`.
```

### Comparing `vbcore-2.1.0rc0/vbcore/dispatcher.py` & `vbcore-2.2.0rc0/vbcore/dispatcher.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/enums.py` & `vbcore-2.2.0rc0/vbcore/enums.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/exceptions.py` & `vbcore-2.2.0rc0/vbcore/exceptions.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/factory.py` & `vbcore-2.2.0rc0/vbcore/factory.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/files.py` & `vbcore-2.2.0rc0/vbcore/files.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/http/batch.py` & `vbcore-2.2.0rc0/vbcore/http/batch.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,31 +14,28 @@
 class HTTPBatch(HTTPBase, AsyncBatchExecutor):
     def __init__(
         self,
         endpoint: OptStr = None,
         dump_body: DumpBodyType = False,
         timeout: int = 10,
         raise_on_exc: bool = False,
-        logger=None,
     ):
-        HTTPBase.__init__(self, endpoint, dump_body, timeout, raise_on_exc, logger)
+        HTTPBase.__init__(self, endpoint, dump_body, timeout, raise_on_exc)
         AsyncBatchExecutor.__init__(self, return_exceptions=not self._raise_on_exc)
 
     async def http_request(
         self,
         dump_body: t.Optional[DumpBodyType] = None,
         timeout: OptInt = None,
         **kwargs,
     ) -> ResponseData:
         dump_body = self.dump_body_flags(dump_body, **kwargs)
 
         try:
-            self._logger.info(
-                "%s", self.dump_request(ObjectDict(**kwargs), dump_body[0])
-            )
+            self.log.info("%s", self.dump_request(ObjectDict(**kwargs), dump_body[0]))
             async with aiohttp.ClientSession(
                 timeout=aiohttp.ClientTimeout(
                     sock_read=timeout or self._timeout,
                     sock_connect=timeout or self._timeout,
                 )
             ) as session, session.request(**kwargs) as resp:
                 try:
@@ -52,27 +49,27 @@
                         status=resp.status,
                         headers={**resp.headers},
                     )
                     log_resp = response
                     log_resp.text = response.body
                     log_resp = self.dump_response(log_resp, dump_body[1])
                     resp.raise_for_status()
-                    self._logger.info("%s", log_resp)
+                    self.log.info("%s", log_resp)
                 except aiohttp.ClientResponseError as exc:
-                    self._logger.warning("%s", log_resp)
+                    self.log.warning("%s", log_resp)
                     if self._raise_on_exc is True:
                         raise  # pragma: no cover
                     response.exception = exc
                 return response
         except (
             aiohttp.ClientError,
             aiohttp.ServerTimeoutError,
             asyncio.TimeoutError,
         ) as exc:
-            self._logger.exception(exc)
+            self.log.exception(exc)
             if self._raise_on_exc is True:
                 raise  # pragma: no cover
 
             return ResponseData(
                 body={}, status=httpcode.SERVICE_UNAVAILABLE, headers={}, exception=exc
             )
```

### Comparing `vbcore-2.1.0rc0/vbcore/http/client.py` & `vbcore-2.2.0rc0/vbcore/http/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import logging
 import typing as t
 
 from requests import auth, exceptions as http_exc, request as send_request, Response
 
 from vbcore.datastruct import ObjectDict
 from vbcore.http.headers import HeaderEnum
 from vbcore.misc import get_uuid
 from vbcore.types import OptStr
 
+from ..loggers import VBLoggerMixin
 from . import httpcode
 from .httpdumper import LazyHTTPDumper
 from .methods import HttpMethod
 
 HTTPStatusError = (http_exc.HTTPError,)
 NetworkError = (http_exc.ConnectionError, http_exc.Timeout)
 all_errors = (*HTTPStatusError, *NetworkError)
@@ -48,28 +48,26 @@
         return not self.__eq__(other)
 
     def __call__(self, response):
         response.headers["Authorization"] = f"{self.token_type} {self.token}"
         return response
 
 
-class HTTPBase(LazyHTTPDumper):
+class HTTPBase(LazyHTTPDumper, VBLoggerMixin):
     def __init__(
         self,
         endpoint: str,
         dump_body: DumpBodyType = False,
         timeout: int = 10,
         raise_on_exc: bool = False,
-        logger=None,
     ):
         self._timeout = timeout
         self._endpoint = endpoint
         self._raise_on_exc = raise_on_exc
         self._dump_body = self.normalize_dump_flags(dump_body)
-        self._logger = logger or logging.getLogger(self.__module__)
 
     @classmethod
     def normalize_dump_flags(
         cls,
         dump_body: t.Optional[DumpBodyType] = None,
     ) -> t.Tuple[bool, bool]:
         if isinstance(dump_body, bool):
@@ -156,32 +154,32 @@
     ) -> ResponseData:
         kwargs["auth"] = self.get_auth()
         dump_body = self.dump_body_flags(dump_body, **kwargs)
 
         try:
             url = self.normalize_url(uri)
             req = ObjectDict(method=method, url=url, **kwargs)
-            self._logger.info("%s", self.dump_request(req, dump_body=dump_body[0]))
+            self.log.info("%s", self.dump_request(req, dump_body=dump_body[0]))
             timeout = kwargs.pop("timeout", None) or self._timeout
             response = send_request(method, url, timeout=timeout, **kwargs)
         except NetworkError as exc:
-            self._logger.exception(exc)
+            self.log.exception(exc)
             if raise_on_exc or self._raise_on_exc:
                 raise  # pragma: no cover
 
             return self.prepare_response(
                 status=httpcode.SERVICE_UNAVAILABLE, exception=exc
             )
 
         log_resp = self.dump_response(response, dump_body=dump_body[1])
         try:
             response.raise_for_status()
-            self._logger.info("%s", log_resp)
+            self.log.info("%s", log_resp)
         except HTTPStatusError as exc:
-            self._logger.warning("%s", log_resp)
+            self.log.warning("%s", log_resp)
             response = exc.response
             if raise_on_exc or self._raise_on_exc:
                 raise
 
         body: t.Any = response.text
         if kwargs.get("stream") is True:
             chunk_size = kwargs.pop("chunk_size", None)
```

### Comparing `vbcore-2.1.0rc0/vbcore/http/gql.py` & `vbcore-2.2.0rc0/vbcore/http/gql.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/http/headers.py` & `vbcore-2.2.0rc0/vbcore/http/headers.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/http/httpcode.py` & `vbcore-2.2.0rc0/vbcore/http/httpcode.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/http/httpdumper.py` & `vbcore-2.2.0rc0/vbcore/http/httpdumper.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/http/proxy.py` & `vbcore-2.2.0rc0/vbcore/http/proxy.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/http/rpc.py` & `vbcore-2.2.0rc0/vbcore/http/rpc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/http/useragent.py` & `vbcore-2.2.0rc0/vbcore/http/useragent.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     browser: Client
     device: Device
 
     def __str__(self):
         return self.raw
 
     @classmethod
-    def parse(cls, user_agent: str):
+    def parse(cls, user_agent: str) -> "UserAgent":
         parsed = cls.parser_class(user_agent)
 
         return cls(
             raw=parsed.ua_string,
             browser=Client(
                 family=parsed.browser.family,
                 version=Version(
```

### Comparing `vbcore-2.1.0rc0/vbcore/importer.py` & `vbcore-2.2.0rc0/vbcore/importer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,82 +1,85 @@
 import importlib
 import typing as t
 from types import ModuleType
 
 from vbcore.exceptions import VBException
+from vbcore.types import OptStr
 
 
 class ImporterError(VBException):
     pass
 
 
 class ImporterModuleError(ImporterError):
-    def __init__(self, name, exc: Exception):
+    def __init__(self, name: str, exc: Exception):
         self.name = name
         self.exception = exc
         super().__init__(f"unable to import module: {name}", orig=exc)
 
 
 class ImporterValueError(ImporterError):
     def __init__(self, name: str):
         self.name = name
         super().__init__(f"class not registered: '{name}'")
 
 
-class ImporterSubclassError(ImporterError):
-    def __init__(self, item: t.Any, subclass_of: t.Type):
+class ImporterClassError(ImporterError):
+    def __init__(self, item: t.Any, class_: t.Type):
         self.item = item
-        self.subclass_of = subclass_of
-        class_name = f"{subclass_of.__module__}:{subclass_of.__name__}"
-        super().__init__(f"'{item}' must be subclass of '{class_name}'")
+        self.class_ = class_
+        self.class_name = f"{class_.__module__}:{class_.__name__}"
+        super().__init__(str(self))
 
 
-class ImporterInstanceError(ImporterError):
-    def __init__(self, item: t.Any, instance_of: t.Type):
-        self.item = item
-        self.instance_of = instance_of
-        class_name = f"{instance_of.__module__}:{instance_of.__name__}"
-        super().__init__(f"'{item}' must be instance of '{class_name}'")
+class ImporterSubclassError(ImporterClassError):
+    def __str__(self) -> str:
+        return f"'{self.item}' must be subclass of '{self.class_name}'"
+
+
+class ImporterInstanceError(ImporterClassError):
+    def __str__(self) -> str:
+        return f"'{self.item}' must be instance of '{self.class_name}'"
 
 
 class ImporterAttributeError(ImporterError):
     def __init__(self, module: ModuleType, attribute: t.Optional[str] = None):
         self.module = module
         self.attribute = attribute
         super().__init__(f"attribute '{attribute}' not found in module '{module}'")
 
 
 class Importer:
     attribute_separator: str = ":"
 
     @classmethod
-    def check_subclass(cls, item: t.Any, subclass_of: t.Optional[t.Type]):
+    def check_subclass(cls, item: t.Any, subclass_of: t.Optional[t.Type]) -> None:
         if subclass_of and isinstance(item, type) and not issubclass(item, subclass_of):
             raise ImporterSubclassError(item, subclass_of)
 
     @classmethod
-    def check_isinstance(cls, item: t.Any, instance_of: t.Optional[t.Type]):
+    def check_isinstance(cls, item: t.Any, instance_of: t.Optional[t.Type]) -> None:
         if instance_of and not isinstance(item, instance_of):
             raise ImporterInstanceError(item, instance_of)
 
     @classmethod
-    def parse_string(cls, name: str) -> t.Tuple[str, t.Optional[str]]:
+    def parse_string(cls, name: str) -> t.Tuple[str, OptStr]:
         if cls.attribute_separator in name:
             mod, attr = name.split(cls.attribute_separator)
             return mod, attr
         return name, None
 
     @classmethod
     def from_module(
         cls,
         name: str,
         *args,
         subclass_of: t.Optional[t.Type] = None,
         instance_of: t.Optional[t.Type] = None,
-        package: t.Optional[str] = None,
+        package: OptStr = None,
         call_with: bool = False,
         raise_exc: bool = True,
         **kwargs,
     ) -> t.Any:
         mod, attr = cls.parse_string(name)
 
         try:
@@ -106,15 +109,15 @@
 
         return imported(*args, **kwargs) if args or kwargs else imported()
 
 
 class ImporterFactory:
     def __init__(
         self,
-        package: t.Optional[str] = None,
+        package: OptStr = None,
         base_class: t.Optional[t.Type] = None,
         classes: t.Optional[t.Dict[str, str]] = None,
     ):
         self.package = package
         self.base_class = base_class
         self.classes: t.Optional[t.Dict[str, str]] = {}
         self.register_classes(classes or {})
```

### Comparing `vbcore-2.1.0rc0/vbcore/json.py` & `vbcore-2.2.0rc0/vbcore/json.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/jsonschema/schemas/jsonrpc.py` & `vbcore-2.2.0rc0/vbcore/jsonschema/schemas/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/jsonschema/support.py` & `vbcore-2.2.0rc0/vbcore/jsonschema/support.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/lambdas.py` & `vbcore-2.2.0rc0/vbcore/lambdas.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/loggers.py` & `vbcore-2.2.0rc0/vbcore/loggers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import logging
 import logging.config
 import os
 import socket
 import struct
 import typing as t
+from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from dataclasses import dataclass
 from datetime import datetime
+from functools import cached_property
 
 from vbcore import json
-from vbcore.base import Static
+from vbcore.base import Decorator, Static
 from vbcore.context import ContextCorrelationId, ContextMetadata
 from vbcore.files import FileHandler
 from vbcore.types import OptStr
 
 ALERT = logging.WARN + 5
 TRACE = logging.DEBUG - 5
 DEFAULT_LISTENER_PORT = logging.config.DEFAULT_LOGGING_CONFIG_PORT
@@ -34,14 +36,29 @@
             self._log(TRACE, msg, args, **kwargs)
 
 
 class VBRootLogger(logging.RootLogger, VBLogger):
     pass
 
 
+def patch_logging():
+    setattr(logging, "ALERT", ALERT)  # noqa: B010
+    setattr(logging, "TRACE", TRACE)  # noqa: B010
+
+    logging.addLevelName(ALERT, "ALERT")
+    logging.addLevelName(TRACE, "TRACE")
+    logging.setLoggerClass(VBLogger)
+
+    root_logger = VBRootLogger(logging.WARNING)
+    logging.Logger.manager = logging.Manager(root_logger)
+    logging.root = root_logger
+
+    logging.captureWarnings(os.environ.get("LOG_CAPTURE_WARNING", True))
+
+
 @dataclass(frozen=True, kw_only=True)
 class LoggingSettings:
     level: str = "INFO"
     force: bool = True
     config_file: OptStr = None
     listen_for_reload: bool = False
     listener_daemon: bool = True
@@ -156,20 +173,53 @@
             "%s%s",
             message or "execution time: ",
             datetime.now() - start_time,
             extra=kwargs,
         )
 
 
-def patch_logging():
-    setattr(logging, "ALERT", ALERT)  # noqa: B010
-    setattr(logging, "TRACE", TRACE)  # noqa: B010
+LogClass = t.TypeVar("LogClass", bound=logging.Logger)
 
-    logging.addLevelName(ALERT, "ALERT")
-    logging.addLevelName(TRACE, "TRACE")
-    logging.setLoggerClass(VBLogger)
 
-    __root_logger = VBRootLogger(logging.WARNING)
-    logging.Logger.manager = logging.Manager(__root_logger)
-    logging.root = __root_logger
+class LoggerMixin(ABC, t.Generic[LogClass]):
+    @classmethod
+    @abstractmethod
+    def logger(cls, name: OptStr = None) -> LogClass:
+        """returns the logger instance"""
 
-    logging.captureWarnings(os.environ.get("LOG_CAPTURE_WARNING", True))
+    @cached_property
+    def log(self) -> LogClass:
+        return self.logger()
+
+
+class VBLoggerMixin(LoggerMixin[VBLogger]):
+    @classmethod
+    def logger(cls, name: OptStr = None) -> VBLogger:
+        return Log.get(name or cls.__module__)
+
+
+class LogError(Decorator, VBLoggerMixin):
+    def __init__(
+        self,
+        message: str = "",
+        logger: OptStr = None,
+        reraise: bool = True,
+        only: t.Tuple[t.Type[Exception], ...] = (),
+    ):
+        self.message = message
+        self.reraise = reraise
+        self.logger_name = logger
+        self.only_execs = only or (Exception,)
+
+    def finally_hook(self) -> None:
+        """hook called at finally stage of error handling"""
+
+    def perform(self, function: t.Callable, *args, **kwargs) -> t.Any:
+        try:
+            return super().perform(function, *args, **kwargs)
+        except self.only_execs as exc:
+            self.logger(self.logger_name).exception(self.message or exc)
+            if self.reraise:
+                raise
+        finally:
+            self.finally_hook()
+        return None
```

### Comparing `vbcore-2.1.0rc0/vbcore/misc.py` & `vbcore-2.2.0rc0/vbcore/misc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/net/helpers.py` & `vbcore-2.2.0rc0/vbcore/net/helpers.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/net/sendmail.py` & `vbcore-2.2.0rc0/vbcore/net/sendmail.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 from dataclasses import dataclass
 from email.mime.application import MIMEApplication
 from email.mime.base import MIMEBase
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from email.utils import formatdate, make_msgid, parseaddr
 
-from email_validator import caching_resolver, validate_email, ValidatedEmail
-
 from vbcore.files import FileHandler
-from vbcore.misc import CommonRegex, get_uuid
+from vbcore.misc import get_uuid
 from vbcore.types import CoupleStr, OptStr, StrDict, StrList, StrTuple
 
 AddressType = t.Union[str, StrTuple]
 
 
 @dataclass(frozen=True)
 class SMTPResponse:
@@ -58,20 +56,14 @@
 
 class SendMail:
     def __init__(self, params: SMTPParams, **kwargs):
         self.params = params
         self._smtp_args = kwargs
 
     @classmethod
-    def validate_email(cls, email: str, restricted: bool = True) -> ValidatedEmail:
-        if restricted and not CommonRegex.is_valid_email(email):
-            raise ValueError(f"invalid email: {email}")
-        return validate_email(email, dns_resolver=caching_resolver())
-
-    @classmethod
     def prepare_addresses(cls, addr: AddressType) -> str:
         return ",".join(addr) if isinstance(addr, tuple) else addr
 
     @classmethod
     def add_attachments(cls, message: MIMEBase, files: StrList):
         for filename in files:
             with FileHandler(filename).open_binary() as file:
```

### Comparing `vbcore-2.1.0rc0/vbcore/net/sftp.py` & `vbcore-2.2.0rc0/vbcore/net/ftpclient.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import contextlib
 import os.path
 import re
 from dataclasses import dataclass
 from enum import Enum
+from ftplib import FTP  # nosec
 from functools import cached_property
 from typing import Generator, Optional, Union
 
 from paramiko import DSSKey, ECDSAKey, Ed25519Key, PKey, RSAKey, SFTPClient, Transport
 from paramiko.common import DEFAULT_MAX_PACKET_SIZE, DEFAULT_WINDOW_SIZE
 
+from vbcore.base import BaseDTO
 from vbcore.enums import EnumMixin
+from vbcore.loggers import VBLoggerMixin
 from vbcore.types import OptStr, StrList
 
 
 class AlgoKeyEnum(EnumMixin, Enum):
     RSA = RSAKey
     DSS = DSSKey
     ECDSA = ECDSAKey
@@ -33,24 +36,27 @@
     gss_deleg_creds: bool = True
     gss_host: OptStr = None
     gss_auth: bool = False
     gss_trust_dns: bool = True
 
 
 @dataclass(frozen=True, kw_only=True)
-class SFTPOptions:
+class SFTPOptions(BaseDTO):
     host: str
     port: int
     user: OptStr = None
     password: OptStr = None
     private_key_file: OptStr = None
     key_type: Union[str, AlgoKeyEnum] = AlgoKeyEnum.RSA
+    timeout: int = 300
+    debug: bool = False
+    encoding: str = "utf-8"
 
 
-class SFTPHandler:
+class SFTPHandler(VBLoggerMixin):
     def __init__(
         self,
         options: SFTPOptions,
         transport_options: Optional[TransportOptions] = None,
     ):
         self.options = options
         self.transport_options = transport_options or TransportOptions()
@@ -107,19 +113,19 @@
         self.disconnect()
 
     def walk(self, remote_path: str = ".") -> StrList:
         with self.context() as conn:
             return conn.listdir(path=remote_path)
 
     def download(self, remote: str, local: str) -> None:
-        self.sftp.logger.info("downloading '%s' -> '%s' ...", remote, local)
+        self.log.info("downloading '%s' -> '%s' ...", remote, local)
         self.sftp.get(remote, local)
 
     def upload(self, local: str, remote: str) -> None:
-        self.sftp.logger.info("uploading '%s' -> '%s' ...", local, remote)
+        self.log.info("uploading '%s' -> '%s' ...", local, remote)
         self.sftp.put(local, remote)
 
     def download_file(self, remote: str, local: str) -> None:
         with self.context():
             self.download(remote, local)
 
     def upload_file(self, local: str, remote: str) -> None:
@@ -132,15 +138,15 @@
         only: Optional[re.Pattern] = None,
         exclude: Optional[re.Pattern] = None,
     ) -> bool:
         is_filtered = bool(
             exclude and exclude.match(filename) or only and not only.match(filename)
         )
         if is_filtered:
-            self.sftp.logger.info("file '%s' filtered", filename)
+            self.log.info("file '%s' filtered", filename)
         return is_filtered
 
     def upload_dir(
         self,
         local_path: str = ".",
         remote_path: str = ".",
         only: Optional[re.Pattern] = None,
@@ -174,7 +180,63 @@
 
                 self.download(
                     os.path.join(remote_path, filename),
                     os.path.join(local_path, filename),
                 )
                 counter += 1
         return counter
+
+
+@dataclass(frozen=True, kw_only=True)
+class FTPOptions(BaseDTO):
+    host: str
+    port: int
+    user: OptStr = None
+    password: OptStr = None
+    timeout: int = 300
+    debug: bool = False
+    encoding: str = "utf-8"
+
+
+class FTPHandler(VBLoggerMixin):
+    def __init__(self, options: FTPOptions):
+        self.options = options
+        self.client = FTP(timeout=options.timeout, encoding=options.encoding)  # nosec
+
+    @contextlib.contextmanager
+    def connect(self) -> Generator[FTP, None, None]:
+        opts = self.options
+        with self.client as ftp:
+            ftp.debugging = 3 if opts.debug else 0
+            ftp.connect(opts.host, opts.port)
+            ftp.login(opts.user, opts.password or "")
+            yield ftp
+
+    def download_file(self, remote_path: str, local_path: str):
+        with self.connect() as conn:
+            with open(local_path, "wb") as file:
+                self.log.info("downloading '%s' -> '%s'...", remote_path, local_path)
+                conn.retrbinary(f"RETR {remote_path}", file.write)
+
+    def upload_file(self, local_path: str, remote_path: str):
+        with self.connect() as conn:
+            with open(local_path, "rb") as file:
+                self.log.info("uploading '%s' -> '%s'...", local_path, remote_path)
+                conn.storbinary(f"STOR {remote_path}", file)
+
+    def upload_dir(
+        self,
+        local_path: str = ".",
+        remote_path: str = ".",
+        only: Optional[re.Pattern] = None,
+        exclude: Optional[re.Pattern] = None,
+    ) -> int:
+        raise NotImplementedError
+
+    def download_dir(
+        self,
+        remote_path: str = ".",
+        local_path: str = ".",
+        only: Optional[re.Pattern] = None,
+        exclude: Optional[re.Pattern] = None,
+    ) -> int:
+        raise NotImplementedError
```

### Comparing `vbcore-2.1.0rc0/vbcore/net/socks_smtp.py` & `vbcore-2.2.0rc0/vbcore/net/socks_smtp.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/rule_engine/base.py` & `vbcore-2.2.0rc0/vbcore/rule_engine/base.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/rule_engine/engine.py` & `vbcore-2.2.0rc0/vbcore/rule_engine/engine.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/standalone/scheduler.py` & `vbcore-2.2.0rc0/vbcore/standalone/scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from io import StringIO
 
 from apscheduler import events as scheduler_events
 from apscheduler.job import Job
 from apscheduler.schedulers.base import BaseScheduler
 from apscheduler.schedulers.blocking import BlockingScheduler
 
-from vbcore.base import BaseLoggerMixin
 from vbcore.datastruct.lazy import Dumper, LazyDump
+from vbcore.loggers import VBLoggerMixin
 from vbcore.misc import get_uuid
 from vbcore.types import OptDict, StrDict
 
 
-class APScheduler(BaseLoggerMixin):
+class APScheduler(VBLoggerMixin):
     def __init__(
         self,
         *args,
         scheduler: t.Type[BaseScheduler] = BlockingScheduler,
         gconfig: StrDict = None,
         events_to_listen: int = None,
         auto_start: bool = False,
```

### Comparing `vbcore-2.1.0rc0/vbcore/standalone/wsgi_gunicorn.py` & `vbcore-2.2.0rc0/vbcore/standalone/wsgi_gunicorn.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/stringutils/misc.py` & `vbcore-2.2.0rc0/vbcore/stringutils/misc.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/stringutils/notations.py` & `vbcore-2.2.0rc0/vbcore/stringutils/notations.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/system.py` & `vbcore-2.2.0rc0/vbcore/system.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/tester/asserter.py` & `vbcore-2.2.0rc0/vbcore/tester/asserter.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/tester/fetchmail.py` & `vbcore-2.2.0rc0/vbcore/tester/fetchmail.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/tester/helpers.py` & `vbcore-2.2.0rc0/vbcore/tester/helpers.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/tester/http.py` & `vbcore-2.2.0rc0/vbcore/tester/http.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/tools/cli.py` & `vbcore-2.2.0rc0/vbcore/tools/cli.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/tools/crypto.py` & `vbcore-2.2.0rc0/vbcore/tools/crypto.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/tools/database.py` & `vbcore-2.2.0rc0/vbcore/tools/database.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/tools/entrypoint.py` & `vbcore-2.2.0rc0/vbcore/tools/entrypoint.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import click
 
 from vbcore.loggers import SetupLoggers
 from vbcore.tools.cli import Cli
 from vbcore.tools.crypto import main as main_crypto
 from vbcore.tools.database import main as main_database
+from vbcore.tools.ftpclient import main as main_ftpclient
 from vbcore.tools.initializer.init import main as main_init
 from vbcore.tools.scheduler import main as main_scheduler
 from vbcore.tools.sendmail import sendmail as main_sendmail
-from vbcore.tools.sftp import main as main_sftp
 from vbcore.tools.wsgi_gunicorn import main as main_gunicorn
 from vbcore.version import __version__
 
 SetupLoggers()
 
 main = click.Group()
 
@@ -26,13 +26,13 @@
 
 
 main.add_command(main_database)
 main.add_command(main_crypto)
 main.add_command(main_init)
 main.add_command(main_scheduler)
 main.add_command(main_sendmail)
-main.add_command(main_sftp)
+main.add_command(main_ftpclient)
 main.add_command(main_gunicorn)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `vbcore-2.1.0rc0/vbcore/tools/initializer/init.py` & `vbcore-2.2.0rc0/vbcore/tools/initializer/init.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.gitignore` & `vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/.gitignore`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/.pylintrc` & `vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/.pylintrc`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/Makefile` & `vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/Makefile`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/README.md` & `vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/README.md`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/devops/gitlab-ci.yml` & `vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/devops/gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/liccheck.ini` & `vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/liccheck.ini`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/tools/initializer/skeleton/setup.py` & `vbcore-2.2.0rc0/vbcore/tools/initializer/skeleton/setup.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/tools/scheduler.py` & `vbcore-2.2.0rc0/vbcore/tools/scheduler.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/tools/sendmail.py` & `vbcore-2.2.0rc0/vbcore/tools/sendmail.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/tools/wsgi_gunicorn.py` & `vbcore-2.2.0rc0/vbcore/tools/wsgi_gunicorn.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 import os
 from multiprocessing import cpu_count
+from typing import TYPE_CHECKING
 
 import click
 from gunicorn.util import getcwd
 
-from vbcore.standalone.wsgi_gunicorn import GUnicornServer, WorkerType
+from vbcore.datastruct.lazy import LazyImporter
 from vbcore.tools.cli import CliOpt, CliReqOpt
 
+if TYPE_CHECKING:
+    from vbcore.standalone.wsgi_gunicorn import GUnicornServer, WorkerType
+else:
+    GUnicornServer, WorkerType = LazyImporter.import_many(
+        "vbcore.standalone.wsgi_gunicorn:GUnicornServer",
+        "vbcore.standalone.wsgi_gunicorn:WorkerType",
+        message="you must install gunicorn",
+    )
+
 
 @click.command(name="gunicorn")
 @CliReqOpt.string("-a", "--app")
 @CliOpt.multi("-b", "--bind", envvar="GU_BIND", default=["127.0.0.1:8000"])
 @CliOpt.integer("-w", "--workers", envvar="GU_WORKERS", default=cpu_count())
 @CliOpt.integer("-t", "--threads", envvar="GU_THREADS", default=cpu_count() * 2 + 1)
 @CliOpt.integer("--worker-connections", envvar="GU_WORKER_CONNECTIONS", default=1000)
```

### Comparing `vbcore-2.1.0rc0/vbcore/types.py` & `vbcore-2.2.0rc0/vbcore/types.py`

 * *Files identical despite different names*

### Comparing `vbcore-2.1.0rc0/vbcore/yaml.py` & `vbcore-2.2.0rc0/vbcore/yaml.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # based on:
 # https://github.com/nameko/nameko/blob/a719cb1487f643769e2d13daf255c20551490f43/nameko/cli/main.py#L102-L111
 
 import os
 import re
-import sys
 
 import yaml
 
 from .datastruct import ObjectDict
+from .loggers import Log
 
 ENV_VAR_MATCHER = re.compile(
     r"""
         \${        # match characters `${` literally
         ([^}:\s]+) # 1st group: matches any character except `}` or `:`
         :?         # matches the literal `:` character zero or one times
         ([^}]+)?   # 2nd group: matches any character except `}`
@@ -34,35 +34,34 @@
 def loads(data, loader=None, as_object: bool = True):
     data = yaml.load(data, Loader=loader or yaml.Loader)  # nosec
     if as_object:
         return ObjectDict.normalize(data)
     return data
 
 
-def load_yaml_file(filename: str, encoding="utf-8", **kwargs):
+def load_yaml_file(filename: str, encoding: str = "utf-8", **kwargs):
     with open(filename, encoding=encoding) as f:
         return loads(f, **kwargs)
 
 
-def load_optional_yaml_file(filename: str, default=None, debug: bool = False, **kwargs):
+def load_optional_yaml_file(filename: str, default=None, **kwargs):
     try:
         return load_yaml_file(filename, **kwargs)
     except OSError as exc:
-        if debug is True:
-            print(f"WARN: {exc}", file=sys.stderr)
+        Log.get(__name__).warning(exc, exc_info=True)
         return ObjectDict() if default is None else default
 
 
 def _replace_env_var(match):
     env_var, default = match.groups()
     value = os.environ.get(env_var, None)
     if value is None:
         if default is None:
             # regex module return None instead of ''
-            # if engine didn't entered default capture group
+            # if engine did not enter default capture group
             default = ""
 
         value = default
         while IMPLICIT_ENV_VAR_MATCHER.match(value):
             value = ENV_VAR_MATCHER.sub(_replace_env_var, value)
     return value
```

### Comparing `vbcore-2.1.0rc0/vbcore.egg-info/SOURCES.txt` & `vbcore-2.2.0rc0/vbcore.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -104,17 +104,17 @@
 vbcore/http/rpc.py
 vbcore/http/useragent.py
 vbcore/jsonschema/__init__.py
 vbcore/jsonschema/support.py
 vbcore/jsonschema/schemas/__init__.py
 vbcore/jsonschema/schemas/jsonrpc.py
 vbcore/net/__init__.py
+vbcore/net/ftpclient.py
 vbcore/net/helpers.py
 vbcore/net/sendmail.py
-vbcore/net/sftp.py
 vbcore/net/socks_smtp.py
 vbcore/rule_engine/__init__.py
 vbcore/rule_engine/base.py
 vbcore/rule_engine/engine.py
 vbcore/standalone/__init__.py
 vbcore/standalone/scheduler.py
 vbcore/standalone/wsgi_gunicorn.py
@@ -131,17 +131,17 @@
 vbcore/tester/plugins/fixtures.py
 vbcore/tester/plugins/startup.py
 vbcore/tools/__init__.py
 vbcore/tools/cli.py
 vbcore/tools/crypto.py
 vbcore/tools/database.py
 vbcore/tools/entrypoint.py
+vbcore/tools/ftpclient.py
 vbcore/tools/scheduler.py
 vbcore/tools/sendmail.py
-vbcore/tools/sftp.py
 vbcore/tools/wsgi_gunicorn.py
 vbcore/tools/initializer/__init__.py
 vbcore/tools/initializer/init.py
 vbcore/tools/initializer/skeleton/.bumpversion.cfg
 vbcore/tools/initializer/skeleton/.coveragerc
 vbcore/tools/initializer/skeleton/.dockerignore
 vbcore/tools/initializer/skeleton/.editorconfig
```

### Comparing `vbcore-2.1.0rc0/vbcore.egg-info/requires.txt` & `vbcore-2.2.0rc0/vbcore.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 sqlalchemy
 sqlalchemy_schemadisplay
 argon2-cffi
 bcrypt
 aiohttp
 requests
 user_agents
-email_validator
 pysocks
 paramiko
 apscheduler
 chardet
 jsonschema
 rule_engine
 gql
@@ -52,13 +51,12 @@
 
 [http]
 aiohttp
 requests
 user_agents
 
 [net]
-email_validator
 pysocks
 paramiko
 
 [scheduler]
 apscheduler
```

