# Comparing `tmp/lemur-1.4.0.tar.gz` & `tmp/lemur-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemur-1.4.0.tar", last modified: Tue Apr  4 20:36:32 2023, max compression
+gzip compressed data, was "lemur-1.5.0.tar", last modified: Wed Jul  5 22:38:48 2023, max compression
```

## Comparing `lemur-1.4.0.tar` & `lemur-1.5.0.tar`

### file list

```diff
@@ -1,468 +1,468 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:36:32.462933 lemur-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-04 20:35:19.000000 lemur-1.4.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-04 20:35:19.000000 lemur-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-04 20:35:19.000000 lemur-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-04 20:35:32.486644 lemur-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-04 20:35:19.000000 lemur-1.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-04 20:35:19.000000 lemur-1.4.0/bower.json
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-04 20:35:19.000000 lemur-1.4.0/gulpfile.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.414647 lemur-1.4.0/lemur/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.414647 lemur-1.4.0/lemur/acme_providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/acme_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/acme_providers/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.414647 lemur-1.4.0/lemur/api_keys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/api_keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/api_keys/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/api_keys/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/api_keys/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/api_keys/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/api_keys/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.414647 lemur-1.4.0/lemur/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/auth/ldap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/auth/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/auth/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    23702 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/auth/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.414647 lemur-1.4.0/lemur/authorities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/authorities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/authorities/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/authorities/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/authorities/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    19912 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/authorities/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.418647 lemur-1.4.0/lemur/authorizations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/authorizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/authorizations/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/authorizations/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.418647 lemur-1.4.0/lemur/certificates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/certificates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41946 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/certificates/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/certificates/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    16828 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/certificates/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    18872 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/certificates/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    48692 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/certificates/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/certificates/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/certificates/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)    63990 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/certificates/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.422647 lemur-1.4.0/lemur/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37661 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/common/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/common/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/common/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/common/health.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/common/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/common/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/common/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/common/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    16858 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/common/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/default.conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.422647 lemur-1.4.0/lemur/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/defaults/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/defaults/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.422647 lemur-1.4.0/lemur/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/deployment/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.422647 lemur-1.4.0/lemur/destinations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/destinations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/destinations/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/destinations/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/destinations/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    15233 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/destinations/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.422647 lemur-1.4.0/lemur/dns_providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/dns_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/dns_providers/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/dns_providers/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/dns_providers/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/dns_providers/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/dns_providers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/dns_providers/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.422647 lemur-1.4.0/lemur/domains/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/domains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/domains/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/domains/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/domains/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/domains/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.426647 lemur-1.4.0/lemur/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/endpoints/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/endpoints/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/endpoints/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/endpoints/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.426647 lemur-1.4.0/lemur/logs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/logs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/logs/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/logs/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/logs/views.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19476 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.426647 lemur-1.4.0/lemur/notifications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/notifications/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21762 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/notifications/messaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/notifications/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/notifications/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/notifications/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    16547 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/notifications/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.426647 lemur-1.4.0/lemur/pending_certificates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/pending_certificates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/pending_certificates/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/pending_certificates/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/pending_certificates/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/pending_certificates/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    18984 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/pending_certificates/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.426647 lemur-1.4.0/lemur/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.430647 lemur-1.4.0/lemur/plugins/base/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/base/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/base/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.430647 lemur-1.4.0/lemur/plugins/bases/
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/bases/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/bases/destination.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/bases/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/bases/issuer.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/bases/membership.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/bases/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/bases/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/bases/source.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/bases/tls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.430647 lemur-1.4.0/lemur/plugins/lemur_acme/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_acme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26261 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_acme/acme_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_acme/challenge_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_acme/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_acme/dyn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9980 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_acme/nsone.py
--rw-r--r--   0 runner    (1001) docker     (123)    17777 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_acme/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_acme/powerdns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_acme/route53.py
--rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_acme/ultradns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.430647 lemur-1.4.0/lemur/plugins/lemur_adcs/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_adcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_adcs/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.430647 lemur-1.4.0/lemur/plugins/lemur_atlas/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_atlas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_atlas/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.430647 lemur-1.4.0/lemur/plugins/lemur_atlas_redis/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_atlas_redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_atlas_redis/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.434646 lemur-1.4.0/lemur/plugins/lemur_aws/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_aws/cloudfront.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_aws/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_aws/elb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_aws/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)    27186 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_aws/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_aws/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_aws/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_aws/sts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.434646 lemur-1.4.0/lemur/plugins/lemur_azure_dest/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_azure_dest/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6430 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_azure_dest/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.434646 lemur-1.4.0/lemur/plugins/lemur_cfssl/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_cfssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_cfssl/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.434646 lemur-1.4.0/lemur/plugins/lemur_cryptography/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_cryptography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9811 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_cryptography/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.434646 lemur-1.4.0/lemur/plugins/lemur_csr/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_csr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_csr/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.434646 lemur-1.4.0/lemur/plugins/lemur_digicert/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_digicert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23108 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_digicert/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.434646 lemur-1.4.0/lemur/plugins/lemur_email/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_email/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.434646 lemur-1.4.0/lemur/plugins/lemur_email/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_email/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_email/templates/authority_expiration.html
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_email/templates/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_email/templates/expiration.html
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_email/templates/expiration_summary.html
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_email/templates/expiring_deployed_certificate.html
--rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_email/templates/failed.html
--rw-r--r--   0 runner    (1001) docker     (123)    10451 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_email/templates/issued.html
--rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_email/templates/reissue_failed.html
--rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_email/templates/reissued_with_no_endpoints.html
--rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_email/templates/revocation.html
--rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_email/templates/rotation.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.438646 lemur-1.4.0/lemur/plugins/lemur_entrust/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_entrust/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_entrust/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.438646 lemur-1.4.0/lemur/plugins/lemur_jks/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_jks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_jks/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.438646 lemur-1.4.0/lemur/plugins/lemur_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_kubernetes/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.438646 lemur-1.4.0/lemur/plugins/lemur_openssl/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_openssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_openssl/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.438646 lemur-1.4.0/lemur/plugins/lemur_sftp/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_sftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_sftp/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.438646 lemur-1.4.0/lemur/plugins/lemur_slack/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_slack/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.438646 lemur-1.4.0/lemur/plugins/lemur_vault_dest/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_vault_dest/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13290 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_vault_dest/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.438646 lemur-1.4.0/lemur/plugins/lemur_verisign/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_verisign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/lemur_verisign/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/plugins/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.438646 lemur-1.4.0/lemur/policies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/policies/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/policies/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/policies/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/policies/service.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/pytest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.438646 lemur-1.4.0/lemur/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/reporting/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/reporting/service.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/reporting/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.442646 lemur-1.4.0/lemur/roles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/roles/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/roles/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/roles/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/roles/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.442646 lemur-1.4.0/lemur/sources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/sources/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/sources/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/sources/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/sources/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/sources/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.406648 lemur-1.4.0/lemur/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.442646 lemur-1.4.0/lemur/static/app/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/.buildignore
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/404.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.442646 lemur-1.4.0/lemur/static/app/angular/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.442646 lemur-1.4.0/lemur/static/app/angular/api_keys/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.442646 lemur-1.4.0/lemur/static/app/angular/api_keys/api_key/
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/api_keys/api_key/api_key.js
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/api_keys/api_key/api_key.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/api_keys/services.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.442646 lemur-1.4.0/lemur/static/app/angular/api_keys/view/
--rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/api_keys/view/view.js
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/api_keys/view/view.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/app.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.442646 lemur-1.4.0/lemur/static/app/angular/authentication/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.442646 lemur-1.4.0/lemur/static/app/angular/authentication/login/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/authentication/login/login.js
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/authentication/login/login.tpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.442646 lemur-1.4.0/lemur/static/app/angular/authentication/logout/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/authentication/logout/logout.js
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/authentication/logout/logout.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/authentication/services.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.442646 lemur-1.4.0/lemur/static/app/angular/authorities/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.446646 lemur-1.4.0/lemur/static/app/angular/authorities/authority/
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/authorities/authority/authority.js
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/authorities/authority/authorityWizard.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/authorities/authority/distinguishedName.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/authorities/authority/edit.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/authorities/authority/extensions.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/authorities/authority/options.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/authorities/authority/permissions.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/authorities/authority/select.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/authorities/authority/tracking.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/authorities/services.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.446646 lemur-1.4.0/lemur/static/app/angular/authorities/view/
--rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/authorities/view/view.js
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/authorities/view/view.tpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.446646 lemur-1.4.0/lemur/static/app/angular/certificates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.446646 lemur-1.4.0/lemur/static/app/angular/certificates/certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/certificates/certificate/certificate.js
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/certificates/certificate/certificateWizard.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/certificates/certificate/destinations.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/certificates/certificate/distinguishedName.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/certificates/certificate/edit.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/certificates/certificate/export.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/certificates/certificate/notifications.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/certificates/certificate/options.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/certificates/certificate/replaces.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/certificates/certificate/revoke.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/certificates/certificate/tracking.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/certificates/certificate/upload.js
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/certificates/certificate/upload.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/certificates/services.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.446646 lemur-1.4.0/lemur/static/app/angular/certificates/view/
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/certificates/view/view.js
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/certificates/view/view.tpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.454645 lemur-1.4.0/lemur/static/app/angular/components/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/components/filters.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.454645 lemur-1.4.0/lemur/static/app/angular/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/dashboard/dashboard.js
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/dashboard/dashboard.tpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.454645 lemur-1.4.0/lemur/static/app/angular/destinations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.454645 lemur-1.4.0/lemur/static/app/angular/destinations/destination/
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/destinations/destination/destination.js
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/destinations/destination/destination.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/destinations/services.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.454645 lemur-1.4.0/lemur/static/app/angular/destinations/view/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/destinations/view/view.js
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/destinations/view/view.tpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.454645 lemur-1.4.0/lemur/static/app/angular/dns_providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.458645 lemur-1.4.0/lemur/static/app/angular/dns_providers/dns_provider/
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/dns_providers/dns_provider/dns_provider.js
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/dns_providers/dns_provider/dns_provider.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/dns_providers/services.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.458645 lemur-1.4.0/lemur/static/app/angular/dns_providers/view/
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/dns_providers/view/view.js
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/dns_providers/view/view.tpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.458645 lemur-1.4.0/lemur/static/app/angular/domains/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.458645 lemur-1.4.0/lemur/static/app/angular/domains/domain/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/domains/domain/domain.js
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/domains/domain/domain.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/domains/services.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.458645 lemur-1.4.0/lemur/static/app/angular/domains/view/
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/domains/view/view.js
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/domains/view/view.tpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.458645 lemur-1.4.0/lemur/static/app/angular/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/endpoints/services.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.458645 lemur-1.4.0/lemur/static/app/angular/endpoints/view/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/endpoints/view/view.js
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/endpoints/view/view.tpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.462645 lemur-1.4.0/lemur/static/app/angular/logs/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/logs/services.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.462645 lemur-1.4.0/lemur/static/app/angular/logs/view/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/logs/view/view.js
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/logs/view/view.tpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.462645 lemur-1.4.0/lemur/static/app/angular/notifications/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.462645 lemur-1.4.0/lemur/static/app/angular/notifications/notification/
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/notifications/notification/notification.js
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/notifications/notification/notification.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/notifications/services.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.462645 lemur-1.4.0/lemur/static/app/angular/notifications/view/
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/notifications/view/view.js
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/notifications/view/view.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/pager.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.462645 lemur-1.4.0/lemur/static/app/angular/pending_certificates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.466645 lemur-1.4.0/lemur/static/app/angular/pending_certificates/pending_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/pending_certificates/pending_certificate/cancel.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/pending_certificates/pending_certificate/destinations.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/pending_certificates/pending_certificate/edit.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/pending_certificates/pending_certificate/notifications.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/pending_certificates/pending_certificate/pending_certificate.js
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/pending_certificates/pending_certificate/replaces.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/pending_certificates/pending_certificate/upload.js
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/pending_certificates/pending_certificate/upload.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/pending_certificates/services.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.466645 lemur-1.4.0/lemur/static/app/angular/pending_certificates/view/
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/pending_certificates/view/view.js
--rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/pending_certificates/view/view.tpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.466645 lemur-1.4.0/lemur/static/app/angular/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/plugins/services.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.466645 lemur-1.4.0/lemur/static/app/angular/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.466645 lemur-1.4.0/lemur/static/app/angular/roles/role/
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/roles/role/role.js
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/roles/role/role.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/roles/role/roleSelect.tpl.html
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/roles/services.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.466645 lemur-1.4.0/lemur/static/app/angular/roles/view/
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/roles/view/view.js
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/roles/view/view.tpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.466645 lemur-1.4.0/lemur/static/app/angular/sources/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/sources/services.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.466645 lemur-1.4.0/lemur/static/app/angular/sources/source/
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/sources/source/source.js
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/sources/source/source.tpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.470644 lemur-1.4.0/lemur/static/app/angular/sources/view/
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/sources/view/view.js
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/sources/view/view.tpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.470644 lemur-1.4.0/lemur/static/app/angular/users/
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/users/services.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.470644 lemur-1.4.0/lemur/static/app/angular/users/user/
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/users/user/user.js
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/users/user/user.tpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.470644 lemur-1.4.0/lemur/static/app/angular/users/view/
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/users/view/view.js
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/users/view/view.tpl.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.470644 lemur-1.4.0/lemur/static/app/angular/welcome/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/welcome/welcome.html
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/angular/wizard.html
--rw-r--r--   0 runner    (1001) docker     (123)    11153 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.470644 lemur-1.4.0/lemur/static/app/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/static/app/styles/lemur.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.486644 lemur-1.4.0/lemur/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11326 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11320 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.486644 lemur-1.4.0/lemur/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/plugins/destination_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/plugins/issuer_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/plugins/notification_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/plugins/source_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_authorities.py
--rw-r--r--   0 runner    (1001) docker     (123)    59087 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_destinations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_dns_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_issuer_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_ldap.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_messaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_pending_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/test_verify.py
--rw-r--r--   0 runner    (1001) docker     (123)    38874 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/tests/vectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.486644 lemur-1.4.0/lemur/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/users/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/users/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/users/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/users/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-04 20:35:19.000000 lemur-1.4.0/lemur/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-04 20:36:32.462933 lemur-1.4.0/lemur-package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.414647 lemur-1.4.0/lemur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-04 20:35:32.000000 lemur-1.4.0/lemur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13735 2023-04-04 20:35:32.000000 lemur-1.4.0/lemur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 20:35:32.000000 lemur-1.4.0/lemur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-04 20:35:32.000000 lemur-1.4.0/lemur.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 20:35:32.000000 lemur-1.4.0/lemur.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-04-04 20:35:32.000000 lemur-1.4.0/lemur.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-04 20:35:32.000000 lemur-1.4.0/lemur.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-04 20:35:19.000000 lemur-1.4.0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-04 20:35:19.000000 lemur-1.4.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-04-04 20:35:19.000000 lemur-1.4.0/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-04 20:35:19.000000 lemur-1.4.0/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-04-04 20:35:19.000000 lemur-1.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-04 20:35:32.486644 lemur-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-04-04 20:35:19.000000 lemur-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:32.486644 lemur-1.4.0/trustores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 20:35:19.000000 lemur-1.4.0/trustores/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:38:48.054980 lemur-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-05 22:37:45.000000 lemur-1.5.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-07-05 22:37:45.000000 lemur-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-05 22:37:45.000000 lemur-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-05 22:37:56.671522 lemur-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-05 22:37:45.000000 lemur-1.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-05 22:37:45.000000 lemur-1.5.0/bower.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-05 22:37:45.000000 lemur-1.5.0/gulpfile.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.635519 lemur-1.5.0/lemur/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.639519 lemur-1.5.0/lemur/acme_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/acme_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/acme_providers/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.639519 lemur-1.5.0/lemur/api_keys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/api_keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/api_keys/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/api_keys/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/api_keys/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/api_keys/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17699 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/api_keys/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.639519 lemur-1.5.0/lemur/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/auth/ldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/auth/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/auth/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23702 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/auth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.639519 lemur-1.5.0/lemur/authorities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/authorities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/authorities/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/authorities/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/authorities/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19912 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/authorities/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.639519 lemur-1.5.0/lemur/authorizations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/authorizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/authorizations/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/authorizations/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.643519 lemur-1.5.0/lemur/certificates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/certificates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43757 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/certificates/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/certificates/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16901 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/certificates/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18872 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/certificates/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49034 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/certificates/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/certificates/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/certificates/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63990 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/certificates/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.643519 lemur-1.5.0/lemur/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37661 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/common/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/common/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/common/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/common/health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/common/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/common/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/common/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/common/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16434 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/common/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/default.conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.643519 lemur-1.5.0/lemur/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/defaults/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/defaults/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.643519 lemur-1.5.0/lemur/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/deployment/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.643519 lemur-1.5.0/lemur/destinations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/destinations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/destinations/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/destinations/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/destinations/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15233 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/destinations/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.643519 lemur-1.5.0/lemur/dns_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/dns_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/dns_providers/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/dns_providers/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/dns_providers/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/dns_providers/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/dns_providers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/dns_providers/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.643519 lemur-1.5.0/lemur/domains/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/domains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/domains/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/domains/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/domains/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/domains/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.647520 lemur-1.5.0/lemur/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/endpoints/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/endpoints/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/endpoints/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/endpoints/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.647520 lemur-1.5.0/lemur/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/logs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/logs/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/logs/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/logs/views.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17372 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.647520 lemur-1.5.0/lemur/notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/notifications/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21762 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/notifications/messaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/notifications/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/notifications/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/notifications/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16547 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/notifications/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.647520 lemur-1.5.0/lemur/pending_certificates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/pending_certificates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/pending_certificates/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/pending_certificates/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/pending_certificates/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11495 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/pending_certificates/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18984 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/pending_certificates/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.647520 lemur-1.5.0/lemur/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.647520 lemur-1.5.0/lemur/plugins/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/base/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/base/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.647520 lemur-1.5.0/lemur/plugins/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/bases/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/bases/destination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/bases/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/bases/issuer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/bases/membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/bases/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/bases/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/bases/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/bases/tls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.651520 lemur-1.5.0/lemur/plugins/lemur_acme/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_acme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26263 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_acme/acme_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_acme/challenge_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_acme/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9386 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_acme/dyn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9980 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_acme/nsone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17777 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_acme/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_acme/powerdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_acme/route53.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_acme/ultradns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.651520 lemur-1.5.0/lemur/plugins/lemur_adcs/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_adcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_adcs/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.651520 lemur-1.5.0/lemur/plugins/lemur_atlas/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_atlas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_atlas/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.651520 lemur-1.5.0/lemur/plugins/lemur_atlas_redis/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_atlas_redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_atlas_redis/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.651520 lemur-1.5.0/lemur/plugins/lemur_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_aws/cloudfront.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_aws/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_aws/elb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_aws/iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27872 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_aws/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_aws/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_aws/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_aws/sts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.651520 lemur-1.5.0/lemur/plugins/lemur_azure_dest/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_azure_dest/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6430 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_azure_dest/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.651520 lemur-1.5.0/lemur/plugins/lemur_cfssl/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_cfssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_cfssl/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.651520 lemur-1.5.0/lemur/plugins/lemur_cryptography/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_cryptography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9811 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_cryptography/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.651520 lemur-1.5.0/lemur/plugins/lemur_csr/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_csr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_csr/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.651520 lemur-1.5.0/lemur/plugins/lemur_digicert/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_digicert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23386 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_digicert/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.651520 lemur-1.5.0/lemur/plugins/lemur_email/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_email/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.655520 lemur-1.5.0/lemur/plugins/lemur_email/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_email/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11771 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_email/templates/authority_expiration.html
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_email/templates/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_email/templates/expiration.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_email/templates/expiration_summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_email/templates/expiring_deployed_certificate.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_email/templates/failed.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10451 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_email/templates/issued.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_email/templates/reissue_failed.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_email/templates/reissued_with_no_endpoints.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_email/templates/revocation.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_email/templates/rotation.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.655520 lemur-1.5.0/lemur/plugins/lemur_entrust/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_entrust/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_entrust/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.655520 lemur-1.5.0/lemur/plugins/lemur_jks/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_jks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_jks/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.655520 lemur-1.5.0/lemur/plugins/lemur_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_kubernetes/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.655520 lemur-1.5.0/lemur/plugins/lemur_openssl/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_openssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_openssl/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.655520 lemur-1.5.0/lemur/plugins/lemur_sftp/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_sftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_sftp/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.655520 lemur-1.5.0/lemur/plugins/lemur_slack/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_slack/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.655520 lemur-1.5.0/lemur/plugins/lemur_vault_dest/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_vault_dest/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13290 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_vault_dest/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.655520 lemur-1.5.0/lemur/plugins/lemur_verisign/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_verisign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/lemur_verisign/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/plugins/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.655520 lemur-1.5.0/lemur/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/policies/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/policies/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/policies/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/policies/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/pytest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.655520 lemur-1.5.0/lemur/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/reporting/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/reporting/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/reporting/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.655520 lemur-1.5.0/lemur/roles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/roles/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/roles/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/roles/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/roles/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.659521 lemur-1.5.0/lemur/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15343 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/sources/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/sources/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/sources/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/sources/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/sources/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.631519 lemur-1.5.0/lemur/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.659521 lemur-1.5.0/lemur/static/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/.buildignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/404.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.659521 lemur-1.5.0/lemur/static/app/angular/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.659521 lemur-1.5.0/lemur/static/app/angular/api_keys/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.659521 lemur-1.5.0/lemur/static/app/angular/api_keys/api_key/
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/api_keys/api_key/api_key.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/api_keys/api_key/api_key.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/api_keys/services.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.659521 lemur-1.5.0/lemur/static/app/angular/api_keys/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/api_keys/view/view.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/api_keys/view/view.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/app.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.659521 lemur-1.5.0/lemur/static/app/angular/authentication/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.659521 lemur-1.5.0/lemur/static/app/angular/authentication/login/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/authentication/login/login.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/authentication/login/login.tpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.659521 lemur-1.5.0/lemur/static/app/angular/authentication/logout/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/authentication/logout/logout.js
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/authentication/logout/logout.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/authentication/services.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.659521 lemur-1.5.0/lemur/static/app/angular/authorities/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.659521 lemur-1.5.0/lemur/static/app/angular/authorities/authority/
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/authorities/authority/authority.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/authorities/authority/authorityWizard.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/authorities/authority/distinguishedName.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/authorities/authority/edit.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/authorities/authority/extensions.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/authorities/authority/options.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/authorities/authority/permissions.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/authorities/authority/select.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/authorities/authority/tracking.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/authorities/services.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.659521 lemur-1.5.0/lemur/static/app/angular/authorities/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     8326 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/authorities/view/view.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/authorities/view/view.tpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.659521 lemur-1.5.0/lemur/static/app/angular/certificates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.663521 lemur-1.5.0/lemur/static/app/angular/certificates/certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    14102 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/certificates/certificate/certificate.js
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/certificates/certificate/certificateWizard.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/certificates/certificate/destinations.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/certificates/certificate/distinguishedName.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/certificates/certificate/edit.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/certificates/certificate/export.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/certificates/certificate/notifications.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/certificates/certificate/options.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/certificates/certificate/replaces.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/certificates/certificate/revoke.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10801 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/certificates/certificate/tracking.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/certificates/certificate/upload.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/certificates/certificate/upload.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12196 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/certificates/services.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.663521 lemur-1.5.0/lemur/static/app/angular/certificates/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/certificates/view/view.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/certificates/view/view.tpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.663521 lemur-1.5.0/lemur/static/app/angular/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/components/filters.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.663521 lemur-1.5.0/lemur/static/app/angular/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/dashboard/dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/dashboard/dashboard.tpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.663521 lemur-1.5.0/lemur/static/app/angular/destinations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.663521 lemur-1.5.0/lemur/static/app/angular/destinations/destination/
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/destinations/destination/destination.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/destinations/destination/destination.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/destinations/services.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.663521 lemur-1.5.0/lemur/static/app/angular/destinations/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/destinations/view/view.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/destinations/view/view.tpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.663521 lemur-1.5.0/lemur/static/app/angular/dns_providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.663521 lemur-1.5.0/lemur/static/app/angular/dns_providers/dns_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/dns_providers/dns_provider/dns_provider.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/dns_providers/dns_provider/dns_provider.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/dns_providers/services.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.663521 lemur-1.5.0/lemur/static/app/angular/dns_providers/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/dns_providers/view/view.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/dns_providers/view/view.tpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.663521 lemur-1.5.0/lemur/static/app/angular/domains/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.663521 lemur-1.5.0/lemur/static/app/angular/domains/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/domains/domain/domain.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/domains/domain/domain.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/domains/services.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.663521 lemur-1.5.0/lemur/static/app/angular/domains/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/domains/view/view.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/domains/view/view.tpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.663521 lemur-1.5.0/lemur/static/app/angular/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/endpoints/services.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.663521 lemur-1.5.0/lemur/static/app/angular/endpoints/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/endpoints/view/view.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/endpoints/view/view.tpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.663521 lemur-1.5.0/lemur/static/app/angular/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/logs/services.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.663521 lemur-1.5.0/lemur/static/app/angular/logs/view/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/logs/view/view.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/logs/view/view.tpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.663521 lemur-1.5.0/lemur/static/app/angular/notifications/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.663521 lemur-1.5.0/lemur/static/app/angular/notifications/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/notifications/notification/notification.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/notifications/notification/notification.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/notifications/services.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.663521 lemur-1.5.0/lemur/static/app/angular/notifications/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/notifications/view/view.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/notifications/view/view.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/pager.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.667521 lemur-1.5.0/lemur/static/app/angular/pending_certificates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.667521 lemur-1.5.0/lemur/static/app/angular/pending_certificates/pending_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/pending_certificates/pending_certificate/cancel.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/pending_certificates/pending_certificate/destinations.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/pending_certificates/pending_certificate/edit.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/pending_certificates/pending_certificate/notifications.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/pending_certificates/pending_certificate/pending_certificate.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/pending_certificates/pending_certificate/replaces.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/pending_certificates/pending_certificate/upload.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/pending_certificates/pending_certificate/upload.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/pending_certificates/services.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.667521 lemur-1.5.0/lemur/static/app/angular/pending_certificates/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/pending_certificates/view/view.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9422 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/pending_certificates/view/view.tpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.667521 lemur-1.5.0/lemur/static/app/angular/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/plugins/services.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.667521 lemur-1.5.0/lemur/static/app/angular/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.667521 lemur-1.5.0/lemur/static/app/angular/roles/role/
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/roles/role/role.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/roles/role/role.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/roles/role/roleSelect.tpl.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/roles/services.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.667521 lemur-1.5.0/lemur/static/app/angular/roles/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/roles/view/view.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/roles/view/view.tpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.667521 lemur-1.5.0/lemur/static/app/angular/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/sources/services.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.667521 lemur-1.5.0/lemur/static/app/angular/sources/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/sources/source/source.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/sources/source/source.tpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.667521 lemur-1.5.0/lemur/static/app/angular/sources/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/sources/view/view.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/sources/view/view.tpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.667521 lemur-1.5.0/lemur/static/app/angular/users/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/users/services.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.667521 lemur-1.5.0/lemur/static/app/angular/users/user/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/users/user/user.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/users/user/user.tpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.667521 lemur-1.5.0/lemur/static/app/angular/users/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/users/view/view.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/users/view/view.tpl.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.667521 lemur-1.5.0/lemur/static/app/angular/welcome/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/welcome/welcome.html
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/angular/wizard.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11153 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.667521 lemur-1.5.0/lemur/static/app/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/static/app/styles/lemur.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.671522 lemur-1.5.0/lemur/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11072 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.671522 lemur-1.5.0/lemur/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/plugins/destination_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/plugins/issuer_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/plugins/notification_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/plugins/source_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_authorities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59087 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_destinations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_dns_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_issuer_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_messaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_pending_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/test_verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38874 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/tests/vectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.671522 lemur-1.5.0/lemur/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/users/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/users/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/users/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/users/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-05 22:37:45.000000 lemur-1.5.0/lemur/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-05 22:38:48.054980 lemur-1.5.0/lemur-package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.639519 lemur-1.5.0/lemur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-05 22:37:56.000000 lemur-1.5.0/lemur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13735 2023-07-05 22:37:56.000000 lemur-1.5.0/lemur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 22:37:56.000000 lemur-1.5.0/lemur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-05 22:37:56.000000 lemur-1.5.0/lemur.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 22:37:56.000000 lemur-1.5.0/lemur.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-07-05 22:37:56.000000 lemur-1.5.0/lemur.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-05 22:37:56.000000 lemur-1.5.0/lemur.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-05 22:37:45.000000 lemur-1.5.0/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-05 22:37:45.000000 lemur-1.5.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-07-05 22:37:45.000000 lemur-1.5.0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-05 22:37:45.000000 lemur-1.5.0/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-05 22:37:45.000000 lemur-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-05 22:37:56.671522 lemur-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-07-05 22:37:45.000000 lemur-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:56.671522 lemur-1.5.0/trustores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:37:45.000000 lemur-1.5.0/trustores/__init__.py
```

### Comparing `lemur-1.4.0/LICENSE` & `lemur-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/PKG-INFO` & `lemur-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemur
-Version: 1.4.0
+Version: 1.5.0
 Summary: Certificate management and orchestration service
 Home-page: https://github.com/Netflix/lemur
 Author: The Lemur developers
 Author-email: security@netflix.com
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

### Comparing `lemur-1.4.0/README.rst` & `lemur-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/bower.json` & `lemur-1.5.0/bower.json`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/gulpfile.js` & `lemur-1.5.0/gulpfile.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/__about__.py` & `lemur-1.5.0/lemur/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,14 @@
     "__copyright__",
 ]
 
 __title__ = "lemur"
 __summary__ = "Certificate management and orchestration service"
 __uri__ = "https://github.com/Netflix/lemur"
 
-__version__ = "1.4.0"
+__version__ = "1.5.0"
 
 __author__ = "The Lemur developers"
 __email__ = "security@netflix.com"
 
 __license__ = "Apache License, Version 2.0"
 __copyright__ = "Copyright 2018 {0}".format(__author__)
```

### Comparing `lemur-1.4.0/lemur/__init__.py` & `lemur-1.5.0/lemur/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,14 +88,16 @@
 
     :param app:
     :return:
     """
     from flask import jsonify
     from werkzeug.exceptions import HTTPException
 
+    custom_response_headers = app.config.get("CUSTOM_RESPONSE_HEADERS", {})
+
     @app.errorhandler(Exception)
     def handle_error(e):
         code = 500
         if isinstance(e, HTTPException):
             code = e.code
 
         app.logger.exception(e)
@@ -103,14 +105,17 @@
 
     @app.before_request
     def before_request():
         g.request_start_time = time.time()
 
     @app.after_request
     def after_request(response):
+        # Update custom response headers
+        response.headers.update(custom_response_headers)
+
         # Return early if we don't have the start time
         if not hasattr(g, "request_start_time"):
             return response
 
         # Get elapsed time in milliseconds
         elapsed = time.time() - g.request_start_time
         elapsed = int(round(1000 * elapsed))
```

### Comparing `lemur-1.4.0/lemur/acme_providers/cli.py` & `lemur-1.5.0/lemur/acme_providers/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,137 +1,148 @@
 import time
 import json
 import arrow
+import click
 
-from flask_script import Manager
 from flask import current_app
 
 from sentry_sdk import capture_exception
 from lemur.common.utils import check_validation
 from lemur.constants import SUCCESS_METRIC_STATUS
 from lemur.plugins import plugins
 from lemur.plugins.lemur_acme.plugin import AcmeHandler
 from lemur.plugins.lemur_aws import s3
 
-manager = Manager(
-    usage="Handles all ACME related tasks"
-)
+
+@click.group(name="acme", help="Handles all ACME related tasks")
+def cli():
+    pass
 
 
-@manager.option(
+@cli.command("dnstest")
+@click.option(
     "-d",
     "--domain",
-    dest="domain",
+    "domain",
     required=True,
-    help="Name of the Domain to store to (ex. \"_acme-chall.test.com\".",
+    help="Name of the Domain to store to (ex. \"_acme-chall.test.com\"."
 )
-@manager.option(
+@click.option(
     "-t",
     "--token",
-    dest="token",
+    "token",
     required=True,
-    help="Value of the Token to store in DNS as content.",
+    help="Value of the Token to store in DNS as content."
 )
+def dnstest_command(domain, token):
+    dnstest(domain, token)
+
+
 def dnstest(domain, token):
     """
     Create, verify, and delete DNS TXT records using an autodetected provider.
     """
-    print("[+] Starting ACME Tests.")
+    click.echo("[+] Starting ACME Tests.")
     change_id = (domain, token)
 
     acme_handler = AcmeHandler()
     acme_handler.autodetect_dns_providers(domain)
     if not acme_handler.dns_providers_for_domain[domain]:
         raise Exception(f"No DNS providers found for domain: {format(domain)}.")
 
     # Create TXT Records
     for dns_provider in acme_handler.dns_providers_for_domain[domain]:
         dns_provider_plugin = acme_handler.get_dns_provider(dns_provider.provider_type)
         dns_provider_options = json.loads(dns_provider.credentials)
         account_number = dns_provider_options.get("account_id")
 
-        print(f"[+] Creating TXT Record in `{dns_provider.name}` provider")
+        click.echo(f"[+] Creating TXT Record in `{dns_provider.name}` provider")
         change_id = dns_provider_plugin.create_txt_record(domain, token, account_number)
 
-    print("[+] Verifying TXT Record has propagated to DNS.")
-    print("[+] This step could take a while...")
+    click.echo("[+] Verifying TXT Record has propagated to DNS.")
+    click.echo("[+] This step could take a while...")
     time.sleep(10)
 
     # Verify TXT Records
     for dns_provider in acme_handler.dns_providers_for_domain[domain]:
         dns_provider_plugin = acme_handler.get_dns_provider(dns_provider.provider_type)
         dns_provider_options = json.loads(dns_provider.credentials)
         account_number = dns_provider_options.get("account_id")
 
         try:
             dns_provider_plugin.wait_for_dns_change(change_id, account_number)
-            print(f"[+] Verified TXT Record in `{dns_provider.name}` provider")
+            click.echo(f"[+] Verified TXT Record in `{dns_provider.name}` provider")
         except Exception:
             capture_exception()
             current_app.logger.debug(
                 f"Unable to resolve DNS challenge for change_id: {change_id}, account_id: "
                 f"{account_number}",
                 exc_info=True,
             )
-            print(f"[+] Unable to Verify TXT Record in `{dns_provider.name}` provider")
+            click.echo(f"[+] Unable to Verify TXT Record in `{dns_provider.name}` provider")
 
     time.sleep(10)
 
     # Delete TXT Records
     for dns_provider in acme_handler.dns_providers_for_domain[domain]:
         dns_provider_plugin = acme_handler.get_dns_provider(dns_provider.provider_type)
         dns_provider_options = json.loads(dns_provider.credentials)
         account_number = dns_provider_options.get("account_id")
 
         # TODO(csine@: Add Exception Handling
         dns_provider_plugin.delete_txt_record(change_id, account_number, domain, token)
-        print(f"[+] Deleted TXT Record in `{dns_provider.name}` provider")
+        click.echo(f"[+] Deleted TXT Record in `{dns_provider.name}` provider")
 
     status = SUCCESS_METRIC_STATUS
-    print("[+] Done with ACME Tests.")
+    click.echo("[+] Done with ACME Tests.")
 
 
-@manager.option(
+@cli.command("upload_acme_token_s3")
+@click.option(
     "-t",
     "--token",
-    dest="token",
+    "token",
     default="date: " + arrow.utcnow().format("YYYY-MM-DDTHH-mm-ss"),
     required=False,
-    help="Value of the Token",
+    help="Value of the Token to store in DNS as content."
 )
-@manager.option(
+@click.option(
     "-n",
     "--token_name",
-    dest="token_name",
+    "token_name",
     default="Token-" + arrow.utcnow().format("YYYY-MM-DDTHH-mm-ss"),
     required=False,
-    help="path",
+    help="path"
 )
-@manager.option(
+@click.option(
     "-p",
     "--prefix",
-    dest="prefix",
+    "prefix",
     default="test/",
     required=False,
-    help="S3 bucket prefix",
+    help="S3 bucket prefix"
 )
-@manager.option(
+@click.option(
     "-a",
     "--account_number",
-    dest="account_number",
+    "account_number",
     required=True,
-    help="AWS Account",
+    help="AWS Account"
 )
-@manager.option(
+@click.option(
     "-b",
     "--bucket_name",
-    dest="bucket_name",
+    "bucket_name",
     required=True,
     help="Bucket Name",
 )
+def upload_acme_token_s3_command(token, token_name, prefix, account_number, bucket_name):
+    upload_acme_token_s3(token, token_name, prefix, account_number, bucket_name)
+
+
 def upload_acme_token_s3(token, token_name, prefix, account_number, bucket_name):
     """
     This method serves for testing the upload_acme_token to S3, fetching the token to verify it, and then deleting it.
     It mainly serves for testing purposes.
     :param token:
     :param token_name:
     :param prefix:
