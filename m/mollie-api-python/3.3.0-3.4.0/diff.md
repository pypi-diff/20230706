# Comparing `tmp/mollie-api-python-3.3.0.tar.gz` & `tmp/mollie-api-python-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mollie-api-python-3.3.0.tar", last modified: Tue Jun 13 07:15:24 2023, max compression
+gzip compressed data, was "mollie-api-python-3.4.0.tar", last modified: Thu Jul  6 07:12:20 2023, max compression
```

## Comparing `mollie-api-python-3.3.0.tar` & `mollie-api-python-3.4.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:15:24.007722 mollie-api-python-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-06-13 07:15:24.007722 mollie-api-python-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:15:23.995721 mollie-api-python-3.3.0/mollie/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:15:23.999721 mollie-api-python-3.3.0/mollie/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13595 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:15:24.003722 mollie-api-python-3.3.0/mollie/api/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/balance_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/capture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/chargeback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/issuer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/mandate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/onboarding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/order_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/payment_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/refund.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/settlement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/shipment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/objects/subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:15:24.007722 mollie-api-python-3.3.0/mollie/api/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/balances.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/captures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/chargebacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/customers.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/invoices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/mandates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/onboarding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/order_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/orders.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/payment_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/payments.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/refunds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/settlements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/shipments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/resources/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/api/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/mollie/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:15:24.007722 mollie-api-python-3.3.0/mollie_api_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-06-13 07:15:23.000000 mollie-api-python-3.3.0/mollie_api_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-13 07:15:23.000000 mollie-api-python-3.3.0/mollie_api_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:15:23.000000 mollie-api-python-3.3.0/mollie_api_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-13 07:15:23.000000 mollie-api-python-3.3.0/mollie_api_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 07:15:23.000000 mollie-api-python-3.3.0/mollie_api_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 07:15:24.007722 mollie-api-python-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-13 07:15:09.000000 mollie-api-python-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:12:20.579783 mollie-api-python-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-07-06 07:12:20.579783 mollie-api-python-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15155 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:12:20.571782 mollie-api-python-3.4.0/mollie/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:12:20.571782 mollie-api-python-3.4.0/mollie/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:12:20.575783 mollie-api-python-3.4.0/mollie/api/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/balance_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/chargeback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/issuer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/mandate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/onboarding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/order_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/payment_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/refund.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/settlement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/shipment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/objects/subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:12:20.579783 mollie-api-python-3.4.0/mollie/api/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/balances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/captures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/chargebacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/customers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/invoices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/mandates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/onboarding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/order_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/payment_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/payments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/refunds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/settlements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/shipments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/resources/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/mollie/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:12:20.579783 mollie-api-python-3.4.0/mollie_api_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-07-06 07:12:20.000000 mollie-api-python-3.4.0/mollie_api_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-07-06 07:12:20.000000 mollie-api-python-3.4.0/mollie_api_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:12:20.000000 mollie-api-python-3.4.0/mollie_api_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-06 07:12:20.000000 mollie-api-python-3.4.0/mollie_api_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 07:12:20.000000 mollie-api-python-3.4.0/mollie_api_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 07:12:20.579783 mollie-api-python-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-06 07:12:08.000000 mollie-api-python-3.4.0/setup.py
```

### Comparing `mollie-api-python-3.3.0/LICENSE.txt` & `mollie-api-python-3.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/PKG-INFO` & `mollie-api-python-3.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mollie-api-python
-Version: 3.3.0
+Version: 3.4.0
 Summary: Mollie API client for Python
 Home-page: https://github.com/mollie/mollie-api-python
 Author: Mollie B.V.
 Author-email: info@mollie.com
 Maintainer: Four Digits B.V.
 Maintainer-email: info@fourdigits.nl
 License: BSD