@@ -184,9 +195,9 @@
     p = plugins.get("aws-s3")
     p.upload_acme_token(token_name, token, additional_options)
 
     if not prefix.endswith("/"):
         prefix + "/"
 
     token_res = s3.get(bucket_name, prefix + token_name, account_number=account_number)
-    assert(token_res == token)
+    assert (token_res == token)
     s3.delete(bucket_name, prefix + token_name, account_number=account_number)
```

### Comparing `lemur-1.4.0/lemur/api_keys/cli.py` & `lemur-1.5.0/lemur/plugins/bases/notification.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,69 @@
 """
-.. module: lemur.api_keys.cli
+.. module: lemur.plugins.bases.notification
     :platform: Unix
     :copyright: (c) 2018 by Netflix Inc., see AUTHORS for more
     :license: Apache, see LICENSE for more details.
-.. moduleauthor:: Eric Coan <kungfury@instructure.com>
+
+.. moduleauthor:: Kevin Glisson <kglisson@netflix.com>
 """
-from flask_script import Manager
-from lemur.api_keys import service as api_key_service
-from lemur.auth.service import create_token
-
-from datetime import datetime
-
-manager = Manager(usage="Handles all api key related tasks.")
-
-
-@manager.option(
-    "-u", "--user-id", dest="uid", help="The User ID this access key belongs too."
-)
-@manager.option("-n", "--name", dest="name", help="The name of this API Key.")
-@manager.option(
-    "-t", "--ttl", dest="ttl", help="The TTL of this API Key. -1 for forever."
-)
-def create(uid, name, ttl):
+from lemur.common.utils import check_validation
+from lemur.plugins.base import Plugin
+
+
+class NotificationPlugin(Plugin):
     """
-    Create a new api key for a user.
-    :return:
+    This is the base class from which all of the supported
+    issuers will inherit from.
     """
-    print("[+] Creating a new api key.")
-    key = api_key_service.create(
-        user_id=uid,
-        name=name,
-        ttl=ttl,
-        issued_at=int(datetime.utcnow().timestamp()),
-        revoked=False,
-    )
-    print("[+] Successfully created a new api key. Generating a JWT...")
-    jwt = create_token(uid, key.id, key.ttl)
-    print("[+] Your JWT is: {jwt}".format(jwt=jwt))
 
+    type = "notification"
+
+    def send(self, notification_type, message, targets, options, **kwargs):
+        raise NotImplementedError
+
+    def get_recipients(self, options, additional_recipients):
+        """
+        Given a set of options (which should include configured recipient info), returns the parsed list of recipients
+        from those options plus the additional recipients specified. The returned value has no duplicates.
 
-@manager.option("-a", "--api-key-id", dest="aid", help="The API Key ID to revoke.")
-def revoke(aid):
+        For any notification types where recipients can't be dynamically modified, this returns only the additional recipients.
+        """
+        return additional_recipients
+
+
+class ExpirationNotificationPlugin(NotificationPlugin):
     """
-    Revokes an api key for a user.
-    :return:
+    This is the base class for all expiration notification plugins.
+    It contains some default options that are needed for all expiration
+    notification plugins.
     """
-    print("[-] Revoking the API Key api key.")
-    api_key_service.revoke(aid=aid)
-    print("[+] Successfully revoked the api key")
+
+    default_options = [
+        {
+            "name": "interval",
+            "type": "int",
+            "required": True,
+            "validation": check_validation(r"^\d+$"),
+            "helpMessage": "Number of days to be alert before expiration.",
+        },
+        {
+            "name": "unit",
+            "type": "select",
+            "required": True,
+            "validation": check_validation(""),
+            "available": ["days", "weeks", "months"],
+            "helpMessage": "Interval unit",
+        },
+    ]
+
+    @property
+    def options(self):
+        """
+        Gets/sets options for the plugin.
+
+        :return:
+        """
+        return self.default_options + self.additional_options
+
+    def send(self, notification_type, message, excluded_targets, options, **kwargs):
+        raise NotImplementedError
```

### Comparing `lemur-1.4.0/lemur/api_keys/models.py` & `lemur-1.5.0/lemur/api_keys/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
     :synopsis: This module contains all of the models need to create an api key within Lemur.
     :copyright: (c) 2018 by Netflix Inc., see AUTHORS for more
     :license: Apache, see LICENSE for more details.
 .. moduleauthor:: Eric Coan <kungfury@instructure.com>
 """
 from sqlalchemy import BigInteger, Boolean, Column, ForeignKey, Integer, String
 
-from lemur.database import db
+from lemur.database import BaseModel
 
 
-class ApiKey(db.Model):
+class ApiKey(BaseModel):
     __tablename__ = "api_keys"
     id = Column(Integer, primary_key=True)
     name = Column(String)
     user_id = Column(Integer, ForeignKey("users.id"))
     ttl = Column(BigInteger)
     issued_at = Column(BigInteger)
     revoked = Column(Boolean)
```

### Comparing `lemur-1.4.0/lemur/api_keys/schemas.py` & `lemur-1.5.0/lemur/api_keys/schemas.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/api_keys/service.py` & `lemur-1.5.0/lemur/api_keys/service.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/api_keys/views.py` & `lemur-1.5.0/lemur/api_keys/views.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/auth/ldap.py` & `lemur-1.5.0/lemur/auth/ldap.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/auth/permissions.py` & `lemur-1.5.0/lemur/auth/permissions.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from flask import current_app
 from flask_principal import Permission, RoleNeed
 
 # Permissions
 operator_permission = Permission(RoleNeed("operator"))
 admin_permission = Permission(RoleNeed("admin"))
 
-CertificateOwner = namedtuple("certificate", ["method", "value"])
+CertificateOwner = namedtuple("CertificateOwner", ["method", "value"])
 CertificateOwnerNeed = partial(CertificateOwner, "role")
 
 
 class SensitiveDomainPermission(Permission):
     def __init__(self):
         needs = [RoleNeed("admin")]
         sensitive_domain_roles = current_app.config.get("SENSITIVE_DOMAIN_ROLES", [])
@@ -45,28 +45,28 @@
 
 
 class ApiKeyCreatorPermission(Permission):
     def __init__(self):
         super(ApiKeyCreatorPermission, self).__init__(RoleNeed("admin"))
 
 
-RoleMember = namedtuple("role", ["method", "value"])
+RoleMember = namedtuple("RoleMember", ["method", "value"])
 RoleMemberNeed = partial(RoleMember, "member")
 
 
 class RoleMemberPermission(Permission):
     def __init__(self, role_id):
         needs = [RoleNeed("admin"), RoleMemberNeed(role_id)]
         super(RoleMemberPermission, self).__init__(*needs)
 
 
-AuthorityCreator = namedtuple("authority", ["method", "value"])
+AuthorityCreator = namedtuple("AuthorityCreator", ["method", "value"])
 AuthorityCreatorNeed = partial(AuthorityCreator, "authorityUse")
 
-AuthorityOwner = namedtuple("authority", ["method", "value"])
+AuthorityOwner = namedtuple("AuthorityOwner", ["method", "value"])
 AuthorityOwnerNeed = partial(AuthorityOwner, "role")
 
 
 class AuthorityPermission(Permission):
     def __init__(self, authority_id, roles):
         needs = [RoleNeed("admin"), AuthorityCreatorNeed(str(authority_id))]
         for r in roles:
```

### Comparing `lemur-1.4.0/lemur/auth/service.py` & `lemur-1.5.0/lemur/auth/service.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/auth/views.py` & `lemur-1.5.0/lemur/auth/views.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/authorities/models.py` & `lemur-1.5.0/lemur/authorities/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
     ForeignKey,
     DateTime,
     DefaultClause,
     Boolean,
 )
 from sqlalchemy.dialects.postgresql import JSON
 
-from lemur.database import db
+from lemur.database import BaseModel, db
 from lemur.plugins.base import plugins
 from lemur.models import roles_authorities
 
 
-class Authority(db.Model):
+class Authority(BaseModel):
     __tablename__ = "authorities"
     id = Column(Integer, primary_key=True)
     owner = Column(String(128), nullable=False)
     name = Column(String(128), unique=True)
     body = Column(Text())
     chain = Column(Text())
     active = Column(Boolean, default=True)
```

### Comparing `lemur-1.4.0/lemur/authorities/schemas.py` & `lemur-1.5.0/lemur/authorities/schemas.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/authorities/service.py` & `lemur-1.5.0/lemur/authorities/service.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/authorities/views.py` & `lemur-1.5.0/lemur/authorities/views.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/authorizations/models.py` & `lemur-1.5.0/lemur/authorizations/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,20 +3,20 @@
     :platform: unix
     :copyright: (c) 2018 by Netflix Inc., see AUTHORS for more
     :license: Apache, see LICENSE for more details.
 .. moduleauthor:: Netflix Secops <secops@netflix.com>
 """
 from sqlalchemy import Column, Integer, String
 from sqlalchemy_utils import JSONType
-from lemur.database import db
+from lemur.database import BaseModel
 
 from lemur.plugins.base import plugins
 
 
-class Authorization(db.Model):
+class Authorization(BaseModel):
     __tablename__ = "pending_dns_authorizations"
     id = Column(Integer, primary_key=True, autoincrement=True)
     account_number = Column(String(128))
     domains = Column(JSONType)
     dns_provider_type = Column(String(128))
     options = Column(JSONType)
```

### Comparing `lemur-1.4.0/lemur/authorizations/service.py` & `lemur-1.5.0/lemur/authorizations/service.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/certificates/cli.py` & `lemur-1.5.0/lemur/certificates/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,17 +3,18 @@
     :platform: Unix
     :copyright: (c) 2018 by Netflix Inc., see AUTHORS for more
     :license: Apache, see LICENSE for more details.
 .. moduleauthor:: Kevin Glisson <kglisson@netflix.com>
 """
 import arrow
 import sys
+import click
+
 from flask import current_app
 from flask_principal import Identity, identity_changed
-from flask_script import Manager
 from sqlalchemy import or_
 from tabulate import tabulate
 from time import sleep
 from sentry_sdk import capture_exception
 
 from lemur import database
 from lemur.authorities.models import Authority
@@ -27,42 +28,45 @@
     get_all_pending_reissue,
     get_by_name,
     get_all_valid_certs,
     get,
     get_all_certs_attached_to_endpoint_without_autorotate,
     get_all_certs_attached_to_destination_without_autorotate,
     revoke as revoke_certificate,
-    list_duplicate_certs_by_authority,
-    get_certificates_with_same_prefix_with_rotate_on,
+    list_recent_valid_certs_issued_by_authority,
+    get_certificates_with_same_cn_with_rotate_on,
     identify_and_persist_expiring_deployed_certificates,
     send_certificate_expiration_metrics
 )
 from lemur.certificates.verify import verify_string
 from lemur.constants import SUCCESS_METRIC_STATUS, FAILURE_METRIC_STATUS, CRLReason
 from lemur.deployment import service as deployment_service
 from lemur.domains.models import Domain
 from lemur.endpoints import service as endpoint_service
 from lemur.extensions import metrics
 from lemur.notifications.messaging import send_rotation_notification, send_reissue_no_endpoints_notification, \
     send_reissue_failed_notification
 from lemur.plugins.base import plugins
 from sqlalchemy.orm.exc import MultipleResultsFound
 
-manager = Manager(usage="Handles all certificate related tasks.")
+
+@click.group(name="certificates", help="Handles all certificate related tasks.")
+def cli():
+    pass
 
 
 def print_certificate_details(details):
     """
     Print the certificate details with formatting.
     :param details:
     :return:
     """
     details, errors = CertificateOutputSchema().dump(details)
-    print("[+] Re-issuing certificate with the following details: ")
-    print(
+    click.echo("[+] Re-issuing certificate with the following details: ")
+    click.echo(
         "\t[+] Common Name: {common_name}\n"
         "\t[+] Subject Alternate Names: {sans}\n"
         "\t[+] Authority: {authority_name}\n"
         "\t[+] Validity Start: {validity_start}\n"
         "\t[+] Validity End: {validity_end}\n".format(
             common_name=details["commonName"],
             sans=",".join(
@@ -82,15 +86,15 @@
     :param certificate_name:
     :return:
     """
     if certificate_name:
         cert = get_by_name(certificate_name)
 
         if not cert:
-            print("[-] No certificate found with name: {0}".format(certificate_name))
+            click.echo("[-] No certificate found with name: {0}".format(certificate_name))
             sys.exit(1)
 
         return cert
 
 
 def validate_endpoint(endpoint_name):
     """
@@ -98,15 +102,15 @@
     :param endpoint_name:
     :return:
     """
     if endpoint_name:
         endpoint = endpoint_service.get_by_name(endpoint_name)
 
         if not endpoint:
-            print("[-] No endpoint found with name: {0}".format(endpoint_name))
+            click.echo("[-] No endpoint found with name: {0}".format(endpoint_name))
             sys.exit(1)
 
         return endpoint
 
 
 def validate_endpoint_from_source(endpoint_name, source):
     """
@@ -115,15 +119,15 @@
     :param source:
     :return:
     """
     if endpoint_name and source:
         endpoint = endpoint_service.get_by_name_and_source(endpoint_name, source)
 
         if not endpoint:
-            print("[-] No endpoint found from source {0} with name: {1}".format(source, endpoint_name))
+            click.echo("[-] No endpoint found from source {0} with name: {1}".format(source, endpoint_name))
             sys.exit(1)
 
         return endpoint
 
 
 def request_rotation(endpoint, certificate, message, commit):
     """
@@ -147,15 +151,15 @@
 
         except Exception as e:
             capture_exception(extra={"certificate_name": str(certificate.name),
                                      "endpoint": str(endpoint.dnsname)})
             current_app.logger.exception(
                 f"Error rotating certificate: {certificate.name}", exc_info=True
             )
-            print(
+            click.echo(
                 "[!] Failed to rotate endpoint {0} to certificate {1} reason: {2}".format(
                     endpoint.name, certificate.name, e
                 )
             )
 
     metrics.send("endpoint_rotation", "counter", 1, metric_tags={"status": status,
                                                                  "certificate_name": str(certificate.name),
@@ -169,95 +173,100 @@
     :param notify:
     :param commit:
     :return:
     """
     status = FAILURE_METRIC_STATUS
     notify = notify and certificate.notify
     try:
-        print("[+] {0} is eligible for re-issuance".format(certificate.name))
+        click.echo("[+] {0} is eligible for re-issuance".format(certificate.name))
 
         # set the lemur identity for all cli commands
         identity_changed.send(current_app._get_current_object(), identity=Identity(1))
 
         details = get_certificate_primitives(certificate)
         print_certificate_details(details)
 
         if commit:
             new_cert = reissue_certificate(certificate, notify=notify, replace=True)
-            print("[+] New certificate named: {0}".format(new_cert.name))
+            click.echo("[+] New certificate named: {0}".format(new_cert.name))
             if notify and isinstance(new_cert, Certificate):  # let celery handle PendingCertificates
                 send_reissue_no_endpoints_notification(certificate, new_cert)
 
         status = SUCCESS_METRIC_STATUS
 
     except Exception as e:
         capture_exception(extra={"certificate_name": str(certificate.name)})
         current_app.logger.exception(
             f"Error reissuing certificate: {certificate.name}", exc_info=True
         )
-        print(f"[!] Failed to reissue certificate: {certificate.name}. Reason: {e}")
+        click.echo(f"[!] Failed to reissue certificate: {certificate.name}. Reason: {e}")
         if notify:
             send_reissue_failed_notification(certificate)
 
     metrics.send(
         "certificate_reissue",
         "counter",
         1,
         metric_tags={"status": status, "certificate": certificate.name},
     )
 
 
-@manager.option(
+@click.option(
     "-e",
     "--endpoint",
-    dest="endpoint_name",
+    "endpoint_name",
     help="Name of the endpoint you wish to rotate.",
 )
-@manager.option(
+@click.option(
     "-s",
     "--source",
-    dest="source",
+    "source",
     help="Source of the endpoint you wish to rotate.",
 )
-@manager.option(
+@click.option(
     "-n",
     "--new-certificate",
-    dest="new_certificate_name",
+    "new_certificate_name",
     help="Name of the certificate you wish to rotate to.",
 )
-@manager.option(
+@click.option(
     "-o",
     "--old-certificate",
-    dest="old_certificate_name",
+    "old_certificate_name",
     help="Name of the certificate you wish to rotate.",
 )
-@manager.option(
+@click.option(
     "-a",
     "--notify",
-    dest="message",
-    action="store_true",
+    "message",
+    type=bool,
+    default=False,
     help="Send a rotation notification to the certificates owner.",
 )
-@manager.option(
+@click.option(
     "-c",
     "--commit",
-    dest="commit",
-    action="store_true",
+    "commit",
+    type=bool,
     default=False,
     help="Persist changes.",
 )
+def rotate_command(endpoint_name, source, new_certificate_name, old_certificate_name, message, commit):
+    rotate(endpoint_name, source, new_certificate_name, old_certificate_name, message, commit)
+
+
 def rotate(endpoint_name, source, new_certificate_name, old_certificate_name, message, commit):
     """
     Rotates an endpoint and reissues it if it has not already been replaced. If it has
     been replaced, will use the replacement certificate for the rotation.
     """
     if commit:
-        print("[!] Running in COMMIT mode.")
+        click.echo("[!] Running in COMMIT mode.")
 
-    print("[+] Starting endpoint rotation.")
+    click.echo("[+] Starting endpoint rotation.")
 
     status = FAILURE_METRIC_STATUS
 
     log_data = {
         "function": f"{__name__}.{sys._getframe().f_code.co_name}",
     }
 
@@ -266,62 +275,62 @@
         new_cert = validate_certificate(new_certificate_name)
         if source:
             endpoint = validate_endpoint_from_source(endpoint_name, source)
         else:
             try:
                 endpoint = validate_endpoint(endpoint_name)
             except MultipleResultsFound as e:
-                print("[!] Multiple endpoints found with name {0}, try narrowing the search down to an endpoint from a specific source by re-running this command with the --source flag.".format(endpoint_name))
+                click.echo("[!] Multiple endpoints found with name {0}, try narrowing the search down to an endpoint from a specific source by re-running this command with the --source flag.".format(endpoint_name))
                 log_data["message"] = "Multiple endpoints found with same name, unable to perform rotation"
                 log_data["duplicated_endpoint_name"] = endpoint_name
                 current_app.logger.info(log_data)
                 raise
 
         if endpoint and new_cert:
-            print(
+            click.echo(
                 f"[+] Rotating endpoint: {endpoint.name} to certificate {new_cert.name}"
             )
             log_data["message"] = "Rotating one endpoint"
             log_data["endpoint"] = endpoint.dnsname
             log_data["certificate"] = new_cert.name
             request_rotation(endpoint, new_cert, message, commit)
             current_app.logger.info(log_data)
 
         elif old_cert and new_cert:
-            print(f"[+] Rotating all endpoints from {old_cert.name} to {new_cert.name}")
+            click.echo(f"[+] Rotating all endpoints from {old_cert.name} to {new_cert.name}")
             log_data["certificate"] = new_cert.name
             log_data["certificate_old"] = old_cert.name
             log_data["message"] = "Rotating endpoint from old to new cert"
             for endpoint in old_cert.endpoints:
-                print(f"[+] Rotating {endpoint.name}")
+                click.echo(f"[+] Rotating {endpoint.name}")
                 log_data["endpoint"] = endpoint.dnsname
                 request_rotation(endpoint, new_cert, message, commit)
                 current_app.logger.info(log_data)
 
         else:
             # No certificate name or endpoint is provided. We will now fetch all endpoints,
             # which are associated with a certificate that has been replaced
-            print("[+] Rotating all endpoints that have new certificates available")
+            click.echo("[+] Rotating all endpoints that have new certificates available")
             for endpoint in endpoint_service.get_all_pending_rotation():
 
                 log_data["message"] = "Rotating endpoint from old to new cert"
                 if len(endpoint.certificate.replaced) > 1:
                     log_data["message"] = f"Multiple replacement certificates found, going with the first one out of " \
                                           f"{len(endpoint.certificate.replaced)}"
 
                 log_data["endpoint"] = endpoint.dnsname
                 log_data["certificate"] = endpoint.certificate.replaced[0].name
-                print(
+                click.echo(
                     f"[+] Rotating {endpoint.name} to {endpoint.certificate.replaced[0].name}"
                 )
                 request_rotation(endpoint, endpoint.certificate.replaced[0], message, commit)
                 current_app.logger.info(log_data)
 
         status = SUCCESS_METRIC_STATUS
-        print("[+] Done!")
+        click.echo("[+] Done!")
 
     except Exception as e:
         capture_exception(
             extra={
                 "old_certificate_name": str(old_certificate_name),
                 "new_certificate_name": str(new_certificate_name),
                 "endpoint_name": str(endpoint_name),
@@ -347,74 +356,80 @@
 def request_rotation_region(endpoint, new_cert, message, commit, log_data, region):
     if region in endpoint.dnsname:
         log_data["message"] = "Rotating endpoint in region"
         request_rotation(endpoint, new_cert, message, commit)
     else:
         log_data["message"] = "Skipping rotation, region mismatch"
 
-    print(log_data)
+    click.echo(log_data)
     current_app.logger.info(log_data)
 
 
-@manager.option(
+@cli.command("rotate_region")
+@click.option(
     "-e",
     "--endpoint",
-    dest="endpoint_name",
+    "endpoint_name",
     help="Name of the endpoint you wish to rotate.",
 )
-@manager.option(
+@click.option(
     "-n",
     "--new-certificate",
-    dest="new_certificate_name",
+    "new_certificate_name",
     help="Name of the certificate you wish to rotate to.",
 )
-@manager.option(
+@click.option(
     "-o",
     "--old-certificate",
-    dest="old_certificate_name",
+    "old_certificate_name",
     help="Name of the certificate you wish to rotate.",
 )
-@manager.option(
+@click.option(
     "-a",
     "--notify",
-    dest="message",
-    action="store_true",
+    "message",
+    type=bool,
+    default=False,
     help="Send a rotation notification to the certificates owner.",
 )
-@manager.option(
+@click.option(
     "-c",
     "--commit",
-    dest="commit",
-    action="store_true",
+    "commit",
+    type=bool,
     default=False,
     help="Persist changes.",
 )
-@manager.option(
+@click.option(
     "-r",
     "--region",
-    dest="region",
+    "region",
     required=True,
     help="Region in which to rotate the endpoint.",
 )
+def rotate_region_command(endpoint_name, new_certificate_name, old_certificate_name, message, commit, region):
+    rotate_region(endpoint_name, new_certificate_name, old_certificate_name, message, commit, region)
+
+
 def rotate_region(endpoint_name, new_certificate_name, old_certificate_name, message, commit, region):
     """
     Rotates an endpoint in a defined region it if it has not already been replaced. If it has
     been replaced, will use the replacement certificate for the rotation.
     :param old_certificate_name: Name of the certificate you wish to rotate.
     :param new_certificate_name: Name of the certificate you wish to rotate to.
     :param endpoint_name: Name of the endpoint you wish to rotate.
     :param message: Send a rotation notification to the certificates owner.
     :param commit: Persist changes.
     :param region: Region in which to rotate the endpoint.
     #todo: merge this method with rotate()
     """
     if commit:
-        print("[!] Running in COMMIT mode.")
+        click.echo("[!] Running in COMMIT mode.")
 
-    print("[+] Starting endpoint rotation.")
+    click.echo("[+] Starting endpoint rotation.")
     status = FAILURE_METRIC_STATUS
 
     log_data = {
         "function": f"{__name__}.{sys._getframe().f_code.co_name}",
         "region": region,
     }
 
@@ -428,30 +443,30 @@
             log_data["certificate"] = new_cert.name
             request_rotation_region(endpoint, new_cert, message, commit, log_data, region)
 
         elif old_cert and new_cert:
             log_data["certificate"] = new_cert.name
             log_data["certificate_old"] = old_cert.name
             log_data["message"] = "Rotating endpoint from old to new cert"
-            print(log_data)
+            click.echo(log_data)
             current_app.logger.info(log_data)
             for endpoint in old_cert.endpoints:
                 log_data["endpoint"] = endpoint.dnsname
                 request_rotation_region(endpoint, new_cert, message, commit, log_data, region)
 
         else:
             log_data["message"] = "Rotating all endpoints that have new certificates available"
-            print(log_data)
+            click.echo(log_data)
             current_app.logger.info(log_data)
             all_pending_rotation_endpoints = endpoint_service.get_all_pending_rotation()
             for endpoint in all_pending_rotation_endpoints:
                 log_data["endpoint"] = endpoint.dnsname
                 if region not in endpoint.dnsname:
                     log_data["message"] = "Skipping rotation, region mismatch"
-                    print(log_data)
+                    click.echo(log_data)
                     current_app.logger.info(log_data)
                     metrics.send(
                         "endpoint_rotation_region_skipped",
                         "counter",
                         1,
                         metric_tags={
                             "region": region,
@@ -479,15 +494,15 @@
                         "new_certificate_name": str(log_data["certificate"]),
                         "endpoint_name": str(endpoint.dnsname),
                         "message": str(message),
                         "region": str(region),
                     },
                 )
         status = SUCCESS_METRIC_STATUS
-        print("[+] Done!")
+        click.echo("[+] Done!")
 
     except Exception as e:
         capture_exception(
             extra={
                 "old_certificate_name": str(old_certificate_name),
                 "new_certificate_name": str(new_certificate_name),
                 "endpoint": str(endpoint_name),
@@ -508,85 +523,96 @@
             "message": str(message),
             "endpoint": str(globals().get("endpoint")),
             "region": str(region),
         },
     )
 
 
-@manager.option(
+@cli.command("reissue")
+@click.option(
     "-o",
     "--old-certificate",
-    dest="old_certificate_name",
+    "old_certificate_name",
     help="Name of the certificate you wish to reissue.",
 )
-@manager.option(
+@click.option(
     "-a",
     "--notify",
-    dest="notify",
-    action="store_true",
+    "notify",
+    type=bool,
+    default=False,
     help="Send a re-issue failed notification to the certificates owner (if re-issuance fails).",
 )
-@manager.option(
+@click.option(
     "-c",
     "--commit",
-    dest="commit",
-    action="store_true",
+    "commit",
+    type=bool,
     default=False,
     help="Persist changes.",
 )
+def reissue_command(old_certificate_name, notify, commit):
+    reissue(old_certificate_name, notify, commit)
+
+
 def reissue(old_certificate_name, notify, commit):
     """
     Reissues certificate with the same parameters as it was originally issued with.
     If not time period is provided, reissues certificate as valid from today to
     today + length of original.
     """
     if commit:
-        print("[!] Running in COMMIT mode.")
+        click.echo("[!] Running in COMMIT mode.")
 
-    print("[+] Starting certificate re-issuance.")
+    click.echo("[+] Starting certificate re-issuance.")
 
     status = FAILURE_METRIC_STATUS
 
     try:
         old_cert = validate_certificate(old_certificate_name)
 
         if not old_cert:
             for certificate in get_all_pending_reissue():
                 request_reissue(certificate, notify, commit)
         else:
             request_reissue(old_cert, notify, commit)
 
         status = SUCCESS_METRIC_STATUS
-        print("[+] Done!")
+        click.echo("[+] Done!")
     except Exception as e:
         capture_exception()
         current_app.logger.exception("Error reissuing certificate.", exc_info=True)
-        print("[!] Failed to reissue certificates. Reason: {}".format(e))
+        click.echo("[!] Failed to reissue certificates. Reason: {}".format(e))
 
     metrics.send(
         "certificate_reissue_job", "counter", 1, metric_tags={"status": status}
     )
 
 
-@manager.option(
+@cli.command("query")
+@click.option(
     "-f",
     "--fqdns",
-    dest="fqdns",
+    "fqdns",
     help="FQDNs to query. Multiple fqdns specified via comma.",
 )
-@manager.option("-i", "--issuer", dest="issuer", help="Issuer to query for.")
-@manager.option("-o", "--owner", dest="owner", help="Owner to query for.")
-@manager.option(
+@click.option("-i", "--issuer", "issuer", help="Issuer to query for.")
+@click.option("-o", "--owner", "owner", help="Owner to query for.")
+@click.option(
     "-e",
     "--expired",
-    dest="expired",
+    "expired",
     type=bool,
     default=False,
     help="Include expired certificates.",
 )
+def query_command(fqdns, issuer, owner, expired):
+    query(fqdns, issuer, owner, expired)
+
+
 def query(fqdns, issuer, owner, expired):
     """Prints certificates that match the query params."""
     table = []
 
     q = database.session_query(Certificate)
     if issuer:
         sub_query = (
@@ -615,23 +641,23 @@
                     Certificate.domains.any(Domain.name.ilike("%{0}%".format(f))),
                 )
             )
 
     for c in q.all():
         table.append([c.id, c.name, c.owner, c.issuer])
 
-    print(tabulate(table, headers=["Id", "Name", "Owner", "Issuer"], tablefmt="csv"))
+    click.echo(tabulate(table, headers=["Id", "Name", "Owner", "Issuer"], tablefmt="csv"))
 
 
 def worker(data, commit, reason):
     parts = [x for x in data.split(" ") if x]
     try:
         cert = get(int(parts[0].strip()))
 
-        print("[+] Revoking certificate. Id: {0} Name: {1}".format(cert.id, cert.name))
+        click.echo("[+] Revoking certificate. Id: {0} Name: {1}".format(cert.id, cert.name))
         if commit:
             revoke_certificate(cert, reason)
 
         metrics.send(
             "certificate_revoke",
             "counter",
             1,
@@ -642,68 +668,81 @@
         capture_exception()
         metrics.send(
             "certificate_revoke",
             "counter",
             1,
             metric_tags={"status": FAILURE_METRIC_STATUS},
         )
-        print("[!] Failed to revoke certificates. Reason: {}".format(e))
+        click.echo("[!] Failed to revoke certificates. Reason: {}".format(e))
+
+
+@cli.command("clear_pending")
+def clear_pending_command():
+    clear_pending()
 
 
-@manager.command
 def clear_pending():
     """
     Function clears all pending certificates.
     :return:
     """
     v = plugins.get("verisign-issuer")
     v.clear_pending_certificates()
 
 
-@manager.option("-p", "--path", dest="path", help="Absolute file path to a Lemur query csv.")
-@manager.option("-id", "--certid", dest="cert_id", help="ID of the certificate to be revoked")
-@manager.option("-r", "--reason", dest="reason", default="unspecified", help="CRL Reason as per RFC 5280 section 5.3.1")
-@manager.option("-m", "--message", dest="message", help="Message explaining reason for revocation")
-@manager.option(
+@cli.command("revoke")
+@click.option("-p", "--path", "path", help="Absolute file path to a Lemur query csv.")
+@click.option("-id", "--certid", "cert_id", help="ID of the certificate to be revoked")
+@click.option("-r", "--reason", "reason", default="unspecified", help="CRL Reason as per RFC 5280 section 5.3.1")
+@click.option("-m", "--message", "message", help="Message explaining reason for revocation")
+@click.option(
     "-c",
     "--commit",
-    dest="commit",
-    action="store_true",
+    "commit",
+    type=bool,
     default=False,
     help="Persist changes.",
 )
+def revoke_command(path, cert_id, reason, message, commit):
+    revoke(path, cert_id, reason, message, commit)
+
+
 def revoke(path, cert_id, reason, message, commit):
     """
     Revokes given certificate.
     """
     if not path and not cert_id:
-        print("[!] No input certificates mentioned to revoke")
+        click.echo("[!] No input certificates mentioned to revoke")
         return
     if path and cert_id:
-        print("[!] Please mention single certificate id (-id) or input file (-p)")
+        click.echo("[!] Please mention single certificate id (-id) or input file (-p)")
         return
 
     if commit:
-        print("[!] Running in COMMIT mode.")
+        click.echo("[!] Running in COMMIT mode.")
 
-    print("[+] Starting certificate revocation.")
+    click.echo("[+] Starting certificate revocation.")
 
     if reason not in CRLReason.__members__:
         reason = CRLReason.unspecified.name
     comments = {"comments": message, "crl_reason": reason}
 
     if cert_id:
         worker(cert_id, commit, comments)
     else:
         with open(path, "r") as f:
             for x in f.readlines()[2:]:
                 worker(x, commit, comments)
 
 
-@manager.command
+@cli.command("check_revoked")
+def check_revoked_command():
+    check_revoked()
+
+
 def check_revoked():
     """
     Function attempts to update Lemur's internal cache with revoked
     certificates. This is called periodically by Lemur. It checks both
     CRLs and OCSP to see if a certificate is revoked. If Lemur is unable
     encounters an issue with verification it marks the certificate status
     as `unknown`.
@@ -788,15 +827,19 @@
     metrics.send(
         "certificate_revoked_checked",
         "gauge",
         (page - 1) * count + len(certs),
     )
 
 
-@manager.command
+@cli.command("automatically_enable_autorotate_with_endpoint")
+def automatically_enable_autorotate_with_endpoint_command():
+    automatically_enable_autorotate_with_endpoint()
+
+
 def automatically_enable_autorotate_with_endpoint():
     """
     This function automatically enables auto-rotation for unexpired certificates that are
     attached to an endpoint but do not have autorotate enabled.
 
     WARNING: This will overwrite the Auto-rotate toggle!
     """
@@ -830,15 +873,19 @@
                                   "authority_name": log_data["authority_name"],
                                   "destination_names": log_data["destination_names"]
                                   })
         cert.rotation = True
         database.update(cert)
 
 
-@manager.command
+@cli.command("automatically_enable_autorotate_with_destination")
+def automatically_enable_autorotate_with_destination_command():
+    automatically_enable_autorotate_with_destination()
+
+
 def automatically_enable_autorotate_with_destination():
     """
     This function automatically enables auto-rotation for unexpired certificates that are
     attached to a destination but do not have autorotate enabled.
 
     WARNING: This will overwrite the Auto-rotate toggle!
     """
@@ -873,15 +920,19 @@
                                   "authority_name": log_data["authority_name"],
                                   "destination_names": log_data["destination_names"]
                                   })
         cert.rotation = True
         database.update(cert)
 
 
-@manager.command
+@cli.command("deactivate_entrust_certificates")
+def deactivate_entrust_certificates_command():
+    deactivate_entrust_certificates()
+
+
 def deactivate_entrust_certificates():
     """
     Attempt to deactivate test certificates issued by Entrust
     """
 
     log_data = {
         "function": f"{__name__}.{sys._getframe().f_code.co_name}",
@@ -918,23 +969,28 @@
 
         except Exception as e:
             current_app.logger.info(log_data)
             capture_exception()
             current_app.logger.exception(e)
 
 
-@manager.option("-c", "--commit", dest="commit", action="store_true", default=False, help="Persist changes.")
+@cli.command("disable_rotation_of_duplicate_certificates")
+@click.option("-c", "--commit", "commit", type=bool, default=False, help="Persist changes.")
+def disable_rotation_of_duplicate_certificates_command(commit):
+    disable_rotation_of_duplicate_certificates(commit)
+
+
 def disable_rotation_of_duplicate_certificates(commit):
     log_data = {
         "function": f"{__name__}.{sys._getframe().f_code.co_name}",
         "message": "Disabling auto-rotate for duplicate certificates"
     }
 
     if commit:
-        print("[!] Running in COMMIT mode.")
+        click.echo("[!] Running in COMMIT mode.")
 
     authority_names = current_app.config.get("AUTHORITY_TO_DISABLE_ROTATE_OF_DUPLICATE_CERTIFICATES")
     if not authority_names:
         log_data["message"] = "Skipping task: No authorities configured"
         current_app.logger.debug(log_data)
         return
 
@@ -954,114 +1010,112 @@
     if invalid_authorities:
         log_data["warning"] = f"Non-existing authorities: {invalid_authorities}"
     if not authority_ids:
         log_data["message"] = "Skipping task: No valid authorities configured"
         current_app.logger.error(log_data)
         return
 
-    duplicate_candidate_certs = list_duplicate_certs_by_authority(authority_ids, days_since_issuance)
+    duplicate_candidate_certs = list_recent_valid_certs_issued_by_authority(authority_ids, days_since_issuance)
 
-    log_data["certs_with_serial_number_count"] = len(duplicate_candidate_certs)
+    log_data["duplicate_candidate_certs_count"] = len(duplicate_candidate_certs)
     current_app.logger.info(log_data)
 
     skipped_certs = []
     rotation_disabled_certs = []
-    unique_prefix = []
+    unique_common_names = []
     failed_certs = []
 
     for duplicate_candidate_cert in duplicate_candidate_certs:
         success, duplicates = process_duplicates(duplicate_candidate_cert,
+                                                 days_since_issuance,
                                                  skipped_certs,
                                                  rotation_disabled_certs,
-                                                 unique_prefix,
+                                                 unique_common_names,
                                                  commit
                                                  )
         if not success:
             for cert in duplicates:
                 failed_certs.append(cert.name)
                 metrics.send("disable_rotation_duplicates", "counter", 1,
                              metric_tags={"status": "failed", "certificate": cert.name}
                              )
 
-    # certs_with_serial_number_count + unique_cert_prefix_count should be equal to
+    # certs_with_serial_number_count + unique_common_names_count should be equal to
     # rotation_disabled_cert_count + rotation_disabled_cert_count + failed_to_determine_if_duplicate_count
     log_data["message"] = "Summary of task run"
-    log_data["unique_cert_prefix_count"] = len(unique_prefix)
+    log_data["unique_common_names_count"] = len(unique_common_names)
     log_data["rotation_disabled_cert_count"] = len(rotation_disabled_certs)
     log_data["certificate_with_no_change_count"] = len(skipped_certs)
     log_data["failed_to_determine_if_duplicate_count"] = len(failed_certs)
 
     current_app.logger.info(log_data)
 
 
-def process_duplicates(duplicate_candidate_cert, skipped_certs, rotation_disabled_certs, processed_unique_prefix, commit):
+def process_duplicates(duplicate_candidate_cert, days_since_issuance, skipped_certs, rotation_disabled_certs, processed_unique_cn, commit):
     """
-    Process duplicates with same prefix as duplicate_candidate_cert
+    Process duplicate_candidate_cert to see if there are more certs with exact same details (logic in `is_duplicate()`).
+    If Yes, turn off auto
+
 
     :param duplicate_candidate_cert: Name of the certificate which has duplicates
+    :param days_since_issuance: If not none, include certificates issued in only last days_since_issuance days
     :param skipped_certs: List of certificates which will continue to have rotation on (no change)
     :param rotation_disabled_certs: List of certificates for which rotation got disabled as part of this job
-    :param processed_unique_prefix: List of unique prefixes to avoid rework
+    :param processed_unique_cn: List of unique common names to avoid rework
     :return: Success - True or False; If False, set of duplicates which were not processed
     """
-    name_without_serial_num = duplicate_candidate_cert.name[:duplicate_candidate_cert.name.rindex("-")]
-    if name_without_serial_num in processed_unique_prefix:
+    if duplicate_candidate_cert.cn in processed_unique_cn:
         return True, None
 
-    processed_unique_prefix.append(name_without_serial_num)
+    processed_unique_cn.append(duplicate_candidate_cert.cn)
 
-    prefix_to_match = name_without_serial_num + '%'
-    certs_with_same_prefix = get_certificates_with_same_prefix_with_rotate_on(prefix_to_match)
+    certs_with_same_cn = get_certificates_with_same_cn_with_rotate_on(duplicate_candidate_cert.cn,
+                                                                      duplicate_candidate_cert.date_created)
 
-    if len(certs_with_same_prefix) == 1:
+    if len(certs_with_same_cn) == 1:
         # this is the only cert with rotation ON, no further action needed
-        skipped_certs.append(certs_with_same_prefix[0].name)
+        skipped_certs.append(certs_with_same_cn[0].name)
         metrics.send("disable_rotation_duplicates", "counter", 1,
-                     metric_tags={"status": "skipped", "certificate": certs_with_same_prefix[0].name}
+                     metric_tags={"status": "skipped", "certificate": certs_with_same_cn[0].name}
                      )
         return True, None
 
     skip_cert = False
     certs_to_stay_on_autorotate = []
 
-    for matching_cert in certs_with_same_prefix:
-        if matching_cert.name == name_without_serial_num:
-            # There exists a cert with name same as the prefix (most likely there will always be one)
-            # Keep auto rotate on for this one if no cert has endpoint associated
-            fallback_cert_to_rotate = name_without_serial_num
-
+    for matching_cert in certs_with_same_cn:
         if matching_cert.name == duplicate_candidate_cert.name:
             # Same cert, no need to compare
             continue
 
-        # Even if one of the cert with same prefix has different details, skip this set of certs
-        # it's safe to do so and this logic can be revisited
+        # Even if one of the certs has different details, skip this set of certs
+        # It's safe to do so and this logic can be revisited
         if not is_duplicate(matching_cert, duplicate_candidate_cert):
             skip_cert = True
             break
 
-        # Find certs with endpoint, auto-rotate needs to be on for these
+        # If cert is attached to an endpoint, auto-rotate needs to stay ON
         if matching_cert.endpoints:
             certs_to_stay_on_autorotate.append(matching_cert.name)
 
     if skip_cert:
         # Not reporting failure for skipping cert since they are not duplicates,
         # comparision is working as intended
-        for skipped_cert in certs_with_same_prefix:
+        for skipped_cert in certs_with_same_cn:
             skipped_certs.append(skipped_cert.name)
             metrics.send("disable_rotation_duplicates", "counter", 1,
                          metric_tags={"status": "skipped", "certificate": skipped_cert.name}
                          )
         return True, None
 
-    # If no certificate has endpoint, pick fallback_cert_to_rotate or any one to allow one certificate to auto-rotate.
+    # If no certificate has endpoint, allow autorotaion of only input duplicate_candidate_cert
     if not certs_to_stay_on_autorotate:
-        certs_to_stay_on_autorotate.append(fallback_cert_to_rotate if fallback_cert_to_rotate else certs_with_same_prefix[0])
+        certs_to_stay_on_autorotate.append(duplicate_candidate_cert.name)
 
-    for matching_cert in certs_with_same_prefix:
+    for matching_cert in certs_with_same_cn:
         if matching_cert.name in certs_to_stay_on_autorotate:
             skipped_certs.append(matching_cert.name)
             metrics.send("disable_rotation_duplicates", "counter", 1,
                          metric_tags={"status": "skipped", "certificate": matching_cert.name}
                          )
         else:
             # disable rotation and update DB
@@ -1078,14 +1132,15 @@
 def is_duplicate(matching_cert, compare_to):
     if (
         matching_cert.owner != compare_to.owner
         or matching_cert.san != compare_to.san
         or matching_cert.key_type != compare_to.key_type
         or matching_cert.not_before.date() != compare_to.not_before.date()
         or matching_cert.not_after.date() != compare_to.not_after.date()
+        or matching_cert.authority_id != compare_to.authority_id
     ):
         return False
 
     matching_destinations = [destination.label for destination in matching_cert.destinations]
     compare_to_destinations = [destination.label for destination in compare_to.destinations]
 
     if (len(matching_destinations) == len(compare_to_destinations)
@@ -1094,60 +1149,68 @@
         compare_to_sans = [domain.name for domain in compare_to.domains]
 
         return len(matching_sans) == len(compare_to_sans) and set(matching_sans) == set(compare_to_sans)
 
     return False
 
 
-@manager.option(
+@cli.command("identify_expiring_deployed_certificates")
+@click.option(
     "-e",
     "--exclude",
-    dest="exclude_domains",
-    action="append",
+    "exclude_domains",
+    multiple=True,
     default=[],
     help="Domains that should be excluded from check.",
 )
-@manager.option(
+@click.option(
     "-eo",
     "--exclude-owners",
-    dest="exclude_owners",
-    action="append",
+    "exclude_owners",
+    multiple=True,
     default=[],
     help="Owners that should be excluded from check.",
 )
-@manager.option(
+@click.option(
     "-c",
     "--commit",
-    dest="commit",
-    action="store_true",
+    "commit",
     default=False,
     help="Persist changes.",
 )
+def identify_expiring_deployed_certificates_command(exclude_domains, exclude_owners, commit):
+    identify_expiring_deployed_certificates(exclude_domains, exclude_owners, commit)
+
+
 def identify_expiring_deployed_certificates(exclude_domains, exclude_owners, commit):
     status = FAILURE_METRIC_STATUS
     try:
         identify_and_persist_expiring_deployed_certificates(exclude_domains, exclude_owners, commit)
         status = SUCCESS_METRIC_STATUS
     except Exception:
         capture_exception()
         current_app.logger.exception("Error identifying expiring deployed certificates", exc_info=True)
 
     metrics.send("identify_expiring_deployed_certificates", "counter", 1, metric_tags={"status": status})
 
 
-@manager.command
+@cli.command("expiration_metrics")
+def expiration_metrics_command(expiry_window):
+    expiration_metrics(expiry_window)
+
+
 def expiration_metrics(expiry_window):
     """
     Iterates over all certificates and emits a metric for the days remaining for a certificate to expire.
     This is used for building custom dashboards and alerts for certificate expiry.
     """
     try:
-        print("Starting to publish metrics for time left until cert expirations")
+        click.echo("Starting to publish metrics for time left until cert expirations")
         success, failure = send_certificate_expiration_metrics(expiry_window)
-        print(
+        click.echo(
             f"Finished publishing metrics for time left until cert expirations! Sent: {success}"
         )
         status = SUCCESS_METRIC_STATUS
     except Exception as e:
         status = FAILURE_METRIC_STATUS
         capture_exception()
```

### Comparing `lemur-1.4.0/lemur/certificates/hooks.py` & `lemur-1.5.0/lemur/certificates/hooks.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/certificates/models.py` & `lemur-1.5.0/lemur/certificates/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from sqlalchemy.sql.expression import case, extract
 from sqlalchemy_utils.types.arrow import ArrowType
 from werkzeug.utils import cached_property
 
 
 from lemur.common import defaults, utils, validators
 from lemur.constants import SUCCESS_METRIC_STATUS, FAILURE_METRIC_STATUS
-from lemur.database import db
+from lemur.database import BaseModel
 from lemur.domains.models import Domain
 from lemur.extensions import metrics
 from lemur.models import (
     certificate_source_associations,
     certificate_destination_associations,
     certificate_notification_associations,
     certificate_replacement_associations,
@@ -93,15 +93,15 @@
         root, end = get_sequence(cert.name)
         if end:
             ends.append(end)
 
     return "{0}-{1}".format(root, max(ends) + 1)
 
 
-class Certificate(db.Model):
+class Certificate(BaseModel):
     __tablename__ = "certificates"
     __table_args__ = (
         Index(
             "ix_certificates_cn",
             "cn",
             postgresql_ops={"cn": "gin_trgm_ops"},
             postgresql_using="gin",
@@ -326,32 +326,32 @@
 
     @hybrid_property
     def expired(self):
         # can't compare offset-naive and offset-aware datetimes
         if arrow.Arrow.fromdatetime(self.not_after) <= arrow.utcnow():
             return True
 
-    @expired.expression
+    @expired.expression  # type: ignore
     def expired(cls):
         return case([(cls.not_after <= arrow.utcnow(), True)], else_=False)
 
     @hybrid_property
     def revoked(self):
         if "revoked" == self.status:
             return True
 
-    @revoked.expression
+    @revoked.expression  # type: ignore
     def revoked(cls):
         return case([(cls.status == "revoked", True)], else_=False)
 
     @hybrid_property
     def has_private_key(self):
         return self.private_key is not None
 
-    @has_private_key.expression
+    @has_private_key.expression  # type: ignore
     def has_private_key(cls):
         return case([(cls.private_key.is_(None), True)], else_=False)
 
     @hybrid_property
     def in_rotation_window(self):
         """
         Determines if a certificate is available for rotation based
@@ -360,15 +360,15 @@
         """
         now = arrow.utcnow()
         end = now + timedelta(days=self.rotation_policy.days)
 
         if self.not_after <= end:
             return True
 
-    @in_rotation_window.expression
+    @in_rotation_window.expression  # type: ignore
     def in_rotation_window(cls):
         """
         Determines if a certificate is available for rotation based
         on the rotation policy associated.
         :return:
         """
         return case(
@@ -435,15 +435,15 @@
 
         return return_extensions
 
     def __repr__(self):
         return "Certificate(name={name})".format(name=self.name)
 
 
-class CertificateAssociation(db.Model):
+class CertificateAssociation(BaseModel):
     __tablename__ = 'certificate_associations'
     __table_args__ = (
         Index(
             "certificate_associations_ix",
             "domain_id",
             "certificate_id",
             unique=True
```

### Comparing `lemur-1.4.0/lemur/certificates/schemas.py` & `lemur-1.5.0/lemur/certificates/schemas.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/certificates/service.py` & `lemur-1.5.0/lemur/certificates/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import arrow
 from cryptography import x509
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, serialization
 from flask import current_app
 from sentry_sdk import capture_exception
 from sqlalchemy import and_, func, or_, not_, cast, Integer
-from sqlalchemy.sql import text
 from sqlalchemy.sql.expression import false, true
 
 from lemur import database
 from lemur.authorities.models import Authority
 from lemur.certificates.models import Certificate, CertificateAssociation
 from lemur.certificates.schemas import CertificateOutputSchema, CertificateInputSchema
 from lemur.common.utils import generate_private_key, truthiness, parse_serial, get_certificate_via_tls, windowed_query
@@ -279,56 +278,62 @@
         return Certificate.query.filter_by(
             body=cert["body"].strip(), chain=cert["chain"].strip()
         ).all()
     else:
         return Certificate.query.filter_by(body=cert["body"].strip(), chain=None).all()
 
 
-def list_duplicate_certs_by_authority(authority_ids, days_since_issuance):
+def list_recent_valid_certs_issued_by_authority(authority_ids, days_since_issuance):
     """
-    Find duplicate certificates issued by given authorities that are still valid, not replaced, have auto-rotation ON,
-    with names that are forced to be unique using serial number like 'some.name.prefix-YYYYMMDD-YYYYMMDD-serialnumber',
-    thus the pattern "%-[0-9]{8}-[0-9]{8}-%"
-    :param authority_ids:
+    Find certificates issued by given authorities in last days_since_issuance number of days, that are still valid,
+    not replaced, have auto-rotation ON.
+
+    :param authority_ids: list of authority ids
     :param days_since_issuance: If not none, include certificates issued in only last days_since_issuance days
-    :return: List of certificates matching criteria
+    :return: List of certificates matching the criteria
     """
 
     now = arrow.now().format("YYYY-MM-DD")
     query = database.session_query(Certificate)\
         .filter(Certificate.authority_id.in_(authority_ids))\
         .filter(Certificate.not_after >= now)\
         .filter(Certificate.rotation == true())\
-        .filter(not_(Certificate.replaced.any()))\
-        .filter(text("name ~ '.*-[0-9]{8}-[0-9]{8}-.*'"))
+        .filter(not_(Certificate.replaced.any()))
 
     if days_since_issuance:
         issuance_window = (
             arrow.now().shift(days=-days_since_issuance).format("YYYY-MM-DD")
         )
         query = query.filter(Certificate.date_created >= issuance_window)
 
     return query.all()
 
 
-def get_certificates_with_same_prefix_with_rotate_on(prefix):
+def get_certificates_with_same_cn_with_rotate_on(cn, date_created):
     """
-    Find certificates with given prefix that are still valid, not replaced and marked for auto-rotate
+    Find certificates with given common name created on date_created that are still valid, not replaced and marked for
+    auto-rotate
 
-    :param prefix: prefix to match
-    :return:
+    :param cn: common name to match
+    :param date_created: creation date
+    :return: List of certificates matching the criteria
     """
     now = arrow.now().format("YYYY-MM-DD")
-    return (
-        Certificate.query.filter(Certificate.name.like(prefix))
-        .filter(Certificate.rotation == true())
-        .filter(Certificate.not_after >= now)
+    date_created_min = date_created.floor('day')
+    date_created_max = date_created.ceil('day')
+
+    query = database.session_query(Certificate)\
+        .filter(Certificate.cn.like(cn))\
+        .filter(Certificate.rotation == true())\
+        .filter(Certificate.not_after >= now)\
+        .filter(Certificate.date_created >= date_created_min)\
+        .filter(Certificate.date_created <= date_created_max)\
         .filter(not_(Certificate.replaced.any()))
-        .all()
-    )
+
+    return query.all()
 
 
 def export(cert, export_plugin):
     """
     Exports a certificate to the requested format. This format
     may be a binary format.
 
@@ -478,16 +483,18 @@
     """
     # Validate destinations do not overlap accounts for the same plugin
     if "destinations" in kwargs:
         dest_plugin_accounts = {}
         for dest in kwargs["destinations"]:
             plugin_accounts = dest_plugin_accounts.setdefault(dest.plugin_name, {})
             account = get_plugin_option("accountNumber", dest.options)
-            if account in plugin_accounts:
-                raise Exception(f"Too many destinations for plugin {dest.plugin_name} and account {account}")
+            dest_plugin = plugins.get(dest.plugin_name)
+            if account in plugin_accounts and not dest_plugin.allow_multiple_per_account():
+                raise Exception(f"Duplicate destinations for plugin {dest.plugin_name} and account {account} are not "
+                                f"allowed")
             plugin_accounts[account] = True
 
     try:
         cert_body, private_key, cert_chain, external_id, csr = mint(**kwargs)
     except Exception:
         log_data = {
             "message": "Exception minting certificate",
```

### Comparing `lemur-1.4.0/lemur/certificates/utils.py` & `lemur-1.5.0/lemur/certificates/utils.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/certificates/verify.py` & `lemur-1.5.0/lemur/certificates/verify.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,19 @@
             # Ignore 'no such process' error
             pass
         raise Exception(f"OCSP lookup timed out: {url}, certificate serial number {cert.serial_number:02X}")
 
     p_message = message.decode("utf-8")
 
     if "unauthorized" in p_message:
-        # indicates the OCSP server does not know this certificate
+        # indicates the OCSP server does not know this certificate. this is a retriable error.
         metrics.send("check_revocation_ocsp_verify", "counter", 1, metric_tags={"status": "unauthorized", "url": url})
-        raise Exception(f"OCSP unauthorized error: {url}, certificate serial number {cert.serial_number:02X}. Response:"
-                        f" {p_message}")
+        current_app.logger.warning(f"OCSP unauthorized error: {url}, "
+                                   f"certificate serial number {cert.serial_number:02X}. Response: {p_message}")
+        return None
 
     elif "error" in p_message or "Error" in p_message:
         metrics.send("check_revocation_ocsp_verify", "counter", 1, metric_tags={"status": "error", "url": url})
         raise Exception(f"Got error when parsing response from OCSP url: {url}, certificate serial number "
                         f"{cert.serial_number:02X}. Response: {p_message}")
 
     elif "revoked" in p_message:
@@ -122,15 +123,15 @@
                 response = requests.get(point, timeout=(3.05, 6))
 
                 if response.status_code != 200:
                     raise Exception(f"Unable to retrieve CRL: {point}, serial {cert.serial_number:02X}")
             except InvalidSchema:
                 # Unhandled URI scheme (like ldap://); skip this distribution point.
                 continue
-            except ConnectionError or Timeout:
+            except (ConnectionError, Timeout):
                 raise Exception(f"Unable to retrieve CRL: {point}, serial {cert.serial_number:02X}")
 
             crl_cache[point] = x509.load_der_x509_crl(
                 response.content, backend=default_backend()
             )
         else:
             current_app.logger.debug("CRL point is cached {}".format(point))
@@ -188,15 +189,15 @@
             verify_result = crl_verify(cert, cert_path)
         except Exception as e:
             capture_exception()
             current_app.logger.warning(e)
             crl_err = 1
 
     if verify_result is None:
-        current_app.logger.debug("Failed to verify {}".format(cert.serial_number))
+        current_app.logger.warning("Failed to verify {}".format(cert.serial_number))
 
     return verify_result, ocsp_err, crl_err
 
 
 def verify_string(cert_string, issuer_string):
     """
     Verify a certificate given only it's string value
```

### Comparing `lemur-1.4.0/lemur/certificates/views.py` & `lemur-1.5.0/lemur/certificates/views.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/common/celery.py` & `lemur-1.5.0/lemur/common/celery.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
     Report a generic failure metric as tasks to our metrics broker every time a task fails.
     This metric can be used for alerting.
     https://docs.celeryproject.org/en/latest/userguide/signals.html#task-failure
     """
     with flask_app.app_context():
         log_data = {
             "function": f"{__name__}.{sys._getframe().f_code.co_name}",
-            "Message": "Celery Task Failure",
+            "message": "Celery Task Failure",
         }
 
         # Add traceback if exception info is in the kwargs
         einfo = kwargs.get("einfo")
         if einfo:
             log_data["traceback"] = einfo.traceback
 
@@ -215,15 +215,15 @@
     Report a generic failure metric as tasks to our metrics broker every time a task is revoked.
     This metric can be used for alerting.
     https://docs.celeryproject.org/en/latest/userguide/signals.html#task-revoked
     """
     with flask_app.app_context():
         log_data = {
             "function": f"{__name__}.{sys._getframe().f_code.co_name}",
-            "Message": "Celery Task Revoked",
+            "message": "Celery Task Revoked",
         }
 
         error_tags = get_celery_request_tags(**kwargs)
 
         log_data.update(error_tags)
         current_app.logger.error(log_data)
         metrics.send("celery.revoked_task", "TIMER", 1, metric_tags=error_tags)
```

### Comparing `lemur-1.4.0/lemur/common/defaults.py` & `lemur-1.5.0/lemur/common/defaults.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/common/fields.py` & `lemur-1.5.0/lemur/common/fields.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/common/health.py` & `lemur-1.5.0/lemur/common/health.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/common/managers.py` & `lemur-1.5.0/lemur/common/managers.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/common/missing.py` & `lemur-1.5.0/lemur/common/missing.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/common/redis.py` & `lemur-1.5.0/lemur/common/redis.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/common/schema.py` & `lemur-1.5.0/lemur/common/schema.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/common/utils.py` & `lemur-1.5.0/lemur/common/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,27 +54,23 @@
     return base64.b64decode(base64_input.encode()).decode()
 
 
 def get_psuedo_random_string():
     """
     Create a random and strongish challenge.
     """
-    challenge = "".join(secrets.choice(string.ascii_uppercase) for x in range(6))  # noqa
-    challenge += "".join(secrets.choice("~!@#$%^&*()_+") for x in range(6))  # noqa
-    challenge += "".join(secrets.choice(string.ascii_lowercase) for x in range(6))
-    challenge += "".join(secrets.choice(string.digits) for x in range(6))  # noqa
+    chars = string.ascii_uppercase + string.ascii_lowercase + string.digits + "~!@#$%^&*()_+"
+    challenge = ''.join(secrets.choice(chars) for x in range(24))
     return challenge
 
 
 def get_random_secret(length):
     """ Similar to get_pseudo_random_string, but accepts a length parameter. """
-    secret_key = ''.join(secrets.choice(string.ascii_uppercase) for x in range(round(length / 4)))
-    secret_key = secret_key + ''.join(secrets.choice("~!@#$%^&*()_+") for x in range(round(length / 4)))
-    secret_key = secret_key + ''.join(secrets.choice(string.ascii_lowercase) for x in range(round(length / 4)))
-    return secret_key + ''.join(secrets.choice(string.digits) for x in range(round(length / 4)))
+    chars = string.ascii_uppercase + string.ascii_lowercase + string.digits + "~!@#$%^&*()_+"
+    return ''.join(secrets.choice(chars) for x in range(length))
 
 
 def get_state_token_secret():
     return base64.b64encode(get_random_secret(32).encode('utf8'))
 
 
 def parse_certificate(body):
@@ -504,11 +500,11 @@
     """
     if full_chain == '' or full_chain.count("BEGIN CERTIFICATE") <= 1:
         return full_chain
     full_chain_certs = CERT_PEM_REGEX.findall(full_chain.encode())
     pem_certificate = OpenSSL.crypto.dump_certificate(
         OpenSSL.crypto.FILETYPE_PEM,
         OpenSSL.crypto.load_certificate(
-            OpenSSL.crypto.FILETYPE_PEM, ''.join(cert.decode() for cert in full_chain_certs[:-1])
+            OpenSSL.crypto.FILETYPE_PEM, ''.join(cert.decode() for cert in full_chain_certs[:-1]).encode()
         ),
     ).decode()
     return pem_certificate
```

### Comparing `lemur-1.4.0/lemur/common/validators.py` & `lemur-1.5.0/lemur/common/validators.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/constants.py` & `lemur-1.5.0/lemur/constants.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/database.py` & `lemur-1.5.0/lemur/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,26 @@
 
     :copyright: (c) 2018 by Netflix Inc., see AUTHORS for more
     :license: Apache, see LICENSE for more details.
 
 .. moduleauthor:: Kevin Glisson <kglisson@netflix.com>
 """
 from inflection import underscore
+from flask_sqlalchemy.model import DefaultMeta
 from sqlalchemy import exc, func, distinct
 from sqlalchemy.orm import make_transient, lazyload
 from sqlalchemy.sql import and_, or_
 
 from lemur.exceptions import AttrNotFound, DuplicateError
 from lemur.extensions import db
 
 
+BaseModel: DefaultMeta = db.Model
+
+
 def filter_none(kwargs):
     """
     Remove all `None` values from a  given dict. SQLAlchemy does not
     like to have values that are None passed to it.
 
     :param kwargs: Dict to filter
     :return: Dict without any 'None' values
@@ -82,15 +86,15 @@
     """
     db.session.add(model)
 
 
 def get_model_column(model, field):
     if field in getattr(model, "sensitive_fields", ()):
         raise AttrNotFound(field)
-    column = model.__table__.columns._data.get(field, None)
+    column = model.__table__.columns.get(field, None)
     if column is None:
         raise AttrNotFound(field)
 
     return column
 
 
 def find_all(query, model, kwargs):
```

### Comparing `lemur-1.4.0/lemur/defaults/schemas.py` & `lemur-1.5.0/lemur/defaults/schemas.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/defaults/views.py` & `lemur-1.5.0/lemur/defaults/views.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/destinations/models.py` & `lemur-1.5.0/lemur/destinations/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,20 +4,20 @@
     :copyright: (c) 2018 by Netflix Inc., see AUTHORS for more
     :license: Apache, see LICENSE for more details.
 .. moduleauthor:: Kevin Glisson <kglisson@netflix.com>
 """
 from sqlalchemy import Column, Integer, String, Text
 from sqlalchemy.orm import validates
 from sqlalchemy_utils import JSONType
-from lemur.database import db
+from lemur.database import BaseModel
 
 from lemur.plugins.base import plugins
 
 
-class Destination(db.Model):
+class Destination(BaseModel):
     __tablename__ = "destinations"
     id = Column(Integer, primary_key=True)
     label = Column(String(32))
     options = Column(JSONType)
     description = Column(Text())
     plugin_name = Column(String(32))
```

### Comparing `lemur-1.4.0/lemur/destinations/schemas.py` & `lemur-1.5.0/lemur/destinations/schemas.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/destinations/service.py` & `lemur-1.5.0/lemur/destinations/service.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/destinations/views.py` & `lemur-1.5.0/lemur/destinations/views.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/dns_providers/cli.py` & `lemur-1.5.0/lemur/dns_providers/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,48 @@
-from flask_script import Manager
-
 import sys
+import click
+
 from sentry_sdk import capture_exception
 
 from lemur.constants import SUCCESS_METRIC_STATUS
 from lemur.plugins.lemur_acme.acme_handlers import AcmeDnsHandler
 from lemur.dns_providers.service import get_all_dns_providers, set_domains
 from lemur.extensions import metrics
 
-manager = Manager(
-    usage="Iterates through all DNS providers and sets DNS zones in the database."
-)
+
+@click.group(name="dns_providers", help="Iterates through all DNS providers and sets DNS zones in the database.")
+def cli():
+    pass
+
+
+@cli.command("get_all_zones")
+def get_all_zones_command():
+    get_all_zones()
 
 
-@manager.command
 def get_all_zones():
     """
     Retrieves all DNS providers from the database. Refreshes the zones associated with each DNS provider
     """
-    print("[+] Starting dns provider zone lookup and configuration.")
+    click.echo("[+] Starting dns provider zone lookup and configuration.")
     dns_providers = get_all_dns_providers()
     acme_dns_handler = AcmeDnsHandler()
 
     function = f"{__name__}.{sys._getframe().f_code.co_name}"
     log_data = {
         "function": function,
         "message": "",
     }
 
     for dns_provider in dns_providers:
         try:
             zones = acme_dns_handler.get_all_zones(dns_provider)
             set_domains(dns_provider, zones)
         except Exception as e:
-            print("[+] Error with DNS Provider {}: {}".format(dns_provider.name, e))
+            click.echo("[+] Error with DNS Provider {}: {}".format(dns_provider.name, e))
             log_data["message"] = f"get all zones failed for {dns_provider} {e}."
             capture_exception(extra=log_data)
 
     status = SUCCESS_METRIC_STATUS
 
     metrics.send("get_all_zones", "counter", 1, metric_tags={"status": status})
-    print("[+] Done with dns provider zone lookup and configuration.")
+    click.echo("[+] Done with dns provider zone lookup and configuration.")
```

### Comparing `lemur-1.4.0/lemur/dns_providers/models.py` & `lemur-1.5.0/lemur/dns_providers/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from sqlalchemy import Column, Integer, String, text
 from sqlalchemy.dialects.postgresql import JSON
 from sqlalchemy.orm import relationship
 from sqlalchemy_utils import ArrowType
 
-from lemur.database import db
+from lemur.database import BaseModel
 from lemur.plugins.base import plugins
 from lemur.utils import Vault
 
 
-class DnsProvider(db.Model):
+class DnsProvider(BaseModel):
     __tablename__ = "dns_providers"
     id = Column(Integer(), primary_key=True)
     name = Column(String(length=256), unique=True, nullable=True)
     description = Column(String(length=1024), nullable=True)
     provider_type = Column(String(length=256), nullable=True)
     credentials = Column(Vault, nullable=True)
     api_endpoint = Column(String(length=256), nullable=True)
```

### Comparing `lemur-1.4.0/lemur/dns_providers/schemas.py` & `lemur-1.5.0/lemur/dns_providers/schemas.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/dns_providers/service.py` & `lemur-1.5.0/lemur/dns_providers/service.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/dns_providers/util.py` & `lemur-1.5.0/lemur/dns_providers/util.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/dns_providers/views.py` & `lemur-1.5.0/lemur/dns_providers/views.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/domains/schemas.py` & `lemur-1.5.0/lemur/domains/schemas.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/domains/service.py` & `lemur-1.5.0/lemur/domains/service.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/domains/views.py` & `lemur-1.5.0/lemur/domains/views.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/endpoints/models.py` & `lemur-1.5.0/lemur/endpoints/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,50 +11,50 @@
 from sqlalchemy.ext.associationproxy import association_proxy
 from sqlalchemy import Column, Integer, String, Boolean, ForeignKey
 from sqlalchemy.ext.hybrid import hybrid_property
 from sqlalchemy.sql.expression import case
 
 from sqlalchemy_utils import ArrowType
 
-from lemur.database import db
+from lemur.database import BaseModel
 
 from lemur.models import policies_ciphers
 
 BAD_CIPHERS = ["Protocol-SSLv3", "Protocol-SSLv2", "Protocol-TLSv1"]
 
 
-class Cipher(db.Model):
+class Cipher(BaseModel):
     __tablename__ = "ciphers"
     id = Column(Integer, primary_key=True)
     name = Column(String(128), nullable=False)
 
     @hybrid_property
     def deprecated(self):
         return self.name in BAD_CIPHERS
 
-    @deprecated.expression
+    @deprecated.expression  # type: ignore
     def deprecated(cls):
         return case([(cls.name in BAD_CIPHERS, True)], else_=False)
 
 
-class Policy(db.Model):
+class Policy(BaseModel):
     ___tablename__ = "policies"
     id = Column(Integer, primary_key=True)
     name = Column(String(128), nullable=True)
     ciphers = relationship("Cipher", secondary=policies_ciphers, backref="policy")
 
 
-class EndpointDnsAlias(db.Model):
+class EndpointDnsAlias(BaseModel):
     __tablename__ = "endpoint_dnsalias"
     id = Column(Integer, primary_key=True)
     endpoint_id = Column(Integer, ForeignKey('endpoints.id'))
     alias = Column(String(256))
 
 
-class Endpoint(db.Model):
+class Endpoint(BaseModel):
     __tablename__ = "endpoints"
     id = Column(Integer, primary_key=True)
     owner = Column(String(128))
     name = Column(String(128))
     dnsname = Column(String(256))
     aliases = relationship("EndpointDnsAlias", backref="endpoint")
     type = Column(String(128))
```

### Comparing `lemur-1.4.0/lemur/endpoints/schemas.py` & `lemur-1.5.0/lemur/endpoints/schemas.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/endpoints/service.py` & `lemur-1.5.0/lemur/endpoints/service.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/endpoints/views.py` & `lemur-1.5.0/lemur/endpoints/views.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/exceptions.py` & `lemur-1.5.0/lemur/exceptions.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/extensions.py` & `lemur-1.5.0/lemur/extensions.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/factory.py` & `lemur-1.5.0/lemur/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import stat
 
 from logging import Formatter, StreamHandler
 from logging.handlers import RotatingFileHandler
 
 from flask import Flask, current_app
 from flask_replicated import FlaskReplicated
+from click import get_current_context
 
 import sentry_sdk
 from sentry_sdk.integrations.celery import CeleryIntegration
 from sentry_sdk.integrations.redis import RedisIntegration
 from sentry_sdk.integrations.sqlalchemy import SqlalchemyIntegration
 from sentry_sdk.integrations.flask import FlaskIntegration
 
@@ -53,39 +54,57 @@
     else:
         blueprints = blueprints + DEFAULT_BLUEPRINTS
 
     if not app_name:
         app_name = __name__
 
     app = Flask(app_name)
+    ctx = get_current_context(silent=True)
+
+    # get config option value from command line
+    if ctx and config is None:
+        script_info = ctx.obj
+        if script_info:
+            config = script_info.config
+
     configure_app(app, config)
     configure_blueprints(app, blueprints)
     configure_extensions(app)
     configure_logging(app)
     configure_database(app)
     install_plugins(app)
 
     @app.teardown_appcontext
     def teardown(exception=None):
         if db.session:
             db.session.remove()
 
+    @app.shell_context_processor
+    def shell_context():
+        return {'app': app, 'db': db}
+
     return app
 
 
 def from_file(file_path, silent=False):
     """
     Updates the values in the config from a Python file.  This function
     behaves as if the file was imported as module with the
 
     :param file_path:
     :param silent:
     """
-    module_spec = importlib.util.spec_from_file_location("config", file_path)
-    d = importlib.util.module_from_spec(module_spec)
+
+    if os.path.isfile(file_path):
+        module_spec = importlib.util.spec_from_file_location("config", file_path)
+        d = importlib.util.module_from_spec(module_spec)
+    else:
+        raise FileNotFoundError(
+            f"Unable to load config file: `{file_path}`"
+        )
 
     try:
         with open(file_path) as config_file:
             exec(  # nosec: config file safe
                 compile(config_file.read(), file_path, "exec"), d.__dict__
             )
     except IOError as e:
@@ -157,20 +176,24 @@
             # associating users to errors
             send_default_pii=True,
             shutdown_timeout=60,
             environment=app.config.get("LEMUR_ENV", ''),
         )
 
     if app.config["CORS"]:
-        app.config["CORS_HEADERS"] = "Content-Type"
+        # set cors defaults, if not in config
+        if "CORS_ORIGINS" not in app.config:
+            app.config["CORS_ORIGINS"] = "*"
+        if "CORS_ALLOW_HEADERS" not in app.config:
+            app.config["CORS_ALLOW_HEADERS"] = ["Authorization", "Content-Type"]
+
+        # cors init app
         cors.init_app(
             app,
             resources=r"/api/*",
-            headers="Content-Type",
-            origin="*",
             supports_credentials=True,
         )
 
 
 def configure_blueprints(app, blueprints):
     """
     We prefix our APIs with their given version so that we can support
```

### Comparing `lemur-1.4.0/lemur/logs/models.py` & `lemur-1.5.0/lemur/logs/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 .. moduleauthor:: Kevin Glisson <kglisson@netflix.com>
 """
 from sqlalchemy import Column, Integer, ForeignKey, DefaultClause, func, Enum
 
 from sqlalchemy_utils.types.arrow import ArrowType
 
-from lemur.database import db
+from lemur.database import BaseModel
 
 
-class Log(db.Model):
+class Log(BaseModel):
     __tablename__ = "logs"
     id = Column(Integer, primary_key=True)
     certificate_id = Column(Integer, ForeignKey("certificates.id"))
     log_type = Column(
         Enum(
             "key_view",
             "create_cert",
```

### Comparing `lemur-1.4.0/lemur/logs/schemas.py` & `lemur-1.5.0/lemur/logs/schemas.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/logs/service.py` & `lemur-1.5.0/lemur/logs/service.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     :param certificate:
     :return:
     """
     log_data = {
         "function": "lemur-audit",
         "action": type,
         "user": user.email,
-        "certificate": certificate.name
+        "certificate": certificate.name,
+        "message": f"[lemur-audit] action: {type}, user: {user.email}, certificate: {certificate.name}."
     }
     # format before August 2021: f"[lemur-audit] action: {type}, user: {user.email}, certificate: {certificate.name}."
     current_app.logger.info(log_data)
 
     view = Log(user_id=user.id, log_type=type, certificate_id=certificate.id)
     database.add(view)
     database.commit()
@@ -49,15 +50,16 @@
 
     user = g.current_user.email if hasattr(g, 'current_user') else "LEMUR"
     log_data = {
         "function": "lemur-audit",
         "action": action,
         "user": user,
         "entity": entity,
-        "details": message
+        "details": message,
+        "message": f"[lemur-audit] action: {action}, user: {user}, entity: {entity}, details: {message}."
     }
     # format before August 2021: f"[lemur-audit] action: {action}, user: {user}, entity: {entity}, details: {message}"
     current_app.logger.info(log_data)
 
 
 def get_all():
     """
```

### Comparing `lemur-1.4.0/lemur/logs/views.py` & `lemur-1.5.0/lemur/logs/views.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/manage.py` & `lemur-1.5.0/lemur/manage.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 #!/usr/bin/env python
 from __future__ import unicode_literals  # at top of module
 
+import click
 import os
 import sys
 import base64
 import requests
 import json
 
-from gunicorn.config import make_settings
-
 from cryptography.fernet import Fernet
 
 from flask import current_app
-from flask_script import Manager, Command, Option, prompt_pass
-from flask_migrate import Migrate, MigrateCommand, stamp
-from flask_script.commands import ShowUrls, Clean, Server
-
-from lemur.dns_providers.cli import manager as dns_provider_manager
-from lemur.acme_providers.cli import manager as acme_manager
-from lemur.sources.cli import manager as source_manager
-from lemur.policies.cli import manager as policy_manager
-from lemur.reporting.cli import manager as report_manager
-from lemur.certificates.cli import manager as certificate_manager
-from lemur.notifications.cli import manager as notification_manager
-from lemur.pending_certificates.cli import manager as pending_certificate_manager
+from flask.cli import FlaskGroup, pass_script_info
+from flask_migrate.cli import db
+from flask_migrate import stamp
+
+from lemur.dns_providers.cli import cli as dns_provider_cli
+from lemur.acme_providers.cli import cli as acme_cli
+from lemur.sources.cli import cli as source_cli
+from lemur.policies.cli import cli as policy_cli
+from lemur.reporting.cli import cli as report_cli
+from lemur.certificates.cli import cli as certificate_cli
+from lemur.notifications.cli import cli as notification_cli
+from lemur.pending_certificates.cli import cli as pending_certificate_cli
+
 
 from lemur import database
 from lemur.users import service as user_service
 from lemur.roles import service as role_service
 from lemur.policies import service as policy_service
 from lemur.notifications import service as notification_service
 
@@ -48,18 +48,21 @@
 from lemur.endpoints.models import Endpoint  # noqa
 from lemur.policies.models import RotationPolicy  # noqa
 from lemur.pending_certificates.models import PendingCertificate  # noqa
 from lemur.dns_providers.models import DnsProvider  # noqa
 
 from sqlalchemy.sql import text
 
-manager = Manager(create_app)
-manager.add_option("-c", "--config", dest="config_path", required=False)
 
-migrate = Migrate(create_app)
+@click.group(cls=FlaskGroup, create_app=create_app)
+@click.option('-c', '--config', help="Path to default configuration file for Lemur.")
+@pass_script_info
+def cli(script_info, config):
+    script_info.config = config
+
 
 REQUIRED_VARIABLES = [
     "LEMUR_SECURITY_TEAM_EMAIL",
     "LEMUR_DEFAULT_ORGANIZATIONAL_UNIT",
     "LEMUR_DEFAULT_ORGANIZATION",
     "LEMUR_DEFAULT_LOCATION",
     "LEMUR_DEFAULT_COUNTRY",
@@ -83,38 +86,38 @@
 # General
 
 # These will need to be set to `True` if you are developing locally
 CORS = False
 debug = False
 
 # this is the secret key used by flask session management
-SECRET_KEY = '{flask_secret_key}'
+SECRET_KEY = "{flask_secret_key}"
 
 # You should consider storing these separately from your config
-LEMUR_TOKEN_SECRET = '{secret_token}'
-LEMUR_ENCRYPTION_KEYS = '{encryption_key}'
+LEMUR_TOKEN_SECRET = "{secret_token}"
+LEMUR_ENCRYPTION_KEYS = "{encryption_key}"
 
 # this is the secret used to generate oauth state tokens
 OAUTH_STATE_TOKEN_SECRET = {oauth_state_token_secret}
 
 # List of domain regular expressions that non-admin users can issue
 LEMUR_ALLOWED_DOMAINS = []
 
 # Mail Server
 
-LEMUR_EMAIL = ''
+LEMUR_EMAIL = ""
 LEMUR_SECURITY_TEAM_EMAIL = []
 
 # Certificate Defaults
 
-LEMUR_DEFAULT_COUNTRY = ''
-LEMUR_DEFAULT_STATE = ''
-LEMUR_DEFAULT_LOCATION = ''
-LEMUR_DEFAULT_ORGANIZATION = ''
-LEMUR_DEFAULT_ORGANIZATIONAL_UNIT = ''
+LEMUR_DEFAULT_COUNTRY = ""
+LEMUR_DEFAULT_STATE = ""
+LEMUR_DEFAULT_LOCATION = ""
+LEMUR_DEFAULT_ORGANIZATION = ""
+LEMUR_DEFAULT_ORGANIZATIONAL_UNIT = ""
 
 # Authentication Providers
 ACTIVE_PROVIDERS = []
 
 # Metrics Providers
 METRIC_PROVIDERS = []
 
@@ -124,54 +127,47 @@
 LOG_FILE = "lemur.log"
 LOG_UPGRADE_FILE = "db_upgrade.log"
 
 
 # Database
 
 # modify this if you are not using a local database
-SQLALCHEMY_DATABASE_URI = 'postgresql://lemur:lemur@localhost:5432/lemur'
+SQLALCHEMY_DATABASE_URI = "postgresql://lemur:lemur@localhost:5432/lemur"
 
 # AWS
 
-#LEMUR_INSTANCE_PROFILE = 'Lemur'
+#LEMUR_INSTANCE_PROFILE = "Lemur"
 
 # Issuers
 
 # These will be dependent on which 3rd party that Lemur is
 # configured to use.
 
-# VERISIGN_URL = ''
-# VERISIGN_PEM_PATH = ''
-# VERISIGN_FIRST_NAME = ''
-# VERISIGN_LAST_NAME = ''
-# VERSIGN_EMAIL = ''
+# VERISIGN_URL = ""
+# VERISIGN_PEM_PATH = ""
+# VERISIGN_FIRST_NAME = ""
+# VERISIGN_LAST_NAME = ""
+# VERSIGN_EMAIL = ""
 """
 
 
-@MigrateCommand.command
-def create():
+def create_all():
     database.db.engine.execute(text("CREATE EXTENSION IF NOT EXISTS pg_trgm"))
     database.db.create_all()
     stamp(revision="head")
 
 
-@MigrateCommand.command
-def drop_all():
-    database.db.drop_all()
-
+@db.command("create", help="Create all lemur database tables")
+def create():
+    create_all()
 
-@manager.shell
-def make_shell_context():
-    """
-    Creates a python REPL with several default imports
-    in the context of the current_app
 
-    :return:
-    """
-    return dict(current_app=current_app)
+@db.command("drop_all", help="Drop all lemur database tables")
+def drop_all():
+    database.db.drop_all()
 
 
 def generate_settings():
     """
     This command is run when ``default_path`` doesn't exist, or ``init`` is
     run and returns a string representing the default data to put into their
     settings file.
@@ -184,275 +180,241 @@
         flask_secret_key=base64.b64encode(os.urandom(KEY_LENGTH)).decode("utf-8"),
         oauth_state_token_secret=base64.b64encode(os.urandom(KEY_LENGTH)),
     )
 
     return output
 
 
-class InitializeApp(Command):
+@cli.command("init")
+@click.option("-p", "--password", "password")
+def initialize_app(password):
     """
     This command will bootstrap our database with any destinations as
     specified by our config.
 
     Additionally a Lemur user will be created as a default user
     and be used when certificates are discovered by Lemur.
     """
+    create_all()
+    user = user_service.get_by_username("lemur")
 
-    option_list = (Option("-p", "--password", dest="password"),)
-
-    def run(self, password):
-        create()
-        user = user_service.get_by_username("lemur")
-
-        admin_role = role_service.get_by_name("admin")
-
-        if admin_role:
-            sys.stdout.write("[-] Admin role already created, skipping...!\n")
-        else:
-            # we create an admin role
-            admin_role = role_service.create(
-                "admin", description="This is the Lemur administrator role."
-            )
-            sys.stdout.write("[+] Created 'admin' role\n")
+    admin_role = role_service.get_by_name("admin")
 
-        operator_role = role_service.get_by_name("operator")
+    if admin_role:
+        click.echo("[-] Admin role already created, skipping...!")
+    else:
+        # we create an admin role
+        admin_role = role_service.create(
+            "admin", description="This is the Lemur administrator role."
+        )
+        click.echo("[+] Created 'admin' role")
 
-        if operator_role:
-            sys.stdout.write("[-] Operator role already created, skipping...!\n")
-        else:
-            # we create an operator role
-            operator_role = role_service.create(
-                "operator", description="This is the Lemur operator role."
-            )
-            sys.stdout.write("[+] Created 'operator' role\n")
+    operator_role = role_service.get_by_name("operator")
 
-        global_cert_issuer_role = role_service.get_by_name("global_cert_issuer")
+    if operator_role:
+        click.echo("[-] Operator role already created, skipping...!")
+    else:
+        # we create an operator role
+        operator_role = role_service.create(
+            "operator", description="This is the Lemur operator role."
+        )
+        click.echo("[+] Created 'operator' role")
 
-        if global_cert_issuer_role:
-            sys.stdout.write("[-] global_cert_issuer role already created, skipping...!\n")
-        else:
-            # we create a global_cert_issuer role
-            global_cert_issuer_role = role_service.create(
-                "global_cert_issuer", description="This is the Lemur global_cert_issuer role."
-            )
-            sys.stdout.write("[+] Created 'global_cert_issuer' role\n")
+    global_cert_issuer_role = role_service.get_by_name("global_cert_issuer")
 
-        read_only_role = role_service.get_by_name("read-only")
+    if global_cert_issuer_role:
+        click.echo("[-] global_cert_issuer role already created, skipping...!")
+    else:
+        # we create a global_cert_issuer role
+        global_cert_issuer_role = role_service.create(
+            "global_cert_issuer", description="This is the Lemur global_cert_issuer role."
+        )
+        click.echo("[+] Created 'global_cert_issuer' role")
 
-        if read_only_role:
-            sys.stdout.write("[-] Read only role already created, skipping...!\n")
-        else:
-            # we create an read only role
-            read_only_role = role_service.create(
-                "read-only", description="This is the Lemur read only role."
-            )
-            sys.stdout.write("[+] Created 'read-only' role\n")
+    read_only_role = role_service.get_by_name("read-only")
 
-        if not user:
-            if not password:
-                sys.stdout.write("We need to set Lemur's password to continue!\n")
-                password = prompt_pass("Password")
-                password1 = prompt_pass("Confirm Password")
-
-                if password != password1:
-                    sys.stderr.write("[!] Passwords do not match!\n")
-                    sys.exit(1)
+    if read_only_role:
+        click.echo("[-] Read only role already created, skipping...!")
+    else:
+        # we create an read only role
+        read_only_role = role_service.create(
+            "read-only", description="This is the Lemur read only role."
+        )
+        click.echo("[+] Created 'read-only' role")
 
-            user_service.create(
-                "lemur", password, "lemur@nobody.com", True, None, [admin_role]
-            )
-            sys.stdout.write(
-                "[+] Created the user 'lemur' and granted it the 'admin' role!\n"
-            )
+    if not user:
+        if not password:
+            click.echo("We need to set Lemur's password to continue!")
+            password = click.prompt("Password", hide_input=True)
+            password1 = click.prompt("Confirm Password", hide_input=True)
 
-        else:
-            sys.stdout.write(
-                "[-] Default user has already been created, skipping...!\n"
-            )
+            if password != password1:
+                click.echo("[!] Passwords do not match!")
+                sys.exit(1)
 
-        intervals = current_app.config.get(
-            "LEMUR_DEFAULT_EXPIRATION_NOTIFICATION_INTERVALS", []
+        user_service.create(
+            "lemur", password, "lemur@nobody.com", True, None, [admin_role]
         )
-        sys.stdout.write(
-            "[!] Creating {num} notifications for {intervals} days as specified by LEMUR_DEFAULT_EXPIRATION_NOTIFICATION_INTERVALS\n".format(
-                num=len(intervals), intervals=",".join([str(x) for x in intervals])
-            )
+        click.echo(
+            "[+] Created the user 'lemur' and granted it the 'admin' role!\n"
         )
 
-        recipients = current_app.config.get("LEMUR_SECURITY_TEAM_EMAIL")
-        sys.stdout.write("[+] Creating expiration email notifications!\n")
-        sys.stdout.write(
-            "[!] Using {0} as specified by LEMUR_SECURITY_TEAM_EMAIL for notifications\n".format(
-                recipients
-            )
+    else:
+        click.echo(
+            "[-] Default user has already been created, skipping...!\n"
         )
-        notification_service.create_default_expiration_notifications(
-            "DEFAULT_SECURITY", recipients=recipients
+
+    intervals = current_app.config.get(
+        "LEMUR_DEFAULT_EXPIRATION_NOTIFICATION_INTERVALS", []
+    )
+    click.echo(
+        "[!] Creating {num} notifications for {intervals} days as specified by LEMUR_DEFAULT_EXPIRATION_NOTIFICATION_INTERVALS".format(
+            num=len(intervals), intervals=",".join([str(x) for x in intervals])
         )
+    )
 
-        _DEFAULT_ROTATION_INTERVAL = "default"
-        default_rotation_interval = policy_service.get_by_name(
-            _DEFAULT_ROTATION_INTERVAL
+    recipients = current_app.config.get("LEMUR_SECURITY_TEAM_EMAIL")
+    click.echo("[+] Creating expiration email notifications!")
+    click.echo(
+        "[!] Using {0} as specified by LEMUR_SECURITY_TEAM_EMAIL for notifications".format(
+            recipients
         )
+    )
+    notification_service.create_default_expiration_notifications(
+        "DEFAULT_SECURITY", recipients=recipients
+    )
 
-        if default_rotation_interval:
-            sys.stdout.write(
-                "[-] Default rotation interval policy already created, skipping...!\n"
-            )
-        else:
-            days = current_app.config.get("LEMUR_DEFAULT_ROTATION_INTERVAL", 30)
-            sys.stdout.write(
-                "[+] Creating default certificate rotation policy of {days} days before issuance.\n".format(
-                    days=days
-                )
+    _DEFAULT_ROTATION_INTERVAL = "default"
+    default_rotation_interval = policy_service.get_by_name(
+        _DEFAULT_ROTATION_INTERVAL
+    )
+
+    if default_rotation_interval:
+        click.echo(
+            "[-] Default rotation interval policy already created, skipping...!\n"
+        )
+    else:
+        days = current_app.config.get("LEMUR_DEFAULT_ROTATION_INTERVAL", 30)
+        click.echo(
+            "[+] Creating default certificate rotation policy of {days} days before issuance.".format(
+                days=days
             )
-            policy_service.create(days=days, name=_DEFAULT_ROTATION_INTERVAL)
+        )
+        policy_service.create(days=days, name=_DEFAULT_ROTATION_INTERVAL)
 
-        sys.stdout.write("[/] Done!\n")
+    click.echo("[/] Done!")
 
 
-class CreateUser(Command):
+@cli.command("create_user")
+@click.option("-u", "--username", "username", required=True)
+@click.option("-e", "--email", "email", required=True)
+@click.option("-a", "--active", "active", type=bool, default=True, show_default=True)
+@click.option("-r", "--roles", "roles", multiple=True, required=True)
+@click.option("-p", "--password", "password")
+def create_user(username, email, active, roles, password):
     """
     This command allows for the creation of a new user within Lemur.
     """
+    role_objs = []
+    for r in roles:
+        role_obj = role_service.get_by_name(r)
+        if role_obj:
+            role_objs.append(role_obj)
+        else:
+            click.echo("[!] Cannot find role {0}".format(r))
+            sys.exit(1)
 
-    option_list = (
-        Option("-u", "--username", dest="username", required=True),
-        Option("-e", "--email", dest="email", required=True),
-        Option("-a", "--active", dest="active", default=True),
-        Option("-r", "--roles", dest="roles", action="append", default=[]),
-        Option("-p", "--password", dest="password", default=None),
-    )
-
-    def run(self, username, email, active, roles, password):
-        role_objs = []
-        for r in roles:
-            role_obj = role_service.get_by_name(r)
-            if role_obj:
-                role_objs.append(role_obj)
-            else:
-                sys.stderr.write("[!] Cannot find role {0}\n".format(r))
-                sys.exit(1)
-
-        if not password:
-            password1 = prompt_pass("Password")
-            password2 = prompt_pass("Confirm Password")
-            password = password1
+    if not password:
+        password1 = click.prompt("Password", hide_input=True)
+        password2 = click.prompt("Confirm Password", hide_input=True)
+        password = password1
 
-            if password1 != password2:
-                sys.stderr.write("[!] Passwords do not match!\n")
-                sys.exit(1)
+        if password1 != password2:
+            click.echo("[!] Passwords do not match!")
+            sys.exit(1)
 
-        user_service.create(username, password, email, active, None, role_objs)
-        sys.stdout.write("[+] Created new user: {0}\n".format(username))
+    user_service.create(username, password, email, active, None, role_objs)
+    click.echo("[+] Created new user: {0}".format(username))
 
 
-class ResetPassword(Command):
+@cli.command("reset_password")
+@click.option("-u", "--username", "username", required=True)
+def reset_password(username):
     """
     This command allows you to reset a user's password.
     """
+    user = user_service.get_by_username(username)
 
-    option_list = (Option("-u", "--username", dest="username", required=True),)
-
-    def run(self, username):
-        user = user_service.get_by_username(username)
-
-        if not user:
-            sys.stderr.write("[!] No user found for username: {0}\n".format(username))
-            sys.exit(1)
-
-        sys.stderr.write("[+] Resetting password for {0}\n".format(username))
-        password1 = prompt_pass("Password")
-        password2 = prompt_pass("Confirm Password")
-
-        if password1 != password2:
-            sys.stderr.write("[!] Passwords do not match\n")
-            sys.exit(1)
-
-        user.password = password1
-        user.hash_password()
-        database.commit()
-
-
-class CreateRole(Command):
+    if not user:
+        click.echo("[!] No user found for username: {0}".format(username))
+        sys.exit(1)
+
+    click.echo("[+] Resetting password for {0}".format(username))
+    password1 = click.prompt("Password", hide_input=True)
+    password2 = click.prompt("Confirm Password", hide_input=True)
+
+    if password1 != password2:
+        click.echo("[!] Passwords do not match")
+        sys.exit(1)
+
+    user.password = password1
+    user.hash_password()
+    database.commit()
+
+
+@cli.command("create_role")
+@click.option("-n", "--name", "name", required=True)
+@click.option("-u", "--users", "users", multiple=True, required=True)
+@click.option("-d", "--description", "description", default=[])
+def create_role(name, users, description):
     """
     This command allows for the creation of a new role within Lemur
     """
-
-    option_list = (
-        Option("-n", "--name", dest="name", required=True),
-        Option("-u", "--users", dest="users", default=[]),
-        Option("-d", "--description", dest="description", required=True),
-    )
-
-    def run(self, name, users, description):
-        user_objs = []
-        for u in users:
-            user_obj = user_service.get_by_username(u)
-            if user_obj:
-                user_objs.append(user_obj)
-            else:
-                sys.stderr.write("[!] Cannot find user {0}".format(u))
-                sys.exit(1)
-        role_service.create(name, description=description, users=users)
-        sys.stdout.write("[+] Created new role: {0}".format(name))
+    user_objs = []
+    for u in users:
+        user_obj = user_service.get_by_username(u)
+        if user_obj:
+            user_objs.append(user_obj)
+        else:
+            click.echo("[!] Cannot find user {0}".format(u))
+            sys.exit(1)
+    role_service.create(name, description=description, users=users)
+    click.echo("[+] Created new role: {0}".format(name))
 
 
-class LemurServer(Command):
+@cli.command("start", context_settings=dict(ignore_unknown_options=True, allow_extra_args=True))
+def start():
     """
     This is the main Lemur server, it runs the flask app with gunicorn and
     uses any configuration options passed to it.
 
 
     You can pass all standard gunicorn flags to this command as if you were
     running gunicorn itself.
 
     For example:
 
     lemur start -w 4 -b 127.0.0.0:8002
 
     Will start gunicorn with 4 workers bound to 127.0.0.0:8002
     """
+    from gunicorn.app.wsgiapp import WSGIApplication
+    app = WSGIApplication()
 
-    description = "Run the app within Gunicorn"
-
-    def get_options(self):
-        settings = make_settings()
-        options = []
-        for setting, klass in settings.items():
-            if klass.cli:
-                if klass.action:
-                    if klass.action == "store_const":
-                        options.append(
-                            Option(*klass.cli, const=klass.const, action=klass.action)
-                        )
-                    else:
-                        options.append(Option(*klass.cli, action=klass.action))
-                else:
-                    options.append(Option(*klass.cli))
-
-        return options
+    # run startup tasks on an app like object
+    validate_conf(current_app, REQUIRED_VARIABLES)
 
-    def run(self, *args, **kwargs):
-        from gunicorn.app.wsgiapp import WSGIApplication
+    app.app_uri = "lemur:create_app()"
 
-        app = WSGIApplication()
+    return app.run()
 
-        # run startup tasks on an app like object
-        validate_conf(current_app, REQUIRED_VARIABLES)
 
-        app.app_uri = 'lemur:create_app(config_path="{0}")'.format(
-            current_app.config.get("CONFIG_PATH")
-        )
-
-        return app.run()
-
-
-@manager.command
-def create_config(config_path=None):
+@cli.command("create_config")
+@click.option("-c", "--config", "config_path")
+def create_config(config_path):
     """
     Creates a new configuration file if one does not already exist
     """
     if not config_path:
         config_path = DEFAULT_CONFIG_PATH
 
     config_path = os.path.expanduser(config_path)
@@ -461,18 +423,18 @@
     if not os.path.exists(dir):
         os.makedirs(dir)
 
     config = generate_settings()
     with open(config_path, "w") as f:
         f.write(config)
 
-    sys.stdout.write("[+] Created a new configuration file {0}\n".format(config_path))
+    click.echo("[+] Created a new configuration file {0}".format(config_path))
 
 
-@manager.command
+@cli.command("lock")
 def lock(path=None):
     """
     Encrypts a given path. This directory can be used to store secrets needed for normal
     Lemur operation. This is especially useful for storing secrets needed for communication
     with third parties (e.g. external certificate authorities).
 
     Lemur does not assume anything about the contents of the directory and will attempt to
@@ -483,77 +445,77 @@
 
     :param: path
     """
     if not path:
         path = os.path.expanduser("~/.lemur/keys")
 
     dest_dir = os.path.join(path, "encrypted")
-    sys.stdout.write("[!] Generating a new key...\n")
+    click.echo("[!] Generating a new key...")
 
     key = Fernet.generate_key()
 
     if not os.path.exists(dest_dir):
-        sys.stdout.write("[+] Creating encryption directory: {0}\n".format(dest_dir))
+        click.echo("[+] Creating encryption directory: {0}".format(dest_dir))
         os.makedirs(dest_dir)
 
     for root, dirs, files in os.walk(os.path.join(path, "decrypted")):
         for f in files:
             source = os.path.join(root, f)
             dest = os.path.join(dest_dir, f + ".enc")
             with open(source, "rb") as in_file, open(dest, "wb") as out_file:
                 f = Fernet(key)
                 data = f.encrypt(in_file.read())
                 out_file.write(data)
-                sys.stdout.write(
-                    "[+] Writing file: {0} Source: {1}\n".format(dest, source)
+                click.echo(
+                    "[+] Writing file: {0} Source: {1}".format(dest, source)
                 )
 
-    sys.stdout.write("[+] Keys have been encrypted with key {0}\n".format(key))
+    click.echo("[+] Keys have been encrypted with key {0}".format(key))
 
 
-@manager.command
+@cli.command("unlock")
 def unlock(path=None):
     """
     Decrypts all of the files in a given directory with provided password.
     This is most commonly used during the startup sequence of Lemur
     allowing it to go from source code to something that can communicate
     with external services.
 
     Path defaults ~/.lemur/keys
 
     :param: path
     """
-    key = prompt_pass("[!] Please enter the encryption password")
+    key = click.prompt("[!] Please enter the encryption password", type=str)
 
     if not path:
         path = os.path.expanduser("~/.lemur/keys")
 
     dest_dir = os.path.join(path, "decrypted")
     source_dir = os.path.join(path, "encrypted")
 
     if not os.path.exists(dest_dir):
-        sys.stdout.write("[+] Creating decryption directory: {0}\n".format(dest_dir))
+        click.echo("[+] Creating decryption directory: {0}".format(dest_dir))
         os.makedirs(dest_dir)
 
     for root, dirs, files in os.walk(source_dir):
         for f in files:
             source = os.path.join(source_dir, f)
             dest = os.path.join(dest_dir, ".".join(f.split(".")[:-1]))
             with open(source, "rb") as in_file, open(dest, "wb") as out_file:
                 f = Fernet(key)
                 data = f.decrypt(in_file.read())
                 out_file.write(data)
-                sys.stdout.write(
-                    "[+] Writing file: {0} Source: {1}\n".format(dest, source)
+                click.echo(
+                    "[+] Writing file: {0} Source: {1}".format(dest, source)
                 )
 
-    sys.stdout.write("[+] Keys have been unencrypted!\n")
+    click.echo("[+] Keys have been unencrypted!")
 
 
-@manager.command
+@cli.command("publish_verisign_units")
 def publish_verisign_units():
     """
     Simple function that queries verisign for API units and posts the mertics to
     Atlas API for other teams to consume.
     :return:
     """
     from lemur.plugins import plugins
@@ -579,29 +541,22 @@
             }
         ]
 
         requests.post("http://localhost:8078/metrics", data=json.dumps(metric))
 
 
 def main():
-    manager.add_command("start", LemurServer())
-    manager.add_command("runserver", Server(host="127.0.0.1", threaded=True))
-    manager.add_command("clean", Clean())
-    manager.add_command("show_urls", ShowUrls())
-    manager.add_command("db", MigrateCommand)
-    manager.add_command("init", InitializeApp())
-    manager.add_command("create_user", CreateUser())
-    manager.add_command("reset_password", ResetPassword())
-    manager.add_command("create_role", CreateRole())
-    manager.add_command("source", source_manager)
-    manager.add_command("certificate", certificate_manager)
-    manager.add_command("notify", notification_manager)
-    manager.add_command("report", report_manager)
-    manager.add_command("policy", policy_manager)
-    manager.add_command("pending_certs", pending_certificate_manager)
-    manager.add_command("dns_providers", dns_provider_manager)
-    manager.add_command("acme", acme_manager)
-    manager.run()
+
+    cli.add_command(acme_cli, "acme")
+    cli.add_command(certificate_cli, "certificate")
+    cli.add_command(dns_provider_cli, "dns_providers")
+    cli.add_command(db, "db")
+    cli.add_command(notification_cli, "notify")
+    cli.add_command(pending_certificate_cli, "pending_certs")
+    cli.add_command(policy_cli, "policy")
+    cli.add_command(report_cli, "report")
+    cli.add_command(source_cli, "source")
+    cli()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `lemur-1.4.0/lemur/metrics.py` & `lemur-1.5.0/lemur/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 .. module: lemur.metrics
     :copyright: (c) 2018 by Netflix Inc., see AUTHORS for more
     :license: Apache, see LICENSE for more details.
 """
+from typing import List
+
 from flask import current_app
 from lemur.plugins.base import plugins
 
 
 class Metrics(object):
     """
     :param app: The Flask application object. Defaults to None.
     """
 
-    _providers = []
+    _providers: List[str] = []
 
     def __init__(self, app=None):
         if app is not None:
             self.init_app(app)
 
     def init_app(self, app):
         """Initializes the application with the extension.
```

### Comparing `lemur-1.4.0/lemur/models.py` & `lemur-1.5.0/lemur/models.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/notifications/cli.py` & `lemur-1.5.0/lemur/notifications/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 """
 .. module: lemur.notifications.cli
     :platform: Unix
     :copyright: (c) 2018 by Netflix Inc., see AUTHORS for more
     :license: Apache, see LICENSE for more details.
 .. moduleauthor:: Kevin Glisson <kglisson@netflix.com>
 """
+import click
+
 from flask import current_app
-from flask_script import Manager
 from sentry_sdk import capture_exception
 
 from lemur.certificates.service import get_expiring_deployed_certificates
 from lemur.constants import SUCCESS_METRIC_STATUS, FAILURE_METRIC_STATUS
 from lemur.extensions import metrics
 from lemur.notifications.messaging import send_expiration_notifications, \
     send_expiring_deployed_certificate_notifications
 from lemur.notifications.messaging import send_authority_expiration_notifications
 from lemur.notifications.messaging import send_security_expiration_summary
 
-manager = Manager(usage="Handles notification related tasks.")
+
+@click.group(name="notify", help="Handles notification related tasks.")
+def cli():
+    pass
 
 
-@manager.option(
+@cli.command("expirations")
+@click.option(
     "-e",
     "--exclude",
-    dest="exclude",
-    action="append",
+    "exclude",
+    multiple=True,
     default=[],
     help="Common name matching of certificates that should be excluded from notification",
 )
-@manager.option(
+@click.option(
     "-d",
     "--disabled-notification-plugins",
-    dest="disabled_notification_plugins",
-    action="append",
+    "disabled_notification_plugins",
+    multiple=True,
     default=[],
     help="List of notification plugins for which notifications should NOT be sent",
 )
+def expirations_command(exclude, disabled_notification_plugins):
+    expirations(exclude, disabled_notification_plugins)
+
+
 def expirations(exclude, disabled_notification_plugins):
     """
     Runs Lemur's notification engine, that looks for expiring certificates and sends
     notifications out to those that have subscribed to them.
 
     Every certificate receives notifications by default. When expiration notifications are handled outside of Lemur
     we exclude their names (or matching) from expiration notifications.
@@ -70,17 +79,17 @@
     Runs Lemur's notification engine, that looks for expiring certificate authority certificates and sends
     notifications out to the security team and owner.
 
     :return:
     """
     status = FAILURE_METRIC_STATUS
     try:
-        print("Starting to notify subscribers about expiring certificate authority certificates!")
+        click.echo("Starting to notify subscribers about expiring certificate authority certificates!")
         success, failed = send_authority_expiration_notifications()
-        print(
+        click.echo(
             "Finished notifying subscribers about expiring certificate authority certificates! "
             f"Sent: {success} Failed: {failed}"
         )
         status = SUCCESS_METRIC_STATUS
     except Exception as e:
         capture_exception()
```

### Comparing `lemur-1.4.0/lemur/notifications/messaging.py` & `lemur-1.5.0/lemur/notifications/messaging.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/notifications/models.py` & `lemur-1.5.0/lemur/notifications/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
     :license: Apache, see LICENSE for more details.
 .. moduleauthor:: Kevin Glisson <kglisson@netflix.com>
 """
 from sqlalchemy.orm import relationship
 from sqlalchemy import Integer, String, Column, Boolean, Text
 from sqlalchemy_utils import JSONType
 
-from lemur.database import db
+from lemur.database import BaseModel
 from lemur.plugins.base import plugins
 from lemur.models import (
     certificate_notification_associations,
     pending_cert_notification_associations,
 )
 
 
-class Notification(db.Model):
+class Notification(BaseModel):
     __tablename__ = "notifications"
     id = Column(Integer, primary_key=True)
     label = Column(String(128), unique=True)
     description = Column(Text())
     options = Column(JSONType)
     active = Column(Boolean, default=True)
     plugin_name = Column(String(32))
```

### Comparing `lemur-1.4.0/lemur/notifications/schemas.py` & `lemur-1.5.0/lemur/notifications/schemas.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/notifications/service.py` & `lemur-1.5.0/lemur/notifications/service.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/notifications/views.py` & `lemur-1.5.0/lemur/notifications/views.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/pending_certificates/cli.py` & `lemur-1.5.0/lemur/pending_certificates/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 """
 .. module: lemur.pending_certificates.cli
 
 .. moduleauthor:: James Chuong <jchuong@instartlogic.com>
 .. moduleauthor:: Curtis Castrapel <ccastrapel@netflix.com>
 """
 
+import click
 import copy
 import sys
 
 from flask import current_app
-from flask_script import Manager
 
 from lemur.authorities.service import get as get_authority
 from lemur.constants import ACME_ADDITIONAL_ATTEMPTS
 from lemur.notifications.messaging import send_pending_failure_notification
 from lemur.pending_certificates import service as pending_certificate_service
 from lemur.plugins.base import plugins
 
 
-manager = Manager(usage="Handles pending certificate related tasks.")
+@click.group(name="pending_certs", help="Handles pending certificate related tasks.")
+def cli():
+    pass
 
 
-@manager.option(
-    "-i", dest="ids", action="append", help="IDs of pending certificates to fetch"
+@cli.command("fetch")
+@click.option(
+    "-i",
+    "ids",
+    multiple=True,
+    help="IDs of pending certificates to fetch"
 )
+def fetch_command(ids):
+    fetch(ids)
+
+
 def fetch(ids):
     """
     Attempt to get full certificate for each pending certificate listed.
 
     Args:
         ids: a list of ids of PendingCertificates (passed in by manager options when run as CLI)
              `python manager.py pending_certs fetch -i 123 321 all`
@@ -49,20 +59,24 @@
             pending_certificate_service.update(cert.id, resolved_cert_id=final_cert.id)
             pending_certificate_service.update(cert.id, resolved=True)
             # add metrics to metrics extension
             new += 1
         else:
             pending_certificate_service.increment_attempt(cert)
             failed += 1
-    print(
+    click.echo(
         "[+] Certificates: New: {new} Failed: {failed}".format(new=new, failed=failed)
     )
 
 
-@manager.command
+@cli.command("fetch_all_acme")
+def fetch_all_acme_command():
+    fetch_all_acme()
+
+
 def fetch_all_acme():
     """
     Attempt to get full certificates for each pending certificate listed with the acme-issuer. This is more efficient
     for acme-issued certificates because it will configure all of the DNS challenges prior to resolving any
     certificates.
     """
 
@@ -123,12 +137,12 @@
                 )
             current_app.logger.error(error_log)
     log_data["message"] = "Complete"
     log_data["new"] = new
     log_data["failed"] = failed
     log_data["wrong_issuer"] = wrong_issuer
     current_app.logger.debug(log_data)
-    print(
+    click.echo(
         "[+] Certificates: New: {new} Failed: {failed} Not using ACME: {wrong_issuer}".format(
             new=new, failed=failed, wrong_issuer=wrong_issuer
         )
     )
```

### Comparing `lemur-1.4.0/lemur/pending_certificates/models.py` & `lemur-1.5.0/lemur/pending_certificates/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 )
 from sqlalchemy.orm import relationship
 from sqlalchemy_utils import JSONType
 from sqlalchemy_utils.types.arrow import ArrowType
 
 from lemur.certificates.models import get_sequence
 from lemur.common import defaults, utils
-from lemur.database import db
+from lemur.database import BaseModel
 from lemur.models import (
     pending_cert_source_associations,
     pending_cert_destination_associations,
     pending_cert_notification_associations,
     pending_cert_replacement_associations,
     pending_cert_role_associations,
 )
@@ -54,15 +54,15 @@
         root, end = get_sequence(cert.name)
         if end:
             ends.append(end)
 
     return "{0}-{1}".format(root, max(ends) + 1)
 
 
-class PendingCertificate(db.Model):
+class PendingCertificate(BaseModel):
     __tablename__ = "pending_certs"
     id = Column(Integer, primary_key=True)
     external_id = Column(String(128))
     owner = Column(String(128), nullable=False)
     name = Column(String(256), unique=True)
     description = Column(String(1024))
     notify = Column(Boolean, default=True)
```

### Comparing `lemur-1.4.0/lemur/pending_certificates/schemas.py` & `lemur-1.5.0/lemur/pending_certificates/schemas.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/pending_certificates/service.py` & `lemur-1.5.0/lemur/pending_certificates/service.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/pending_certificates/views.py` & `lemur-1.5.0/lemur/pending_certificates/views.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/base/manager.py` & `lemur-1.5.0/lemur/plugins/base/manager.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/base/v1.py` & `lemur-1.5.0/lemur/plugins/base/v1.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     :copyright: (c) 2018 by Netflix Inc., see AUTHORS for more
     :license: Apache, see LICENSE for more details.
 
 .. moduleauthor:: Kevin Glisson <kglisson@netflix.com>
 """
 from flask import current_app
 from threading import local
+from typing import Optional, Dict, List, Any
 import re
 
 
 # stolen from https://github.com/getsentry/sentry/
 class PluginMount(type):
     def __new__(cls, name, bases, attrs):
         new_cls = type.__new__(cls, name, bases, attrs)
@@ -36,26 +37,26 @@
     >>>     def get_title(self):
     >>>         return 'My Plugin'
     As a general rule all inherited methods should allow ``**kwargs`` to ensure
     ease of future compatibility.
     """
 
     # Generic plugin information
-    title = None
-    slug = None
-    description = None
+    title: Optional[str] = None
+    slug: Optional[str] = None
+    description: Optional[str] = None
     version = None
-    author = None
-    author_url = None
+    author: Optional[str] = None
+    author_url: Optional[str] = None
     resource_links = ()
 
     # Configuration specifics
     conf_key = None
     conf_title = None
-    options = {}
+    options: List[Dict[str, Any]] = []
 
     # Global enabled state
     enabled = True
     can_disable = True
 
     def is_enabled(self):
         """
```

### Comparing `lemur-1.4.0/lemur/plugins/bases/authorization.py` & `lemur-1.5.0/lemur/plugins/bases/authorization.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/bases/destination.py` & `lemur-1.5.0/lemur/plugins/bases/destination.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,20 @@
     requires_key = True
     sync_as_source = False
     sync_as_source_name = ""
 
     def upload(self, name, body, private_key, cert_chain, options, **kwargs):
         raise NotImplementedError
 
+    def allow_multiple_per_account(self):
+        """
+        Specifies whether or not multiple of this destination type may be added per AWS account.
+        """
+        return False
+
 
 class ExportDestinationPlugin(DestinationPlugin):
     default_options = [
         {
             "name": "exportPlugin",
             "type": "export-plugin",
             "required": True,
```

### Comparing `lemur-1.4.0/lemur/plugins/bases/export.py` & `lemur-1.5.0/lemur/plugins/bases/export.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/bases/issuer.py` & `lemur-1.5.0/lemur/plugins/bases/issuer.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/bases/membership.py` & `lemur-1.5.0/lemur/plugins/bases/membership.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/bases/source.py` & `lemur-1.5.0/lemur/plugins/bases/source.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_acme/acme_handlers.py` & `lemur-1.5.0/lemur/plugins/lemur_acme/acme_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,20 +202,21 @@
             if eab_kid and eab_hmac_key:
                 # external account binding (eab_kid and eab_hmac_key could be potentially single use to establish
                 # long-term credentials)
                 eab = messages.ExternalAccountBinding.from_data(account_public_key=key.public_key(),
                                                                 kid=eab_kid,
                                                                 hmac_key=eab_hmac_key,
                                                                 directory=client.directory)
-                registration = client.new_account_and_tos(
-                    messages.NewRegistration.from_data(email=email, external_account_binding=eab)
+                registration = client.new_account(
+                    messages.NewRegistration.from_data(email=email, external_account_binding=eab,
+                                                       terms_of_service_agreed=True)
                 )
             else:
-                registration = client.new_account_and_tos(
-                    messages.NewRegistration.from_data(email=email)
+                registration = client.new_account(
+                    messages.NewRegistration.from_data(email=email, terms_of_service_agreed=True)
                 )
 
             # if store_account is checked, add the private_key and registration resources to the options
             if options['store_account']:
                 new_options = json.loads(authority.options)
                 # the key returned by fields_to_partial_json is missing the key type, so we add it manually
                 key_dict = key.fields_to_partial_json()
@@ -543,18 +544,15 @@
 
     def cleanup_dns_challenges(self, acme_client, authorizations):
         """
         Best effort attempt to delete DNS challenges that may not have been deleted previously. This is usually called
         on an exception
 
         :param acme_client:
-        :param account_number:
-        :param dns_provider:
         :param authorizations:
-        :param dns_provider_options:
         :return:
         """
         for authz_record in authorizations:
             dns_providers = self.dns_providers_for_domain.get(authz_record.target_domain)
             for dns_provider in dns_providers:
                 # Grab account number (For Route53)
                 dns_provider_options = json.loads(dns_provider.credentials)
```

### Comparing `lemur-1.4.0/lemur/plugins/lemur_acme/challenge_types.py` & `lemur-1.5.0/lemur/plugins/lemur_acme/challenge_types.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_acme/cloudflare.py` & `lemur-1.5.0/lemur/plugins/lemur_acme/cloudflare.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_acme/dyn.py` & `lemur-1.5.0/lemur/plugins/lemur_acme/dyn.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_acme/nsone.py` & `lemur-1.5.0/lemur/plugins/lemur_acme/nsone.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_acme/plugin.py` & `lemur-1.5.0/lemur/plugins/lemur_acme/plugin.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_acme/powerdns.py` & `lemur-1.5.0/lemur/plugins/lemur_acme/powerdns.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_acme/route53.py` & `lemur-1.5.0/lemur/plugins/lemur_acme/route53.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,26 @@
         time.sleep(5)
 
 
 @sts_client("route53")
 def find_zone_id(domain, client=None):
     paginator = client.get_paginator("list_hosted_zones")
     zones = []
+    match_length = 0
     for page in paginator.paginate():
         for zone in page["HostedZones"]:
             if domain.endswith(zone["Name"]) or (domain + ".").endswith(zone["Name"]):
                 if not zone["Config"]["PrivateZone"]:
-                    zones.append((zone["Name"], zone["Id"]))
+                    if len(zone["Name"]) > match_length:
+                        # reset the list, as we have found a longer match
+                        zones = [(zone["Name"], zone["Id"])]
+                        match_length = len(zone["Name"])
+                    elif len(zone["Name"]) == match_length:
+                        # add all equal length zones, though only the first one will be returned
+                        zones.append((zone["Name"], zone["Id"]))
 
     if not zones:
         raise ValueError("Unable to find a Route53 hosted zone for {}".format(domain))
     return zones[0][1]
 
 
 @sts_client("route53")
```

### Comparing `lemur-1.4.0/lemur/plugins/lemur_acme/ultradns.py` & `lemur-1.5.0/lemur/plugins/lemur_acme/ultradns.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_adcs/plugin.py` & `lemur-1.5.0/lemur/plugins/lemur_adcs/plugin.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_atlas/plugin.py` & `lemur-1.5.0/lemur/plugins/lemur_atlas/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,16 @@
     :platform: Unix
     :copyright: (c) 2018 by Netflix Inc., see AUTHORS for more
     :license: Apache, see LICENSE for more details.
 
 .. moduleauthor:: Kevin Glisson <kglisson@netflix.com>
 """
 import json
+from typing import Any, Dict
+
 import requests
 from requests.exceptions import ConnectionError
 from datetime import datetime
 
 from flask import current_app
 from lemur.plugins import lemur_atlas as atlas
 from lemur.plugins.bases.metric import MetricPlugin
@@ -41,15 +43,15 @@
             "required": False,
             "help_message": "If no host is provided localhost is assumed",
             "default": "localhost",
         },
         {"name": "sidecar_port", "type": "int", "required": False, "default": 8078},
     ]
 
-    metric_data = {}
+    metric_data: Dict[str, Any] = {}
     sidecar_host = None
     sidecar_port = None
 
     def submit(
         self, metric_name, metric_type, metric_value, metric_tags=None, options=None
     ):
         if not options:
```

### Comparing `lemur-1.4.0/lemur/plugins/lemur_atlas_redis/plugin.py` & `lemur-1.5.0/lemur/plugins/lemur_atlas_redis/plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .. module: lemur.plugins.lemur_atlas_redis.plugin
     :platform: Unix
     :copyright: (c) 2018 by Netflix Inc., see AUTHORS for more
     :license: Apache, see LICENSE for more details.
 
 .. moduleauthor:: Jay Zarfoss
 """
+from typing import Dict, Any
 
 from redis import Redis
 import json
 from datetime import datetime
 
 from flask import current_app
 from lemur.plugins import lemur_atlas as atlas
@@ -41,15 +42,15 @@
             "required": False,
             "help_message": "If no host is provided localhost is assumed",
             "default": "localhost",
         },
         {"name": "redis_port", "type": "int", "required": False, "default": 28527},
     ]
 
-    metric_data = {}
+    metric_data: Dict[str, Any] = {}
     redis_host = None
     redis_port = None
 
     def submit(
         self, metric_name, metric_type, metric_value, metric_tags=None, options=None
     ):
         if not options:
```

### Comparing `lemur-1.4.0/lemur/plugins/lemur_aws/cloudfront.py` & `lemur-1.5.0/lemur/plugins/lemur_aws/cloudfront.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,18 @@
         while True:
             response = get_distributions(**kwargs)
 
             list = response.get("DistributionList")
             if not list:
                 return distributions
 
-            distributions += list["Items"]
+            items = list.get("Items")
+            if not items:
+                return distributions
+            distributions += items
 
             if not list.get("IsTruncated"):
                 return distributions
             else:
                 kwargs.update(dict(Marker=list["NextMarker"]))
     except Exception as e:  # noqa
         metrics.send("list_all_distributions_error", "counter", 1)
```

### Comparing `lemur-1.4.0/lemur/plugins/lemur_aws/ec2.py` & `lemur-1.5.0/lemur/plugins/lemur_aws/ec2.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_aws/elb.py` & `lemur-1.5.0/lemur/plugins/lemur_aws/elb.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_aws/iam.py` & `lemur-1.5.0/lemur/plugins/lemur_aws/iam.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_aws/plugin.py` & `lemur-1.5.0/lemur/plugins/lemur_aws/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,15 +313,15 @@
                 "region": region,
                 "number_of_load_balancers": len(elbs)
             })
 
             for e in elbs:
                 try:
                     endpoints.extend(get_elb_endpoints(account_number, region, e))
-                except Exception as e:  # noqa
+                except Exception:  # noqa
                     capture_exception()
                     continue
 
             # fetch advanced ELBs
             elbs_v2 = elb.get_all_elbs_v2(account_number=account_number, region=region)
             current_app.logger.info({
                 "message": "Describing advanced load balancers",
@@ -587,33 +587,36 @@
         super(S3DestinationPlugin, self).__init__(*args, **kwargs)
 
     def upload(self, name, body, private_key, chain, options, **kwargs):
         files = self.export(body, private_key, chain, options)
         function = f"{__name__}.{sys._getframe().f_code.co_name}"
 
         for ext, passphrase, data in files:
-            filename = join(self.get_option("prefix", options), f"{name}.{ext}")
+            filename = join(self.get_option("prefix", options), f"{name}.{ext.lstrip('.')}")
             response = s3.put(
                 self.get_option("bucket", options),
                 self.get_option("region", options),
                 filename,
                 data,
                 self.get_option("encrypt", options),
                 account_number=self.get_option("accountNumber", options),
             )
             res = "Success" if response else "Failure"
             log_data = {
                 "function": function,
-                "message": "upload acme token challenge",
+                "message": "upload s3 file",
                 "result": res,
                 "bucket_name": self.get_option("bucket", options),
                 "filename": filename
             }
             current_app.logger.info(log_data)
 
+    def allow_multiple_per_account(self):
+        return True
+
     def upload_acme_token(self, token_path, token, options, **kwargs):
         """
         This is called from the acme http challenge
 
         :param self:
         :param token_path:
         :param token:
@@ -677,18 +680,32 @@
         current_app.logger.info(log_data)
         metrics.send(f"{function}", "counter", 1, metric_tags={"result": res,
                                                                "bucket_name": bucket_name,
                                                                "filename": filename})
         return response
 
     def clean(self, certificate, options, **kwargs):
+        files = self.export(certificate.body, certificate.private_key, certificate.chain, options)
+        function = f"{__name__}.{sys._getframe().f_code.co_name}"
         prefix = self.get_option("prefix", options)
-        s3.delete(bucket_name=self.get_option("bucket", options),
-                  prefixed_object_name=join(prefix, f"{certificate.name}.pem"),
+
+        for ext, passphrase, data in files:
+            filename = join(prefix, f"{certificate.name}.{ext.lstrip('.')}")
+            response = s3.delete(bucket_name=self.get_option("bucket", options),
+                  prefixed_object_name=filename,
                   account_number=self.get_option("accountNumber", options))
+            res = "Success" if response else "Failure"
+            log_data = {
+                "function": function,
+                "message": "delete s3 file",
+                "result": res,
+                "bucket_name": self.get_option("bucket", options),
+                "filename": filename
+            }
+            current_app.logger.info(log_data)
 
 
 class SNSNotificationPlugin(ExpirationNotificationPlugin):
     title = "AWS SNS"
     slug = "aws-sns"
     description = "Sends notifications to AWS SNS"
     version = aws.VERSION
```

### Comparing `lemur-1.4.0/lemur/plugins/lemur_aws/s3.py` & `lemur-1.5.0/lemur/plugins/lemur_aws/s3.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_aws/sns.py` & `lemur-1.5.0/lemur/plugins/lemur_aws/sns.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_aws/sts.py` & `lemur-1.5.0/lemur/plugins/lemur_aws/sts.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_azure_dest/plugin.py` & `lemur-1.5.0/lemur/plugins/lemur_azure_dest/plugin.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_cfssl/plugin.py` & `lemur-1.5.0/lemur/plugins/lemur_cfssl/plugin.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_cryptography/plugin.py` & `lemur-1.5.0/lemur/plugins/lemur_cryptography/plugin.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_csr/plugin.py` & `lemur-1.5.0/lemur/plugins/lemur_csr/plugin.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_digicert/plugin.py` & `lemur-1.5.0/lemur/plugins/lemur_digicert/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,18 @@
     https://www.digicert.com/services/v2/documentation
 
     Original Implementation:
     Chris Dorros, github.com/opendns/lemur-digicert
 
 .. moduleauthor:: Kevin Glisson <kglisson@netflix.com>
 """
+import copy
+import ipaddress
 import json
+from typing import Any, Dict, List
 
 import arrow
 import pem
 import requests
 import sys
 from cryptography import x509
 from flask import current_app, g
@@ -106,16 +109,17 @@
     :param options:
     :return:
     """
     names = []
     # add SANs if present
     if options.get("extensions"):
         for san in options["extensions"]["sub_alt_names"]["names"]:
-            if isinstance(san, x509.DNSName):
-                names.append(san.value)
+            is_ip_addr = (isinstance(san, x509.IPAddress) and (isinstance(san.value, ipaddress.IPv4Address) or isinstance(san.value, ipaddress.IPv6Address)))
+            if isinstance(san, x509.DNSName) or is_ip_addr:
+                names.append(str(san.value))
     return names
 
 
 def map_fields(options, csr):
     """Set the incoming issuer options to DigiCert fields/options.
 
     :param options:
@@ -237,15 +241,15 @@
     Handle the DigiCert CIS API response and any errors it might have experienced.
     :param response:
     :return:
     """
     if response.status_code == 404:
         raise Exception("DigiCert: order not in issued state")
     elif response.status_code == 406:
-        log_header = session.headers
+        log_header = copy.deepcopy(session.headers)
         log_header.pop("X-DC-DEVKEY")
         reset_cis_session(session)
         raise Exception("DigiCert: wrong header request format: " + str(log_header))
     elif response.status_code > 399:
         raise Exception("DigiCert rejected request with the error: " + response.text)
     if response.url.endswith("download"):
         return response.content
@@ -481,15 +485,15 @@
     slug = "digicert-cis-source"
     description = "Enables the use of Digicert as a source of existing certificates."
     version = digicert.VERSION
 
     author = "Kevin Glisson"
     author_url = "https://github.com/netflix/lemur.git"
 
-    additional_options = []
+    additional_options: List[Dict[str, Any]] = []
 
     def __init__(self, *args, **kwargs):
         """Initialize source with appropriate details."""
         required_vars = [
             "DIGICERT_CIS_API_KEY",
             "DIGICERT_CIS_URL",
             "DIGICERT_CIS_ROOTS",
```

### Comparing `lemur-1.4.0/lemur/plugins/lemur_email/plugin.py` & `lemur-1.5.0/lemur/plugins/lemur_email/plugin.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_email/templates/authority_expiration.html` & `lemur-1.5.0/lemur/plugins/lemur_email/templates/authority_expiration.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_email/templates/config.py` & `lemur-1.5.0/lemur/plugins/lemur_email/templates/config.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_email/templates/expiration.html` & `lemur-1.5.0/lemur/plugins/lemur_email/templates/expiration.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_email/templates/expiration_summary.html` & `lemur-1.5.0/lemur/plugins/lemur_email/templates/expiration_summary.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_email/templates/expiring_deployed_certificate.html` & `lemur-1.5.0/lemur/plugins/lemur_email/templates/expiring_deployed_certificate.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_email/templates/failed.html` & `lemur-1.5.0/lemur/plugins/lemur_email/templates/failed.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_email/templates/issued.html` & `lemur-1.5.0/lemur/plugins/lemur_email/templates/issued.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_email/templates/reissue_failed.html` & `lemur-1.5.0/lemur/plugins/lemur_email/templates/reissue_failed.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_email/templates/reissued_with_no_endpoints.html` & `lemur-1.5.0/lemur/plugins/lemur_email/templates/reissued_with_no_endpoints.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_email/templates/revocation.html` & `lemur-1.5.0/lemur/plugins/lemur_email/templates/revocation.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_email/templates/rotation.html` & `lemur-1.5.0/lemur/plugins/lemur_email/templates/rotation.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_entrust/plugin.py` & `lemur-1.5.0/lemur/plugins/lemur_entrust/plugin.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_jks/plugin.py` & `lemur-1.5.0/lemur/plugins/lemur_jks/plugin.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_kubernetes/plugin.py` & `lemur-1.5.0/lemur/plugins/lemur_kubernetes/plugin.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_openssl/plugin.py` & `lemur-1.5.0/lemur/plugins/lemur_openssl/plugin.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,23 +31,42 @@
 
     if p.returncode != 0:
         current_app.logger.debug(" ".join(command))
         current_app.logger.error(stderr)
         raise Exception(stderr)
 
 
-def create_pkcs12(cert, chain, p12_tmp, key, alias, passphrase):
+def get_openssl_version():
+    """
+    :return: the openssl version, if it can be determined
+    """
+    command = ['openssl', 'version']
+    p = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    current_app.logger.debug(command)
+    stdout, stderr = p.communicate()
+
+    if p.returncode != 0:
+        current_app.logger.debug(" ".join(command))
+        current_app.logger.error(stderr)
+        raise Exception(stderr)
+
+    if stdout.startswith(b'OpenSSL'):
+        return stdout.split()[1]
+
+
+def create_pkcs12(cert, chain, p12_tmp, key, alias, passphrase, legacy: bool = False):
     """
     Creates a pkcs12 formated file.
     :param cert:
     :param chain:
     :param p12_tmp:
     :param key:
     :param alias:
     :param passphrase:
+    :param legacy: should legacy insecure encryption be used (for support with ancient Java versions)
     """
     assert isinstance(cert, str)
     if chain is not None:
         assert isinstance(chain, str)
     assert isinstance(key, str)
 
     with mktempfile() as key_tmp:
@@ -57,31 +76,37 @@
         # Create PKCS12 keystore from private key and public certificate
         with mktempfile() as cert_tmp:
             with open(cert_tmp, "w") as f:
                 if chain:
                     f.writelines([cert.strip() + "\n", chain.strip() + "\n"])
                 else:
                     f.writelines([cert.strip() + "\n"])
+            cmd = [
+                "openssl",
+                "pkcs12",
+                "-export",
+                "-name",
+                alias,
+                "-in",
+                cert_tmp,
+                "-inkey",
+                key_tmp,
+                "-out",
+                p12_tmp,
+                "-password",
+                "pass:{}".format(passphrase),
+            ]
+
+            if legacy:
+                version = get_openssl_version()
+                if version and version >= b'3':
+                    cmd.append("-legacy")
 
             run_process(
-                [
-                    "openssl",
-                    "pkcs12",
-                    "-export",
-                    "-name",
-                    alias,
-                    "-in",
-                    cert_tmp,
-                    "-inkey",
-                    key_tmp,
-                    "-out",
-                    p12_tmp,
-                    "-password",
-                    "pass:{}".format(passphrase),
-                ]
+                cmd
             )
 
 
 class OpenSSLExportPlugin(ExportPlugin):
     title = "OpenSSL"
     slug = "openssl-export"
     description = "Is a loose interface to openssl and support various formats"
@@ -91,15 +116,15 @@
     author_url = "https://github.com/netflix/lemur"
 
     options = [
         {
             "name": "type",
             "type": "select",
             "required": True,
-            "available": ["PKCS12 (.p12)"],
+            "available": ["PKCS12 (.p12)", "legacy PKCS12 (.p12)"],
             "helpMessage": "Choose the format you wish to export",
         },
         {
             "name": "passphrase",
             "type": "str",
             "required": False,
             "helpMessage": "If no passphrase is given one will be generated for you, we highly recommend this.",
@@ -138,14 +163,21 @@
         with mktemppath() as output_tmp:
             if type == "PKCS12 (.p12)":
                 if not key:
                     raise Exception("Private Key required by {0}".format(type))
 
                 create_pkcs12(body, chain, output_tmp, key, alias, passphrase)
                 extension = "p12"
+            elif type == "legacy PKCS12 (.p12)":
+                if not key:
+                    raise Exception("Private Key required by {0}".format(type))
+
+                create_pkcs12(body, chain, output_tmp, key, alias, passphrase, legacy=True)
+                extension = "p12"
+
             else:
                 raise Exception("Unable to export, unsupported type: {0}".format(type))
 
             with open(output_tmp, "rb") as f:
                 raw = f.read()
 
         return extension, passphrase, raw
```

### Comparing `lemur-1.4.0/lemur/plugins/lemur_sftp/plugin.py` & `lemur-1.5.0/lemur/plugins/lemur_sftp/plugin.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_slack/plugin.py` & `lemur-1.5.0/lemur/plugins/lemur_slack/plugin.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_vault_dest/plugin.py` & `lemur-1.5.0/lemur/plugins/lemur_vault_dest/plugin.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/lemur_verisign/plugin.py` & `lemur-1.5.0/lemur/plugins/lemur_verisign/plugin.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/utils.py` & `lemur-1.5.0/lemur/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/plugins/views.py` & `lemur-1.5.0/lemur/plugins/views.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/policies/models.py` & `lemur-1.5.0/lemur/policies/models.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,18 +4,18 @@
     :synopsis: This module contains all of the models need to create a certificate policy within Lemur.
     :copyright: (c) 2018 by Netflix Inc., see AUTHORS for more
     :license: Apache, see LICENSE for more details.
 .. moduleauthor:: Kevin Glisson <kglisson@netflix.com>
 """
 from sqlalchemy import Column, Integer, String
 
-from lemur.database import db
+from lemur.database import BaseModel
 
 
-class RotationPolicy(db.Model):
+class RotationPolicy(BaseModel):
     __tablename__ = "rotation_policies"
     id = Column(Integer, primary_key=True)
     name = Column(String)
     days = Column(Integer)
 
     def __repr__(self):
         return "RotationPolicy(days={days}, name={name})".format(
```

### Comparing `lemur-1.4.0/lemur/policies/service.py` & `lemur-1.5.0/lemur/policies/service.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/reporting/cli.py` & `lemur-1.5.0/lemur/reporting/cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,47 @@
 """
 .. module: lemur.reporting.cli
     :platform: Unix
     :copyright: (c) 2018 by Netflix Inc., see AUTHORS for more
     :license: Apache, see LICENSE for more details.
 .. moduleauthor:: Kevin Glisson <kglisson@netflix.com>
 """
+import click
+
 from tabulate import tabulate
-from flask_script import Manager
 
 from lemur.reporting.service import fqdns, expiring_certificates
 
-manager = Manager(usage="Reporting related tasks.")
+
+@click.group(name="report", help="Reporting related tasks.")
+def cli():
+    pass
 
 
-@manager.option(
+@cli.command("fqdn")
+@click.option(
     "-v",
     "--validity",
-    dest="validity",
-    choices=["all", "expired", "valid"],
+    "validity",
+    type=click.Choice(["all", "expired", "valid"], case_sensitive=False),
     default="all",
     help="Filter certificates by validity.",
 )
-@manager.option(
+@click.option(
     "-d",
     "--deployment",
-    dest="deployment",
-    choices=["all", "deployed", "ready"],
+    "deployment",
+    type=click.Choice(["all", "deployed", "ready"], case_sensitive=False),
     default="all",
     help="Filter by deployment status.",
 )
+def fqdn_command(deployment, validity):
+    fqdn(deployment, validity)
+
+
 def fqdn(deployment, validity):
     """
     Generates a report in order to determine the number of FQDNs covered by Lemur issued certificates.
     """
     headers = [
         "FQDN",
         "Root Domain",
@@ -53,33 +62,43 @@
                     cert.owner,
                     cert.not_after,
                     cert.validity_range.days,
                     cert.validity_remaining.days,
                 ]
             )
 
-    print(tabulate(rows, headers=headers))
+    click.echo(tabulate(rows, headers=headers))
 
 
-@manager.option("-ttl", "--ttl", dest="ttl", default=30, help="Days til expiration.")
-@manager.option(
+@cli.command("expiring")
+@click.option("-ttl",
+              "--ttl",
+              "ttl",
+              default=30,
+              help="Days til expiration."
+)
+@click.option(
     "-d",
     "--deployment",
-    dest="deployment",
-    choices=["all", "deployed", "ready"],
+    "deployment",
+    type=click.Choice(["all", "deployed", "ready"], case_sensitive=False),
     default="all",
     help="Filter by deployment status.",
 )
+def expiring_command(ttl, deployment):
+    expiring(ttl, deployment)
+
+
 def expiring(ttl, deployment):
     """
     Returns certificates expiring in the next n days.
     """
     headers = ["Common Name", "Owner", "Issuer", "Validity End", "Endpoint"]
     rows = []
 
     for cert in expiring_certificates(ttl=ttl, deployment=deployment).all():
         for endpoint in cert.endpoints:
             rows.append(
                 [cert.cn, cert.owner, cert.issuer, cert.not_after, endpoint.dnsname]
             )
 
-    print(tabulate(rows, headers=headers))
+    click.echo(tabulate(rows, headers=headers))
```

### Comparing `lemur-1.4.0/lemur/reporting/service.py` & `lemur-1.5.0/lemur/reporting/service.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/roles/models.py` & `lemur-1.5.0/lemur/roles/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 
 .. moduleauthor:: Kevin Glisson <kglisson@netflix.com>
 
 """
 from sqlalchemy.orm import relationship
 from sqlalchemy import Boolean, Column, Integer, String, Text, ForeignKey
 
-from lemur.database import db
+from lemur.database import BaseModel
 from lemur.utils import Vault
 from lemur.models import (
     roles_users,
     roles_authorities,
     roles_certificates,
     pending_cert_role_associations,
 )
 
 
-class Role(db.Model):
+class Role(BaseModel):
     __tablename__ = "roles"
     id = Column(Integer, primary_key=True)
     name = Column(String(128), unique=True)
     username = Column(String(128))
     password = Column(Vault)
     description = Column(Text)
     authority_id = Column(Integer, ForeignKey("authorities.id"))
```

### Comparing `lemur-1.4.0/lemur/roles/schemas.py` & `lemur-1.5.0/lemur/roles/schemas.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/roles/service.py` & `lemur-1.5.0/lemur/roles/service.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/roles/views.py` & `lemur-1.5.0/lemur/roles/views.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/schemas.py` & `lemur-1.5.0/lemur/schemas.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/sources/cli.py` & `lemur-1.5.0/lemur/sources/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 .. module: lemur.sources.cli
     :platform: Unix
     :copyright: (c) 2018 by Netflix Inc., see AUTHORS for more
     :license: Apache, see LICENSE for more details.
 .. moduleauthor:: Kevin Glisson <kglisson@netflix.com>
 """
 from copy import deepcopy
+import click
 import sys
 import time
 
 from tabulate import tabulate
-from flask_script import Manager
 from flask import current_app
 from sentry_sdk import capture_exception
 
 from lemur.constants import SUCCESS_METRIC_STATUS, FAILURE_METRIC_STATUS
 
 from lemur.extensions import metrics
 from lemur.plugins.base import plugins
@@ -22,63 +22,65 @@
 
 from lemur.destinations import service as dest_service
 from lemur.sources import service as source_service
 from lemur.users import service as user_service
 from lemur.certificates import service as certificate_service
 
 
-manager = Manager(usage="Handles all source related tasks.")
+@click.group(name="source", help="Handles all source related tasks.")
+def cli():
+    pass
 
 
 def validate_sources(source_strings):
     sources = []
     if not source_strings:
         table = []
         for source in source_service.get_all():
             table.append([source.label, source.active, source.description])
 
-        print("No source specified choose from below:")
-        print(tabulate(table, headers=["Label", "Active", "Description"]))
+        click.echo("No source specified choose from below:")
+        click.echo(tabulate(table, headers=["Label", "Active", "Description"]))
         sys.exit(1)
 
     if "all" in source_strings:
         sources = source_service.get_all()
     else:
         for source_str in source_strings:
             source = source_service.get_by_label(source_str)
 
             if not source:
-                print(
+                click.echo(
                     "Unable to find specified source with label: {0}".format(source_str)
                 )
                 sys.exit(1)
 
             sources.append(source)
     return sources
 
 
 def validate_destinations(destination_strings):
     if not destination_strings:
         table = []
         for dest in dest_service.get_all():
             table.append([dest.label, dest.description])
 
-        print("No destination specified choose from below:")
-        print(tabulate(table, headers=["Label", "Description"]))
+        click.echo("No destination specified choose from below:")
+        click.echo(tabulate(table, headers=["Label", "Description"]))
         sys.exit(1)
 
     if "all" in destination_strings:
         return dest_service.get_all()
 
     destinations = []
     for label in destination_strings:
         dest = dest_service.get_by_label(label)
 
         if not dest:
-            print(
+            click.echo(
                 "Unable to find specified destination with label: {0}".format(label)
             )
             sys.exit(1)
 
         destinations.append(dest)
     return destinations
 
@@ -97,62 +99,67 @@
         certificate_service.database.update(certificate)
         return SUCCESS_METRIC_STATUS
     except Exception as e:
         current_app.logger.exception(e)
         capture_exception()
 
 
-@manager.option(
+@cli.command("sync")
+@click.option(
     "-s",
     "--sources",
-    dest="source_strings",
-    action="append",
+    "source_strings",
+    multiple=True,
     help="Sources to operate on.",
 )
-@manager.option(
+@click.option(
     "-ttl",
     "--time-to-live",
+    "ttl",
     type=int,
-    dest="ttl",
     default=2,
     help="Time in hours, after which endpoint has not been refreshed, to remove endpoints from the source.",
 )
+def sync_command(source_strings, ttl):
+    sync(source_strings, ttl)
+
+
 def sync(source_strings, ttl):
     sources = validate_sources(source_strings)
     for source in sources:
         status = FAILURE_METRIC_STATUS
 
         start_time = time.time()
-        print("[+] Staring to sync source: {label} and expire endpoints ttl={ttl}h\n".format(
+        click.echo("[+] Staring to sync source: {label} and expire endpoints ttl={ttl}h\n".format(
             label=source.label, ttl=ttl))
         user = user_service.get_by_username("lemur")
 
         try:
             data = source_service.sync(source, user, ttl_hours=ttl)
-            print(
+            click.echo(
                 "[+] Certificates: New: {new} Updated: {updated}".format(
                     new=data["certificates"][0], updated=data["certificates"][1]
                 )
             )
-            print(
+            click.echo(
                 "[+] Endpoints: New: {new} Updated: {updated} Expired: {expired}".format(
                     new=data["endpoints"][0], updated=data["endpoints"][1], expired=data["endpoints"][2]
                 )
             )
-            print(
+            click.echo(
                 "[+] Finished syncing source: {label}. Run Time: {time}".format(
                     label=source.label, time=(time.time() - start_time)
                 )
             )
             status = SUCCESS_METRIC_STATUS
 
         except Exception as e:
             current_app.logger.exception(e)
 
-            print("[X] Failed syncing source {label}!\n".format(label=source.label))
+            click.echo("[X] Failed syncing source {label}!\n".format(label=source.label))
 
             capture_exception()
             metrics.send(
                 "source_sync_fail",
                 "counter",
                 1,
                 metric_tags={"source": source.label, "status": status},
@@ -162,43 +169,48 @@
             "source_sync",
             "counter",
             1,
             metric_tags={"source": source.label, "status": status},
         )
 
 
-@manager.option(
+@cli.command("clean")
+@click.option(
     "-s",
     "--sources",
-    dest="source_strings",
-    action="append",
+    "source_strings",
+    multiple=True,
     help="Sources to operate on.",
 )
-@manager.option(
+@click.option(
     "-c",
     "--commit",
-    dest="commit",
-    action="store_true",
+    "commit",
+    type=bool,
     default=False,
     help="Persist changes.",
 )
+def clean_command(source_strings, commit):
+    clean(source_strings, commit)
+
+
 def clean(source_strings, commit):
     sources = validate_sources(source_strings)
     for source in sources:
         s = plugins.get(source.plugin_name)
 
         if not hasattr(s, "clean"):
             info_text = f"Cannot clean source: {source.label}, source plugin does not implement 'clean()'"
             current_app.logger.warning(info_text)
-            print(info_text)
+            click.echo(info_text)
             continue
 
         start_time = time.time()
 
-        print("[+] Staring to clean source: {label}!\n".format(label=source.label))
+        click.echo("[+] Staring to clean source: {label}!\n".format(label=source.label))
 
         cleaned = 0
         certificates = certificate_service.get_all_pending_cleaning_expired(source)
         for certificate in certificates:
             status = FAILURE_METRIC_STATUS
             if commit:
                 status = execute_clean(s, certificate, source)
@@ -211,56 +223,60 @@
             )
             current_app.logger.warning(f"Removed {certificate.name} from source {source.label} during cleaning")
             cleaned += 1
 
         info_text = f"[+] Finished cleaning source: {source.label}. " \
                     f"Removed {cleaned} certificates from source. " \
                     f"Run Time: {(time.time() - start_time)}\n"
-        print(info_text)
+        click.echo(info_text)
         current_app.logger.warning(info_text)
 
 
-@manager.option(
+@cli.command("clean_unused_and_expiring_within_days")
+@click.option(
     "-s",
     "--sources",
-    dest="source_strings",
-    action="append",
+    "source_strings",
+    multiple=True,
     help="Sources to operate on.",
 )
-@manager.option(
+@click.option(
     "-d",
     "--days",
-    dest="days_to_expire",
+    "days_to_expire",
     type=int,
-    action="store",
     required=True,
     help="The expiry range within days.",
 )
-@manager.option(
+@click.option(
     "-c",
     "--commit",
-    dest="commit",
-    action="store_true",
+    "commit",
+    type=bool,
     default=False,
     help="Persist changes.",
 )
+def clean_unused_and_expiring_within_days_command(source_strings, days_to_expire, commit):
+    clean_unused_and_expiring_within_days(source_strings, days_to_expire, commit)
+
+
 def clean_unused_and_expiring_within_days(source_strings, days_to_expire, commit):
     sources = validate_sources(source_strings)
     for source in sources:
         s = plugins.get(source.plugin_name)
 
         if not hasattr(s, "clean"):
             info_text = f"Cannot clean source: {source.label}, source plugin does not implement 'clean()'"
             current_app.logger.warning(info_text)
-            print(info_text)
+            click.echo(info_text)
             continue
 
         start_time = time.time()
 
-        print("[+] Staring to clean source: {label}!\n".format(label=source.label))
+        click.echo("[+] Staring to clean source: {label}!\n".format(label=source.label))
 
         cleaned = 0
         certificates = certificate_service.get_all_pending_cleaning_expiring_in_days(source, days_to_expire)
         for certificate in certificates:
             status = FAILURE_METRIC_STATUS
             if commit:
                 status = execute_clean(s, certificate, source)
@@ -273,56 +289,60 @@
             )
             current_app.logger.warning(f"Removed {certificate.name} from source {source.label} during cleaning")
             cleaned += 1
 
         info_text = f"[+] Finished cleaning source: {source.label}. " \
                     f"Removed {cleaned} certificates from source. " \
                     f"Run Time: {(time.time() - start_time)}\n"
-        print(info_text)
+        click.echo(info_text)
         current_app.logger.warning(info_text)
 
 
-@manager.option(
+@cli.command("clean_unused_and_issued_since_days")
+@click.option(
     "-s",
     "--sources",
-    dest="source_strings",
-    action="append",
+    "source_strings",
+    multiple=True,
     help="Sources to operate on.",
 )
-@manager.option(
+@click.option(
     "-d",
     "--days",
-    dest="days_since_issuance",
+    "days_since_issuance",
     type=int,
-    action="store",
     required=True,
     help="Days since issuance.",
 )
-@manager.option(
+@click.option(
     "-c",
     "--commit",
-    dest="commit",
-    action="store_true",
+    "commit",
+    type=bool,
     default=False,
     help="Persist changes.",
 )
+def clean_unused_and_issued_since_days_command(source_strings, days_since_issuance, commit):
+    clean_unused_and_issued_since_days(source_strings, days_since_issuance, commit)
+
+
 def clean_unused_and_issued_since_days(source_strings, days_since_issuance, commit):
     sources = validate_sources(source_strings)
     for source in sources:
         s = plugins.get(source.plugin_name)
 
         if not hasattr(s, "clean"):
             info_text = f"Cannot clean source: {source.label}, source plugin does not implement 'clean()'"
             current_app.logger.warning(info_text)
-            print(info_text)
+            click.echo(info_text)
             continue
 
         start_time = time.time()
 
-        print("[+] Staring to clean source: {label}!\n".format(label=source.label))
+        click.echo("[+] Staring to clean source: {label}!\n".format(label=source.label))
 
         cleaned = 0
         certificates = certificate_service.get_all_pending_cleaning_issued_since_days(source, days_since_issuance)
         for certificate in certificates:
             status = FAILURE_METRIC_STATUS
             if commit:
                 status = execute_clean(s, certificate, source)
@@ -335,44 +355,54 @@
             )
             current_app.logger.warning(f"Removed {certificate.name} from source {source.label} during cleaning")
             cleaned += 1
 
         info_text = f"[+] Finished cleaning source: {source.label}. " \
                     f"Removed {cleaned} certificates from source. " \
                     f"Run Time: {(time.time() - start_time)}\n"
-        print(info_text)
+        click.echo(info_text)
         current_app.logger.warning(info_text)
 
 
-@manager.option(
+@cli.command("sync_source_destination")
+@click.option(
     "-d",
     "--destinations",
-    dest="labels",
-    action="append",
+    "labels",
+    multiple=True,
     help="Destinations to operate on.",
 )
+def sync_source_destination_command(labels):
+    sync_source_destination(labels)
+
+
 def sync_source_destination(labels):
     """
     This command will sync destination and source, to make sure eligible destinations are also present as source.
     Destination eligibility is determined on the sync_as_source attribute of the plugin.
     The destination sync_as_source_name provides the name of the suitable source-plugin.
     We use (account number, IAM path) tuple uniqueness to avoid duplicate sources.
 
     Lemur now does this automatically during destination create and update, so this command is primarily useful
     for migrating legacy destinations.  Set "-d all" to sync all destinations.
     """
     destinations = validate_destinations(labels)
     for destination in destinations:
         if source_service.add_aws_destination_to_sources(destination):
             info_text = f"[+] New source added: {destination.label}.\n"
-            print(info_text)
+            click.echo(info_text)
             current_app.logger.warning(info_text)
 
 
-@manager.option("-s", "--source", dest="source_label")
+@cli.command("enable_cloudfront")
+@click.option("-s", "--source", "source_label")
+def enable_cloudfront_command(source_label):
+    enable_cloudfront(source_label)
+
+
 def enable_cloudfront(source_label):
     """
     Given the label of a legacy AWS source (without path or endpointType options), set up the source for CloudFront:
 
     #. Update the source options to the newest template, inheriting the existing values.
     #. Set ``path`` to "/" and ``endpointType`` to "elb" to restrict the source to discovering ELBs and related certs only.
     #. Create a new source (and destination) for the same accountNumber with ``path`` as "/cloudfront/" and ``endpointType`` as "cloudfront"
@@ -408,13 +438,13 @@
 
         cloudfront_options = deepcopy(new_options)
         set_plugin_option("path", "/cloudfront/", cloudfront_options)
         set_plugin_option("endpointType", "cloudfront", cloudfront_options)
         source_service.create(cloudfront_label, source.plugin_name, cloudfront_options,
                               f"CloudFront certificates and distributions for {source_label}")
 
-        print(f"[+] Limited source {source_label} to discover ELBs and ELB certificates.\n")
-        print(f"[+] Created source {cloudfront_label} to discover CloudFront distributions and certificates.\n")
+        click.echo(f"[+] Limited source {source_label} to discover ELBs and ELB certificates.\n")
+        click.echo(f"[+] Created source {cloudfront_label} to discover CloudFront distributions and certificates.\n")
 
     except ValidationError as e:
-        print(f"[+] Error: {str(e)}")
+        click.echo(f"[+] Error: {str(e)}")
         sys.exit(1)
```

### Comparing `lemur-1.4.0/lemur/sources/models.py` & `lemur-1.5.0/lemur/sources/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,21 +4,21 @@
     :copyright: (c) 2018 by Netflix Inc., see AUTHORS for more
     :license: Apache, see LICENSE for more details.
 .. moduleauthor:: Kevin Glisson <kglisson@netflix.com>
 """
 from sqlalchemy.orm import relationship
 from sqlalchemy import Column, Integer, String, Text, Boolean
 from sqlalchemy_utils import JSONType
-from lemur.database import db
+from lemur.database import BaseModel
 
 from lemur.plugins.base import plugins
 from sqlalchemy_utils import ArrowType
 
 
-class Source(db.Model):
+class Source(BaseModel):
     __tablename__ = "sources"
     id = Column(Integer, primary_key=True)
     label = Column(String(32), unique=True)
     options = Column(JSONType)
     description = Column(Text())
     plugin_name = Column(String(32))
     active = Column(Boolean, default=True)
```

### Comparing `lemur-1.4.0/lemur/sources/schemas.py` & `lemur-1.5.0/lemur/sources/schemas.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/sources/service.py` & `lemur-1.5.0/lemur/sources/service.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/sources/views.py` & `lemur-1.5.0/lemur/sources/views.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/404.html` & `lemur-1.5.0/lemur/static/app/404.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/api_keys/api_key/api_key.js` & `lemur-1.5.0/lemur/static/app/angular/api_keys/api_key/api_key.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/api_keys/api_key/api_key.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/api_keys/api_key/api_key.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/api_keys/services.js` & `lemur-1.5.0/lemur/static/app/angular/api_keys/services.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/api_keys/view/view.js` & `lemur-1.5.0/lemur/static/app/angular/api_keys/view/view.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/api_keys/view/view.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/api_keys/view/view.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/app.js` & `lemur-1.5.0/lemur/static/app/angular/app.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/authentication/login/login.js` & `lemur-1.5.0/lemur/static/app/angular/authentication/login/login.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/authentication/login/login.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/authentication/login/login.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/authentication/services.js` & `lemur-1.5.0/lemur/static/app/angular/authentication/services.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/authorities/authority/authority.js` & `lemur-1.5.0/lemur/static/app/angular/authorities/authority/authority.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/authorities/authority/authorityWizard.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/authorities/authority/authorityWizard.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/authorities/authority/distinguishedName.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/authorities/authority/distinguishedName.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/authorities/authority/edit.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/authorities/authority/edit.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/authorities/authority/extensions.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/authorities/authority/extensions.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/authorities/authority/options.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/authorities/authority/options.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/authorities/authority/permissions.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/authorities/authority/permissions.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/authorities/authority/tracking.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/authorities/authority/tracking.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/authorities/services.js` & `lemur-1.5.0/lemur/static/app/angular/authorities/services.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/authorities/view/view.js` & `lemur-1.5.0/lemur/static/app/angular/authorities/view/view.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/authorities/view/view.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/authorities/view/view.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/certificates/certificate/certificate.js` & `lemur-1.5.0/lemur/static/app/angular/certificates/certificate/certificate.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/certificates/certificate/certificateWizard.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/certificates/certificate/certificateWizard.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/certificates/certificate/destinations.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/certificates/certificate/destinations.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/certificates/certificate/distinguishedName.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/certificates/certificate/distinguishedName.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/certificates/certificate/edit.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/certificates/certificate/edit.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/certificates/certificate/export.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/certificates/certificate/export.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/certificates/certificate/notifications.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/certificates/certificate/notifications.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/certificates/certificate/options.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/certificates/certificate/options.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/certificates/certificate/replaces.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/certificates/certificate/replaces.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/certificates/certificate/revoke.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/certificates/certificate/revoke.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/certificates/certificate/tracking.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/certificates/certificate/tracking.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/certificates/certificate/upload.js` & `lemur-1.5.0/lemur/static/app/angular/certificates/certificate/upload.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/certificates/certificate/upload.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/certificates/certificate/upload.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/certificates/services.js` & `lemur-1.5.0/lemur/static/app/angular/certificates/services.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/certificates/view/view.js` & `lemur-1.5.0/lemur/static/app/angular/certificates/view/view.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/certificates/view/view.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/certificates/view/view.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/dashboard/dashboard.js` & `lemur-1.5.0/lemur/static/app/angular/dashboard/dashboard.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/dashboard/dashboard.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/dashboard/dashboard.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/destinations/destination/destination.js` & `lemur-1.5.0/lemur/static/app/angular/destinations/destination/destination.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/destinations/destination/destination.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/destinations/destination/destination.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/destinations/services.js` & `lemur-1.5.0/lemur/static/app/angular/destinations/services.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/destinations/view/view.js` & `lemur-1.5.0/lemur/static/app/angular/destinations/view/view.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/destinations/view/view.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/destinations/view/view.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/dns_providers/dns_provider/dns_provider.js` & `lemur-1.5.0/lemur/static/app/angular/dns_providers/dns_provider/dns_provider.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/dns_providers/dns_provider/dns_provider.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/dns_providers/dns_provider/dns_provider.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/dns_providers/services.js` & `lemur-1.5.0/lemur/static/app/angular/dns_providers/services.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/dns_providers/view/view.js` & `lemur-1.5.0/lemur/static/app/angular/dns_providers/view/view.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/dns_providers/view/view.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/dns_providers/view/view.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/domains/domain/domain.js` & `lemur-1.5.0/lemur/static/app/angular/domains/domain/domain.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/domains/domain/domain.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/domains/domain/domain.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/domains/services.js` & `lemur-1.5.0/lemur/static/app/angular/domains/services.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/domains/view/view.js` & `lemur-1.5.0/lemur/static/app/angular/domains/view/view.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/domains/view/view.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/domains/view/view.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/endpoints/services.js` & `lemur-1.5.0/lemur/static/app/angular/endpoints/services.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/endpoints/view/view.js` & `lemur-1.5.0/lemur/static/app/angular/endpoints/view/view.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/endpoints/view/view.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/endpoints/view/view.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/logs/view/view.js` & `lemur-1.5.0/lemur/static/app/angular/logs/view/view.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/logs/view/view.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/logs/view/view.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/notifications/notification/notification.js` & `lemur-1.5.0/lemur/static/app/angular/notifications/notification/notification.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/notifications/notification/notification.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/notifications/notification/notification.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/notifications/services.js` & `lemur-1.5.0/lemur/static/app/angular/notifications/services.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/notifications/view/view.js` & `lemur-1.5.0/lemur/static/app/angular/notifications/view/view.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/notifications/view/view.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/notifications/view/view.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/pager.html` & `lemur-1.5.0/lemur/static/app/angular/pager.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/pending_certificates/pending_certificate/cancel.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/pending_certificates/pending_certificate/cancel.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/pending_certificates/pending_certificate/destinations.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/pending_certificates/pending_certificate/destinations.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/pending_certificates/pending_certificate/edit.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/pending_certificates/pending_certificate/edit.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/pending_certificates/pending_certificate/notifications.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/pending_certificates/pending_certificate/notifications.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/pending_certificates/pending_certificate/pending_certificate.js` & `lemur-1.5.0/lemur/static/app/angular/pending_certificates/pending_certificate/pending_certificate.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/pending_certificates/pending_certificate/replaces.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/pending_certificates/pending_certificate/replaces.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/pending_certificates/pending_certificate/upload.js` & `lemur-1.5.0/lemur/static/app/angular/pending_certificates/pending_certificate/upload.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/pending_certificates/pending_certificate/upload.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/pending_certificates/pending_certificate/upload.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/pending_certificates/services.js` & `lemur-1.5.0/lemur/static/app/angular/pending_certificates/services.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/pending_certificates/view/view.js` & `lemur-1.5.0/lemur/static/app/angular/pending_certificates/view/view.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/pending_certificates/view/view.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/pending_certificates/view/view.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/plugins/services.js` & `lemur-1.5.0/lemur/static/app/angular/plugins/services.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/roles/role/role.js` & `lemur-1.5.0/lemur/static/app/angular/roles/role/role.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/roles/role/role.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/roles/role/role.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/roles/role/roleSelect.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/roles/role/roleSelect.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/roles/services.js` & `lemur-1.5.0/lemur/static/app/angular/roles/services.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/roles/view/view.js` & `lemur-1.5.0/lemur/static/app/angular/roles/view/view.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/roles/view/view.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/roles/view/view.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/sources/services.js` & `lemur-1.5.0/lemur/static/app/angular/sources/services.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/sources/source/source.js` & `lemur-1.5.0/lemur/static/app/angular/sources/source/source.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/sources/source/source.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/sources/source/source.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/sources/view/view.js` & `lemur-1.5.0/lemur/static/app/angular/sources/view/view.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/sources/view/view.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/sources/view/view.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/users/services.js` & `lemur-1.5.0/lemur/static/app/angular/users/services.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/users/user/user.js` & `lemur-1.5.0/lemur/static/app/angular/users/user/user.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/users/user/user.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/users/user/user.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/users/view/view.js` & `lemur-1.5.0/lemur/static/app/angular/users/view/view.js`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/users/view/view.tpl.html` & `lemur-1.5.0/lemur/static/app/angular/users/view/view.tpl.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/welcome/welcome.html` & `lemur-1.5.0/lemur/static/app/angular/welcome/welcome.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/angular/wizard.html` & `lemur-1.5.0/lemur/static/app/angular/wizard.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/favicon.ico` & `lemur-1.5.0/lemur/static/app/favicon.ico`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/index.html` & `lemur-1.5.0/lemur/static/app/index.html`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/static/app/styles/lemur.css` & `lemur-1.5.0/lemur/static/app/styles/lemur.css`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/conf.py` & `lemur-1.5.0/lemur/tests/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,16 @@
 import string
 
 _basedir = os.path.abspath(os.path.dirname(__file__))
 
 
 # generate random secrets for unittest
 def get_random_secret(length):
-    secret_key = ''.join(secrets.choice(string.ascii_uppercase) for x in range(round(length / 4)))
-    secret_key = secret_key + ''.join(secrets.choice("~!@#$%^&*()_+") for x in range(round(length / 4)))
-    secret_key = secret_key + ''.join(secrets.choice(string.ascii_lowercase) for x in range(round(length / 4)))
-    return secret_key + ''.join(secrets.choice(string.digits) for x in range(round(length / 4)))
+    chars = string.ascii_uppercase + string.ascii_lowercase + string.digits + "~!@#$%^&*()_+"
+    return ''.join(secrets.choice(chars) for x in range(length))
 
 
 THREADS_PER_PAGE = 8
 
 # General
 
 # These will need to be set to `True` if you are developing locally
```

### Comparing `lemur-1.4.0/lemur/tests/conftest.py` & `lemur-1.5.0/lemur/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/factories.py` & `lemur-1.5.0/lemur/tests/factories.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 from datetime import date
+from typing import List
 
 from factory import Sequence, post_generation, SubFactory
 from factory.alchemy import SQLAlchemyModelFactory
 from factory.fuzzy import FuzzyChoice, FuzzyText, FuzzyDate, FuzzyInteger
 
 from lemur.database import db
 from lemur.authorities.models import Authority
@@ -262,15 +263,15 @@
 class UserFactory(BaseFactory):
     """User Factory."""
 
     username = Sequence(lambda n: "user{0}".format(n))
     email = Sequence(lambda n: "user{0}@example.com".format(n))
     active = True
     password = FuzzyText(length=24)
-    certificates = []
+    certificates: List[Certificate] = []
 
     class Meta:
         """Factory Configuration."""
 
         model = User
 
     @post_generation
@@ -278,15 +279,15 @@
         if not create:
             return
 
         if extracted:
             for role in extracted:
                 self.roles.append(role)
 
-    @post_generation
+    @post_generation  # type: ignore
     def certificates(self, create, extracted, **kwargs):
         if not create:
             return
 
         if extracted:
             for cert in extracted:
                 self.certificates.append(cert)
```

### Comparing `lemur-1.4.0/lemur/tests/plugins/issuer_plugin.py` & `lemur-1.5.0/lemur/tests/plugins/issuer_plugin.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_api_keys.py` & `lemur-1.5.0/lemur/tests/test_api_keys.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_authorities.py` & `lemur-1.5.0/lemur/tests/test_authorities.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_certificates.py` & `lemur-1.5.0/lemur/tests/test_certificates.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_defaults.py` & `lemur-1.5.0/lemur/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_destinations.py` & `lemur-1.5.0/lemur/tests/test_destinations.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_dns_providers.py` & `lemur-1.5.0/lemur/tests/test_dns_providers.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_domains.py` & `lemur-1.5.0/lemur/tests/test_domains.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_endpoints.py` & `lemur-1.5.0/lemur/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_issuer_manager.py` & `lemur-1.5.0/lemur/tests/test_issuer_manager.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_ldap.py` & `lemur-1.5.0/lemur/tests/test_ldap.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_logs.py` & `lemur-1.5.0/lemur/tests/test_logs.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_messaging.py` & `lemur-1.5.0/lemur/tests/test_messaging.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_missing.py` & `lemur-1.5.0/lemur/tests/test_missing.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_notifications.py` & `lemur-1.5.0/lemur/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_oauth.py` & `lemur-1.5.0/lemur/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_pending_certificates.py` & `lemur-1.5.0/lemur/tests/test_pending_certificates.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_roles.py` & `lemur-1.5.0/lemur/tests/test_roles.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_schemas.py` & `lemur-1.5.0/lemur/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_sources.py` & `lemur-1.5.0/lemur/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_users.py` & `lemur-1.5.0/lemur/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_utils.py` & `lemur-1.5.0/lemur/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,20 +119,20 @@
     assert (get_key_type_from_certificate(ECDSA_SECP384r1_CERT_STR) == "ECCSECP384R1")
 
 
 def test_convert_pkcs7_bytes_to_pem():
     from lemur.common.utils import convert_pkcs7_bytes_to_pem
     from lemur.common.utils import parse_certificate
     cert_chain = convert_pkcs7_bytes_to_pem(CERT_CHAIN_PKCS7_PEM)
-    assert(len(cert_chain) == 3)
+    assert (len(cert_chain) == 3)
 
     leaf = cert_chain[1]
     root = cert_chain[2]
 
-    assert(parse_certificate("\n".join(str(root).splitlines())) == ROOTCA_CERT)
+    assert (parse_certificate("\n".join(str(root).splitlines())) == ROOTCA_CERT)
     assert (parse_certificate("\n".join(str(leaf).splitlines())) == INTERMEDIATE_CERT)
 
 
 def test_encryption(client):
     from lemur.common.utils import data_encrypt, data_decrypt
     plaintext = "encrypt this string"
     assert (data_decrypt(data_encrypt(plaintext)) == plaintext)
```

### Comparing `lemur-1.4.0/lemur/tests/test_validators.py` & `lemur-1.5.0/lemur/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/test_verify.py` & `lemur-1.5.0/lemur/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/tests/vectors.py` & `lemur-1.5.0/lemur/tests/vectors.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/users/models.py` & `lemur-1.5.0/lemur/users/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 """
 from sqlalchemy.orm import relationship
 from sqlalchemy import Integer, String, Column, Boolean
 from sqlalchemy.event import listen
 
 from sqlalchemy_utils.types.arrow import ArrowType
 
-from lemur.database import db
+from lemur.database import BaseModel, db
 from lemur.models import roles_users
 
 from lemur.extensions import bcrypt
 
 
 def hash_password(mapper, connect, target):
     """
@@ -28,15 +28,15 @@
     :param mapper:
     :param connect:
     :param target:
     """
     target.hash_password()
 
 
-class User(db.Model):
+class User(BaseModel):
     __tablename__ = "users"
     id = Column(Integer, primary_key=True)
     password = Column(String(128))
     active = Column(Boolean())
     confirmed_at = Column(ArrowType())
     username = Column(String(255), nullable=False, unique=True)
     email = Column(String(128), unique=True)
```

### Comparing `lemur-1.4.0/lemur/users/schemas.py` & `lemur-1.5.0/lemur/users/schemas.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/users/service.py` & `lemur-1.5.0/lemur/users/service.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/users/views.py` & `lemur-1.5.0/lemur/users/views.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur/utils.py` & `lemur-1.5.0/lemur/utils.py`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur.egg-info/PKG-INFO` & `lemur-1.5.0/lemur.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemur
-Version: 1.4.0
+Version: 1.5.0
 Summary: Certificate management and orchestration service
 Home-page: https://github.com/Netflix/lemur
 Author: The Lemur developers
 Author-email: security@netflix.com
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

### Comparing `lemur-1.4.0/lemur.egg-info/SOURCES.txt` & `lemur-1.5.0/lemur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur.egg-info/entry_points.txt` & `lemur-1.5.0/lemur.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/lemur.egg-info/requires.txt` & `lemur-1.5.0/lemur.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,409 +1,426 @@
-acme==2.4.0
-alembic==1.7.7
-alembic-autogenerate-enums==0.0.2
-amqp==5.1.0
+acme==2.6.0
+alembic==1.11.1
+alembic-autogenerate-enums==0.1.1
+amqp==5.1.1
 aniso8601==9.0.1
 arrow==1.2.3
-async-timeout==4.0.2
 asyncpool==1.0
-attrs==21.4.0
-bcrypt==3.2.0
-beautifulsoup4==4.10.0
-billiard==3.6.4.0
-blinker==1.4
-boto3==1.26.94
-botocore==1.29.100
-celery[redis]==5.2.7
-certbot==2.4.0
-certifi==2022.12.7
+attrs==23.1.0
+bcrypt==4.0.1
+beautifulsoup4==4.12.2
+billiard==4.1.0
+blinker==1.6.2
+boto3==1.26.165
+botocore==1.29.165
+celery[redis]==5.3.1
+certbot==2.6.0
+certifi==2023.5.7
 certsrv==2.1.1
-cffi==1.15.0
-charset-normalizer==2.0.12
-click==8.1.0
+cffi==1.15.1
+charset-normalizer==3.1.0
+click==8.1.3
 click-didyoumean==0.3.0
 click-plugins==1.1.1
-click-repl==0.2.0
-cloudflare==2.11.1
+click-repl==0.3.0
+cloudflare==2.11.6
 configargparse==1.5.3
-configobj==5.0.6
-cryptography==39.0.2
+configobj==5.0.8
+cryptography==41.0.1
 decorator==5.1.1
-distro==1.7.0
+distro==1.8.0
 dnspython==1.15.0
 dnspython3==1.15.0
 dyn==1.8.6
-flask==1.1.2
+flask==2.3.2
 flask-bcrypt==1.0.1
-flask-cors==3.0.10
+flask-cors==4.0.0
 flask-mail==0.9.1
-flask-migrate==2.7.0
+flask-migrate==4.0.4
 flask-principal==0.4.0
 flask-replicated==2.1
-flask-restful==0.3.9
-flask-script==2.0.6
+flask-restful==0.3.10
 flask-sqlalchemy==2.5.1
 future==0.18.3
 gunicorn==20.1.0
-hvac==1.1.0
-idna==3.3
+hvac==1.1.1
+idna==3.4
 inflection==0.5.1
-itsdangerous==2.0.1
+itsdangerous==2.1.2
 javaobj-py3==0.4.3
-jinja2==3.0.3
-jmespath==1.0.0
+jinja2==3.1.2
+jmespath==1.0.1
 josepy==1.13.0
-jsonlines==3.0.0
-kombu==5.2.4
+jsonlines==3.1.0
+kombu==5.3.1
 lockfile==0.12.2
 logmatic-python==0.1.7
-mako==1.2.2
-markupsafe==2.1.1
+mako==1.2.4
+markupsafe==2.1.3
 marshmallow==2.21.0
 marshmallow-sqlalchemy==0.23.1
 ndg-httpsclient==0.5.1
-paramiko==3.1.0
+paramiko==3.2.0
 parsedatetime==2.6
-pem==21.2.0
-prompt-toolkit==3.0.28
-psycopg2==2.9.5
-pyasn1==0.4.8
-pyasn1-modules==0.2.8
+pem==23.1.0
+prompt-toolkit==3.0.38
+psycopg2==2.9.6
+pyasn1==0.5.0
+pyasn1-modules==0.3.0
 pycparser==2.21
-pycryptodomex==3.14.1
+pycryptodomex==3.18.0
 pyhcl==0.4.4
 pyjks==20.0.0
-pyjwt==2.6.0
+pyjwt==2.7.0
 pynacl==1.5.0
-pyopenssl==23.1.0
+pyopenssl==23.2.0
 pyrfc3339==1.1
 python-dateutil==2.8.2
-python-json-logger==2.0.2
+python-json-logger==2.0.7
 python-ldap==3.4.3
-pytz==2022.1
+pytz==2023.3
 pyyaml==6.0
-redis==4.5.4
-requests==2.28.2
+redis==4.6.0
+requests==2.31.0
 retrying==1.3.4
-s3transfer==0.6.0
-sentry-sdk==1.9.0
+s3transfer==0.6.1
+sentry-sdk==1.26.0
 six==1.16.0
-soupsieve==2.3.1
+soupsieve==2.4.1
 sqlalchemy==1.3.24
-sqlalchemy-utils==0.40.0
+sqlalchemy-utils==0.41.1
 tabulate==0.9.0
 twofish==0.3.0
-urllib3==1.26.9
+typing-extensions==4.6.3
+tzdata==2023.3
+urllib3==1.26.16
 validators==0.20.0
 vine==5.0.0
-wcwidth==0.2.5
-werkzeug==2.0.3
+wcwidth==0.2.6
+werkzeug==2.3.6
 xmltodict==0.13.0
 
 [dev]
-bleach==4.1.0
-certifi==2022.12.7
-cffi==1.15.0
+bleach==6.0.0
+certifi==2023.5.7
 cfgv==3.3.1
-charset-normalizer==2.0.12
-commonmark==0.9.1
-cryptography==39.0.2
-distlib==0.3.4
-docutils==0.18.1
-filelock==3.6.0
-flake8==4.0.1
-identify==2.4.12
-idna==3.3
-importlib-metadata==4.11.3
-invoke==2.0.0
-jeepney==0.8.0
-keyring==23.5.0
+charset-normalizer==3.1.0
+distlib==0.3.6
+docutils==0.20.1
+filelock==3.12.2
+flake8==6.0.0
+identify==2.5.24
+idna==3.4
+importlib-metadata==6.7.0
+invoke==2.1.3
+jaraco-classes==3.2.3
+keyring==24.2.0
+markdown-it-py==3.0.0
 marshmallow==2.21.0
 marshmallow-sqlalchemy==0.23.1
-mccabe==0.6.1
-nodeenv==1.7.0
-packaging==21.3
-pkginfo==1.8.2
-platformdirs==2.5.1
-pre-commit==3.1.0
-pycodestyle==2.8.0
-pycparser==2.21
-pyflakes==2.4.0
-pygments==2.11.2
-pyparsing==3.0.7
+mccabe==0.7.0
+mdurl==0.1.2
+more-itertools==9.1.0
+nodeenv==1.8.0
+pkginfo==1.9.6
+platformdirs==3.8.0
+pre-commit==3.3.3
+pycodestyle==2.10.0
+pyflakes==3.0.1
+pygments==2.15.1
 pyyaml==6.0
-readme-renderer==35.0
-requests==2.28.2
-requests-toolbelt==0.9.1
+readme-renderer==40.0
+requests==2.31.0
+requests-toolbelt==1.0.0
 rfc3986==2.0.0
-rich==12.1.0
-secretstorage==3.3.1
+rich==13.4.2
 six==1.16.0
 sqlalchemy==1.3.24
 twine==4.0.2
-urllib3==1.26.9
-virtualenv==20.14.0
+urllib3==1.26.16
+virtualenv==20.23.1
 webencodings==0.5.1
-zipp==3.7.0
+zipp==3.15.0
 
 [docs]
-acme==2.4.0
-alabaster==0.7.12
-alembic==1.7.7
-amqp==5.1.0
+acme==2.6.0
+alabaster==0.7.13
+alembic==1.11.1
+amqp==5.1.1
 aniso8601==9.0.1
 arrow==1.2.3
-async-timeout==4.0.2
-attrs==21.4.0
-aws-sam-translator==1.44.0
-aws-xray-sdk==2.9.0
-babel==2.9.1
+attrs==23.1.0
+aws-sam-translator==1.70.0
+aws-xray-sdk==2.12.0
+babel==2.12.1
 bandit==1.7.5
-bcrypt==3.2.0
-beautifulsoup4==4.10.0
-billiard==3.6.4.0
-black==23.1.0
-blinker==1.4
-boto3==1.26.94
-botocore==1.29.100
-celery[redis]==5.2.7
-certbot==2.4.0
-certifi==2022.12.7
+bcrypt==4.0.1
+beautifulsoup4==4.12.2
+billiard==4.1.0
+black==23.3.0
+blinker==1.6.2
+boto3==1.26.165
+botocore==1.29.165
+celery[redis]==5.3.1
+certbot==2.6.0
+certifi==2023.5.7
 certsrv==2.1.1
-cffi==1.15.0
-cfn-lint==0.58.4
-charset-normalizer==2.0.12
-click==8.1.0
+cffi==1.15.1
+cfn-lint==0.77.10
+charset-normalizer==3.1.0
+click==8.1.3
 click-didyoumean==0.3.0
 click-plugins==1.1.1
-click-repl==0.2.0
-cloudflare==2.11.1
+click-repl==0.3.0
+cloudflare==2.11.6
 configargparse==1.5.3
-configobj==5.0.6
-coverage==6.5.0
-cryptography==39.0.2
-distro==1.7.0
+configobj==5.0.8
+coverage==7.2.7
+cryptography==41.0.1
+distro==1.8.0
 dnspython==1.15.0
 dnspython3==1.15.0
-docker==5.0.3
+docker==6.1.3
 docutils==0.18.1
 dyn==1.8.6
-ecdsa==0.17.0
+ecdsa==0.18.0
 factory-boy==3.2.1
-faker==17.6.0
-fakeredis==2.10.1
-flask==1.1.2
+faker==18.11.2
+fakeredis==2.15.0
+flask==2.3.2
 flask-bcrypt==1.0.1
-flask-cors==3.0.10
+flask-cors==4.0.0
 flask-mail==0.9.1
-flask-migrate==2.7.0
+flask-migrate==4.0.4
 flask-principal==0.4.0
 flask-replicated==2.1
-flask-restful==0.3.9
-flask-script==2.0.6
+flask-restful==0.3.10
 flask-sqlalchemy==2.5.1
 freezegun==1.2.2
-future==0.18.3
-gitdb==4.0.9
-gitpython==3.1.30
-graphql-core==3.2.0
+gitdb==4.0.10
+gitpython==3.1.31
+graphql-core==3.2.3
 gunicorn==20.1.0
-hvac==1.1.0
-idna==3.3
-imagesize==1.3.0
+hvac==1.1.1
+idna==3.4
+imagesize==1.4.1
 inflection==0.5.1
-iniconfig==1.1.1
-itsdangerous==2.0.1
+iniconfig==2.0.0
+itsdangerous==2.1.2
 javaobj-py3==0.4.3
-jinja2==3.0.3
-jmespath==1.0.0
+jinja2==3.1.2
+jmespath==1.0.1
 josepy==1.13.0
 jschema-to-python==1.2.3
-jsondiff==1.3.1
-jsonlines==3.0.0
-jsonpatch==1.32
-jsonpickle==2.1.0
-jsonpointer==2.2
-jsonschema==3.2.0
+jsondiff==2.0.0
+jsonlines==3.1.0
+jsonpatch==1.33
+jsonpickle==3.0.1
+jsonpointer==2.4
+jsonschema==4.17.3
+jsonschema-spec==0.1.6
 junit-xml==1.9
-kombu==5.2.4
+kombu==5.3.1
+lazy-object-proxy==1.9.0
 logmatic-python==0.1.7
-mako==1.2.2
-markdown-it-py==2.2.0
-markupsafe==2.1.1
+mako==1.2.4
+markdown-it-py==3.0.0
+markupsafe==2.1.3
 marshmallow==2.21.0
 marshmallow-sqlalchemy==0.23.1
 mdurl==0.1.2
-moto[all]==3.1.1
-mypy-extensions==0.4.3
-networkx==2.7.1
+moto[all]==4.1.12
+mpmath==1.3.0
+mypy-extensions==1.0.0
+networkx==3.1
 nose==1.3.7
-packaging==23.0
-paramiko==3.1.0
+openapi-schema-validator==0.4.4
+openapi-spec-validator==0.5.7
+packaging==23.1
+paramiko==3.2.0
 parsedatetime==2.6
-pathspec==0.9.0
-pbr==5.8.1
-pem==21.2.0
-platformdirs==2.5.1
-pluggy==1.0.0
-prompt-toolkit==3.0.28
-py==1.11.0
-pyasn1==0.4.8
-pyasn1-modules==0.2.8
+pathable==0.4.3
+pathspec==0.11.1
+pbr==5.11.1
+pem==23.1.0
+platformdirs==3.8.0
+pluggy==1.2.0
+prompt-toolkit==3.0.38
+py-partiql-parser==0.3.3
+pyasn1==0.5.0
+pyasn1-modules==0.3.0
 pycparser==2.21
-pycryptodomex==3.14.1
-pyflakes==2.4.0
-pygments==2.14.0
+pycryptodomex==3.18.0
+pydantic==1.10.9
+pyflakes==3.0.1
+pygments==2.15.1
 pyhcl==0.4.4
 pyjks==20.0.0
-pyjwt==2.6.0
+pyjwt==2.7.0
 pynacl==1.5.0
-pyopenssl==23.1.0
+pyopenssl==23.2.0
+pyparsing==3.1.0
 pyrfc3339==1.1
-pyrsistent==0.18.1
-pytest==7.1.3
+pyrsistent==0.19.3
+pytest==7.4.0
 pytest-flask==1.2.0
-pytest-mock==3.10.0
+pytest-mock==3.11.1
 python-dateutil==2.8.2
 python-jose[cryptography]==3.3.0
-python-json-logger==2.0.2
-pytz==2022.1
+python-json-logger==2.0.7
+pytz==2023.3
 pyyaml==6.0
-redis==4.5.4
-requests==2.28.2
-requests-mock==1.10.0
-responses==0.20.0
+redis==4.6.0
+regex==2023.6.3
+requests==2.31.0
+requests-mock==1.11.0
+responses==0.23.1
 retrying==1.3.4
-rich==13.3.2
-rsa==4.8
-s3transfer==0.6.0
+rfc3339-validator==0.1.4
+rich==13.4.2
+rsa==4.9
+s3transfer==0.6.1
 sarif-om==1.0.4
-sentry-sdk==1.9.0
+sentry-sdk==1.26.0
 six==1.16.0
 smmap==5.0.0
 snowballstemmer==2.2.0
 sortedcontainers==2.4.0
-soupsieve==2.3.1
-sphinx==6.1.3
-sphinx-rtd-theme==1.2.0
-sphinxcontrib-applehelp==1.0.2
+soupsieve==2.4.1
+sphinx==6.2.1
+sphinx-rtd-theme==1.2.2
+sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-httpdomain==1.8.1
-sphinxcontrib-jquery==2.0.0
+sphinxcontrib-jquery==4.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 sqlalchemy==1.3.24
-sqlalchemy-utils==0.40.0
+sqlalchemy-utils==0.41.1
 sshpubkeys==3.3.1
-stevedore==3.5.0
+stevedore==5.1.0
+sympy==1.12
 tabulate==0.9.0
-tomli==2.0.1
 twofish==0.3.0
-urllib3==1.26.9
+types-pyyaml==6.0.12.10
+typing-extensions==4.6.3
+tzdata==2023.3
+urllib3==1.26.16
 vine==5.0.0
-wcwidth==0.2.5
-websocket-client==1.3.1
-werkzeug==2.0.3
-wrapt==1.14.0
+wcwidth==0.2.6
+websocket-client==1.6.1
+werkzeug==2.3.6
+wrapt==1.15.0
 xmltodict==0.13.0
 
 [tests]
-acme==2.4.0
-alembic==1.7.7
-async-timeout==4.0.2
-attrs==21.4.0
-aws-sam-translator==1.44.0
-aws-xray-sdk==2.9.0
+acme==2.6.0
+alembic==1.11.1
+attrs==23.1.0
+aws-sam-translator==1.70.0
+aws-xray-sdk==2.12.0
 bandit==1.7.5
-black==23.1.0
-boto3==1.26.94
-botocore==1.29.100
-certbot==2.4.0
-certifi==2022.12.7
-cffi==1.15.0
-cfn-lint==0.58.4
-charset-normalizer==2.0.12
-click==8.1.0
+black==23.3.0
+blinker==1.6.2
+boto3==1.26.165
+botocore==1.29.165
+certbot==2.6.0
+certifi==2023.5.7
+cffi==1.15.1
+cfn-lint==0.77.10
+charset-normalizer==3.1.0
+click==8.1.3
 configargparse==1.5.3
-configobj==5.0.6
-coverage==6.5.0
-cryptography==39.0.2
-distro==1.7.0
-docker==5.0.3
-ecdsa==0.17.0
+configobj==5.0.8
+coverage==7.2.7
+cryptography==41.0.1
+distro==1.8.0
+docker==6.1.3
+ecdsa==0.18.0
 factory-boy==3.2.1
-faker==17.6.0
-fakeredis==2.10.1
-flask==1.1.2
-flask-migrate==2.7.0
+faker==18.11.2
+fakeredis==2.15.0
+flask==2.3.2
+flask-migrate==4.0.4
 flask-sqlalchemy==2.5.1
 freezegun==1.2.2
-future==0.18.3
-gitdb==4.0.9
-gitpython==3.1.30
-graphql-core==3.2.0
-idna==3.3
-iniconfig==1.1.1
-itsdangerous==2.0.1
-jinja2==3.0.3
-jmespath==1.0.0
+gitdb==4.0.10
+gitpython==3.1.31
+graphql-core==3.2.3
+idna==3.4
+iniconfig==2.0.0
+itsdangerous==2.1.2
+jinja2==3.1.2
+jmespath==1.0.1
 josepy==1.13.0
 jschema-to-python==1.2.3
-jsondiff==1.3.1
-jsonpatch==1.32
-jsonpickle==2.1.0
-jsonpointer==2.2
-jsonschema==3.2.0
+jsondiff==2.0.0
+jsonpatch==1.33
+jsonpickle==3.0.1
+jsonpointer==2.4
+jsonschema==4.17.3
+jsonschema-spec==0.1.6
 junit-xml==1.9
-mako==1.2.2
-markdown-it-py==2.2.0
-markupsafe==2.1.1
+lazy-object-proxy==1.9.0
+mako==1.2.4
+markdown-it-py==3.0.0
+markupsafe==2.1.3
 marshmallow==2.21.0
 marshmallow-sqlalchemy==0.23.1
 mdurl==0.1.2
-moto[all]==3.1.1
-mypy-extensions==0.4.3
-networkx==2.7.1
+moto[all]==4.1.12
+mpmath==1.3.0
+mypy-extensions==1.0.0
+networkx==3.1
 nose==1.3.7
-packaging==23.0
+openapi-schema-validator==0.4.4
+openapi-spec-validator==0.5.7
+packaging==23.1
 parsedatetime==2.6
-pathspec==0.9.0
-pbr==5.8.1
-platformdirs==2.5.1
-pluggy==1.0.0
-py==1.11.0
-pyasn1==0.4.8
+pathable==0.4.3
+pathspec==0.11.1
+pbr==5.11.1
+platformdirs==3.8.0
+pluggy==1.2.0
+py-partiql-parser==0.3.3
+pyasn1==0.5.0
 pycparser==2.21
-pyflakes==2.4.0
-pygments==2.14.0
-pyopenssl==23.1.0
+pydantic==1.10.9
+pyflakes==3.0.1
+pygments==2.15.1
+pyopenssl==23.2.0
+pyparsing==3.1.0
 pyrfc3339==1.1
-pyrsistent==0.18.1
-pytest==7.1.3
+pyrsistent==0.19.3
+pytest==7.4.0
 pytest-flask==1.2.0
-pytest-mock==3.10.0
+pytest-mock==3.11.1
 python-dateutil==2.8.2
 python-jose[cryptography]==3.3.0
-pytz==2022.1
+pytz==2023.3
 pyyaml==6.0
-redis==4.5.4
-requests==2.28.2
-requests-mock==1.10.0
-responses==0.20.0
-rich==13.3.2
-rsa==4.8
-s3transfer==0.6.0
+redis==4.6.0
+regex==2023.6.3
+requests==2.31.0
+requests-mock==1.11.0
+responses==0.23.1
+rfc3339-validator==0.1.4
+rich==13.4.2
+rsa==4.9
+s3transfer==0.6.1
 sarif-om==1.0.4
 six==1.16.0
 smmap==5.0.0
 sortedcontainers==2.4.0
 sqlalchemy==1.3.24
 sshpubkeys==3.3.1
-stevedore==3.5.0
-tomli==2.0.1
-urllib3==1.26.9
-websocket-client==1.3.1
-werkzeug==2.0.3
-wrapt==1.14.0
+stevedore==5.1.0
+sympy==1.12
+types-pyyaml==6.0.12.10
+typing-extensions==4.6.3
+urllib3==1.26.16
+websocket-client==1.6.1
+werkzeug==2.3.6
+wrapt==1.15.0
 xmltodict==0.13.0
```

### Comparing `lemur-1.4.0/package.json` & `lemur-1.5.0/package.json`

 * *Files identical despite different names*

### Comparing `lemur-1.4.0/requirements-dev.txt` & `lemur-1.5.0/requirements-dev.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,114 +1,106 @@
 #
-# This file is autogenerated by pip-compile with python 3.9
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.9
+# by the following command:
 #
-#    pip-compile --no-emit-index-url --output-file=requirements-dev.txt requirements-dev.in
+#    pip-compile --no-emit-index-url --output-file=requirements-dev.txt --resolver=backtracking requirements-dev.in
 #
-bleach==4.1.0
+bleach==6.0.0
     # via readme-renderer
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
-cffi==1.15.0
-    # via cryptography
 cfgv==3.3.1
     # via pre-commit
-charset-normalizer==2.0.12
+charset-normalizer==3.1.0
     # via requests
-commonmark==0.9.1
-    # via rich
-cryptography==39.0.2
-    # via secretstorage
-distlib==0.3.4
+distlib==0.3.6
     # via virtualenv
-docutils==0.18.1
+docutils==0.20.1
     # via readme-renderer
-filelock==3.6.0
+filelock==3.12.2
     # via virtualenv
-flake8==4.0.1
+flake8==6.0.0
     # via -r requirements-dev.in
-identify==2.4.12
+identify==2.5.24
     # via pre-commit
-idna==3.3
+idna==3.4
     # via requests
-importlib-metadata==4.11.3
+importlib-metadata==6.7.0
     # via
     #   keyring
     #   twine
-invoke==2.0.0
+invoke==2.1.3
     # via -r requirements-dev.in
-jeepney==0.8.0
-    # via
-    #   keyring
-    #   secretstorage
-keyring==23.5.0
+jaraco-classes==3.2.3
+    # via keyring
+keyring==24.2.0
     # via twine
+markdown-it-py==3.0.0
+    # via rich
 marshmallow==2.21.0
     # via
     #   -r requirements-dev.in
     #   marshmallow-sqlalchemy
 marshmallow-sqlalchemy==0.23.1
     # via -r requirements-dev.in
-mccabe==0.6.1
+mccabe==0.7.0
     # via flake8
-nodeenv==1.7.0
+mdurl==0.1.2
+    # via markdown-it-py
+more-itertools==9.1.0
+    # via jaraco-classes
+nodeenv==1.8.0
     # via
     #   -r requirements-dev.in
     #   pre-commit
-packaging==21.3
-    # via bleach
-pkginfo==1.8.2
+pkginfo==1.9.6
     # via twine
-platformdirs==2.5.1
+platformdirs==3.8.0
     # via virtualenv
-pre-commit==3.1.0
+pre-commit==3.3.3
     # via -r requirements-dev.in
-pycodestyle==2.8.0
+pycodestyle==2.10.0
     # via flake8
-pycparser==2.21
-    # via cffi
-pyflakes==2.4.0
+pyflakes==3.0.1
     # via flake8
-pygments==2.11.2
+pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
-pyparsing==3.0.7
-    # via packaging
 pyyaml==6.0
     # via
     #   -r requirements-dev.in
     #   pre-commit
-readme-renderer==35.0
+readme-renderer==40.0
     # via twine
-requests==2.28.2
+requests==2.31.0
     # via
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.9.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==12.1.0
+rich==13.4.2
     # via twine
-secretstorage==3.3.1
-    # via keyring
 six==1.16.0
-    # via
-    #   bleach
-    #   virtualenv
+    # via bleach
 sqlalchemy==1.3.24
     # via
     #   -r requirements-dev.in
     #   marshmallow-sqlalchemy
 twine==4.0.2
     # via -r requirements-dev.in
-urllib3==1.26.9
+urllib3==1.26.16
     # via
+    #   -r requirements-dev.in
     #   requests
     #   twine
-virtualenv==20.14.0
+virtualenv==20.23.1
     # via pre-commit
 webencodings==0.5.1
     # via bleach
-zipp==3.7.0
+zipp==3.15.0
     # via importlib-metadata
+
+# The following packages are considered to be unsafe in a requirements file:
+# setuptools
```

### Comparing `lemur-1.4.0/requirements-docs.txt` & `lemur-1.5.0/requirements-docs.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,560 +1,591 @@
 #
-# This file is autogenerated by pip-compile with python 3.9
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.9
+# by the following command:
 #
-#    pip-compile --no-emit-index-url --output-file=requirements-docs.txt requirements-docs.in
+#    pip-compile --no-emit-index-url --output-file=requirements-docs.txt --resolver=backtracking requirements-docs.in
 #
-acme==2.4.0
+acme==2.6.0
     # via
     #   -r requirements-docs.in
     #   -r requirements-tests.txt
     #   certbot
-alabaster==0.7.12
+alabaster==0.7.13
     # via sphinx
-alembic==1.7.7
+alembic==1.11.1
     # via
     #   -r requirements-tests.txt
     #   flask-migrate
-amqp==5.1.0
+amqp==5.1.1
     # via kombu
 aniso8601==9.0.1
     # via flask-restful
 arrow==1.2.3
     # via -r requirements-docs.in
-async-timeout==4.0.2
-    # via
-    #   -r requirements-tests.txt
-    #   redis
-attrs==21.4.0
+attrs==23.1.0
     # via
     #   -r requirements-tests.txt
     #   jschema-to-python
     #   jsonlines
     #   jsonschema
-    #   pytest
     #   sarif-om
-aws-sam-translator==1.44.0
+aws-sam-translator==1.70.0
     # via
     #   -r requirements-tests.txt
     #   cfn-lint
-aws-xray-sdk==2.9.0
+aws-xray-sdk==2.12.0
     # via
     #   -r requirements-tests.txt
     #   moto
-babel==2.9.1
+babel==2.12.1
     # via sphinx
 bandit==1.7.5
     # via -r requirements-tests.txt
-bcrypt==3.2.0
+bcrypt==4.0.1
     # via
     #   flask-bcrypt
     #   paramiko
-beautifulsoup4==4.10.0
+beautifulsoup4==4.12.2
     # via cloudflare
-billiard==3.6.4.0
+billiard==4.1.0
     # via celery
-black==23.1.0
+black==23.3.0
     # via -r requirements-tests.txt
-blinker==1.4
+blinker==1.6.2
     # via
+    #   -r requirements-tests.txt
+    #   flask
     #   flask-mail
     #   flask-principal
-boto3==1.26.94
+boto3==1.26.165
     # via
     #   -r requirements-docs.in
     #   -r requirements-tests.txt
     #   aws-sam-translator
     #   moto
-botocore==1.29.100
+botocore==1.29.165
     # via
     #   -r requirements-docs.in
     #   -r requirements-tests.txt
     #   aws-xray-sdk
     #   boto3
     #   moto
     #   s3transfer
-celery[redis]==5.2.7
+celery[redis]==5.3.1
     # via -r requirements-docs.in
-certbot==2.4.0
+certbot==2.6.0
     # via
     #   -r requirements-docs.in
     #   -r requirements-tests.txt
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   -r requirements-tests.txt
     #   requests
     #   sentry-sdk
 certsrv==2.1.1
     # via -r requirements-docs.in
-cffi==1.15.0
+cffi==1.15.1
     # via
     #   -r requirements-tests.txt
-    #   bcrypt
     #   cryptography
     #   pynacl
-cfn-lint==0.58.4
+cfn-lint==0.77.10
     # via
     #   -r requirements-tests.txt
     #   moto
-charset-normalizer==2.0.12
+charset-normalizer==3.1.0
     # via
     #   -r requirements-tests.txt
     #   requests
-click==8.1.0
+click==8.1.3
     # via
     #   -r requirements-tests.txt
     #   black
     #   celery
     #   click-didyoumean
     #   click-plugins
     #   click-repl
     #   flask
 click-didyoumean==0.3.0
     # via celery
 click-plugins==1.1.1
     # via celery
-click-repl==0.2.0
+click-repl==0.3.0
     # via celery
-cloudflare==2.11.1
+cloudflare==2.11.6
     # via -r requirements-docs.in
 configargparse==1.5.3
     # via
     #   -r requirements-tests.txt
     #   certbot
-configobj==5.0.6
+configobj==5.0.8
     # via
     #   -r requirements-tests.txt
     #   certbot
-coverage==6.5.0
+coverage==7.2.7
     # via -r requirements-tests.txt
-cryptography==39.0.2
+cryptography==41.0.1
     # via
     #   -r requirements-docs.in
     #   -r requirements-tests.txt
     #   acme
     #   certbot
     #   josepy
     #   moto
     #   paramiko
     #   pyopenssl
     #   python-jose
     #   sshpubkeys
-distro==1.7.0
+distro==1.8.0
     # via
     #   -r requirements-tests.txt
     #   certbot
 dnspython==1.15.0
     # via dnspython3
 dnspython3==1.15.0
     # via -r requirements-docs.in
-docker==5.0.3
+docker==6.1.3
     # via
     #   -r requirements-tests.txt
     #   moto
 docutils==0.18.1
     # via
+    #   -r requirements-docs.in
     #   sphinx
     #   sphinx-rtd-theme
 dyn==1.8.6
     # via -r requirements-docs.in
-ecdsa==0.17.0
+ecdsa==0.18.0
     # via
     #   -r requirements-tests.txt
     #   moto
     #   python-jose
     #   sshpubkeys
 factory-boy==3.2.1
     # via -r requirements-tests.txt
-faker==17.6.0
+faker==18.11.2
     # via
     #   -r requirements-tests.txt
     #   factory-boy
-fakeredis==2.10.1
+fakeredis==2.15.0
     # via -r requirements-tests.txt
-flask==1.1.2
+flask==2.3.2
     # via
     #   -r requirements-docs.in
     #   -r requirements-tests.txt
     #   flask-bcrypt
     #   flask-cors
     #   flask-mail
     #   flask-migrate
     #   flask-principal
     #   flask-restful
-    #   flask-script
     #   flask-sqlalchemy
     #   pytest-flask
 flask-bcrypt==1.0.1
     # via -r requirements-docs.in
-flask-cors==3.0.10
+flask-cors==4.0.0
     # via -r requirements-docs.in
 flask-mail==0.9.1
     # via -r requirements-docs.in
-flask-migrate==2.7.0
+flask-migrate==4.0.4
     # via
     #   -r requirements-docs.in
     #   -r requirements-tests.txt
 flask-principal==0.4.0
     # via -r requirements-docs.in
 flask-replicated==2.1
     # via -r requirements-docs.in
-flask-restful==0.3.9
-    # via -r requirements-docs.in
-flask-script==2.0.6
+flask-restful==0.3.10
     # via -r requirements-docs.in
 flask-sqlalchemy==2.5.1
     # via
     #   -r requirements-docs.in
     #   -r requirements-tests.txt
     #   flask-migrate
 freezegun==1.2.2
     # via -r requirements-tests.txt
-future==0.18.3
-    # via
-    #   -r requirements-tests.txt
-    #   aws-xray-sdk
-gitdb==4.0.9
+gitdb==4.0.10
     # via
     #   -r requirements-tests.txt
     #   gitpython
-gitpython==3.1.30
+gitpython==3.1.31
     # via
     #   -r requirements-tests.txt
     #   bandit
-graphql-core==3.2.0
+graphql-core==3.2.3
     # via
     #   -r requirements-tests.txt
     #   moto
 gunicorn==20.1.0
     # via -r requirements-docs.in
-hvac==1.1.0
+hvac==1.1.1
     # via -r requirements-docs.in
-idna==3.3
+idna==3.4
     # via
     #   -r requirements-tests.txt
-    #   moto
     #   requests
-imagesize==1.3.0
+imagesize==1.4.1
     # via sphinx
 inflection==0.5.1
     # via -r requirements-docs.in
-iniconfig==1.1.1
+iniconfig==2.0.0
     # via
     #   -r requirements-tests.txt
     #   pytest
-itsdangerous==2.0.1
+itsdangerous==2.1.2
     # via
     #   -r requirements-docs.in
     #   -r requirements-tests.txt
     #   flask
 javaobj-py3==0.4.3
     # via pyjks
-jinja2==3.0.3
+jinja2==3.1.2
     # via
     #   -r requirements-tests.txt
     #   flask
     #   moto
     #   sphinx
-jmespath==1.0.0
+jmespath==1.0.1
     # via
     #   -r requirements-tests.txt
     #   boto3
     #   botocore
 josepy==1.13.0
     # via
     #   -r requirements-docs.in
     #   -r requirements-tests.txt
     #   acme
     #   certbot
 jschema-to-python==1.2.3
     # via
     #   -r requirements-tests.txt
     #   cfn-lint
-jsondiff==1.3.1
+jsondiff==2.0.0
     # via
     #   -r requirements-tests.txt
     #   moto
-jsonlines==3.0.0
+jsonlines==3.1.0
     # via cloudflare
-jsonpatch==1.32
+jsonpatch==1.33
     # via
     #   -r requirements-tests.txt
     #   cfn-lint
-jsonpickle==2.1.0
+jsonpickle==3.0.1
     # via
     #   -r requirements-tests.txt
     #   jschema-to-python
-jsonpointer==2.2
+jsonpointer==2.4
     # via
     #   -r requirements-tests.txt
     #   jsonpatch
-jsonschema==3.2.0
+jsonschema==4.17.3
     # via
     #   -r requirements-tests.txt
     #   aws-sam-translator
     #   cfn-lint
+    #   jsonschema-spec
+    #   openapi-schema-validator
+    #   openapi-spec-validator
+jsonschema-spec==0.1.6
+    # via
+    #   -r requirements-tests.txt
+    #   openapi-spec-validator
 junit-xml==1.9
     # via
     #   -r requirements-tests.txt
     #   cfn-lint
-kombu==5.2.4
+kombu==5.3.1
     # via celery
+lazy-object-proxy==1.9.0
+    # via
+    #   -r requirements-tests.txt
+    #   openapi-spec-validator
 logmatic-python==0.1.7
     # via -r requirements-docs.in
-mako==1.2.2
+mako==1.2.4
     # via
     #   -r requirements-tests.txt
     #   alembic
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
     # via
     #   -r requirements-tests.txt
     #   rich
-markupsafe==2.1.1
+markupsafe==2.1.3
     # via
     #   -r requirements-tests.txt
     #   jinja2
     #   mako
-    #   moto
+    #   werkzeug
 marshmallow==2.21.0
     # via
     #   -r requirements-docs.in
     #   -r requirements-tests.txt
     #   marshmallow-sqlalchemy
 marshmallow-sqlalchemy==0.23.1
     # via
     #   -r requirements-docs.in
     #   -r requirements-tests.txt
 mdurl==0.1.2
     # via
     #   -r requirements-tests.txt
     #   markdown-it-py
-moto[all]==3.1.1
+moto[all]==4.1.12
     # via -r requirements-tests.txt
-mypy-extensions==0.4.3
+mpmath==1.3.0
+    # via
+    #   -r requirements-tests.txt
+    #   sympy
+mypy-extensions==1.0.0
     # via
     #   -r requirements-tests.txt
     #   black
-networkx==2.7.1
+networkx==3.1
     # via
     #   -r requirements-tests.txt
     #   cfn-lint
 nose==1.3.7
     # via -r requirements-tests.txt
-packaging==23.0
+openapi-schema-validator==0.4.4
+    # via
+    #   -r requirements-tests.txt
+    #   openapi-spec-validator
+openapi-spec-validator==0.5.7
+    # via
+    #   -r requirements-tests.txt
+    #   moto
+packaging==23.1
     # via
     #   -r requirements-tests.txt
     #   black
+    #   docker
     #   pytest
     #   sphinx
-paramiko==3.1.0
+paramiko==3.2.0
     # via -r requirements-docs.in
 parsedatetime==2.6
     # via
     #   -r requirements-tests.txt
     #   certbot
-pathspec==0.9.0
+pathable==0.4.3
+    # via
+    #   -r requirements-tests.txt
+    #   jsonschema-spec
+pathspec==0.11.1
     # via
     #   -r requirements-tests.txt
     #   black
-pbr==5.8.1
+pbr==5.11.1
     # via
     #   -r requirements-tests.txt
     #   jschema-to-python
     #   sarif-om
     #   stevedore
-pem==21.2.0
+pem==23.1.0
     # via -r requirements-docs.in
-platformdirs==2.5.1
+platformdirs==3.8.0
     # via
     #   -r requirements-tests.txt
     #   black
-pluggy==1.0.0
+pluggy==1.2.0
     # via
     #   -r requirements-tests.txt
     #   pytest
-prompt-toolkit==3.0.28
+prompt-toolkit==3.0.38
     # via click-repl
-py==1.11.0
+py-partiql-parser==0.3.3
     # via
     #   -r requirements-tests.txt
-    #   pytest
-pyasn1==0.4.8
+    #   moto
+pyasn1==0.5.0
     # via
     #   -r requirements-tests.txt
     #   pyasn1-modules
     #   pyjks
     #   python-jose
     #   rsa
-pyasn1-modules==0.2.8
+pyasn1-modules==0.3.0
     # via pyjks
 pycparser==2.21
     # via
     #   -r requirements-tests.txt
     #   cffi
-pycryptodomex==3.14.1
+pycryptodomex==3.18.0
     # via pyjks
-pyflakes==2.4.0
+pydantic==1.10.9
+    # via
+    #   -r requirements-tests.txt
+    #   aws-sam-translator
+pyflakes==3.0.1
     # via -r requirements-tests.txt
-pygments==2.14.0
+pygments==2.15.1
     # via
     #   -r requirements-tests.txt
     #   rich
     #   sphinx
 pyhcl==0.4.4
     # via hvac
 pyjks==20.0.0
     # via -r requirements-docs.in
-pyjwt==2.6.0
+pyjwt==2.7.0
     # via -r requirements-docs.in
 pynacl==1.5.0
     # via paramiko
-pyopenssl==23.1.0
+pyopenssl==23.2.0
     # via
     #   -r requirements-docs.in
     #   -r requirements-tests.txt
     #   acme
     #   josepy
+pyparsing==3.1.0
+    # via
+    #   -r requirements-tests.txt
+    #   moto
 pyrfc3339==1.1
     # via
     #   -r requirements-tests.txt
     #   acme
     #   certbot
-pyrsistent==0.18.1
+pyrsistent==0.19.3
     # via
     #   -r requirements-tests.txt
     #   jsonschema
-pytest==7.1.3
+pytest==7.4.0
     # via
     #   -r requirements-tests.txt
     #   pytest-flask
     #   pytest-mock
 pytest-flask==1.2.0
     # via -r requirements-tests.txt
-pytest-mock==3.10.0
+pytest-mock==3.11.1
     # via -r requirements-tests.txt
 python-dateutil==2.8.2
     # via
     #   -r requirements-tests.txt
     #   arrow
     #   botocore
+    #   celery
     #   faker
     #   freezegun
     #   moto
 python-jose[cryptography]==3.3.0
     # via
     #   -r requirements-tests.txt
     #   moto
-python-json-logger==2.0.2
+python-json-logger==2.0.7
     # via logmatic-python
-pytz==2022.1
+pytz==2023.3
     # via
     #   -r requirements-tests.txt
     #   acme
-    #   babel
-    #   celery
     #   certbot
     #   flask-restful
-    #   moto
     #   pyrfc3339
 pyyaml==6.0
     # via
     #   -r requirements-tests.txt
     #   bandit
     #   cfn-lint
     #   cloudflare
+    #   jsonschema-spec
     #   moto
-redis==4.5.4
+    #   responses
+redis==4.6.0
     # via
     #   -r requirements-docs.in
     #   -r requirements-tests.txt
     #   celery
     #   fakeredis
-requests==2.28.2
+regex==2023.6.3
+    # via
+    #   -r requirements-tests.txt
+    #   cfn-lint
+requests==2.31.0
     # via
     #   -r requirements-tests.txt
     #   acme
     #   certsrv
     #   cloudflare
     #   docker
     #   hvac
+    #   jsonschema-spec
     #   moto
     #   requests-mock
     #   responses
     #   sphinx
-requests-mock==1.10.0
+requests-mock==1.11.0
     # via -r requirements-tests.txt
-responses==0.20.0
+responses==0.23.1
     # via
     #   -r requirements-tests.txt
     #   moto
 retrying==1.3.4
     # via -r requirements-docs.in
-rich==13.3.2
+rfc3339-validator==0.1.4
+    # via
+    #   -r requirements-tests.txt
+    #   openapi-schema-validator
+rich==13.4.2
     # via
     #   -r requirements-tests.txt
     #   bandit
-rsa==4.8
+rsa==4.9
     # via
     #   -r requirements-tests.txt
     #   python-jose
-s3transfer==0.6.0
+s3transfer==0.6.1
     # via
     #   -r requirements-tests.txt
     #   boto3
 sarif-om==1.0.4
     # via
     #   -r requirements-tests.txt
     #   cfn-lint
-sentry-sdk==1.9.0
+sentry-sdk==1.26.0
     # via -r requirements-docs.in
 six==1.16.0
     # via
     #   -r requirements-tests.txt
-    #   bcrypt
-    #   cfn-lint
-    #   click-repl
     #   configobj
     #   ecdsa
-    #   flask-cors
     #   flask-restful
-    #   jsonschema
     #   junit-xml
     #   python-dateutil
     #   requests-mock
     #   retrying
+    #   rfc3339-validator
     #   sphinxcontrib-httpdomain
 smmap==5.0.0
     # via
     #   -r requirements-tests.txt
     #   gitdb
 snowballstemmer==2.2.0
     # via sphinx
 sortedcontainers==2.4.0
     # via
     #   -r requirements-tests.txt
     #   fakeredis
-soupsieve==2.3.1
+soupsieve==2.4.1
     # via beautifulsoup4
-sphinx==6.1.3
+sphinx==6.2.1
     # via
     #   -r requirements-docs.in
     #   sphinx-rtd-theme
     #   sphinxcontrib-httpdomain
-sphinx-rtd-theme==1.2.0
+    #   sphinxcontrib-jquery
+sphinx-rtd-theme==1.2.2
     # via -r requirements-docs.in
-sphinxcontrib-applehelp==1.0.2
+sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
 sphinxcontrib-httpdomain==1.8.1
     # via -r requirements-docs.in
-sphinxcontrib-jquery==2.0.0
+sphinxcontrib-jquery==4.1
     # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.3
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.5
     # via sphinx
@@ -562,59 +593,72 @@
     # via
     #   -r requirements-docs.in
     #   -r requirements-tests.txt
     #   alembic
     #   flask-sqlalchemy
     #   marshmallow-sqlalchemy
     #   sqlalchemy-utils
-sqlalchemy-utils==0.40.0
+sqlalchemy-utils==0.41.1
     # via -r requirements-docs.in
 sshpubkeys==3.3.1
     # via
     #   -r requirements-tests.txt
     #   moto
-stevedore==3.5.0
+stevedore==5.1.0
     # via
     #   -r requirements-tests.txt
     #   bandit
-tabulate==0.9.0
-    # via -r requirements-docs.in
-tomli==2.0.1
+sympy==1.12
     # via
     #   -r requirements-tests.txt
-    #   pytest
+    #   cfn-lint
+tabulate==0.9.0
+    # via -r requirements-docs.in
 twofish==0.3.0
     # via pyjks
-urllib3==1.26.9
+types-pyyaml==6.0.12.10
+    # via
+    #   -r requirements-tests.txt
+    #   responses
+typing-extensions==4.6.3
+    # via
+    #   -r requirements-tests.txt
+    #   alembic
+    #   aws-sam-translator
+    #   pydantic
+tzdata==2023.3
+    # via celery
+urllib3==1.26.16
     # via
     #   -r requirements-tests.txt
     #   botocore
+    #   docker
     #   requests
     #   responses
     #   sentry-sdk
 vine==5.0.0
     # via
     #   -r requirements-docs.in
     #   amqp
     #   celery
     #   kombu
-wcwidth==0.2.5
+wcwidth==0.2.6
     # via prompt-toolkit
-websocket-client==1.3.1
+websocket-client==1.6.1
     # via
     #   -r requirements-tests.txt
     #   docker
-werkzeug==2.0.3
+werkzeug==2.3.6
     # via
     #   -r requirements-docs.in
     #   -r requirements-tests.txt
     #   flask
     #   moto
     #   pytest-flask
-wrapt==1.14.0
+wrapt==1.15.0
     # via
     #   -r requirements-tests.txt
     #   aws-xray-sdk
 xmltodict==0.13.0
     # via
     #   -r requirements-docs.in
     #   -r requirements-tests.txt
```

### Comparing `lemur-1.4.0/requirements-tests.txt` & `lemur-1.5.0/requirements-tests.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,302 +1,330 @@
 #
-# This file is autogenerated by pip-compile with python 3.9
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.9
+# by the following command:
 #
-#    pip-compile --no-emit-index-url --output-file=requirements-tests.txt requirements-tests.in
+#    pip-compile --no-emit-index-url --output-file=requirements-tests.txt --resolver=backtracking requirements-tests.in
 #
-acme==2.4.0
+acme==2.6.0
     # via certbot
-alembic==1.7.7
+alembic==1.11.1
     # via flask-migrate
-async-timeout==4.0.2
-    # via redis
-attrs==21.4.0
+attrs==23.1.0
     # via
     #   jschema-to-python
     #   jsonschema
-    #   pytest
     #   sarif-om
-aws-sam-translator==1.44.0
+aws-sam-translator==1.70.0
     # via cfn-lint
-aws-xray-sdk==2.9.0
+aws-xray-sdk==2.12.0
     # via moto
 bandit==1.7.5
     # via -r requirements-tests.in
-black==23.1.0
+black==23.3.0
     # via -r requirements-tests.in
-boto3==1.26.94
+blinker==1.6.2
+    # via flask
+boto3==1.26.165
     # via
     #   aws-sam-translator
     #   moto
-botocore==1.29.100
+botocore==1.29.165
     # via
     #   aws-xray-sdk
     #   boto3
     #   moto
     #   s3transfer
-certbot==2.4.0
+certbot==2.6.0
     # via -r requirements-tests.in
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
-cffi==1.15.0
+cffi==1.15.1
     # via cryptography
-cfn-lint==0.58.4
+cfn-lint==0.77.10
     # via moto
-charset-normalizer==2.0.12
+charset-normalizer==3.1.0
     # via requests
-click==8.1.0
+click==8.1.3
     # via
     #   black
     #   flask
 configargparse==1.5.3
     # via certbot
-configobj==5.0.6
+configobj==5.0.8
     # via certbot
-coverage==6.5.0
+coverage==7.2.7
     # via -r requirements-tests.in
-cryptography==39.0.2
+cryptography==41.0.1
     # via
     #   acme
     #   certbot
     #   josepy
     #   moto
     #   pyopenssl
     #   python-jose
     #   sshpubkeys
-distro==1.7.0
+distro==1.8.0
     # via certbot
-docker==5.0.3
+docker==6.1.3
     # via moto
-ecdsa==0.17.0
+ecdsa==0.18.0
     # via
     #   moto
     #   python-jose
     #   sshpubkeys
 factory-boy==3.2.1
     # via -r requirements-tests.in
-faker==17.6.0
+faker==18.11.2
     # via
     #   -r requirements-tests.in
     #   factory-boy
-fakeredis==2.10.1
+fakeredis==2.15.0
     # via -r requirements-tests.in
-flask==1.1.2
+flask==2.3.2
     # via
     #   -r requirements-tests.in
     #   flask-migrate
     #   flask-sqlalchemy
     #   pytest-flask
-flask-migrate==2.7.0
+flask-migrate==4.0.4
     # via -r requirements-tests.in
 flask-sqlalchemy==2.5.1
     # via flask-migrate
 freezegun==1.2.2
     # via -r requirements-tests.in
-future==0.18.3
-    # via aws-xray-sdk
-gitdb==4.0.9
+gitdb==4.0.10
     # via gitpython
-gitpython==3.1.30
+gitpython==3.1.31
     # via bandit
-graphql-core==3.2.0
+graphql-core==3.2.3
     # via moto
-idna==3.3
-    # via
-    #   moto
-    #   requests
-iniconfig==1.1.1
+idna==3.4
+    # via requests
+iniconfig==2.0.0
     # via pytest
-itsdangerous==2.0.1
+itsdangerous==2.1.2
     # via
     #   -r requirements-tests.in
     #   flask
-jinja2==3.0.3
+jinja2==3.1.2
     # via
     #   -r requirements-tests.in
     #   flask
     #   moto
-jmespath==1.0.0
+jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 josepy==1.13.0
     # via
     #   acme
     #   certbot
 jschema-to-python==1.2.3
     # via cfn-lint
-jsondiff==1.3.1
+jsondiff==2.0.0
     # via moto
-jsonpatch==1.32
+jsonpatch==1.33
     # via cfn-lint
-jsonpickle==2.1.0
+jsonpickle==3.0.1
     # via jschema-to-python
-jsonpointer==2.2
+jsonpointer==2.4
     # via jsonpatch
-jsonschema==3.2.0
+jsonschema==4.17.3
     # via
     #   aws-sam-translator
     #   cfn-lint
+    #   jsonschema-spec
+    #   openapi-schema-validator
+    #   openapi-spec-validator
+jsonschema-spec==0.1.6
+    # via openapi-spec-validator
 junit-xml==1.9
     # via cfn-lint
-mako==1.2.2
+lazy-object-proxy==1.9.0
+    # via openapi-spec-validator
+mako==1.2.4
     # via alembic
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
     # via rich
-markupsafe==2.1.1
+markupsafe==2.1.3
     # via
     #   jinja2
     #   mako
-    #   moto
+    #   werkzeug
 marshmallow==2.21.0
     # via
     #   -r requirements-tests.in
     #   marshmallow-sqlalchemy
 marshmallow-sqlalchemy==0.23.1
     # via -r requirements-tests.in
 mdurl==0.1.2
     # via markdown-it-py
-moto[all]==3.1.1
+moto[all]==4.1.12
     # via -r requirements-tests.in
-mypy-extensions==0.4.3
+mpmath==1.3.0
+    # via sympy
+mypy-extensions==1.0.0
     # via black
-networkx==2.7.1
+networkx==3.1
     # via cfn-lint
 nose==1.3.7
     # via -r requirements-tests.in
-packaging==23.0
+openapi-schema-validator==0.4.4
+    # via openapi-spec-validator
+openapi-spec-validator==0.5.7
+    # via moto
+packaging==23.1
     # via
     #   black
+    #   docker
     #   pytest
 parsedatetime==2.6
     # via certbot
-pathspec==0.9.0
+pathable==0.4.3
+    # via jsonschema-spec
+pathspec==0.11.1
     # via black
-pbr==5.8.1
+pbr==5.11.1
     # via
     #   jschema-to-python
     #   sarif-om
     #   stevedore
-platformdirs==2.5.1
+platformdirs==3.8.0
     # via black
-pluggy==1.0.0
+pluggy==1.2.0
     # via pytest
-py==1.11.0
-    # via pytest
-pyasn1==0.4.8
+py-partiql-parser==0.3.3
+    # via moto
+pyasn1==0.5.0
     # via
     #   python-jose
     #   rsa
 pycparser==2.21
     # via cffi
-pyflakes==2.4.0
+pydantic==1.10.9
+    # via aws-sam-translator
+pyflakes==3.0.1
     # via -r requirements-tests.in
-pygments==2.14.0
+pygments==2.15.1
     # via rich
-pyopenssl==23.1.0
+pyopenssl==23.2.0
     # via
     #   acme
     #   josepy
+pyparsing==3.1.0
+    # via moto
 pyrfc3339==1.1
     # via
     #   acme
     #   certbot
-pyrsistent==0.18.1
+pyrsistent==0.19.3
     # via jsonschema
-pytest==7.1.3
+pytest==7.4.0
     # via
     #   -r requirements-tests.in
     #   pytest-flask
     #   pytest-mock
 pytest-flask==1.2.0
     # via -r requirements-tests.in
-pytest-mock==3.10.0
+pytest-mock==3.11.1
     # via -r requirements-tests.in
 python-dateutil==2.8.2
     # via
     #   botocore
     #   faker
     #   freezegun
     #   moto
 python-jose[cryptography]==3.3.0
     # via moto
-pytz==2022.1
+pytz==2023.3
     # via
     #   acme
     #   certbot
-    #   moto
     #   pyrfc3339
 pyyaml==6.0
     # via
     #   -r requirements-tests.in
     #   bandit
     #   cfn-lint
+    #   jsonschema-spec
     #   moto
-redis==4.5.4
+    #   responses
+redis==4.6.0
     # via
     #   -r requirements-tests.in
     #   fakeredis
-requests==2.28.2
+regex==2023.6.3
+    # via cfn-lint
+requests==2.31.0
     # via
     #   acme
     #   docker
+    #   jsonschema-spec
     #   moto
     #   requests-mock
     #   responses
-requests-mock==1.10.0
+requests-mock==1.11.0
     # via -r requirements-tests.in
-responses==0.20.0
+responses==0.23.1
     # via moto
-rich==13.3.2
+rfc3339-validator==0.1.4
+    # via openapi-schema-validator
+rich==13.4.2
     # via bandit
-rsa==4.8
+rsa==4.9
     # via python-jose
-s3transfer==0.6.0
+s3transfer==0.6.1
     # via boto3
 sarif-om==1.0.4
     # via cfn-lint
 six==1.16.0
     # via
-    #   cfn-lint
     #   configobj
     #   ecdsa
-    #   jsonschema
     #   junit-xml
     #   python-dateutil
     #   requests-mock
+    #   rfc3339-validator
 smmap==5.0.0
     # via gitdb
 sortedcontainers==2.4.0
     # via fakeredis
 sqlalchemy==1.3.24
     # via
     #   -r requirements-tests.in
     #   alembic
     #   flask-sqlalchemy
     #   marshmallow-sqlalchemy
 sshpubkeys==3.3.1
     # via moto
-stevedore==3.5.0
+stevedore==5.1.0
     # via bandit
-tomli==2.0.1
-    # via pytest
-urllib3==1.26.9
+sympy==1.12
+    # via cfn-lint
+types-pyyaml==6.0.12.10
+    # via responses
+typing-extensions==4.6.3
+    # via
+    #   alembic
+    #   aws-sam-translator
+    #   pydantic
+urllib3==1.26.16
     # via
     #   botocore
+    #   docker
     #   requests
     #   responses
-websocket-client==1.3.1
+websocket-client==1.6.1
     # via docker
-werkzeug==2.0.3
+werkzeug==2.3.6
     # via
     #   -r requirements-tests.in
     #   flask
     #   moto
     #   pytest-flask
-wrapt==1.14.0
+wrapt==1.15.0
     # via aws-xray-sdk
 xmltodict==0.13.0
     # via moto
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `lemur-1.4.0/requirements.txt` & `lemur-1.5.0/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,306 +1,303 @@
 #
-# This file is autogenerated by pip-compile with python 3.9
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.9
+# by the following command:
 #
-#    pip-compile --no-emit-index-url --output-file=requirements.txt requirements.in
+#    pip-compile --no-emit-index-url --output-file=requirements.txt --resolver=backtracking requirements.in
 #
-acme==2.4.0
+acme==2.6.0
     # via
     #   -r requirements.in
     #   certbot
-alembic==1.7.7
+alembic==1.11.1
     # via flask-migrate
-alembic-autogenerate-enums==0.0.2
+alembic-autogenerate-enums==0.1.1
     # via -r requirements.in
-amqp==5.1.0
+amqp==5.1.1
     # via kombu
 aniso8601==9.0.1
     # via flask-restful
 arrow==1.2.3
     # via -r requirements.in
-async-timeout==4.0.2
-    # via redis
 asyncpool==1.0
     # via -r requirements.in
-attrs==21.4.0
+attrs==23.1.0
     # via jsonlines
-bcrypt==3.2.0
+bcrypt==4.0.1
     # via
     #   flask-bcrypt
     #   paramiko
-beautifulsoup4==4.10.0
+beautifulsoup4==4.12.2
     # via cloudflare
-billiard==3.6.4.0
+billiard==4.1.0
     # via celery
-blinker==1.4
+blinker==1.6.2
     # via
+    #   flask
     #   flask-mail
     #   flask-principal
-boto3==1.26.94
+boto3==1.26.165
     # via -r requirements.in
-botocore==1.29.100
+botocore==1.29.165
     # via
     #   -r requirements.in
     #   boto3
     #   s3transfer
-celery[redis]==5.2.7
+celery[redis]==5.3.1
     # via -r requirements.in
-certbot==2.4.0
+certbot==2.6.0
     # via -r requirements.in
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   -r requirements.in
     #   requests
     #   sentry-sdk
 certsrv==2.1.1
     # via -r requirements.in
-cffi==1.15.0
+cffi==1.15.1
     # via
-    #   bcrypt
     #   cryptography
     #   pynacl
-charset-normalizer==2.0.12
+charset-normalizer==3.1.0
     # via requests
-click==8.1.0
+click==8.1.3
     # via
     #   celery
     #   click-didyoumean
     #   click-plugins
     #   click-repl
     #   flask
 click-didyoumean==0.3.0
     # via celery
 click-plugins==1.1.1
     # via celery
-click-repl==0.2.0
+click-repl==0.3.0
     # via celery
-cloudflare==2.11.1
+cloudflare==2.11.6
     # via -r requirements.in
 configargparse==1.5.3
     # via certbot
-configobj==5.0.6
+configobj==5.0.8
     # via certbot
-cryptography==39.0.2
+cryptography==41.0.1
     # via
     #   -r requirements.in
     #   acme
     #   certbot
     #   josepy
     #   paramiko
     #   pyopenssl
 decorator==5.1.1
     # via validators
-distro==1.7.0
+distro==1.8.0
     # via certbot
 dnspython==1.15.0
     # via dnspython3
 dnspython3==1.15.0
     # via -r requirements.in
 dyn==1.8.6
     # via -r requirements.in
-flask==1.1.2
+flask==2.3.2
     # via
     #   -r requirements.in
     #   flask-bcrypt
     #   flask-cors
     #   flask-mail
     #   flask-migrate
     #   flask-principal
     #   flask-restful
-    #   flask-script
     #   flask-sqlalchemy
 flask-bcrypt==1.0.1
     # via -r requirements.in
-flask-cors==3.0.10
+flask-cors==4.0.0
     # via -r requirements.in
 flask-mail==0.9.1
     # via -r requirements.in
-flask-migrate==2.7.0
+flask-migrate==4.0.4
     # via -r requirements.in
 flask-principal==0.4.0
     # via -r requirements.in
 flask-replicated==2.1
     # via -r requirements.in
-flask-restful==0.3.9
-    # via -r requirements.in
-flask-script==2.0.6
+flask-restful==0.3.10
     # via -r requirements.in
 flask-sqlalchemy==2.5.1
     # via
     #   -r requirements.in
     #   flask-migrate
 future==0.18.3
     # via -r requirements.in
 gunicorn==20.1.0
     # via -r requirements.in
-hvac==1.1.0
+hvac==1.1.1
     # via -r requirements.in
-idna==3.3
+idna==3.4
     # via requests
 inflection==0.5.1
     # via -r requirements.in
-itsdangerous==2.0.1
+itsdangerous==2.1.2
     # via
     #   -r requirements.in
     #   flask
 javaobj-py3==0.4.3
     # via pyjks
-jinja2==3.0.3
+jinja2==3.1.2
     # via
     #   -r requirements.in
     #   flask
-jmespath==1.0.0
+jmespath==1.0.1
     # via
     #   boto3
     #   botocore
 josepy==1.13.0
     # via
     #   acme
     #   certbot
-jsonlines==3.0.0
+jsonlines==3.1.0
     # via cloudflare
-kombu==5.2.4
+kombu==5.3.1
     # via celery
 lockfile==0.12.2
     # via -r requirements.in
 logmatic-python==0.1.7
     # via -r requirements.in
-mako==1.2.2
+mako==1.2.4
     # via alembic
-markupsafe==2.1.1
+markupsafe==2.1.3
     # via
     #   jinja2
     #   mako
+    #   werkzeug
 marshmallow==2.21.0
     # via
     #   -r requirements.in
     #   marshmallow-sqlalchemy
 marshmallow-sqlalchemy==0.23.1
     # via -r requirements.in
 ndg-httpsclient==0.5.1
     # via -r requirements.in
-paramiko==3.1.0
+paramiko==3.2.0
     # via -r requirements.in
 parsedatetime==2.6
     # via certbot
-pem==21.2.0
+pem==23.1.0
     # via -r requirements.in
-prompt-toolkit==3.0.28
+prompt-toolkit==3.0.38
     # via click-repl
-psycopg2==2.9.5
+psycopg2==2.9.6
     # via -r requirements.in
-pyasn1==0.4.8
+pyasn1==0.5.0
     # via
     #   ndg-httpsclient
     #   pyasn1-modules
     #   pyjks
     #   python-ldap
-pyasn1-modules==0.2.8
+pyasn1-modules==0.3.0
     # via
     #   pyjks
     #   python-ldap
 pycparser==2.21
     # via cffi
-pycryptodomex==3.14.1
+pycryptodomex==3.18.0
     # via pyjks
 pyhcl==0.4.4
     # via hvac
 pyjks==20.0.0
     # via -r requirements.in
-pyjwt==2.6.0
+pyjwt==2.7.0
     # via -r requirements.in
 pynacl==1.5.0
     # via paramiko
-pyopenssl==23.1.0
+pyopenssl==23.2.0
     # via
     #   -r requirements.in
     #   acme
     #   josepy
     #   ndg-httpsclient
 pyrfc3339==1.1
     # via
     #   acme
     #   certbot
 python-dateutil==2.8.2
     # via
     #   arrow
     #   botocore
-python-json-logger==2.0.2
+    #   celery
+python-json-logger==2.0.7
     # via logmatic-python
 python-ldap==3.4.3
     # via -r requirements.in
-pytz==2022.1
+pytz==2023.3
     # via
     #   acme
-    #   celery
     #   certbot
     #   flask-restful
     #   pyrfc3339
 pyyaml==6.0
     # via
     #   -r requirements.in
     #   cloudflare
-redis==4.5.4
+redis==4.6.0
     # via
     #   -r requirements.in
     #   celery
-requests==2.28.2
+requests==2.31.0
     # via
     #   -r requirements.in
     #   acme
     #   certsrv
     #   cloudflare
     #   hvac
 retrying==1.3.4
     # via -r requirements.in
-s3transfer==0.6.0
+s3transfer==0.6.1
     # via boto3
-sentry-sdk==1.9.0
+sentry-sdk==1.26.0
     # via -r requirements.in
 six==1.16.0
     # via
     #   -r requirements.in
-    #   bcrypt
-    #   click-repl
     #   configobj
-    #   flask-cors
     #   flask-restful
     #   python-dateutil
     #   retrying
-soupsieve==2.3.1
+soupsieve==2.4.1
     # via beautifulsoup4
 sqlalchemy==1.3.24
     # via
     #   -r requirements.in
     #   alembic
     #   flask-sqlalchemy
     #   marshmallow-sqlalchemy
     #   sqlalchemy-utils
-sqlalchemy-utils==0.40.0
+sqlalchemy-utils==0.41.1
     # via -r requirements.in
 tabulate==0.9.0
     # via -r requirements.in
 twofish==0.3.0
     # via pyjks
-urllib3==1.26.9
+typing-extensions==4.6.3
+    # via alembic
+tzdata==2023.3
+    # via celery
+urllib3==1.26.16
     # via
     #   botocore
     #   requests
     #   sentry-sdk
 validators==0.20.0
     # via -r requirements.in
 vine==5.0.0
     # via
     #   amqp
     #   celery
     #   kombu
-wcwidth==0.2.5
+wcwidth==0.2.6
     # via prompt-toolkit
-werkzeug==2.0.3
+werkzeug==2.3.6
     # via
     #   -r requirements.in
     #   flask
 xmltodict==0.13.0
     # via -r requirements.in
 
 # The following packages are considered to be unsafe in a requirements file:
```

### Comparing `lemur-1.4.0/setup.py` & `lemur-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,29 @@
 
 import datetime
 import json
 import logging
 import os.path
 import sys
 from subprocess import check_output
+from typing import Dict, Any
 
 from setuptools import Command
 from setuptools import setup, find_packages
 from setuptools.command.develop import develop
 from setuptools.command.install import install
 from setuptools.command.sdist import sdist
 
 ROOT = os.path.realpath(os.path.join(os.path.dirname(__file__)))
 
 # When executing the setup.py, we need to be able to import ourselves, this
 # means that we need to add the src/ directory to the sys.path.
 sys.path.insert(0, ROOT)
 
-about = {}
+about: Dict[str, Any] = {}
 with open(os.path.join(ROOT, 'lemur', '__about__.py')) as f:
     exec(f.read(), about)  # nosec: about file is benign
 
 # Parse requirements files
 with open('requirements.txt') as f:
     install_requirements = f.read().splitlines()
```