@@ -33,15 +33,15 @@
 ## Requirements ##
 To use the Mollie API client, the following things are required:
 
 + Get yourself a free [Mollie account](https://www.mollie.com/signup). No sign up costs.
 + Create a new [Website profile](https://www.mollie.com/dashboard/settings/profiles) to generate API keys and setup your webhook.
 + Now you're ready to use the Mollie API client in test mode.
 + Follow [a few steps](https://www.mollie.com/dashboard/?modal=onboarding) to enable payment methods in live mode, and let us handle the rest.
-+ Python >= 3.7
++ Python >= 3.8
 + Up-to-date OpenSSL (or other SSL/TLS toolkit)
 + Mollie API client for Python has a dependency on [Requests](http://docs.python-requests.org/en/master/) and [Requests-OAuthlib](https://requests-oauthlib.readthedocs.io/en/latest/)
 
 ## Migration to v3 ##
 If your application uses a recent v2 version of the Mollie API client and you're ready to migrate to v3, [read all about the API changes](https://github.com/mollie/mollie-api-python/blob/master/v3-api-changes.md) that we made. Use the docs to quickly find how to update your integration code and use the v3 client correctly.
 
 ## Installation ##
@@ -51,15 +51,15 @@
 
 By far the easiest way to install the Mollie API client is to install it with [pip](https://pip.pypa.io). The command below will install the latest released version of the client.
 ```shell
 $ pip install mollie-api-python
 ```
 You may also git checkout or [download all the files](https://github.com/mollie/mollie-api-python/archive/master.zip), and include the Mollie API client manually.
 
-Create and activate a Python >= 3.7 virtual environment (inside a git checkout or downloaded archive).
+Create and activate a Python >= 3.8 virtual environment (inside a git checkout or downloaded archive).
 
 ```shell
 $ cd mollie-api-python
 $ python -m venv .venv
 $ source .venv/bin/activate
 ```
```

### Comparing `mollie-api-python-3.3.0/README.md` & `mollie-api-python-3.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ## Requirements ##
 To use the Mollie API client, the following things are required:
 
 + Get yourself a free [Mollie account](https://www.mollie.com/signup). No sign up costs.
 + Create a new [Website profile](https://www.mollie.com/dashboard/settings/profiles) to generate API keys and setup your webhook.
 + Now you're ready to use the Mollie API client in test mode.
 + Follow [a few steps](https://www.mollie.com/dashboard/?modal=onboarding) to enable payment methods in live mode, and let us handle the rest.
-+ Python >= 3.7
++ Python >= 3.8
 + Up-to-date OpenSSL (or other SSL/TLS toolkit)
 + Mollie API client for Python has a dependency on [Requests](http://docs.python-requests.org/en/master/) and [Requests-OAuthlib](https://requests-oauthlib.readthedocs.io/en/latest/)
 
 ## Migration to v3 ##
 If your application uses a recent v2 version of the Mollie API client and you're ready to migrate to v3, [read all about the API changes](https://github.com/mollie/mollie-api-python/blob/master/v3-api-changes.md) that we made. Use the docs to quickly find how to update your integration code and use the v3 client correctly.
 
 ## Installation ##
@@ -31,15 +31,15 @@
 
 By far the easiest way to install the Mollie API client is to install it with [pip](https://pip.pypa.io). The command below will install the latest released version of the client.
 ```shell
 $ pip install mollie-api-python
 ```
 You may also git checkout or [download all the files](https://github.com/mollie/mollie-api-python/archive/master.zip), and include the Mollie API client manually.
 
-Create and activate a Python >= 3.7 virtual environment (inside a git checkout or downloaded archive).
+Create and activate a Python >= 3.8 virtual environment (inside a git checkout or downloaded archive).
 
 ```shell
 $ cd mollie-api-python
 $ python -m venv .venv
 $ source .venv/bin/activate
 ```
```

### Comparing `mollie-api-python-3.3.0/mollie/api/client.py` & `mollie-api-python-3.4.0/mollie/api/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,14 @@
         if not hasattr(self, "_client"):
             self._client = requests.Session()
             self._client.verify = True
             self._setup_retry()
 
         url, payload, params = self._format_request_data(path, data, params)
         try:
-
             headers = {
                 "Accept": "application/json",
                 "Authorization": f"Bearer {self.api_key}",
                 "Content-Type": "application/json",
                 "User-Agent": self.user_agent,
                 "X-Mollie-Client-Info": self.UNAME,
             }
@@ -235,15 +234,14 @@
         path: str,
         data: Optional[Dict[str, Any]] = None,
         params: Optional[Dict[str, Any]] = None,
         idempotency_key: str = "",
     ) -> requests.Response:
         url, payload, params = self._format_request_data(path, data, params)
         try:
-
             headers = {
                 "Accept": "application/json",
                 "Content-Type": "application/json",
                 "User-Agent": self.user_agent,
                 "X-Mollie-Client-Info": self.UNAME,
             }
 
@@ -338,15 +336,15 @@
     # TODO Implement https://docs.mollie.com/reference/oauth2/revoke-token
     # def revoke_oauth_token(self, token, type_hint):
     #     ...
 
     def _setup_retry(self) -> None:
         """Configure a retry behaviour on the HTTP client."""
         if self.retry:
-            retry = Retry(connect=self.retry, backoff_factor=1)
+            retry = Retry(connect=self.retry, read=0, backoff_factor=1)
             adapter = requests.adapters.HTTPAdapter(max_retries=retry)
 
             if hasattr(self, "_client"):
                 self._client.mount("https://", adapter)
             elif hasattr(self, "_oauth_client"):
                 self._oauth_client.mount("https://", adapter)
```

### Comparing `mollie-api-python-3.3.0/mollie/api/error.py` & `mollie-api-python-3.4.0/mollie/api/error.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/balance.py` & `mollie-api-python-3.4.0/mollie/api/objects/balance.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/balance_report.py` & `mollie-api-python-3.4.0/mollie/api/objects/invoice.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,61 @@
 from .base import ObjectBase
 
 
-class BalanceReport(ObjectBase):
+class Invoice(ObjectBase):
     @classmethod
     def get_resource_class(cls, client):
-        from ..resources import BalanceReports
+        from ..resources import Invoices
 
-        return BalanceReports(client)
+        return Invoices(client)
 
     @property
-    def resource(self):
-        return self._get_property("resource")
+    def id(self):
+        return self._get_property("id")
+
+    @property
+    def reference(self):
+        return self._get_property("reference")
+
+    @property
+    def vat_number(self):
+        return self._get_property("vatNumber")
+
+    @property
+    def status(self):
+        return self._get_property("status")
 
     @property
-    def balance_id(self):
-        return self._get_property("balanceId")
+    def issued_at(self):
+        return self._get_property("issuedAt")
+
+    @property
+    def paid_at(self):
+        return self._get_property("paidAt")
+
+    @property
+    def due_at(self):
+        return self._get_property("dueAt")
+
+    @property
+    def resource(self):
+        return self._get_property("resource")
 
     @property
-    def time_zone(self):
-        return self._get_property("timeZone")
+    def net_amount(self):
+        return self._get_property("netAmount")
 
     @property
-    def from_(self):
-        # 'from' is a reserverd word in Python, thus 'from_' is used.
-        return self._get_property("from")
+    def vat_amount(self):
+        return self._get_property("vatAmount")
 
     @property
-    def until(self):
-        return self._get_property("until")
+    def gross_amount(self):
+        return self._get_property("grossAmount")
 
     @property
-    def grouping(self):
-        return self._get_property("grouping")
+    def lines(self):
+        return self._get_property("lines") or []
 
     @property
-    def totals(self):
-        return self._get_property("totals")
+    def pdf(self):
+        return self._get_link("pdf")
```

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/balance_transaction.py` & `mollie-api-python-3.4.0/mollie/api/objects/organization.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 from .base import ObjectBase
 
 
-class BalanceTransaction(ObjectBase):
+class Organization(ObjectBase):
     @classmethod
     def get_resource_class(cls, client):
-        from ..resources import BalanceTransactions
+        from ..resources import Organizations
 
-        return BalanceTransactions(client)
+        return Organizations(client)
 
-    @classmethod
-    def get_object_name(cls):
-        # Overwrite get_object_name since BalanceTransactions gets returned by Mollie as balance_transactions.
-        return "balance_transactions"
+    @property
+    def id(self):
+        return self._get_property("id")
 
     @property
     def resource(self):
         return self._get_property("resource")
 
     @property
-    def id(self):
-        return self._get_property("id")
+    def name(self):
+        return self._get_property("name")
+
+    @property
+    def email(self):
+        return self._get_property("email")
 
     @property
-    def type(self):
-        return self._get_property("type")
+    def locale(self):
+        return self._get_property("locale")
 
     @property
-    def result_amount(self):
-        return self._get_property("resultAmount")
+    def address(self):
+        return self._get_property("address")
 
     @property
-    def initial_amount(self):
-        return self._get_property("initialAmount")
+    def registration_number(self):
+        return self._get_property("registrationNumber")
 
     @property
-    def deductions(self):
-        return self._get_property("deductions")
+    def vat_number(self):
+        return self._get_property("vatNumber")
 
     @property
-    def created_at(self):
-        return self._get_property("createdAt")
+    def vat_regulation(self):
+        return self._get_property("vatRegulation")
 
     @property
-    def context(self):
-        return self._get_property("context")
+    def dashboard(self):
+        return self._get_link("dashboard")
+
+    # TODO: Implement https://docs.mollie.com/reference/v2/organizations-api/get-partner
+    # def get_partner(self):
+    #     ...
```

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/base.py` & `mollie-api-python-3.4.0/mollie/api/objects/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,14 @@
+from typing import TYPE_CHECKING, Any
+
 from ..error import EmbedNotFound
 
+if TYPE_CHECKING:
+    from ..client import Client
+
 
 class ObjectBase(dict):
     def __init__(self, data, client):
         """
         Create a new object from API result data.
         """
         super().__init__(data)
@@ -38,9 +43,9 @@
 
     @classmethod
     def get_object_name(cls):
         name = cls.__name__.lower()
         return f"{name}s"
 
     @classmethod
-    def get_resource_class(cls, client):
+    def get_resource_class(cls, client: "Client", **kwargs: Any) -> Any:
         raise NotImplementedError  # pragma: no cover
```

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/capture.py` & `mollie-api-python-3.4.0/mollie/api/objects/chargeback.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,65 @@
+import re
+
 from .base import ObjectBase
 
 
-class Capture(ObjectBase):
+class Chargeback(ObjectBase):
     @classmethod
     def get_resource_class(cls, client):
-        from ..resources import PaymentCaptures
+        from ..resources import Chargebacks
 
-        return PaymentCaptures(client)
+        return Chargebacks(client)
 
     @property
     def id(self):
         return self._get_property("id")
 
     @property
-    def mode(self):
-        return self._get_property("mode")
-
-    @property
     def amount(self):
         return self._get_property("amount")
 
     @property
     def settlement_amount(self):
         return self._get_property("settlementAmount")
 
     @property
-    def payment_id(self):
-        return self._get_property("paymentId")
+    def created_at(self):
+        return self._get_property("createdAt")
 
     @property
-    def shipment_id(self):
-        return self._get_property("shipmentId")
+    def reason(self):
+        return self._get_property("reason")
 
     @property
-    def settlement_id(self):
-        return self._get_property("settlementId")
+    def reversed_at(self):
+        return self._get_property("reversedAt")
 
     @property
-    def created_at(self):
-        return self._get_property("createdAt")
+    def payment_id(self):
+        return self._get_property("paymentId")
+
+    @property
+    def settlement_id(self):
+        """
+        Return the settlement ID.
+
+        It is extracted from the settlement link, since the id is not available as a real property.
+        """
+        url = self._get_link("settlement")
+        if not url:
+            return None
+
+        match = re.findall(r"/settlements/(stl_\w+)$", url)
+        if match:
+            return match[0]
 
     def get_payment(self):
-        """Return the payment for this capture."""
+        """Return the Payment object related to this chargeback."""
         # TODO Use the embedded payment data, if available.
         return self.client.payments.get(self.payment_id)
 
-    def get_shipment(self):
-        """Return the shipment for this capture."""
-        url = self._get_link("shipment")
-        if url:
-            from ..resources import OrderShipments
-
-            # We fake the order object here, since it is not used by from_url()
-            return OrderShipments(self.client, order=None).from_url(url)
-
     def get_settlement(self):
-        """Return the settlement for this capture."""
-        return self.client.settlements.get(self.settlement_id)
+        """Return the Settlement object related to this chargeback, if available."""
+        settlement_id = self.settlement_id
+        if settlement_id is not None:
+            return self.client.settlements.get(settlement_id)
```

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/chargeback.py` & `mollie-api-python-3.4.0/mollie/api/objects/capture.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,67 @@
-import re
+from typing import TYPE_CHECKING, Any
 
 from .base import ObjectBase
 
+if TYPE_CHECKING:
+    from ..client import Client
+    from ..resources import PaymentCaptures
 
-class Chargeback(ObjectBase):
+
+class Capture(ObjectBase):
     @classmethod
-    def get_resource_class(cls, client):
-        from ..resources import Chargebacks
+    def get_resource_class(cls, client: "Client", **kwargs: Any) -> "PaymentCaptures":
+        from ..resources import PaymentCaptures
 
-        return Chargebacks(client)
+        payment = kwargs["payment"]
+        return PaymentCaptures(client, payment)
 
     @property
     def id(self):
         return self._get_property("id")
 
     @property
+    def mode(self):
+        return self._get_property("mode")
+
+    @property
     def amount(self):
         return self._get_property("amount")
 
     @property
     def settlement_amount(self):
         return self._get_property("settlementAmount")
 
     @property
-    def created_at(self):
-        return self._get_property("createdAt")
-
-    @property
-    def reason(self):
-        return self._get_property("reason")
-
-    @property
-    def reversed_at(self):
-        return self._get_property("reversedAt")
-
-    @property
     def payment_id(self):
         return self._get_property("paymentId")
 
     @property
+    def shipment_id(self):
+        return self._get_property("shipmentId")
+
+    @property
     def settlement_id(self):
-        """
-        Return the settlement ID.
+        return self._get_property("settlementId")
 
-        It is extracted from the settlement link, since the id is not available as a real property.
-        """
-        url = self._get_link("settlement")
-        if not url:
-            return None
-
-        match = re.findall(r"/settlements/(stl_\w+)$", url)
-        if match:
-            return match[0]
+    @property
+    def created_at(self):
+        return self._get_property("createdAt")
 
     def get_payment(self):
-        """Return the Payment object related to this chargeback."""
+        """Return the payment for this capture."""
         # TODO Use the embedded payment data, if available.
         return self.client.payments.get(self.payment_id)
 
+    def get_shipment(self):
+        """Return the shipment for this capture."""
+        url = self._get_link("shipment")
+        if url:
+            from ..resources import OrderShipments
+            from .order import Order
+
+            order = Order({}, self.client)
+            return OrderShipments(self.client, order).from_url(url)
+
     def get_settlement(self):
-        """Return the Settlement object related to this chargeback, if available."""
-        settlement_id = self.settlement_id
-        if settlement_id is not None:
-            return self.client.settlements.get(settlement_id)
+        """Return the settlement for this capture."""
+        return self.client.settlements.get(self.settlement_id)
```

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/client.py` & `mollie-api-python-3.4.0/mollie/api/objects/client.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/customer.py` & `mollie-api-python-3.4.0/mollie/api/objects/customer.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/invoice.py` & `mollie-api-python-3.4.0/mollie/api/objects/payment_link.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,61 +1,77 @@
 from .base import ObjectBase
 
 
-class Invoice(ObjectBase):
+class PaymentLink(ObjectBase):
     @classmethod
     def get_resource_class(cls, client):
-        from ..resources import Invoices
+        from ..resources import PaymentLinks
 
-        return Invoices(client)
+        return PaymentLinks(client)
+
+    @classmethod
+    def get_object_name(cls):
+        return "payment_links"
+
+    # Documented properties
+
+    @property
+    def resource(self):
+        return self._get_property("resource")
 
     @property
     def id(self):
         return self._get_property("id")
 
     @property
-    def reference(self):
-        return self._get_property("reference")
+    def description(self):
+        return self._get_property("description")
 
     @property
-    def vat_number(self):
-        return self._get_property("vatNumber")
+    def mode(self):
+        return self._get_property("mode")
 
     @property
-    def status(self):
-        return self._get_property("status")
+    def profile_id(self):
+        return self._get_property("profileId")
 
     @property
-    def issued_at(self):
-        return self._get_property("issuedAt")
+    def amount(self):
+        return self._get_property("amount")
 
     @property
-    def paid_at(self):
-        return self._get_property("paidAt")
+    def redirect_url(self):
+        return self._get_property("redirectUrl")
 
     @property
-    def due_at(self):
-        return self._get_property("dueAt")
+    def webhook_url(self):
+        return self._get_property("webhookUrl")
 
     @property
-    def resource(self):
-        return self._get_property("resource")
+    def created_at(self):
+        return self._get_property("createdAt")
 
     @property
-    def net_amount(self):
-        return self._get_property("netAmount")
+    def paid_at(self):
+        return self._get_property("paidAt")
 
     @property
-    def vat_amount(self):
-        return self._get_property("vatAmount")
+    def updated_at(self):
+        return self._get_property("updatedAt")
 
     @property
-    def gross_amount(self):
-        return self._get_property("grossAmount")
+    def expires_at(self):
+        return self._get_property("expiresAt")
 
-    @property
-    def lines(self):
-        return self._get_property("lines") or []
+    # documented _links
 
     @property
-    def pdf(self):
-        return self._get_link("pdf")
+    def payment_link(self):
+        return self._get_link("paymentLink")
+
+    # additional methods
+
+    def is_paid(self):
+        return self.paid_at is not None
+
+    def has_expiration_date(self):
+        return self.expires_at is not None
```

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/issuer.py` & `mollie-api-python-3.4.0/mollie/api/objects/issuer.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/list.py` & `mollie-api-python-3.4.0/mollie/api/objects/list.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/mandate.py` & `mollie-api-python-3.4.0/mollie/api/objects/onboarding.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,52 @@
 from .base import ObjectBase
 
 
-class Mandate(ObjectBase):
+class Onboarding(ObjectBase):
     @classmethod
     def get_resource_class(cls, client):
-        from ..resources import CustomerMandates
+        from ..resources import Onboarding as OnboardingResource
 
-        return CustomerMandates(client)
+        return OnboardingResource(client)
 
-    STATUS_PENDING = "pending"
-    STATUS_VALID = "valid"
-    STATUS_INVALID = "invalid"
-
-    @property
-    def id(self):
-        return self._get_property("id")
+    STATUS_NEEDS_DATA = "needs-data"
+    STATUS_IN_REVIEW = "in-review"  # Waiting for a valid mandate.
+    STATUS_COMPLETED = "completed"
 
     @property
     def resource(self):
         return self._get_property("resource")
 
     @property
-    def status(self):
-        return self._get_property("status")
-
-    @property
-    def method(self):
-        return self._get_property("method")
+    def name(self):
+        return self._get_property("name")
 
     @property
-    def details(self):
-        return self._get_property("details")
+    def signed_up_at(self):
+        return self._get_property("signedUpAt")
 
     @property
-    def mandate_reference(self):
-        return self._get_property("mandateReference")
+    def status(self):
+        return self._get_property("status")
 
     @property
-    def signature_date(self):
-        return self._get_property("signatureDate")
+    def can_receive_payments(self):
+        return self._get_property("canReceivePayments")
 
     @property
-    def created_at(self):
-        return self._get_property("createdAt")
+    def can_receive_settlements(self):
+        return self._get_property("canReceiveSettlements")
 
-    def is_pending(self):
-        """Check if the mandate is pending."""
-        return self.status == self.STATUS_PENDING
+    def is_needs_data(self):
+        return self.status == self.STATUS_NEEDS_DATA
 
-    def is_valid(self):
-        """Check if the mandate is valid."""
-        return self.status == self.STATUS_VALID
+    def is_in_review(self):
+        return self.status == self.STATUS_IN_REVIEW
 
-    def is_invalid(self):
-        """Check if the mandate is invalid."""
-        return self.status == self.STATUS_INVALID
+    def is_completed(self):
+        return self.status == self.STATUS_COMPLETED
 
-    def get_customer(self):
-        """Return the customer for this mandate."""
-        url = self._get_link("customer")
+    def get_organization(self):
+        """Retrieve the related organization."""
+        url = self._get_link("organization")
         if url:
-            return self.client.customers.from_url(url)
+            return self.client.organizations.from_url(url)
```

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/method.py` & `mollie-api-python-3.4.0/mollie/api/objects/method.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/onboarding.py` & `mollie-api-python-3.4.0/mollie/api/objects/balance_transaction.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,53 @@
+from typing import TYPE_CHECKING, Any
+
 from .base import ObjectBase
 
+if TYPE_CHECKING:
+    from ..client import Client
+    from ..resources import BalanceTransactions
+
 
-class Onboarding(ObjectBase):
+class BalanceTransaction(ObjectBase):
     @classmethod
-    def get_resource_class(cls, client):
-        from ..resources import Onboarding as OnboardingResource
+    def get_resource_class(cls, client: "Client", **kwargs: Any) -> "BalanceTransactions":
+        from ..resources import BalanceTransactions
 
-        return OnboardingResource(client)
+        balance = kwargs["balance"]
+        return BalanceTransactions(client, balance)
 
-    STATUS_NEEDS_DATA = "needs-data"
-    STATUS_IN_REVIEW = "in-review"  # Waiting for a valid mandate.
-    STATUS_COMPLETED = "completed"
+    @classmethod
+    def get_object_name(cls):
+        # Overwrite get_object_name since BalanceTransactions gets returned by Mollie as balance_transactions.
+        return "balance_transactions"
 
     @property
     def resource(self):
         return self._get_property("resource")
 
     @property
-    def name(self):
-        return self._get_property("name")
+    def id(self):
+        return self._get_property("id")
 
     @property
-    def signed_up_at(self):
-        return self._get_property("signedUpAt")
+    def type(self):
+        return self._get_property("type")
 
     @property
-    def status(self):
-        return self._get_property("status")
+    def result_amount(self):
+        return self._get_property("resultAmount")
 
     @property
-    def can_receive_payments(self):
-        return self._get_property("canReceivePayments")
+    def initial_amount(self):
+        return self._get_property("initialAmount")
 
     @property
-    def can_receive_settlements(self):
-        return self._get_property("canReceiveSettlements")
-
-    def is_needs_data(self):
-        return self.status == self.STATUS_NEEDS_DATA
+    def deductions(self):
+        return self._get_property("deductions")
 
-    def is_in_review(self):
-        return self.status == self.STATUS_IN_REVIEW
-
-    def is_completed(self):
-        return self.status == self.STATUS_COMPLETED
+    @property
+    def created_at(self):
+        return self._get_property("createdAt")
 
-    def get_organization(self):
-        """Retrieve the related organization."""
-        url = self._get_link("organization")
-        if url:
-            return self.client.organizations.from_url(url)
+    @property
+    def context(self):
+        return self._get_property("context")
```

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/order.py` & `mollie-api-python-3.4.0/mollie/api/objects/order.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/order_line.py` & `mollie-api-python-3.4.0/mollie/api/objects/order_line.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,23 @@
+from typing import TYPE_CHECKING, Any
+
 from .base import ObjectBase
 
+if TYPE_CHECKING:
+    from ..client import Client
+    from ..resources import OrderLines
+
 
 class OrderLine(ObjectBase):
     @classmethod
-    def get_resource_class(cls, client):
+    def get_resource_class(cls, client: "Client", **kwargs: Any) -> "OrderLines":
         from ..resources import OrderLines
 
-        return OrderLines(client)
+        order = kwargs["order"]
+        return OrderLines(client, order)
 
     STATUS_CREATED = "created"
     STATUS_AUTHORIZED = "authorized"
     STATUS_PAID = "paid"
     STATUS_SHIPPING = "shipping"
     STATUS_CANCELED = "canceled"
     STATUS_COMPLETED = "completed"
```

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/payment.py` & `mollie-api-python-3.4.0/mollie/api/objects/payment.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,16 @@
 
         This is only available for recurring payments.
         """
         url = self._get_link("subscription")
         if url:
             from ..resources import CustomerSubscriptions
 
-            return CustomerSubscriptions(self.client, customer=None).from_url(url)
+            customer = Customer({}, self.client)
+            return CustomerSubscriptions(self.client, customer).from_url(url)
 
     def get_customer(self):
         """Return the customer for this payment."""
         if self.customer_id:
             return self.client.customers.get(self.customer_id)
 
     def get_order(self):
```

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/permission.py` & `mollie-api-python-3.4.0/mollie/api/objects/permission.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/profile.py` & `mollie-api-python-3.4.0/mollie/api/objects/profile.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/refund.py` & `mollie-api-python-3.4.0/mollie/api/objects/refund.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/settlement.py` & `mollie-api-python-3.4.0/mollie/api/objects/settlement.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/shipment.py` & `mollie-api-python-3.4.0/mollie/api/objects/shipment.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/objects/subscription.py` & `mollie-api-python-3.4.0/mollie/api/objects/subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 
 from .base import ObjectBase
 from .customer import Customer
 
 
 class Subscription(ObjectBase):
     @classmethod
-    def get_resource_class(cls, client):
+    def get_resource_class(cls, client, **kwargs):
         from ..resources import CustomerSubscriptions
 
-        return CustomerSubscriptions(client)
+        customer = kwargs["customer"]
+        return CustomerSubscriptions(client, customer)
 
     STATUS_ACTIVE = "active"
     STATUS_PENDING = "pending"  # Waiting for a valid mandate.
     STATUS_CANCELED = "canceled"
     STATUS_SUSPENDED = "suspended"  # Active, but mandate became invalid.
     STATUS_COMPLETED = "completed"
```

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/__init__.py` & `mollie-api-python-3.4.0/mollie/api/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/balances.py` & `mollie-api-python-3.4.0/mollie/api/resources/balances.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/base.py` & `mollie-api-python-3.4.0/mollie/api/resources/base.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/captures.py` & `mollie-api-python-3.4.0/mollie/api/resources/captures.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/chargebacks.py` & `mollie-api-python-3.4.0/mollie/api/resources/chargebacks.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/clients.py` & `mollie-api-python-3.4.0/mollie/api/resources/clients.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/customers.py` & `mollie-api-python-3.4.0/mollie/api/resources/customers.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/invoices.py` & `mollie-api-python-3.4.0/mollie/api/resources/invoices.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/mandates.py` & `mollie-api-python-3.4.0/mollie/api/resources/mandates.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/methods.py` & `mollie-api-python-3.4.0/mollie/api/resources/methods.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/onboarding.py` & `mollie-api-python-3.4.0/mollie/api/resources/onboarding.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/order_lines.py` & `mollie-api-python-3.4.0/mollie/api/resources/order_lines.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/orders.py` & `mollie-api-python-3.4.0/mollie/api/resources/orders.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/organizations.py` & `mollie-api-python-3.4.0/mollie/api/resources/organizations.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/payment_links.py` & `mollie-api-python-3.4.0/mollie/api/resources/payment_links.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/payments.py` & `mollie-api-python-3.4.0/mollie/api/resources/payments.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/permissions.py` & `mollie-api-python-3.4.0/mollie/api/resources/permissions.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/profiles.py` & `mollie-api-python-3.4.0/mollie/api/resources/profiles.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/refunds.py` & `mollie-api-python-3.4.0/mollie/api/resources/refunds.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/settlements.py` & `mollie-api-python-3.4.0/mollie/api/resources/settlements.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/shipments.py` & `mollie-api-python-3.4.0/mollie/api/resources/shipments.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie/api/resources/subscriptions.py` & `mollie-api-python-3.4.0/mollie/api/resources/subscriptions.py`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/mollie_api_python.egg-info/PKG-INFO` & `mollie-api-python-3.4.0/mollie_api_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mollie-api-python
-Version: 3.3.0
+Version: 3.4.0
 Summary: Mollie API client for Python
 Home-page: https://github.com/mollie/mollie-api-python
 Author: Mollie B.V.
 Author-email: info@mollie.com
 Maintainer: Four Digits B.V.
 Maintainer-email: info@fourdigits.nl
 License: BSD
@@ -33,15 +33,15 @@
 ## Requirements ##
 To use the Mollie API client, the following things are required:
 
 + Get yourself a free [Mollie account](https://www.mollie.com/signup). No sign up costs.
 + Create a new [Website profile](https://www.mollie.com/dashboard/settings/profiles) to generate API keys and setup your webhook.
 + Now you're ready to use the Mollie API client in test mode.
 + Follow [a few steps](https://www.mollie.com/dashboard/?modal=onboarding) to enable payment methods in live mode, and let us handle the rest.
-+ Python >= 3.7
++ Python >= 3.8
 + Up-to-date OpenSSL (or other SSL/TLS toolkit)
 + Mollie API client for Python has a dependency on [Requests](http://docs.python-requests.org/en/master/) and [Requests-OAuthlib](https://requests-oauthlib.readthedocs.io/en/latest/)
 
 ## Migration to v3 ##
 If your application uses a recent v2 version of the Mollie API client and you're ready to migrate to v3, [read all about the API changes](https://github.com/mollie/mollie-api-python/blob/master/v3-api-changes.md) that we made. Use the docs to quickly find how to update your integration code and use the v3 client correctly.
 
 ## Installation ##
@@ -51,15 +51,15 @@
 
 By far the easiest way to install the Mollie API client is to install it with [pip](https://pip.pypa.io). The command below will install the latest released version of the client.
 ```shell
 $ pip install mollie-api-python
 ```
 You may also git checkout or [download all the files](https://github.com/mollie/mollie-api-python/archive/master.zip), and include the Mollie API client manually.
 
-Create and activate a Python >= 3.7 virtual environment (inside a git checkout or downloaded archive).
+Create and activate a Python >= 3.8 virtual environment (inside a git checkout or downloaded archive).
 
 ```shell
 $ cd mollie-api-python
 $ python -m venv .venv
 $ source .venv/bin/activate
 ```
```

### Comparing `mollie-api-python-3.3.0/mollie_api_python.egg-info/SOURCES.txt` & `mollie-api-python-3.4.0/mollie_api_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mollie-api-python-3.3.0/setup.py` & `mollie-api-python-3.4.0/setup.py`

 * *Files identical despite different names*

