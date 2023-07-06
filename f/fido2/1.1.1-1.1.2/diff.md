# Comparing `tmp/fido2-1.1.1.tar.gz` & `tmp/fido2-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fido2-1.1.1.tar", max compression
+gzip compressed data, was "fido2-1.1.2.tar", max compression
```

## Comparing `fido2-1.1.1.tar` & `fido2-1.1.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     1330 2023-04-05 08:41:27.538288 fido2-1.1.1/COPYING
--rw-r--r--   0        0        0    11560 2023-04-05 08:41:27.538288 fido2-1.1.1/COPYING.APLv2
--rw-r--r--   0        0        0    17099 2023-04-05 08:41:27.538288 fido2-1.1.1/COPYING.MPLv2
--rw-r--r--   0        0        0     2436 2023-04-05 08:41:27.538288 fido2-1.1.1/examples/acr122u.py
--rw-r--r--   0        0        0    10966 2023-04-05 08:41:27.538288 fido2-1.1.1/examples/acr122usam.py
--rw-r--r--   0        0        0     5839 2023-04-05 08:41:27.538288 fido2-1.1.1/examples/acr1252u.py
--rw-r--r--   0        0        0     3046 2023-04-05 08:41:27.538288 fido2-1.1.1/examples/bio_enrollment.py
--rw-r--r--   0        0        0     4509 2023-04-05 08:41:27.538288 fido2-1.1.1/examples/cred_blob.py
--rw-r--r--   0        0        0     4764 2023-04-05 08:41:27.538288 fido2-1.1.1/examples/credential.py
--rw-r--r--   0        0        0     2570 2023-04-05 08:41:27.538288 fido2-1.1.1/examples/get_info.py
--rw-r--r--   0        0        0     4865 2023-04-05 08:41:27.538288 fido2-1.1.1/examples/hmac_secret.py
--rw-r--r--   0        0        0     5029 2023-04-05 08:41:27.538288 fido2-1.1.1/examples/large_blobs.py
--rw-r--r--   0        0        0     3652 2023-04-05 08:41:27.538288 fido2-1.1.1/examples/multi_device.py
--rw-r--r--   0        0        0     4790 2023-04-05 08:41:27.538288 fido2-1.1.1/examples/resident_key.py
--rw-r--r--   0        0        0    28895 2023-04-05 09:48:20.810839 fido2-1.1.1/examples/server/poetry.lock
--rw-r--r--   0        0        0      501 2023-04-05 08:41:27.553890 fido2-1.1.1/examples/server/pyproject.toml
--rw-r--r--   0        0        0     2495 2023-04-05 08:41:27.553890 fido2-1.1.1/examples/server/README.adoc
--rw-r--r--   0        0        0        0 2023-04-05 08:41:27.553890 fido2-1.1.1/examples/server/server/__init__.py
--rw-r--r--   0        0        0     4055 2023-04-05 08:41:27.553890 fido2-1.1.1/examples/server/server/server.py
--rw-r--r--   0        0        0     1666 2023-04-05 08:41:27.553890 fido2-1.1.1/examples/server/server/static/authenticate.html
--rw-r--r--   0        0        0      589 2023-04-05 08:41:27.553890 fido2-1.1.1/examples/server/server/static/index.html
--rw-r--r--   0        0        0     1679 2023-04-05 08:41:27.553890 fido2-1.1.1/examples/server/server/static/register.html
--rw-r--r--   0        0        0     6075 2023-04-05 08:41:27.553890 fido2-1.1.1/examples/server/server/static/webauthn-json.browser-ponyfill.js
--rw-r--r--   0        0        0    13867 2023-04-05 08:41:27.553890 fido2-1.1.1/examples/server/server/static/webauthn-json.browser-ponyfill.js.map
--rw-r--r--   0        0        0     1032 2023-04-05 08:41:27.553890 fido2-1.1.1/examples/u2f_nfc.py
--rw-r--r--   0        0        0     5900 2023-04-05 08:41:27.553890 fido2-1.1.1/examples/verify_attestation.py
--rw-r--r--   0        0        0     6649 2023-04-05 08:41:27.553890 fido2-1.1.1/examples/verify_attestation_mds3.py
--rw-r--r--   0        0        0     1424 2023-04-05 11:41:15.462491 fido2-1.1.1/fido2/__init__.py
--rw-r--r--   0        0        0     1958 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/attestation/__init__.py
--rw-r--r--   0        0        0     3168 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/attestation/android.py
--rw-r--r--   0        0        0     2458 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/attestation/apple.py
--rw-r--r--   0        0        0     8251 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/attestation/base.py
--rw-r--r--   0        0        0     4383 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/attestation/packed.py
--rw-r--r--   0        0        0    20070 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/attestation/tpm.py
--rw-r--r--   0        0        0     2789 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/attestation/u2f.py
--rw-r--r--   0        0        0     5275 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/cbor.py
--rw-r--r--   0        0        0    34104 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/client.py
--rw-r--r--   0        0        0     9188 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/cose.py
--rw-r--r--   0        0        0     5656 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/ctap.py
--rw-r--r--   0        0        0     9429 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/ctap1.py
--rw-r--r--   0        0        0     1753 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/ctap2/__init__.py
--rw-r--r--   0        0        0    23159 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/ctap2/base.py
--rw-r--r--   0        0        0    13135 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/ctap2/bio.py
--rw-r--r--   0        0        0     7605 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/ctap2/blob.py
--rw-r--r--   0        0        0     4907 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/ctap2/config.py
--rw-r--r--   0        0        0     9089 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/ctap2/credman.py
--rw-r--r--   0        0        0     9609 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/ctap2/extensions.py
--rw-r--r--   0        0        0    15313 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/ctap2/pin.py
--rw-r--r--   0        0        0     3515 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/features.py
--rw-r--r--   0        0        0     9126 2023-04-05 09:49:31.465644 fido2-1.1.1/fido2/hid/__init__.py
--rw-r--r--   0        0        0     4707 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/hid/base.py
--rw-r--r--   0        0        0     8900 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/hid/freebsd.py
--rw-r--r--   0        0        0     3454 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/hid/linux.py
--rw-r--r--   0        0        0    15138 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/hid/macos.py
--rw-r--r--   0        0        0     5280 2023-04-05 09:49:31.465644 fido2-1.1.1/fido2/hid/netbsd.py
--rw-r--r--   0        0        0     4128 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/hid/openbsd.py
--rw-r--r--   0        0        0    12885 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/hid/windows.py
--rw-r--r--   0        0        0    18260 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/mds3.py
--rw-r--r--   0        0        0     9152 2023-04-05 08:41:27.553890 fido2-1.1.1/fido2/pcsc.py
--rw-r--r--   0        0        0   251725 2023-04-05 09:48:20.812838 fido2-1.1.1/fido2/public_suffix_list.dat
--rw-r--r--   0        0        0        0 2023-04-05 08:41:27.569539 fido2-1.1.1/fido2/py.typed
--rw-r--r--   0        0        0     2690 2023-04-05 08:41:27.569539 fido2-1.1.1/fido2/rpid.py
--rw-r--r--   0        0        0    20217 2023-04-05 08:41:27.569539 fido2-1.1.1/fido2/server.py
--rw-r--r--   0        0        0     8862 2023-04-05 08:41:27.569539 fido2-1.1.1/fido2/utils.py
--rw-r--r--   0        0        0    21882 2023-04-05 08:41:27.569539 fido2-1.1.1/fido2/webauthn.py
--rw-r--r--   0        0        0    28909 2023-04-05 08:41:27.569539 fido2-1.1.1/fido2/win_api.py
--rw-r--r--   0        0        0     7542 2023-04-05 11:42:02.463599 fido2-1.1.1/NEWS
--rw-r--r--   0        0        0     1634 2023-04-05 11:41:04.855627 fido2-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4110 2023-04-05 09:49:37.912042 fido2-1.1.1/README.adoc
--rw-r--r--   0        0        0       78 2023-04-05 08:41:27.569539 fido2-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 08:41:27.569539 fido2-1.1.1/tests/hid/__init__.py
--rw-r--r--   0        0        0      799 2023-04-05 08:41:27.569539 fido2-1.1.1/tests/hid/test_base.py
--rw-r--r--   0        0        0    31463 2023-04-05 08:41:27.569539 fido2-1.1.1/tests/test_attestation.py
--rw-r--r--   0        0        0     7173 2023-04-05 08:41:27.569539 fido2-1.1.1/tests/test_cbor.py
--rw-r--r--   0        0        0     9874 2023-04-05 08:41:27.569539 fido2-1.1.1/tests/test_client.py
--rw-r--r--   0        0        0     6507 2023-04-05 08:41:27.569539 fido2-1.1.1/tests/test_cose.py
--rw-r--r--   0        0        0     8205 2023-04-05 08:41:27.569539 fido2-1.1.1/tests/test_ctap1.py
--rw-r--r--   0        0        0    19411 2023-04-05 08:41:27.569539 fido2-1.1.1/tests/test_ctap2.py
--rw-r--r--   0        0        0     2036 2023-04-05 08:41:27.569539 fido2-1.1.1/tests/test_hid.py
--rw-r--r--   0        0        0    21200 2023-04-05 08:41:27.569539 fido2-1.1.1/tests/test_mds3.py
--rw-r--r--   0        0        0     3360 2023-04-05 08:41:27.569539 fido2-1.1.1/tests/test_pcsc.py
--rw-r--r--   0        0        0     2764 2023-04-05 08:41:27.569539 fido2-1.1.1/tests/test_rpid.py
--rw-r--r--   0        0        0     7465 2023-04-05 08:41:27.569539 fido2-1.1.1/tests/test_server.py
--rw-r--r--   0        0        0     2995 2023-04-05 08:41:27.569539 fido2-1.1.1/tests/test_tpm.py
--rw-r--r--   0        0        0     3764 2023-04-05 08:41:27.569539 fido2-1.1.1/tests/test_utils.py
--rw-r--r--   0        0        0    12609 2023-04-05 08:41:27.569539 fido2-1.1.1/tests/test_webauthn.py
--rw-r--r--   0        0        0     4751 2023-04-05 08:41:27.569539 fido2-1.1.1/tests/test_webauthn_legacy_mapping.py
--rw-r--r--   0        0        0     2049 2023-04-05 08:41:27.569539 fido2-1.1.1/tests/utils.py
--rw-r--r--   0        0        0     1396 1970-01-01 00:00:00.000000 fido2-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1330 2023-04-05 08:41:27.538288 fido2-1.1.2/COPYING
+-rw-r--r--   0        0        0    11560 2023-04-05 08:41:27.538288 fido2-1.1.2/COPYING.APLv2
+-rw-r--r--   0        0        0    17099 2023-04-05 08:41:27.538288 fido2-1.1.2/COPYING.MPLv2
+-rw-r--r--   0        0        0     2436 2023-04-05 08:41:27.538288 fido2-1.1.2/examples/acr122u.py
+-rw-r--r--   0        0        0    10966 2023-04-05 08:41:27.538288 fido2-1.1.2/examples/acr122usam.py
+-rw-r--r--   0        0        0     5839 2023-04-05 08:41:27.538288 fido2-1.1.2/examples/acr1252u.py
+-rw-r--r--   0        0        0     2965 2023-06-26 14:38:46.933642 fido2-1.1.2/examples/bio_enrollment.py
+-rw-r--r--   0        0        0     4509 2023-04-05 08:41:27.538288 fido2-1.1.2/examples/cred_blob.py
+-rw-r--r--   0        0        0     4764 2023-04-05 08:41:27.538288 fido2-1.1.2/examples/credential.py
+-rw-r--r--   0        0        0     2570 2023-04-05 08:41:27.538288 fido2-1.1.2/examples/get_info.py
+-rw-r--r--   0        0        0     4865 2023-04-05 08:41:27.538288 fido2-1.1.2/examples/hmac_secret.py
+-rw-r--r--   0        0        0     5029 2023-04-05 08:41:27.538288 fido2-1.1.2/examples/large_blobs.py
+-rw-r--r--   0        0        0     3687 2023-06-26 10:21:13.432352 fido2-1.1.2/examples/multi_device.py
+-rw-r--r--   0        0        0     4790 2023-04-05 08:41:27.538288 fido2-1.1.2/examples/resident_key.py
+-rw-r--r--   0        0        0    28433 2023-07-06 09:58:23.571747 fido2-1.1.2/examples/server/poetry.lock
+-rw-r--r--   0        0        0      501 2023-04-05 08:41:27.553890 fido2-1.1.2/examples/server/pyproject.toml
+-rw-r--r--   0        0        0     2495 2023-04-05 08:41:27.553890 fido2-1.1.2/examples/server/README.adoc
+-rw-r--r--   0        0        0        0 2023-04-05 08:41:27.553890 fido2-1.1.2/examples/server/server/__init__.py
+-rw-r--r--   0        0        0     4055 2023-04-05 08:41:27.553890 fido2-1.1.2/examples/server/server/server.py
+-rw-r--r--   0        0        0     1666 2023-04-05 08:41:27.553890 fido2-1.1.2/examples/server/server/static/authenticate.html
+-rw-r--r--   0        0        0      589 2023-04-05 08:41:27.553890 fido2-1.1.2/examples/server/server/static/index.html
+-rw-r--r--   0        0        0     1679 2023-04-05 08:41:27.553890 fido2-1.1.2/examples/server/server/static/register.html
+-rw-r--r--   0        0        0     6075 2023-04-05 08:41:27.553890 fido2-1.1.2/examples/server/server/static/webauthn-json.browser-ponyfill.js
+-rw-r--r--   0        0        0    13867 2023-04-05 08:41:27.553890 fido2-1.1.2/examples/server/server/static/webauthn-json.browser-ponyfill.js.map
+-rw-r--r--   0        0        0     1032 2023-04-05 08:41:27.553890 fido2-1.1.2/examples/u2f_nfc.py
+-rw-r--r--   0        0        0     5900 2023-04-05 08:41:27.553890 fido2-1.1.2/examples/verify_attestation.py
+-rw-r--r--   0        0        0     6649 2023-04-05 08:41:27.553890 fido2-1.1.2/examples/verify_attestation_mds3.py
+-rw-r--r--   0        0        0     1395 2023-07-06 14:00:58.064261 fido2-1.1.2/fido2/__init__.py
+-rw-r--r--   0        0        0     1958 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/attestation/__init__.py
+-rw-r--r--   0        0        0     3168 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/attestation/android.py
+-rw-r--r--   0        0        0     2458 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/attestation/apple.py
+-rw-r--r--   0        0        0     8251 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/attestation/base.py
+-rw-r--r--   0        0        0     4383 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/attestation/packed.py
+-rw-r--r--   0        0        0    20070 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/attestation/tpm.py
+-rw-r--r--   0        0        0     2789 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/attestation/u2f.py
+-rw-r--r--   0        0        0     5275 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/cbor.py
+-rw-r--r--   0        0        0    33324 2023-07-03 08:05:39.819024 fido2-1.1.2/fido2/client.py
+-rw-r--r--   0        0        0     9188 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/cose.py
+-rw-r--r--   0        0        0     5656 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/ctap.py
+-rw-r--r--   0        0        0     9429 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/ctap1.py
+-rw-r--r--   0        0        0     1753 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/ctap2/__init__.py
+-rw-r--r--   0        0        0    23175 2023-07-06 13:38:45.231534 fido2-1.1.2/fido2/ctap2/base.py
+-rw-r--r--   0        0        0    13135 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/ctap2/bio.py
+-rw-r--r--   0        0        0     7605 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/ctap2/blob.py
+-rw-r--r--   0        0        0     4907 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/ctap2/config.py
+-rw-r--r--   0        0        0     9089 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/ctap2/credman.py
+-rw-r--r--   0        0        0     9609 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/ctap2/extensions.py
+-rw-r--r--   0        0        0    15481 2023-07-03 08:05:39.819024 fido2-1.1.2/fido2/ctap2/pin.py
+-rw-r--r--   0        0        0     3515 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/features.py
+-rw-r--r--   0        0        0     9126 2023-04-05 09:49:31.465644 fido2-1.1.2/fido2/hid/__init__.py
+-rw-r--r--   0        0        0     4707 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/hid/base.py
+-rw-r--r--   0        0        0     8634 2023-07-06 09:58:23.572309 fido2-1.1.2/fido2/hid/freebsd.py
+-rw-r--r--   0        0        0     3454 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/hid/linux.py
+-rw-r--r--   0        0        0    15138 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/hid/macos.py
+-rw-r--r--   0        0        0     5280 2023-04-05 09:49:31.465644 fido2-1.1.2/fido2/hid/netbsd.py
+-rw-r--r--   0        0        0     4128 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/hid/openbsd.py
+-rw-r--r--   0        0        0    12885 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/hid/windows.py
+-rw-r--r--   0        0        0    18260 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/mds3.py
+-rw-r--r--   0        0        0     9152 2023-04-05 08:41:27.553890 fido2-1.1.2/fido2/pcsc.py
+-rw-r--r--   0        0        0   239744 2023-07-06 14:00:57.319237 fido2-1.1.2/fido2/public_suffix_list.dat
+-rw-r--r--   0        0        0        0 2023-04-05 08:41:27.569539 fido2-1.1.2/fido2/py.typed
+-rw-r--r--   0        0        0     2690 2023-04-05 08:41:27.569539 fido2-1.1.2/fido2/rpid.py
+-rw-r--r--   0        0        0    19711 2023-07-06 09:58:23.572309 fido2-1.1.2/fido2/server.py
+-rw-r--r--   0        0        0     8783 2023-07-06 13:29:42.445886 fido2-1.1.2/fido2/utils.py
+-rw-r--r--   0        0        0    21882 2023-04-05 08:41:27.569539 fido2-1.1.2/fido2/webauthn.py
+-rw-r--r--   0        0        0    28909 2023-04-05 08:41:27.569539 fido2-1.1.2/fido2/win_api.py
+-rw-r--r--   0        0        0     7578 2023-07-06 14:00:58.062517 fido2-1.1.2/NEWS
+-rw-r--r--   0        0        0     1585 2023-07-06 14:00:58.064261 fido2-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4110 2023-04-05 09:49:37.912042 fido2-1.1.2/README.adoc
+-rw-r--r--   0        0        0       78 2023-04-05 08:41:27.569539 fido2-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-05 08:41:27.569539 fido2-1.1.2/tests/hid/__init__.py
+-rw-r--r--   0        0        0      799 2023-04-05 08:41:27.569539 fido2-1.1.2/tests/hid/test_base.py
+-rw-r--r--   0        0        0    31501 2023-07-06 09:22:56.159596 fido2-1.1.2/tests/test_attestation.py
+-rw-r--r--   0        0        0     6958 2023-07-06 09:58:23.573279 fido2-1.1.2/tests/test_cbor.py
+-rw-r--r--   0        0        0     9874 2023-04-05 08:41:27.569539 fido2-1.1.2/tests/test_client.py
+-rw-r--r--   0        0        0     6507 2023-04-05 08:41:27.569539 fido2-1.1.2/tests/test_cose.py
+-rw-r--r--   0        0        0     8205 2023-04-05 08:41:27.569539 fido2-1.1.2/tests/test_ctap1.py
+-rw-r--r--   0        0        0    19411 2023-04-05 08:41:27.569539 fido2-1.1.2/tests/test_ctap2.py
+-rw-r--r--   0        0        0     2036 2023-04-05 08:41:27.569539 fido2-1.1.2/tests/test_hid.py
+-rw-r--r--   0        0        0    21200 2023-04-05 08:41:27.569539 fido2-1.1.2/tests/test_mds3.py
+-rw-r--r--   0        0        0     3360 2023-04-05 08:41:27.569539 fido2-1.1.2/tests/test_pcsc.py
+-rw-r--r--   0        0        0     2764 2023-04-05 08:41:27.569539 fido2-1.1.2/tests/test_rpid.py
+-rw-r--r--   0        0        0     7242 2023-07-06 13:27:17.942279 fido2-1.1.2/tests/test_server.py
+-rw-r--r--   0        0        0     2995 2023-04-21 09:03:22.464591 fido2-1.1.2/tests/test_tpm.py
+-rw-r--r--   0        0        0     3764 2023-04-05 08:41:27.569539 fido2-1.1.2/tests/test_utils.py
+-rw-r--r--   0        0        0    12277 2023-07-06 13:27:17.942279 fido2-1.1.2/tests/test_webauthn.py
+-rw-r--r--   0        0        0     4751 2023-04-05 08:41:27.569539 fido2-1.1.2/tests/test_webauthn_legacy_mapping.py
+-rw-r--r--   0        0        0     2049 2023-04-05 08:41:27.569539 fido2-1.1.2/tests/utils.py
+-rw-r--r--   0        0        0     1396 1970-01-01 00:00:00.000000 fido2-1.1.2/PKG-INFO
```

### Comparing `fido2-1.1.1/COPYING` & `fido2-1.1.2/COPYING`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/COPYING.APLv2` & `fido2-1.1.2/COPYING.APLv2`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/COPYING.MPLv2` & `fido2-1.1.2/COPYING.MPLv2`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/examples/acr122u.py` & `fido2-1.1.2/examples/acr122u.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/examples/acr122usam.py` & `fido2-1.1.2/examples/acr122usam.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/examples/acr1252u.py` & `fido2-1.1.2/examples/acr1252u.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/examples/bio_enrollment.py` & `fido2-1.1.2/examples/bio_enrollment.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-# Copyright (c) 2020 Yubico AB
-# All rights reserved.
-#
-#   Redistribution and use in source and binary forms, with or
-#   without modification, are permitted provided that the following
-#   conditions are met:
-#
-#    1. Redistributions of source code must retain the above copyright
-#       notice, this list of conditions and the following disclaimer.
-#    2. Redistributions in binary form must reproduce the above
-#       copyright notice, this list of conditions and the following
-#       disclaimer in the documentation and/or other materials provided
-#       with the distribution.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
-# FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
-# COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
-# INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
-# BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
-# ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-# POSSIBILITY OF SUCH DAMAGE.
-
-"""
-Connects to the first FIDO device found over USB, and attempts to enroll a new
-fingerprint. This requires that a PIN is already set.
-
-NOTE: This uses a draft bio enrollment specification which is not yet final.
-Consider this highly experimental.
-"""
-from fido2.hid import CtapHidDevice
-from fido2.ctap2 import Ctap2, FPBioEnrollment, CaptureError
-from fido2.ctap2.pin import ClientPin
-from fido2.ctap2.bio import BioEnrollment
-from getpass import getpass
-import sys
-
-pin = None
-uv = "discouraged"
-
-for dev in CtapHidDevice.list_devices():
-    try:
-        ctap = Ctap2(dev)
-        if BioEnrollment.is_supported(ctap.info):
-            break
-    except Exception:  # nosec
-        continue
-else:
-    print("No Authenticator supporting bioEnroll found")
-    sys.exit(1)
-
-if not ctap.info.options.get("clientPin"):
-    print("PIN not set for the device!")
-    sys.exit(1)
-
-# Authenticate with PIN
-print("Preparing to enroll a new fingerprint.")
-pin = getpass("Please enter PIN: ")
-client_pin = ClientPin(ctap)
-pin_token = client_pin.get_pin_token(pin, ClientPin.PERMISSION.BIO_ENROLL)
-bio = FPBioEnrollment(ctap, client_pin.protocol, pin_token)
-
-print(bio.enumerate_enrollments())
-
-# Start enrollment
-enroller = bio.enroll()
-template_id = None
-while template_id is None:
-    print("Press your fingerprint against the sensor now...")
-    try:
-        template_id = enroller.capture()
-        print(enroller.remaining, "more scans needed.")
-    except CaptureError as e:
-        print(e)
-bio.set_name(template_id, "Example")
-
-print("Fingerprint registered successfully with ID:", template_id)
+# Copyright (c) 2020 Yubico AB
+# All rights reserved.
+#
+#   Redistribution and use in source and binary forms, with or
+#   without modification, are permitted provided that the following
+#   conditions are met:
+#
+#    1. Redistributions of source code must retain the above copyright
+#       notice, this list of conditions and the following disclaimer.
+#    2. Redistributions in binary form must reproduce the above
+#       copyright notice, this list of conditions and the following
+#       disclaimer in the documentation and/or other materials provided
+#       with the distribution.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
+# FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
+# COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
+# INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
+# BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
+# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
+# ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+# POSSIBILITY OF SUCH DAMAGE.
+
+"""
+Connects to the first FIDO device found over USB, and attempts to enroll a new
+fingerprint. This requires that a PIN is already set.
+
+NOTE: This uses a draft bio enrollment specification which is not yet final.
+Consider this highly experimental.
+"""
+from fido2.hid import CtapHidDevice
+from fido2.ctap2 import Ctap2, FPBioEnrollment, CaptureError
+from fido2.ctap2.pin import ClientPin
+from fido2.ctap2.bio import BioEnrollment
+from getpass import getpass
+import sys
+
+pin = None
+uv = "discouraged"
+
+for dev in CtapHidDevice.list_devices():
+    try:
+        ctap = Ctap2(dev)
+        if BioEnrollment.is_supported(ctap.info):
+            break
+    except Exception:  # nosec
+        continue
+else:
+    print("No Authenticator supporting bioEnroll found")
+    sys.exit(1)
+
+if not ctap.info.options.get("clientPin"):
+    print("PIN not set for the device!")
+    sys.exit(1)
+
+# Authenticate with PIN
+print("Preparing to enroll a new fingerprint.")
+pin = getpass("Please enter PIN: ")
+client_pin = ClientPin(ctap)
+pin_token = client_pin.get_pin_token(pin, ClientPin.PERMISSION.BIO_ENROLL)
+bio = FPBioEnrollment(ctap, client_pin.protocol, pin_token)
+
+print(bio.enumerate_enrollments())
+
+# Start enrollment
+enroller = bio.enroll()
+template_id = None
+while template_id is None:
+    print("Press your fingerprint against the sensor now...")
+    try:
+        template_id = enroller.capture()
+        print(enroller.remaining, "more scans needed.")
+    except CaptureError as e:
+        print(e)
+bio.set_name(template_id, "Example")
+
+print("Fingerprint registered successfully with ID:", template_id)
```

### Comparing `fido2-1.1.1/examples/cred_blob.py` & `fido2-1.1.2/examples/cred_blob.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/examples/credential.py` & `fido2-1.1.2/examples/credential.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/examples/get_info.py` & `fido2-1.1.2/examples/get_info.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/examples/hmac_secret.py` & `fido2-1.1.2/examples/hmac_secret.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/examples/large_blobs.py` & `fido2-1.1.2/examples/large_blobs.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/examples/multi_device.py` & `fido2-1.1.2/examples/multi_device.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,16 +52,17 @@
         return getpass("Enter PIN: ")
 
     def request_uv(self, permissions, rd_id):
         print("User Verification required.")
         return True
 
 
+cli_interaction = CliInteraction()
 clients = [
-    Fido2Client(d, "https://example.com", user_interaction=CliInteraction())
+    Fido2Client(d, "https://example.com", user_interaction=cli_interaction)
     for d in devs
 ]
 
 # Prepare parameters for makeCredential
 rp = {"id": "example.com", "name": "Example RP"}
 user = {"id": b"user_id", "name": "A. User"}
 challenge = b"Y2hhbGxlbmdl"
```

### Comparing `fido2-1.1.1/examples/resident_key.py` & `fido2-1.1.2/examples/resident_key.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/examples/server/poetry.lock` & `fido2-1.1.2/examples/server/poetry.lock`

 * *Files 12% similar despite different names*

```diff
@@ -1,365 +1,365 @@
-# This file is automatically @generated by Poetry 1.4.1 and should not be changed by hand.
-
-[[package]]
-name = "cffi"
-version = "1.15.1"
-description = "Foreign Function Interface for Python calling C code."
-category = "main"
-optional = false
-python-versions = "*"
-files = [
-    {file = "cffi-1.15.1-cp27-cp27m-macosx_10_9_x86_64.whl", hash = "sha256:a66d3508133af6e8548451b25058d5812812ec3798c886bf38ed24a98216fab2"},
-    {file = "cffi-1.15.1-cp27-cp27m-manylinux1_i686.whl", hash = "sha256:470c103ae716238bbe698d67ad020e1db9d9dba34fa5a899b5e21577e6d52ed2"},
-    {file = "cffi-1.15.1-cp27-cp27m-manylinux1_x86_64.whl", hash = "sha256:9ad5db27f9cabae298d151c85cf2bad1d359a1b9c686a275df03385758e2f914"},
-    {file = "cffi-1.15.1-cp27-cp27m-win32.whl", hash = "sha256:b3bbeb01c2b273cca1e1e0c5df57f12dce9a4dd331b4fa1635b8bec26350bde3"},
-    {file = "cffi-1.15.1-cp27-cp27m-win_amd64.whl", hash = "sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e"},
-    {file = "cffi-1.15.1-cp27-cp27mu-manylinux1_i686.whl", hash = "sha256:d61f4695e6c866a23a21acab0509af1cdfd2c013cf256bbf5b6b5e2695827162"},
-    {file = "cffi-1.15.1-cp27-cp27mu-manylinux1_x86_64.whl", hash = "sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b"},
-    {file = "cffi-1.15.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:39d39875251ca8f612b6f33e6b1195af86d1b3e60086068be9cc053aa4376e21"},
-    {file = "cffi-1.15.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:285d29981935eb726a4399badae8f0ffdff4f5050eaa6d0cfc3f64b857b77185"},
-    {file = "cffi-1.15.1-cp310-cp310-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:3eb6971dcff08619f8d91607cfc726518b6fa2a9eba42856be181c6d0d9515fd"},
-    {file = "cffi-1.15.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:21157295583fe8943475029ed5abdcf71eb3911894724e360acff1d61c1d54bc"},
-    {file = "cffi-1.15.1-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:5635bd9cb9731e6d4a1132a498dd34f764034a8ce60cef4f5319c0541159392f"},
-    {file = "cffi-1.15.1-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:2012c72d854c2d03e45d06ae57f40d78e5770d252f195b93f581acf3ba44496e"},
-    {file = "cffi-1.15.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dd86c085fae2efd48ac91dd7ccffcfc0571387fe1193d33b6394db7ef31fe2a4"},
-    {file = "cffi-1.15.1-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01"},
-    {file = "cffi-1.15.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:59c0b02d0a6c384d453fece7566d1c7e6b7bae4fc5874ef2ef46d56776d61c9e"},
-    {file = "cffi-1.15.1-cp310-cp310-win32.whl", hash = "sha256:cba9d6b9a7d64d4bd46167096fc9d2f835e25d7e4c121fb2ddfc6528fb0413b2"},
-    {file = "cffi-1.15.1-cp310-cp310-win_amd64.whl", hash = "sha256:ce4bcc037df4fc5e3d184794f27bdaab018943698f4ca31630bc7f84a7b69c6d"},
-    {file = "cffi-1.15.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:3d08afd128ddaa624a48cf2b859afef385b720bb4b43df214f85616922e6a5ac"},
-    {file = "cffi-1.15.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:3799aecf2e17cf585d977b780ce79ff0dc9b78d799fc694221ce814c2c19db83"},
-    {file = "cffi-1.15.1-cp311-cp311-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a591fe9e525846e4d154205572a029f653ada1a78b93697f3b5a8f1f2bc055b9"},
-    {file = "cffi-1.15.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3548db281cd7d2561c9ad9984681c95f7b0e38881201e157833a2342c30d5e8c"},
-    {file = "cffi-1.15.1-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:91fc98adde3d7881af9b59ed0294046f3806221863722ba7d8d120c575314325"},
-    {file = "cffi-1.15.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:94411f22c3985acaec6f83c6df553f2dbe17b698cc7f8ae751ff2237d96b9e3c"},
-    {file = "cffi-1.15.1-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef"},
-    {file = "cffi-1.15.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:cc4d65aeeaa04136a12677d3dd0b1c0c94dc43abac5860ab33cceb42b801c1e8"},
-    {file = "cffi-1.15.1-cp311-cp311-win32.whl", hash = "sha256:a0f100c8912c114ff53e1202d0078b425bee3649ae34d7b070e9697f93c5d52d"},
-    {file = "cffi-1.15.1-cp311-cp311-win_amd64.whl", hash = "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104"},
-    {file = "cffi-1.15.1-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:50a74364d85fd319352182ef59c5c790484a336f6db772c1a9231f1c3ed0cbd7"},
-    {file = "cffi-1.15.1-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6"},
-    {file = "cffi-1.15.1-cp36-cp36m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:cec7d9412a9102bdc577382c3929b337320c4c4c4849f2c5cdd14d7368c5562d"},
-    {file = "cffi-1.15.1-cp36-cp36m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:4289fc34b2f5316fbb762d75362931e351941fa95fa18789191b33fc4cf9504a"},
-    {file = "cffi-1.15.1-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405"},
-    {file = "cffi-1.15.1-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:6975a3fac6bc83c4a65c9f9fcab9e47019a11d3d2cf7f3c0d03431bf145a941e"},
-    {file = "cffi-1.15.1-cp36-cp36m-win32.whl", hash = "sha256:2470043b93ff09bf8fb1d46d1cb756ce6132c54826661a32d4e4d132e1977adf"},
-    {file = "cffi-1.15.1-cp36-cp36m-win_amd64.whl", hash = "sha256:30d78fbc8ebf9c92c9b7823ee18eb92f2e6ef79b45ac84db507f52fbe3ec4497"},
-    {file = "cffi-1.15.1-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:198caafb44239b60e252492445da556afafc7d1e3ab7a1fb3f0584ef6d742375"},
-    {file = "cffi-1.15.1-cp37-cp37m-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:5ef34d190326c3b1f822a5b7a45f6c4535e2f47ed06fec77d3d799c450b2651e"},
-    {file = "cffi-1.15.1-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8102eaf27e1e448db915d08afa8b41d6c7ca7a04b7d73af6514df10a3e74bd82"},
-    {file = "cffi-1.15.1-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:5df2768244d19ab7f60546d0c7c63ce1581f7af8b5de3eb3004b9b6fc8a9f84b"},
-    {file = "cffi-1.15.1-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:a8c4917bd7ad33e8eb21e9a5bbba979b49d9a97acb3a803092cbc1133e20343c"},
-    {file = "cffi-1.15.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426"},
-    {file = "cffi-1.15.1-cp37-cp37m-win32.whl", hash = "sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9"},
-    {file = "cffi-1.15.1-cp37-cp37m-win_amd64.whl", hash = "sha256:a0b71b1b8fbf2b96e41c4d990244165e2c9be83d54962a9a1d118fd8657d2045"},
-    {file = "cffi-1.15.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:320dab6e7cb2eacdf0e658569d2575c4dad258c0fcc794f46215e1e39f90f2c3"},
-    {file = "cffi-1.15.1-cp38-cp38-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1e74c6b51a9ed6589199c787bf5f9875612ca4a8a0785fb2d4a84429badaf22a"},
-    {file = "cffi-1.15.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a5c84c68147988265e60416b57fc83425a78058853509c1b0629c180094904a5"},
-    {file = "cffi-1.15.1-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:3b926aa83d1edb5aa5b427b4053dc420ec295a08e40911296b9eb1b6170f6cca"},
-    {file = "cffi-1.15.1-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:87c450779d0914f2861b8526e035c5e6da0a3199d8f1add1a665e1cbc6fc6d02"},
-    {file = "cffi-1.15.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4f2c9f67e9821cad2e5f480bc8d83b8742896f1242dba247911072d4fa94c192"},
-    {file = "cffi-1.15.1-cp38-cp38-win32.whl", hash = "sha256:8b7ee99e510d7b66cdb6c593f21c043c248537a32e0bedf02e01e9553a172314"},
-    {file = "cffi-1.15.1-cp38-cp38-win_amd64.whl", hash = "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5"},
-    {file = "cffi-1.15.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:54a2db7b78338edd780e7ef7f9f6c442500fb0d41a5a4ea24fff1c929d5af585"},
-    {file = "cffi-1.15.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"},
-    {file = "cffi-1.15.1-cp39-cp39-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7473e861101c9e72452f9bf8acb984947aa1661a7704553a9f6e4baa5ba64415"},
-    {file = "cffi-1.15.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6c9a799e985904922a4d207a94eae35c78ebae90e128f0c4e521ce339396be9d"},
-    {file = "cffi-1.15.1-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:3bcde07039e586f91b45c88f8583ea7cf7a0770df3a1649627bf598332cb6984"},
-    {file = "cffi-1.15.1-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:33ab79603146aace82c2427da5ca6e58f2b3f2fb5da893ceac0c42218a40be35"},
-    {file = "cffi-1.15.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5d598b938678ebf3c67377cdd45e09d431369c3b1a5b331058c338e201f12b27"},
-    {file = "cffi-1.15.1-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:db0fbb9c62743ce59a9ff687eb5f4afbe77e5e8403d6697f7446e5f609976f76"},
-    {file = "cffi-1.15.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:98d85c6a2bef81588d9227dde12db8a7f47f639f4a17c9ae08e773aa9c697bf3"},
-    {file = "cffi-1.15.1-cp39-cp39-win32.whl", hash = "sha256:40f4774f5a9d4f5e344f31a32b5096977b5d48560c5592e2f3d2c4374bd543ee"},
-    {file = "cffi-1.15.1-cp39-cp39-win_amd64.whl", hash = "sha256:70df4e3b545a17496c9b3f41f5115e69a4f2e77e94e1d2a8e1070bc0c38c8a3c"},
-    {file = "cffi-1.15.1.tar.gz", hash = "sha256:d400bfb9a37b1351253cb402671cea7e89bdecc294e8016a707f6d1d8ac934f9"},
-]
-
-[package.dependencies]
-pycparser = "*"
-
-[[package]]
-name = "click"
-version = "8.1.3"
-description = "Composable command line interface toolkit"
-category = "main"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "click-8.1.3-py3-none-any.whl", hash = "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"},
-    {file = "click-8.1.3.tar.gz", hash = "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e"},
-]
-
-[package.dependencies]
-colorama = {version = "*", markers = "platform_system == \"Windows\""}
-importlib-metadata = {version = "*", markers = "python_version < \"3.8\""}
-
-[[package]]
-name = "colorama"
-version = "0.4.6"
-description = "Cross-platform colored terminal text."
-category = "main"
-optional = false
-python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*,>=2.7"
-files = [
-    {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
-    {file = "colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
-]
-
-[[package]]
-name = "cryptography"
-version = "40.0.1"
-description = "cryptography is a package which provides cryptographic recipes and primitives to Python developers."
-category = "main"
-optional = false
-python-versions = ">=3.6"
-files = [
-    {file = "cryptography-40.0.1-cp36-abi3-macosx_10_12_universal2.whl", hash = "sha256:918cb89086c7d98b1b86b9fdb70c712e5a9325ba6f7d7cfb509e784e0cfc6917"},
-    {file = "cryptography-40.0.1-cp36-abi3-macosx_10_12_x86_64.whl", hash = "sha256:9618a87212cb5200500e304e43691111570e1f10ec3f35569fdfcd17e28fd797"},
-    {file = "cryptography-40.0.1-cp36-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3a4805a4ca729d65570a1b7cac84eac1e431085d40387b7d3bbaa47e39890b88"},
-    {file = "cryptography-40.0.1-cp36-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:63dac2d25c47f12a7b8aa60e528bfb3c51c5a6c5a9f7c86987909c6c79765554"},
-    {file = "cryptography-40.0.1-cp36-abi3-manylinux_2_28_aarch64.whl", hash = "sha256:0a4e3406cfed6b1f6d6e87ed243363652b2586b2d917b0609ca4f97072994405"},
-    {file = "cryptography-40.0.1-cp36-abi3-manylinux_2_28_x86_64.whl", hash = "sha256:1e0af458515d5e4028aad75f3bb3fe7a31e46ad920648cd59b64d3da842e4356"},
-    {file = "cryptography-40.0.1-cp36-abi3-musllinux_1_1_aarch64.whl", hash = "sha256:d8aa3609d337ad85e4eb9bb0f8bcf6e4409bfb86e706efa9a027912169e89122"},
-    {file = "cryptography-40.0.1-cp36-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:cf91e428c51ef692b82ce786583e214f58392399cf65c341bc7301d096fa3ba2"},
-    {file = "cryptography-40.0.1-cp36-abi3-win32.whl", hash = "sha256:650883cc064297ef3676b1db1b7b1df6081794c4ada96fa457253c4cc40f97db"},
-    {file = "cryptography-40.0.1-cp36-abi3-win_amd64.whl", hash = "sha256:a805a7bce4a77d51696410005b3e85ae2839bad9aa38894afc0aa99d8e0c3160"},
-    {file = "cryptography-40.0.1-pp38-pypy38_pp73-macosx_10_12_x86_64.whl", hash = "sha256:cd033d74067d8928ef00a6b1327c8ea0452523967ca4463666eeba65ca350d4c"},
-    {file = "cryptography-40.0.1-pp38-pypy38_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:d36bbeb99704aabefdca5aee4eba04455d7a27ceabd16f3b3ba9bdcc31da86c4"},
-    {file = "cryptography-40.0.1-pp38-pypy38_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:32057d3d0ab7d4453778367ca43e99ddb711770477c4f072a51b3ca69602780a"},
-    {file = "cryptography-40.0.1-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:f5d7b79fa56bc29580faafc2ff736ce05ba31feaa9d4735048b0de7d9ceb2b94"},
-    {file = "cryptography-40.0.1-pp39-pypy39_pp73-macosx_10_12_x86_64.whl", hash = "sha256:7c872413353c70e0263a9368c4993710070e70ab3e5318d85510cc91cce77e7c"},
-    {file = "cryptography-40.0.1-pp39-pypy39_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:28d63d75bf7ae4045b10de5413fb1d6338616e79015999ad9cf6fc538f772d41"},
-    {file = "cryptography-40.0.1-pp39-pypy39_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:6f2bbd72f717ce33100e6467572abaedc61f1acb87b8d546001328d7f466b778"},
-    {file = "cryptography-40.0.1-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:cc3a621076d824d75ab1e1e530e66e7e8564e357dd723f2533225d40fe35c60c"},
-    {file = "cryptography-40.0.1.tar.gz", hash = "sha256:2803f2f8b1e95f614419926c7e6f55d828afc614ca5ed61543877ae668cc3472"},
-]
-
-[package.dependencies]
-cffi = ">=1.12"
-
-[package.extras]
-docs = ["sphinx (>=5.3.0)", "sphinx-rtd-theme (>=1.1.1)"]
-docstest = ["pyenchant (>=1.6.11)", "sphinxcontrib-spelling (>=4.0.1)", "twine (>=1.12.0)"]
-pep8test = ["black", "check-manifest", "mypy", "ruff"]
-sdist = ["setuptools-rust (>=0.11.4)"]
-ssh = ["bcrypt (>=3.1.5)"]
-test = ["iso8601", "pretend", "pytest (>=6.2.0)", "pytest-benchmark", "pytest-cov", "pytest-shard (>=0.1.2)", "pytest-subtests", "pytest-xdist"]
-test-randomorder = ["pytest-randomly"]
-tox = ["tox"]
-
-[[package]]
-name = "fido2"
-version = "1.1.1-dev.0"
-description = "FIDO2/WebAuthn library for implementing clients and servers."
-category = "main"
-optional = false
-python-versions = "^3.7"
-files = []
-develop = false
-
-[package.dependencies]
-cryptography = ">=2.6, !=35, <43"
-
-[package.extras]
-pcsc = ["pyscard (>=1.9,<3)"]
-
-[package.source]
-type = "directory"
-url = "../.."
-
-[[package]]
-name = "flask"
-version = "2.2.3"
-description = "A simple framework for building complex web applications."
-category = "main"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "Flask-2.2.3-py3-none-any.whl", hash = "sha256:c0bec9477df1cb867e5a67c9e1ab758de9cb4a3e52dd70681f59fa40a62b3f2d"},
-    {file = "Flask-2.2.3.tar.gz", hash = "sha256:7eb373984bf1c770023fce9db164ed0c3353cd0b53f130f4693da0ca756a2e6d"},
-]
-
-[package.dependencies]
-click = ">=8.0"
-importlib-metadata = {version = ">=3.6.0", markers = "python_version < \"3.10\""}
-itsdangerous = ">=2.0"
-Jinja2 = ">=3.0"
-Werkzeug = ">=2.2.2"
-
-[package.extras]
-async = ["asgiref (>=3.2)"]
-dotenv = ["python-dotenv"]
-
-[[package]]
-name = "importlib-metadata"
-version = "6.1.0"
-description = "Read metadata from Python packages"
-category = "main"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "importlib_metadata-6.1.0-py3-none-any.whl", hash = "sha256:ff80f3b5394912eb1b108fcfd444dc78b7f1f3e16b16188054bd01cb9cb86f09"},
-    {file = "importlib_metadata-6.1.0.tar.gz", hash = "sha256:43ce9281e097583d758c2c708c4376371261a02c34682491a8e98352365aad20"},
-]
-
-[package.dependencies]
-typing-extensions = {version = ">=3.6.4", markers = "python_version < \"3.8\""}
-zipp = ">=0.5"
-
-[package.extras]
-docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
-perf = ["ipython"]
-testing = ["flake8 (<5)", "flufl.flake8", "importlib-resources (>=1.3)", "packaging", "pyfakefs", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)", "pytest-perf (>=0.9.2)"]
-
-[[package]]
-name = "itsdangerous"
-version = "2.1.2"
-description = "Safely pass data to untrusted environments and back."
-category = "main"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "itsdangerous-2.1.2-py3-none-any.whl", hash = "sha256:2c2349112351b88699d8d4b6b075022c0808887cb7ad10069318a8b0bc88db44"},
-    {file = "itsdangerous-2.1.2.tar.gz", hash = "sha256:5dbbc68b317e5e42f327f9021763545dc3fc3bfe22e6deb96aaf1fc38874156a"},
-]
-
-[[package]]
-name = "jinja2"
-version = "3.1.2"
-description = "A very fast and expressive template engine."
-category = "main"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "Jinja2-3.1.2-py3-none-any.whl", hash = "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"},
-    {file = "Jinja2-3.1.2.tar.gz", hash = "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852"},
-]
-
-[package.dependencies]
-MarkupSafe = ">=2.0"
-
-[package.extras]
-i18n = ["Babel (>=2.7)"]
-
-[[package]]
-name = "markupsafe"
-version = "2.1.2"
-description = "Safely add untrusted strings to HTML/XML markup."
-category = "main"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "MarkupSafe-2.1.2-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7"},
-    {file = "MarkupSafe-2.1.2-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036"},
-    {file = "MarkupSafe-2.1.2-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1"},
-    {file = "MarkupSafe-2.1.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323"},
-    {file = "MarkupSafe-2.1.2-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601"},
-    {file = "MarkupSafe-2.1.2-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1"},
-    {file = "MarkupSafe-2.1.2-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff"},
-    {file = "MarkupSafe-2.1.2-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65"},
-    {file = "MarkupSafe-2.1.2-cp310-cp310-win32.whl", hash = "sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603"},
-    {file = "MarkupSafe-2.1.2-cp310-cp310-win_amd64.whl", hash = "sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156"},
-    {file = "MarkupSafe-2.1.2-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013"},
-    {file = "MarkupSafe-2.1.2-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a"},
-    {file = "MarkupSafe-2.1.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd"},
-    {file = "MarkupSafe-2.1.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6"},
-    {file = "MarkupSafe-2.1.2-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d"},
-    {file = "MarkupSafe-2.1.2-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1"},
-    {file = "MarkupSafe-2.1.2-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc"},
-    {file = "MarkupSafe-2.1.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0"},
-    {file = "MarkupSafe-2.1.2-cp311-cp311-win32.whl", hash = "sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625"},
-    {file = "MarkupSafe-2.1.2-cp311-cp311-win_amd64.whl", hash = "sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3"},
-    {file = "MarkupSafe-2.1.2-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a"},
-    {file = "MarkupSafe-2.1.2-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a"},
-    {file = "MarkupSafe-2.1.2-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a"},
-    {file = "MarkupSafe-2.1.2-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2"},
-    {file = "MarkupSafe-2.1.2-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619"},
-    {file = "MarkupSafe-2.1.2-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513"},
-    {file = "MarkupSafe-2.1.2-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460"},
-    {file = "MarkupSafe-2.1.2-cp37-cp37m-win32.whl", hash = "sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859"},
-    {file = "MarkupSafe-2.1.2-cp37-cp37m-win_amd64.whl", hash = "sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666"},
-    {file = "MarkupSafe-2.1.2-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed"},
-    {file = "MarkupSafe-2.1.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094"},
-    {file = "MarkupSafe-2.1.2-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54"},
-    {file = "MarkupSafe-2.1.2-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419"},
-    {file = "MarkupSafe-2.1.2-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa"},
-    {file = "MarkupSafe-2.1.2-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58"},
-    {file = "MarkupSafe-2.1.2-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba"},
-    {file = "MarkupSafe-2.1.2-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03"},
-    {file = "MarkupSafe-2.1.2-cp38-cp38-win32.whl", hash = "sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2"},
-    {file = "MarkupSafe-2.1.2-cp38-cp38-win_amd64.whl", hash = "sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147"},
-    {file = "MarkupSafe-2.1.2-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f"},
-    {file = "MarkupSafe-2.1.2-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd"},
-    {file = "MarkupSafe-2.1.2-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f"},
-    {file = "MarkupSafe-2.1.2-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4"},
-    {file = "MarkupSafe-2.1.2-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2"},
-    {file = "MarkupSafe-2.1.2-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65"},
-    {file = "MarkupSafe-2.1.2-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c"},
-    {file = "MarkupSafe-2.1.2-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3"},
-    {file = "MarkupSafe-2.1.2-cp39-cp39-win32.whl", hash = "sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7"},
-    {file = "MarkupSafe-2.1.2-cp39-cp39-win_amd64.whl", hash = "sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed"},
-    {file = "MarkupSafe-2.1.2.tar.gz", hash = "sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d"},
-]
-
-[[package]]
-name = "pycparser"
-version = "2.21"
-description = "C parser in Python"
-category = "main"
-optional = false
-python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
-files = [
-    {file = "pycparser-2.21-py2.py3-none-any.whl", hash = "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9"},
-    {file = "pycparser-2.21.tar.gz", hash = "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"},
-]
-
-[[package]]
-name = "typing-extensions"
-version = "4.5.0"
-description = "Backported and Experimental Type Hints for Python 3.7+"
-category = "main"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "typing_extensions-4.5.0-py3-none-any.whl", hash = "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"},
-    {file = "typing_extensions-4.5.0.tar.gz", hash = "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb"},
-]
-
-[[package]]
-name = "werkzeug"
-version = "2.2.3"
-description = "The comprehensive WSGI web application library."
-category = "main"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "Werkzeug-2.2.3-py3-none-any.whl", hash = "sha256:56433961bc1f12533306c624f3be5e744389ac61d722175d543e1751285da612"},
-    {file = "Werkzeug-2.2.3.tar.gz", hash = "sha256:2e1ccc9417d4da358b9de6f174e3ac094391ea1d4fbef2d667865d819dfd0afe"},
-]
-
-[package.dependencies]
-MarkupSafe = ">=2.1.1"
-
-[package.extras]
-watchdog = ["watchdog"]
-
-[[package]]
-name = "zipp"
-version = "3.15.0"
-description = "Backport of pathlib-compatible object wrapper for zip files"
-category = "main"
-optional = false
-python-versions = ">=3.7"
-files = [
-    {file = "zipp-3.15.0-py3-none-any.whl", hash = "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"},
-    {file = "zipp-3.15.0.tar.gz", hash = "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b"},
-]
-
-[package.extras]
-docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
-testing = ["big-O", "flake8 (<5)", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
-
-[metadata]
-lock-version = "2.0"
-python-versions = "^3.7"
-content-hash = "d21c95e6be38b286b3aa30ae191c220faf68523b4fcfddc46e81c694952d7f73"
+# This file is automatically @generated by Poetry 1.4.1 and should not be changed by hand.
+
+[[package]]
+name = "cffi"
+version = "1.15.1"
+description = "Foreign Function Interface for Python calling C code."
+category = "main"
+optional = false
+python-versions = "*"
+files = [
+    {file = "cffi-1.15.1-cp27-cp27m-macosx_10_9_x86_64.whl", hash = "sha256:a66d3508133af6e8548451b25058d5812812ec3798c886bf38ed24a98216fab2"},
+    {file = "cffi-1.15.1-cp27-cp27m-manylinux1_i686.whl", hash = "sha256:470c103ae716238bbe698d67ad020e1db9d9dba34fa5a899b5e21577e6d52ed2"},
+    {file = "cffi-1.15.1-cp27-cp27m-manylinux1_x86_64.whl", hash = "sha256:9ad5db27f9cabae298d151c85cf2bad1d359a1b9c686a275df03385758e2f914"},
+    {file = "cffi-1.15.1-cp27-cp27m-win32.whl", hash = "sha256:b3bbeb01c2b273cca1e1e0c5df57f12dce9a4dd331b4fa1635b8bec26350bde3"},
+    {file = "cffi-1.15.1-cp27-cp27m-win_amd64.whl", hash = "sha256:e00b098126fd45523dd056d2efba6c5a63b71ffe9f2bbe1a4fe1716e1d0c331e"},
+    {file = "cffi-1.15.1-cp27-cp27mu-manylinux1_i686.whl", hash = "sha256:d61f4695e6c866a23a21acab0509af1cdfd2c013cf256bbf5b6b5e2695827162"},
+    {file = "cffi-1.15.1-cp27-cp27mu-manylinux1_x86_64.whl", hash = "sha256:ed9cb427ba5504c1dc15ede7d516b84757c3e3d7868ccc85121d9310d27eed0b"},
+    {file = "cffi-1.15.1-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:39d39875251ca8f612b6f33e6b1195af86d1b3e60086068be9cc053aa4376e21"},
+    {file = "cffi-1.15.1-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:285d29981935eb726a4399badae8f0ffdff4f5050eaa6d0cfc3f64b857b77185"},
+    {file = "cffi-1.15.1-cp310-cp310-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:3eb6971dcff08619f8d91607cfc726518b6fa2a9eba42856be181c6d0d9515fd"},
+    {file = "cffi-1.15.1-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:21157295583fe8943475029ed5abdcf71eb3911894724e360acff1d61c1d54bc"},
+    {file = "cffi-1.15.1-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:5635bd9cb9731e6d4a1132a498dd34f764034a8ce60cef4f5319c0541159392f"},
+    {file = "cffi-1.15.1-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:2012c72d854c2d03e45d06ae57f40d78e5770d252f195b93f581acf3ba44496e"},
+    {file = "cffi-1.15.1-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:dd86c085fae2efd48ac91dd7ccffcfc0571387fe1193d33b6394db7ef31fe2a4"},
+    {file = "cffi-1.15.1-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:fa6693661a4c91757f4412306191b6dc88c1703f780c8234035eac011922bc01"},
+    {file = "cffi-1.15.1-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:59c0b02d0a6c384d453fece7566d1c7e6b7bae4fc5874ef2ef46d56776d61c9e"},
+    {file = "cffi-1.15.1-cp310-cp310-win32.whl", hash = "sha256:cba9d6b9a7d64d4bd46167096fc9d2f835e25d7e4c121fb2ddfc6528fb0413b2"},
+    {file = "cffi-1.15.1-cp310-cp310-win_amd64.whl", hash = "sha256:ce4bcc037df4fc5e3d184794f27bdaab018943698f4ca31630bc7f84a7b69c6d"},
+    {file = "cffi-1.15.1-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:3d08afd128ddaa624a48cf2b859afef385b720bb4b43df214f85616922e6a5ac"},
+    {file = "cffi-1.15.1-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:3799aecf2e17cf585d977b780ce79ff0dc9b78d799fc694221ce814c2c19db83"},
+    {file = "cffi-1.15.1-cp311-cp311-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a591fe9e525846e4d154205572a029f653ada1a78b93697f3b5a8f1f2bc055b9"},
+    {file = "cffi-1.15.1-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:3548db281cd7d2561c9ad9984681c95f7b0e38881201e157833a2342c30d5e8c"},
+    {file = "cffi-1.15.1-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:91fc98adde3d7881af9b59ed0294046f3806221863722ba7d8d120c575314325"},
+    {file = "cffi-1.15.1-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:94411f22c3985acaec6f83c6df553f2dbe17b698cc7f8ae751ff2237d96b9e3c"},
+    {file = "cffi-1.15.1-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef"},
+    {file = "cffi-1.15.1-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:cc4d65aeeaa04136a12677d3dd0b1c0c94dc43abac5860ab33cceb42b801c1e8"},
+    {file = "cffi-1.15.1-cp311-cp311-win32.whl", hash = "sha256:a0f100c8912c114ff53e1202d0078b425bee3649ae34d7b070e9697f93c5d52d"},
+    {file = "cffi-1.15.1-cp311-cp311-win_amd64.whl", hash = "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104"},
+    {file = "cffi-1.15.1-cp36-cp36m-macosx_10_9_x86_64.whl", hash = "sha256:50a74364d85fd319352182ef59c5c790484a336f6db772c1a9231f1c3ed0cbd7"},
+    {file = "cffi-1.15.1-cp36-cp36m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:e263d77ee3dd201c3a142934a086a4450861778baaeeb45db4591ef65550b0a6"},
+    {file = "cffi-1.15.1-cp36-cp36m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:cec7d9412a9102bdc577382c3929b337320c4c4c4849f2c5cdd14d7368c5562d"},
+    {file = "cffi-1.15.1-cp36-cp36m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:4289fc34b2f5316fbb762d75362931e351941fa95fa18789191b33fc4cf9504a"},
+    {file = "cffi-1.15.1-cp36-cp36m-manylinux_2_5_i686.manylinux1_i686.whl", hash = "sha256:173379135477dc8cac4bc58f45db08ab45d228b3363adb7af79436135d028405"},
+    {file = "cffi-1.15.1-cp36-cp36m-manylinux_2_5_x86_64.manylinux1_x86_64.whl", hash = "sha256:6975a3fac6bc83c4a65c9f9fcab9e47019a11d3d2cf7f3c0d03431bf145a941e"},
+    {file = "cffi-1.15.1-cp36-cp36m-win32.whl", hash = "sha256:2470043b93ff09bf8fb1d46d1cb756ce6132c54826661a32d4e4d132e1977adf"},
+    {file = "cffi-1.15.1-cp36-cp36m-win_amd64.whl", hash = "sha256:30d78fbc8ebf9c92c9b7823ee18eb92f2e6ef79b45ac84db507f52fbe3ec4497"},
+    {file = "cffi-1.15.1-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:198caafb44239b60e252492445da556afafc7d1e3ab7a1fb3f0584ef6d742375"},
+    {file = "cffi-1.15.1-cp37-cp37m-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:5ef34d190326c3b1f822a5b7a45f6c4535e2f47ed06fec77d3d799c450b2651e"},
+    {file = "cffi-1.15.1-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8102eaf27e1e448db915d08afa8b41d6c7ca7a04b7d73af6514df10a3e74bd82"},
+    {file = "cffi-1.15.1-cp37-cp37m-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:5df2768244d19ab7f60546d0c7c63ce1581f7af8b5de3eb3004b9b6fc8a9f84b"},
+    {file = "cffi-1.15.1-cp37-cp37m-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:a8c4917bd7ad33e8eb21e9a5bbba979b49d9a97acb3a803092cbc1133e20343c"},
+    {file = "cffi-1.15.1-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426"},
+    {file = "cffi-1.15.1-cp37-cp37m-win32.whl", hash = "sha256:e229a521186c75c8ad9490854fd8bbdd9a0c9aa3a524326b55be83b54d4e0ad9"},
+    {file = "cffi-1.15.1-cp37-cp37m-win_amd64.whl", hash = "sha256:a0b71b1b8fbf2b96e41c4d990244165e2c9be83d54962a9a1d118fd8657d2045"},
+    {file = "cffi-1.15.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:320dab6e7cb2eacdf0e658569d2575c4dad258c0fcc794f46215e1e39f90f2c3"},
+    {file = "cffi-1.15.1-cp38-cp38-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:1e74c6b51a9ed6589199c787bf5f9875612ca4a8a0785fb2d4a84429badaf22a"},
+    {file = "cffi-1.15.1-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:a5c84c68147988265e60416b57fc83425a78058853509c1b0629c180094904a5"},
+    {file = "cffi-1.15.1-cp38-cp38-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:3b926aa83d1edb5aa5b427b4053dc420ec295a08e40911296b9eb1b6170f6cca"},
+    {file = "cffi-1.15.1-cp38-cp38-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:87c450779d0914f2861b8526e035c5e6da0a3199d8f1add1a665e1cbc6fc6d02"},
+    {file = "cffi-1.15.1-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:4f2c9f67e9821cad2e5f480bc8d83b8742896f1242dba247911072d4fa94c192"},
+    {file = "cffi-1.15.1-cp38-cp38-win32.whl", hash = "sha256:8b7ee99e510d7b66cdb6c593f21c043c248537a32e0bedf02e01e9553a172314"},
+    {file = "cffi-1.15.1-cp38-cp38-win_amd64.whl", hash = "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5"},
+    {file = "cffi-1.15.1-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:54a2db7b78338edd780e7ef7f9f6c442500fb0d41a5a4ea24fff1c929d5af585"},
+    {file = "cffi-1.15.1-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:fcd131dd944808b5bdb38e6f5b53013c5aa4f334c5cad0c72742f6eba4b73db0"},
+    {file = "cffi-1.15.1-cp39-cp39-manylinux_2_12_i686.manylinux2010_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7473e861101c9e72452f9bf8acb984947aa1661a7704553a9f6e4baa5ba64415"},
+    {file = "cffi-1.15.1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:6c9a799e985904922a4d207a94eae35c78ebae90e128f0c4e521ce339396be9d"},
+    {file = "cffi-1.15.1-cp39-cp39-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:3bcde07039e586f91b45c88f8583ea7cf7a0770df3a1649627bf598332cb6984"},
+    {file = "cffi-1.15.1-cp39-cp39-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:33ab79603146aace82c2427da5ca6e58f2b3f2fb5da893ceac0c42218a40be35"},
+    {file = "cffi-1.15.1-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5d598b938678ebf3c67377cdd45e09d431369c3b1a5b331058c338e201f12b27"},
+    {file = "cffi-1.15.1-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:db0fbb9c62743ce59a9ff687eb5f4afbe77e5e8403d6697f7446e5f609976f76"},
+    {file = "cffi-1.15.1-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:98d85c6a2bef81588d9227dde12db8a7f47f639f4a17c9ae08e773aa9c697bf3"},
+    {file = "cffi-1.15.1-cp39-cp39-win32.whl", hash = "sha256:40f4774f5a9d4f5e344f31a32b5096977b5d48560c5592e2f3d2c4374bd543ee"},
+    {file = "cffi-1.15.1-cp39-cp39-win_amd64.whl", hash = "sha256:70df4e3b545a17496c9b3f41f5115e69a4f2e77e94e1d2a8e1070bc0c38c8a3c"},
+    {file = "cffi-1.15.1.tar.gz", hash = "sha256:d400bfb9a37b1351253cb402671cea7e89bdecc294e8016a707f6d1d8ac934f9"},
+]
+
+[package.dependencies]
+pycparser = "*"
+
+[[package]]
+name = "click"
+version = "8.1.3"
+description = "Composable command line interface toolkit"
+category = "main"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "click-8.1.3-py3-none-any.whl", hash = "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"},
+    {file = "click-8.1.3.tar.gz", hash = "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e"},
+]
+
+[package.dependencies]
+colorama = {version = "*", markers = "platform_system == \"Windows\""}
+importlib-metadata = {version = "*", markers = "python_version < \"3.8\""}
+
+[[package]]
+name = "colorama"
+version = "0.4.6"
+description = "Cross-platform colored terminal text."
+category = "main"
+optional = false
+python-versions = "!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*,!=3.6.*,>=2.7"
+files = [
+    {file = "colorama-0.4.6-py2.py3-none-any.whl", hash = "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"},
+    {file = "colorama-0.4.6.tar.gz", hash = "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44"},
+]
+
+[[package]]
+name = "cryptography"
+version = "41.0.1"
+description = "cryptography is a package which provides cryptographic recipes and primitives to Python developers."
+category = "main"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "cryptography-41.0.1-cp37-abi3-macosx_10_12_universal2.whl", hash = "sha256:f73bff05db2a3e5974a6fd248af2566134d8981fd7ab012e5dd4ddb1d9a70699"},
+    {file = "cryptography-41.0.1-cp37-abi3-macosx_10_12_x86_64.whl", hash = "sha256:1a5472d40c8f8e91ff7a3d8ac6dfa363d8e3138b961529c996f3e2df0c7a411a"},
+    {file = "cryptography-41.0.1-cp37-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7fa01527046ca5facdf973eef2535a27fec4cb651e4daec4d043ef63f6ecd4ca"},
+    {file = "cryptography-41.0.1-cp37-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b46e37db3cc267b4dea1f56da7346c9727e1209aa98487179ee8ebed09d21e43"},
+    {file = "cryptography-41.0.1-cp37-abi3-manylinux_2_28_aarch64.whl", hash = "sha256:d198820aba55660b4d74f7b5fd1f17db3aa5eb3e6893b0a41b75e84e4f9e0e4b"},
+    {file = "cryptography-41.0.1-cp37-abi3-manylinux_2_28_x86_64.whl", hash = "sha256:948224d76c4b6457349d47c0c98657557f429b4e93057cf5a2f71d603e2fc3a3"},
+    {file = "cryptography-41.0.1-cp37-abi3-musllinux_1_1_aarch64.whl", hash = "sha256:059e348f9a3c1950937e1b5d7ba1f8e968508ab181e75fc32b879452f08356db"},
+    {file = "cryptography-41.0.1-cp37-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:b4ceb5324b998ce2003bc17d519080b4ec8d5b7b70794cbd2836101406a9be31"},
+    {file = "cryptography-41.0.1-cp37-abi3-win32.whl", hash = "sha256:8f4ab7021127a9b4323537300a2acfb450124b2def3756f64dc3a3d2160ee4b5"},
+    {file = "cryptography-41.0.1-cp37-abi3-win_amd64.whl", hash = "sha256:1fee5aacc7367487b4e22484d3c7e547992ed726d14864ee33c0176ae43b0d7c"},
+    {file = "cryptography-41.0.1-pp38-pypy38_pp73-macosx_10_12_x86_64.whl", hash = "sha256:9a6c7a3c87d595608a39980ebaa04d5a37f94024c9f24eb7d10262b92f739ddb"},
+    {file = "cryptography-41.0.1-pp38-pypy38_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:5d092fdfedaec4cbbffbf98cddc915ba145313a6fdaab83c6e67f4e6c218e6f3"},
+    {file = "cryptography-41.0.1-pp38-pypy38_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:1a8e6c2de6fbbcc5e14fd27fb24414507cb3333198ea9ab1258d916f00bc3039"},
+    {file = "cryptography-41.0.1-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:cb33ccf15e89f7ed89b235cff9d49e2e62c6c981a6061c9c8bb47ed7951190bc"},
+    {file = "cryptography-41.0.1-pp39-pypy39_pp73-macosx_10_12_x86_64.whl", hash = "sha256:5f0ff6e18d13a3de56f609dd1fd11470918f770c6bd5d00d632076c727d35485"},
+    {file = "cryptography-41.0.1-pp39-pypy39_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:7bfc55a5eae8b86a287747053140ba221afc65eb06207bedf6e019b8934b477c"},
+    {file = "cryptography-41.0.1-pp39-pypy39_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:eb8163f5e549a22888c18b0d53d6bb62a20510060a22fd5a995ec8a05268df8a"},
+    {file = "cryptography-41.0.1-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:8dde71c4169ec5ccc1087bb7521d54251c016f126f922ab2dfe6649170a3b8c5"},
+    {file = "cryptography-41.0.1.tar.gz", hash = "sha256:d34579085401d3f49762d2f7d6634d6b6c2ae1242202e860f4d26b046e3a1006"},
+]
+
+[package.dependencies]
+cffi = ">=1.12"
+
+[package.extras]
+docs = ["sphinx (>=5.3.0)", "sphinx-rtd-theme (>=1.1.1)"]
+docstest = ["pyenchant (>=1.6.11)", "sphinxcontrib-spelling (>=4.0.1)", "twine (>=1.12.0)"]
+nox = ["nox"]
+pep8test = ["black", "check-sdist", "mypy", "ruff"]
+sdist = ["build"]
+ssh = ["bcrypt (>=3.1.5)"]
+test = ["pretend", "pytest (>=6.2.0)", "pytest-benchmark", "pytest-cov", "pytest-xdist"]
+test-randomorder = ["pytest-randomly"]
+
+[[package]]
+name = "fido2"
+version = "1.1.2-dev.0"
+description = "FIDO2/WebAuthn library for implementing clients and servers."
+category = "main"
+optional = false
+python-versions = "^3.7"
+files = []
+develop = false
+
+[package.dependencies]
+cryptography = ">=2.6, !=35, <44"
+
+[package.extras]
+pcsc = ["pyscard (>=1.9,<3)"]
+
+[package.source]
+type = "directory"
+url = "../.."
+
+[[package]]
+name = "flask"
+version = "2.2.5"
+description = "A simple framework for building complex web applications."
+category = "main"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "Flask-2.2.5-py3-none-any.whl", hash = "sha256:58107ed83443e86067e41eff4631b058178191a355886f8e479e347fa1285fdf"},
+    {file = "Flask-2.2.5.tar.gz", hash = "sha256:edee9b0a7ff26621bd5a8c10ff484ae28737a2410d99b0bb9a6850c7fb977aa0"},
+]
+
+[package.dependencies]
+click = ">=8.0"
+importlib-metadata = {version = ">=3.6.0", markers = "python_version < \"3.10\""}
+itsdangerous = ">=2.0"
+Jinja2 = ">=3.0"
+Werkzeug = ">=2.2.2"
+
+[package.extras]
+async = ["asgiref (>=3.2)"]
+dotenv = ["python-dotenv"]
+
+[[package]]
+name = "importlib-metadata"
+version = "6.7.0"
+description = "Read metadata from Python packages"
+category = "main"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "importlib_metadata-6.7.0-py3-none-any.whl", hash = "sha256:cb52082e659e97afc5dac71e79de97d8681de3aa07ff18578330904a9d18e5b5"},
+    {file = "importlib_metadata-6.7.0.tar.gz", hash = "sha256:1aaf550d4f73e5d6783e7acb77aec43d49da8017410afae93822cc9cca98c4d4"},
+]
+
+[package.dependencies]
+typing-extensions = {version = ">=3.6.4", markers = "python_version < \"3.8\""}
+zipp = ">=0.5"
+
+[package.extras]
+docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
+perf = ["ipython"]
+testing = ["flufl.flake8", "importlib-resources (>=1.3)", "packaging", "pyfakefs", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-mypy (>=0.9.1)", "pytest-perf (>=0.9.2)", "pytest-ruff"]
+
+[[package]]
+name = "itsdangerous"
+version = "2.1.2"
+description = "Safely pass data to untrusted environments and back."
+category = "main"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "itsdangerous-2.1.2-py3-none-any.whl", hash = "sha256:2c2349112351b88699d8d4b6b075022c0808887cb7ad10069318a8b0bc88db44"},
+    {file = "itsdangerous-2.1.2.tar.gz", hash = "sha256:5dbbc68b317e5e42f327f9021763545dc3fc3bfe22e6deb96aaf1fc38874156a"},
+]
+
+[[package]]
+name = "jinja2"
+version = "3.1.2"
+description = "A very fast and expressive template engine."
+category = "main"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "Jinja2-3.1.2-py3-none-any.whl", hash = "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"},
+    {file = "Jinja2-3.1.2.tar.gz", hash = "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852"},
+]
+
+[package.dependencies]
+MarkupSafe = ">=2.0"
+
+[package.extras]
+i18n = ["Babel (>=2.7)"]
+
+[[package]]
+name = "markupsafe"
+version = "2.1.3"
+description = "Safely add untrusted strings to HTML/XML markup."
+category = "main"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "MarkupSafe-2.1.3-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa"},
+    {file = "MarkupSafe-2.1.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57"},
+    {file = "MarkupSafe-2.1.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f"},
+    {file = "MarkupSafe-2.1.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52"},
+    {file = "MarkupSafe-2.1.3-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00"},
+    {file = "MarkupSafe-2.1.3-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6"},
+    {file = "MarkupSafe-2.1.3-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779"},
+    {file = "MarkupSafe-2.1.3-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7"},
+    {file = "MarkupSafe-2.1.3-cp310-cp310-win32.whl", hash = "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431"},
+    {file = "MarkupSafe-2.1.3-cp310-cp310-win_amd64.whl", hash = "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559"},
+    {file = "MarkupSafe-2.1.3-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c"},
+    {file = "MarkupSafe-2.1.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575"},
+    {file = "MarkupSafe-2.1.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee"},
+    {file = "MarkupSafe-2.1.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2"},
+    {file = "MarkupSafe-2.1.3-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9"},
+    {file = "MarkupSafe-2.1.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc"},
+    {file = "MarkupSafe-2.1.3-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9"},
+    {file = "MarkupSafe-2.1.3-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac"},
+    {file = "MarkupSafe-2.1.3-cp311-cp311-win32.whl", hash = "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb"},
+    {file = "MarkupSafe-2.1.3-cp311-cp311-win_amd64.whl", hash = "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686"},
+    {file = "MarkupSafe-2.1.3-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2"},
+    {file = "MarkupSafe-2.1.3-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b"},
+    {file = "MarkupSafe-2.1.3-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707"},
+    {file = "MarkupSafe-2.1.3-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e"},
+    {file = "MarkupSafe-2.1.3-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc"},
+    {file = "MarkupSafe-2.1.3-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48"},
+    {file = "MarkupSafe-2.1.3-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155"},
+    {file = "MarkupSafe-2.1.3-cp37-cp37m-win32.whl", hash = "sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0"},
+    {file = "MarkupSafe-2.1.3-cp37-cp37m-win_amd64.whl", hash = "sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24"},
+    {file = "MarkupSafe-2.1.3-cp38-cp38-macosx_10_9_universal2.whl", hash = "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4"},
+    {file = "MarkupSafe-2.1.3-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0"},
+    {file = "MarkupSafe-2.1.3-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee"},
+    {file = "MarkupSafe-2.1.3-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be"},
+    {file = "MarkupSafe-2.1.3-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e"},
+    {file = "MarkupSafe-2.1.3-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8"},
+    {file = "MarkupSafe-2.1.3-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3"},
+    {file = "MarkupSafe-2.1.3-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d"},
+    {file = "MarkupSafe-2.1.3-cp38-cp38-win32.whl", hash = "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5"},
+    {file = "MarkupSafe-2.1.3-cp38-cp38-win_amd64.whl", hash = "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc"},
+    {file = "MarkupSafe-2.1.3-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198"},
+    {file = "MarkupSafe-2.1.3-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b"},
+    {file = "MarkupSafe-2.1.3-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58"},
+    {file = "MarkupSafe-2.1.3-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e"},
+    {file = "MarkupSafe-2.1.3-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c"},
+    {file = "MarkupSafe-2.1.3-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636"},
+    {file = "MarkupSafe-2.1.3-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea"},
+    {file = "MarkupSafe-2.1.3-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e"},
+    {file = "MarkupSafe-2.1.3-cp39-cp39-win32.whl", hash = "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"},
+    {file = "MarkupSafe-2.1.3-cp39-cp39-win_amd64.whl", hash = "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba"},
+    {file = "MarkupSafe-2.1.3.tar.gz", hash = "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad"},
+]
+
+[[package]]
+name = "pycparser"
+version = "2.21"
+description = "C parser in Python"
+category = "main"
+optional = false
+python-versions = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*"
+files = [
+    {file = "pycparser-2.21-py2.py3-none-any.whl", hash = "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9"},
+    {file = "pycparser-2.21.tar.gz", hash = "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"},
+]
+
+[[package]]
+name = "typing-extensions"
+version = "4.7.1"
+description = "Backported and Experimental Type Hints for Python 3.7+"
+category = "main"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "typing_extensions-4.7.1-py3-none-any.whl", hash = "sha256:440d5dd3af93b060174bf433bccd69b0babc3b15b1a8dca43789fd7f61514b36"},
+    {file = "typing_extensions-4.7.1.tar.gz", hash = "sha256:b75ddc264f0ba5615db7ba217daeb99701ad295353c45f9e95963337ceeeffb2"},
+]
+
+[[package]]
+name = "werkzeug"
+version = "2.2.3"
+description = "The comprehensive WSGI web application library."
+category = "main"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "Werkzeug-2.2.3-py3-none-any.whl", hash = "sha256:56433961bc1f12533306c624f3be5e744389ac61d722175d543e1751285da612"},
+    {file = "Werkzeug-2.2.3.tar.gz", hash = "sha256:2e1ccc9417d4da358b9de6f174e3ac094391ea1d4fbef2d667865d819dfd0afe"},
+]
+
+[package.dependencies]
+MarkupSafe = ">=2.1.1"
+
+[package.extras]
+watchdog = ["watchdog"]
+
+[[package]]
+name = "zipp"
+version = "3.15.0"
+description = "Backport of pathlib-compatible object wrapper for zip files"
+category = "main"
+optional = false
+python-versions = ">=3.7"
+files = [
+    {file = "zipp-3.15.0-py3-none-any.whl", hash = "sha256:48904fc76a60e542af151aded95726c1a5c34ed43ab4134b597665c86d7ad556"},
+    {file = "zipp-3.15.0.tar.gz", hash = "sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b"},
+]
+
+[package.extras]
+docs = ["furo", "jaraco.packaging (>=9)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
+testing = ["big-O", "flake8 (<5)", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=1.3)", "pytest-flake8", "pytest-mypy (>=0.9.1)"]
+
+[metadata]
+lock-version = "2.0"
+python-versions = "^3.7"
+content-hash = "d21c95e6be38b286b3aa30ae191c220faf68523b4fcfddc46e81c694952d7f73"
```

### Comparing `fido2-1.1.1/examples/server/README.adoc` & `fido2-1.1.2/examples/server/README.adoc`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/examples/server/server/server.py` & `fido2-1.1.2/examples/server/server/server.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/examples/server/server/static/authenticate.html` & `fido2-1.1.2/examples/server/server/static/authenticate.html`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/examples/server/server/static/index.html` & `fido2-1.1.2/examples/server/server/static/index.html`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/examples/server/server/static/register.html` & `fido2-1.1.2/examples/server/server/static/register.html`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/examples/server/server/static/webauthn-json.browser-ponyfill.js` & `fido2-1.1.2/examples/server/server/static/webauthn-json.browser-ponyfill.js`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/examples/server/server/static/webauthn-json.browser-ponyfill.js.map` & `fido2-1.1.2/examples/server/server/static/webauthn-json.browser-ponyfill.js.map`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/examples/u2f_nfc.py` & `fido2-1.1.2/examples/u2f_nfc.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/examples/verify_attestation.py` & `fido2-1.1.2/examples/verify_attestation.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/examples/verify_attestation_mds3.py` & `fido2-1.1.2/examples/verify_attestation_mds3.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/__init__.py` & `fido2-1.1.2/fido2/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# Copyright (c) 2013 Yubico AB
-# All rights reserved.
-#
-#   Redistribution and use in source and binary forms, with or
-#   without modification, are permitted provided that the following
-#   conditions are met:
-#
-#    1. Redistributions of source code must retain the above copyright
-#       notice, this list of conditions and the following disclaimer.
-#    2. Redistributions in binary form must reproduce the above
-#       copyright notice, this list of conditions and the following
-#       disclaimer in the documentation and/or other materials provided
-#       with the distribution.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
-# FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
-# COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
-# INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
-# BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
-# ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-# POSSIBILITY OF SUCH DAMAGE.
-
-
-__version__ = "1.1.1"
+# Copyright (c) 2013 Yubico AB
+# All rights reserved.
+#
+#   Redistribution and use in source and binary forms, with or
+#   without modification, are permitted provided that the following
+#   conditions are met:
+#
+#    1. Redistributions of source code must retain the above copyright
+#       notice, this list of conditions and the following disclaimer.
+#    2. Redistributions in binary form must reproduce the above
+#       copyright notice, this list of conditions and the following
+#       disclaimer in the documentation and/or other materials provided
+#       with the distribution.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
+# FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
+# COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
+# INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
+# BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
+# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
+# ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+# POSSIBILITY OF SUCH DAMAGE.
+
+
+__version__ = "1.1.2"
```

### Comparing `fido2-1.1.1/fido2/attestation/__init__.py` & `fido2-1.1.2/fido2/attestation/__init__.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/attestation/android.py` & `fido2-1.1.2/fido2/attestation/android.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/attestation/apple.py` & `fido2-1.1.2/fido2/attestation/apple.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/attestation/base.py` & `fido2-1.1.2/fido2/attestation/base.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/attestation/packed.py` & `fido2-1.1.2/fido2/attestation/packed.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/attestation/tpm.py` & `fido2-1.1.2/fido2/attestation/tpm.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/attestation/u2f.py` & `fido2-1.1.2/fido2/attestation/u2f.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/cbor.py` & `fido2-1.1.2/fido2/cbor.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/cose.py` & `fido2-1.1.2/fido2/cose.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/ctap.py` & `fido2-1.1.2/fido2/ctap.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/ctap1.py` & `fido2-1.1.2/fido2/ctap1.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/ctap2/__init__.py` & `fido2-1.1.2/fido2/ctap2/__init__.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/ctap2/base.py` & `fido2-1.1.2/fido2/ctap2/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     """
     return dict((i, v) for i, v in enumerate(params, 1) if v is not None)
 
 
 class _CborDataObject(_DataClassMapping[int]):
     @classmethod
     def _get_field_key(cls, field: Field) -> int:
-        return fields(cls).index(field) + 1
+        return fields(cls).index(field) + 1  # type: ignore
 
 
 @dataclass(eq=False, frozen=True)
 class Info(_CborDataObject):
     """Binary CBOR encoded response data returned by the CTAP2 GET_INFO command.
 
     :param _: The binary content of the Info data.
```

### Comparing `fido2-1.1.1/fido2/ctap2/bio.py` & `fido2-1.1.2/fido2/ctap2/bio.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/ctap2/blob.py` & `fido2-1.1.2/fido2/ctap2/blob.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/ctap2/config.py` & `fido2-1.1.2/fido2/ctap2/config.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/ctap2/credman.py` & `fido2-1.1.2/fido2/ctap2/credman.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/ctap2/extensions.py` & `fido2-1.1.2/fido2/ctap2/extensions.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/features.py` & `fido2-1.1.2/fido2/features.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/hid/__init__.py` & `fido2-1.1.2/fido2/hid/__init__.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/hid/base.py` & `fido2-1.1.2/fido2/hid/base.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/hid/linux.py` & `fido2-1.1.2/fido2/hid/linux.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/hid/macos.py` & `fido2-1.1.2/fido2/hid/macos.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/hid/netbsd.py` & `fido2-1.1.2/fido2/hid/netbsd.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/hid/openbsd.py` & `fido2-1.1.2/fido2/hid/openbsd.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/hid/windows.py` & `fido2-1.1.2/fido2/hid/windows.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/mds3.py` & `fido2-1.1.2/fido2/mds3.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/pcsc.py` & `fido2-1.1.2/fido2/pcsc.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/rpid.py` & `fido2-1.1.2/fido2/rpid.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/server.py` & `fido2-1.1.2/fido2/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,505 +1,504 @@
-# Copyright (c) 2018 Yubico AB
-# All rights reserved.
-#
-#   Redistribution and use in source and binary forms, with or
-#   without modification, are permitted provided that the following
-#   conditions are met:
-#
-#    1. Redistributions of source code must retain the above copyright
-#       notice, this list of conditions and the following disclaimer.
-#    2. Redistributions in binary form must reproduce the above
-#       copyright notice, this list of conditions and the following
-#       disclaimer in the documentation and/or other materials provided
-#       with the distribution.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
-# FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
-# COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
-# INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
-# BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
-# ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-# POSSIBILITY OF SUCH DAMAGE.
-
-from __future__ import annotations
-
-from .rpid import verify_rp_id
-from .cose import CoseKey
-from .utils import websafe_encode, websafe_decode
-from .webauthn import (
-    CollectedClientData,
-    AuthenticatorData,
-    AttestationObject,
-    AttestedCredentialData,
-    AttestationConveyancePreference,
-    PublicKeyCredentialRpEntity,
-    PublicKeyCredentialUserEntity,
-    AuthenticatorSelectionCriteria,
-    PublicKeyCredentialDescriptor,
-    PublicKeyCredentialType,
-    PublicKeyCredentialParameters,
-    PublicKeyCredentialCreationOptions,
-    PublicKeyCredentialRequestOptions,
-    UserVerificationRequirement,
-    ResidentKeyRequirement,
-    AuthenticatorAttachment,
-    RegistrationResponse,
-    AuthenticationResponse,
-    CredentialCreationOptions,
-    CredentialRequestOptions,
-)
-
-from cryptography.hazmat.primitives import constant_time
-from cryptography.exceptions import InvalidSignature as _InvalidSignature
-from dataclasses import replace
-from urllib.parse import urlparse
-from typing import Sequence, Mapping, Optional, Callable, Union, Tuple, Any, overload
-
-import os
-import logging
-
-logger = logging.getLogger(__name__)
-
-
-VerifyAttestation = Callable[[AttestationObject, bytes], None]
-VerifyOrigin = Callable[[str], bool]
-
-
-def _verify_origin_for_rp(rp_id: str) -> VerifyOrigin:
-    return lambda o: verify_rp_id(rp_id, o)
-
-
-def _validata_challenge(challenge: Optional[bytes]) -> bytes:
-    if challenge is None:
-        challenge = os.urandom(32)
-    else:
-        if not isinstance(challenge, bytes):
-            raise TypeError("Custom challenge must be of type 'bytes'.")
-        if len(challenge) < 16:
-            raise ValueError("Custom challenge length must be >= 16.")
-    return challenge
-
-
-def to_descriptor(
-    credential: AttestedCredentialData, transports=None
-) -> PublicKeyCredentialDescriptor:
-    """Converts an AttestedCredentialData to a PublicKeyCredentialDescriptor.
-
-    :param credential: AttestedCredentialData containing the credential ID to use.
-    :param transports: Optional list of AuthenticatorTransport strings to add to the
-        descriptor.
-    :return: A descriptor of the credential, for use with register_begin or
-        authenticate_begin.
-    :rtype: PublicKeyCredentialDescriptor
-    """
-    return PublicKeyCredentialDescriptor(
-        PublicKeyCredentialType.PUBLIC_KEY, credential.credential_id, transports
-    )
-
-
-def _wrap_credentials(
-    creds: Optional[
-        Sequence[Union[AttestedCredentialData, PublicKeyCredentialDescriptor]]
-    ],
-) -> Optional[Sequence[PublicKeyCredentialDescriptor]]:
-    if creds is None:
-        return None
-    return [
-        to_descriptor(c)
-        if isinstance(c, AttestedCredentialData)
-        else PublicKeyCredentialDescriptor.from_dict(c)
-        for c in creds
-    ]
-
-
-def _ignore_attestation(
-    attestation_object: AttestationObject, client_data_hash: bytes
-) -> None:
-    """Ignore attestation."""
-
-
-class Fido2Server:
-    """FIDO2 server.
-
-    :param rp: Relying party data as `PublicKeyCredentialRpEntity` instance.
-    :param attestation: (optional) Requirement on authenticator attestation.
-    :param verify_origin: (optional) Alternative function to validate an origin.
-    :param verify_attestation: (optional) function to validate attestation, which is
-        invoked with attestation_object and client_data_hash. It should return nothing
-        and raise an exception on failure. By default, attestation is ignored.
-        Attestation is also ignored if `attestation` is set to `none`.
-    """
-
-    def __init__(
-        self,
-        rp: PublicKeyCredentialRpEntity,
-        attestation: Optional[AttestationConveyancePreference] = None,
-        verify_origin: Optional[VerifyOrigin] = None,
-        verify_attestation: Optional[VerifyAttestation] = None,
-    ):
-        self.rp = PublicKeyCredentialRpEntity.from_dict(rp)
-        self._verify = verify_origin or _verify_origin_for_rp(self.rp.id)
-        self.timeout = None
-        self.attestation = AttestationConveyancePreference(attestation)
-        self.allowed_algorithms = [
-            PublicKeyCredentialParameters(PublicKeyCredentialType.PUBLIC_KEY, alg)
-            for alg in CoseKey.supported_algorithms()
-        ]
-        self._verify_attestation = verify_attestation or _ignore_attestation
-        logger.debug(f"Fido2Server initialized for RP: {self.rp}")
-
-    def register_begin(
-        self,
-        user: PublicKeyCredentialUserEntity,
-        credentials: Optional[
-            Sequence[Union[AttestedCredentialData, PublicKeyCredentialDescriptor]]
-        ] = None,
-        resident_key_requirement: Optional[ResidentKeyRequirement] = None,
-        user_verification: Optional[UserVerificationRequirement] = None,
-        authenticator_attachment: Optional[AuthenticatorAttachment] = None,
-        challenge: Optional[bytes] = None,
-        extensions=None,
-    ) -> Tuple[CredentialCreationOptions, Any]:
-        """Return a PublicKeyCredentialCreationOptions registration object and
-        the internal state dictionary that needs to be passed as is to the
-        corresponding `register_complete` call.
-
-        :param user: The dict containing the user data.
-        :param credentials: The list of previously registered credentials, these can be
-            of type AttestedCredentialData, or PublicKeyCredentialDescriptor.
-        :param resident_key_requirement: The desired RESIDENT_KEY_REQUIREMENT level.
-        :param user_verification: The desired USER_VERIFICATION level.
-        :param authenticator_attachment: The desired AUTHENTICATOR_ATTACHMENT
-            or None to not provide a preference (and get both types).
-        :param challenge: A custom challenge to sign and verify or None to use
-            OS-specific random bytes.
-        :return: Registration data, internal state."""
-        if not self.allowed_algorithms:
-            raise ValueError("Server has no allowed algorithms.")
-
-        challenge = _validata_challenge(challenge)
-        descriptors = _wrap_credentials(credentials)
-        state = self._make_internal_state(challenge, user_verification)
-        logger.debug(
-            "Starting new registration, existing credentials: "
-            + ", ".join(d.id.hex() for d in descriptors or [])
-        )
-
-        return (
-            CredentialCreationOptions(
-                PublicKeyCredentialCreationOptions(
-                    self.rp,
-                    user,
-                    challenge,
-                    self.allowed_algorithms,
-                    self.timeout,
-                    descriptors,
-                    AuthenticatorSelectionCriteria(
-                        authenticator_attachment,
-                        resident_key_requirement,
-                        user_verification,
-                    )
-                    if any(
-                        (
-                            authenticator_attachment,
-                            resident_key_requirement,
-                            user_verification,
-                        )
-                    )
-                    else None,
-                    self.attestation,
-                    extensions,
-                )
-            ),
-            state,
-        )
-
-    @overload
-    def register_complete(
-        self,
-        state,
-        response: Union[RegistrationResponse, Mapping[str, Any]],
-    ) -> AuthenticatorData:
-        pass
-
-    @overload
-    def register_complete(
-        self,
-        state,
-        client_data: CollectedClientData,
-        attestation_object: AttestationObject,
-    ) -> AuthenticatorData:
-        pass
-
-    def register_complete(self, state, *args, **kwargs):
-        """Verify the correctness of the registration data received from
-        the client.
-
-        :param state: The state data returned by the corresponding
-            `register_begin`.
-        :param client_data: The client data.
-        :param attestation_object: The attestation object.
-        :return: The authenticator data
-        """
-        response = None
-        if len(args) == 1 and not kwargs:
-            response = args[0]
-        elif set(kwargs) == {"response"} and not args:
-            response = kwargs["response"]
-        if response:
-            registration = RegistrationResponse.from_dict(response)
-            client_data = registration.response.client_data
-            attestation_object = registration.response.attestation_object
-        else:
-            names = ["client_data", "attestation_object"]
-            pos = dict(zip(names, args))
-            data = {**kwargs, **pos}
-            if set(kwargs) & set(pos) or set(data) != set(names):
-                raise TypeError("incorrect arguments passed to register_complete()")
-            client_data = data[names[0]]
-            attestation_object = data[names[1]]
-
-        if client_data.type != CollectedClientData.TYPE.CREATE:
-            raise ValueError("Incorrect type in CollectedClientData.")
-        if not self._verify(client_data.origin):
-            raise ValueError("Invalid origin in CollectedClientData.")
-        if not constant_time.bytes_eq(
-            websafe_decode(state["challenge"]), client_data.challenge
-        ):
-            raise ValueError("Wrong challenge in response.")
-        if not constant_time.bytes_eq(
-            self.rp.id_hash, attestation_object.auth_data.rp_id_hash
-        ):
-            raise ValueError("Wrong RP ID hash in response.")
-        if not attestation_object.auth_data.is_user_present():
-            raise ValueError("User Present flag not set.")
-
-        if (
-            state["user_verification"] == UserVerificationRequirement.REQUIRED
-            and not attestation_object.auth_data.is_user_verified()
-        ):
-            raise ValueError(
-                "User verification required, but User Verified flag not set."
-            )
-
-        if self.attestation not in (None, AttestationConveyancePreference.NONE):
-            logger.debug(f"Verifying attestation of type {attestation_object.fmt}")
-            self._verify_attestation(attestation_object, client_data.hash)
-        # We simply ignore attestation if self.attestation == 'none', as not all
-        # clients strip the attestation.
-
-        auth_data = attestation_object.auth_data
-        assert auth_data.credential_data is not None  # nosec
-        logger.info(
-            "New credential registered: "
-            + auth_data.credential_data.credential_id.hex()
-        )
-        return auth_data
-
-    def authenticate_begin(
-        self,
-        credentials: Optional[
-            Sequence[Union[AttestedCredentialData, PublicKeyCredentialDescriptor]]
-        ] = None,
-        user_verification: Optional[UserVerificationRequirement] = None,
-        challenge: Optional[bytes] = None,
-        extensions=None,
-    ) -> Tuple[CredentialRequestOptions, Any]:
-
-        """Return a PublicKeyCredentialRequestOptions assertion object and the internal
-        state dictionary that needs to be passed as is to the corresponding
-        `authenticate_complete` call.
-
-        :param credentials: The list of previously registered credentials, these can be
-            of type AttestedCredentialData, or PublicKeyCredentialDescriptor.
-        :param user_verification: The desired USER_VERIFICATION level.
-        :param challenge: A custom challenge to sign and verify or None to use
-            OS-specific random bytes.
-        :return: Assertion data, internal state."""
-        challenge = _validata_challenge(challenge)
-        descriptors = _wrap_credentials(credentials)
-        state = self._make_internal_state(challenge, user_verification)
-        if descriptors is None:
-            logger.debug("Starting new authentication without credentials")
-        else:
-            logger.debug(
-                "Starting new authentication, for credentials: "
-                + ", ".join(d.id.hex() for d in descriptors)
-            )
-
-        return (
-            CredentialRequestOptions(
-                PublicKeyCredentialRequestOptions(
-                    challenge,
-                    self.timeout,
-                    self.rp.id,
-                    descriptors,
-                    user_verification,
-                    extensions,
-                )
-            ),
-            state,
-        )
-
-    @overload
-    def authenticate_complete(
-        self,
-        state,
-        credentials: Sequence[AttestedCredentialData],
-        response: Union[AuthenticationResponse, Mapping[str, Any]],
-    ) -> AttestedCredentialData:
-        pass
-
-    @overload
-    def authenticate_complete(
-        self,
-        state,
-        credentials: Sequence[AttestedCredentialData],
-        credential_id: bytes,
-        client_data: CollectedClientData,
-        auth_data: AuthenticatorData,
-        signature: bytes,
-    ) -> AttestedCredentialData:
-        pass
-
-    def authenticate_complete(self, state, credentials, *args, **kwargs):
-        """Verify the correctness of the assertion data received from
-        the client.
-
-        :param state: The state data returned by the corresponding
-            `register_begin`.
-        :param credentials: The list of previously registered credentials.
-        :param credential_id: The credential id from the client response.
-        :param client_data: The client data.
-        :param auth_data: The authenticator data.
-        :param signature: The signature provided by the client."""
-
-        response = None
-        if len(args) == 1 and not kwargs:
-            response = args[0]
-        elif set(kwargs) == {"response"} and not args:
-            response = kwargs["response"]
-        if response:
-            authentication = AuthenticationResponse.from_dict(response)
-            credential_id = authentication.id
-            client_data = authentication.response.client_data
-            auth_data = authentication.response.authenticator_data
-            signature = authentication.response.signature
-        else:
-            names = ["credential_id", "client_data", "auth_data", "signature"]
-            pos = dict(zip(names, args))
-            data = {**kwargs, **pos}
-            if set(kwargs) & set(pos) or set(data) != set(names):
-                raise TypeError("incorrect arguments passed to authenticate_complete()")
-            credential_id = data[names[0]]
-            client_data = data[names[1]]
-            auth_data = data[names[2]]
-            signature = data[names[3]]
-
-        if client_data.type != CollectedClientData.TYPE.GET:
-            raise ValueError("Incorrect type in CollectedClientData.")
-        if not self._verify(client_data.origin):
-            raise ValueError("Invalid origin in CollectedClientData.")
-        if websafe_decode(state["challenge"]) != client_data.challenge:
-            raise ValueError("Wrong challenge in response.")
-        if not constant_time.bytes_eq(self.rp.id_hash, auth_data.rp_id_hash):
-            raise ValueError("Wrong RP ID hash in response.")
-        if not auth_data.is_user_present():
-            raise ValueError("User Present flag not set.")
-
-        if (
-            state["user_verification"] == UserVerificationRequirement.REQUIRED
-            and not auth_data.is_user_verified()
-        ):
-            raise ValueError(
-                "User verification required, but user verified flag not set."
-            )
-
-        for cred in credentials:
-            if cred.credential_id == credential_id:
-                try:
-                    cred.public_key.verify(auth_data + client_data.hash, signature)
-                except _InvalidSignature:
-                    raise ValueError("Invalid signature.")
-                logger.info(f"Credential authenticated: {credential_id.hex()}")
-                return cred
-        raise ValueError("Unknown credential ID.")
-
-    @staticmethod
-    def _make_internal_state(
-        challenge: bytes, user_verification: Optional[UserVerificationRequirement]
-    ):
-        return {
-            "challenge": websafe_encode(challenge),
-            "user_verification": user_verification,
-        }
-
-
-def verify_app_id(app_id: str, origin: str) -> bool:
-    """Checks if a FIDO U2F App ID is usable for a given origin.
-
-    :param app_id: The App ID to validate.
-    :param origin: The origin of the request.
-    :return: True if the App ID is usable by the origin, False if not.
-    """
-    url = urlparse(app_id)
-    if url.scheme != "https":
-        return False
-    hostname = url.hostname
-    if not hostname:
-        return False
-    return verify_rp_id(hostname, origin)
-
-
-class U2FFido2Server(Fido2Server):
-    """Fido2Server which can be used with existing U2F credentials.
-
-    This Fido2Server can be used with existing U2F credentials by using the
-    WebAuthn appid extension, as well as with new WebAuthn credentials.
-    See https://www.w3.org/TR/webauthn/#sctn-appid-extension for details.
-
-    :param app_id: The appId which was used for U2F registration.
-    :param verify_u2f_origin: (optional) Alternative function to validate an
-        origin for U2F credentials.
-    For other parameters, see Fido2Server.
-    """
-
-    def __init__(
-        self,
-        app_id: str,
-        rp: PublicKeyCredentialRpEntity,
-        verify_u2f_origin: Optional[VerifyOrigin] = None,
-        *args,
-        **kwargs,
-    ):
-        super().__init__(rp, *args, **kwargs)
-        if verify_u2f_origin:
-            kwargs["verify_origin"] = verify_u2f_origin
-        else:
-            kwargs["verify_origin"] = lambda o: verify_app_id(app_id, o)
-        self._app_id = app_id
-        self._app_id_server = Fido2Server(
-            replace(PublicKeyCredentialRpEntity.from_dict(rp), id=app_id),
-            *args,
-            **kwargs,
-        )
-
-    def register_begin(self, *args, **kwargs):
-        kwargs.setdefault("extensions", {})["appidExclude"] = self._app_id
-        req, state = super().register_begin(*args, **kwargs)
-        return req, state
-
-    def authenticate_begin(self, *args, **kwargs):
-        kwargs.setdefault("extensions", {})["appid"] = self._app_id
-        req, state = super().authenticate_begin(*args, **kwargs)
-        return req, state
-
-    def authenticate_complete(self, *args, **kwargs):
-        try:
-            return super().authenticate_complete(*args, **kwargs)
-        except ValueError:
-            return self._app_id_server.authenticate_complete(*args, **kwargs)
+# Copyright (c) 2018 Yubico AB
+# All rights reserved.
+#
+#   Redistribution and use in source and binary forms, with or
+#   without modification, are permitted provided that the following
+#   conditions are met:
+#
+#    1. Redistributions of source code must retain the above copyright
+#       notice, this list of conditions and the following disclaimer.
+#    2. Redistributions in binary form must reproduce the above
+#       copyright notice, this list of conditions and the following
+#       disclaimer in the documentation and/or other materials provided
+#       with the distribution.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
+# FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
+# COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
+# INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
+# BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
+# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
+# ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+# POSSIBILITY OF SUCH DAMAGE.
+
+from __future__ import annotations
+
+from .rpid import verify_rp_id
+from .cose import CoseKey
+from .utils import websafe_encode, websafe_decode
+from .webauthn import (
+    CollectedClientData,
+    AuthenticatorData,
+    AttestationObject,
+    AttestedCredentialData,
+    AttestationConveyancePreference,
+    PublicKeyCredentialRpEntity,
+    PublicKeyCredentialUserEntity,
+    AuthenticatorSelectionCriteria,
+    PublicKeyCredentialDescriptor,
+    PublicKeyCredentialType,
+    PublicKeyCredentialParameters,
+    PublicKeyCredentialCreationOptions,
+    PublicKeyCredentialRequestOptions,
+    UserVerificationRequirement,
+    ResidentKeyRequirement,
+    AuthenticatorAttachment,
+    RegistrationResponse,
+    AuthenticationResponse,
+    CredentialCreationOptions,
+    CredentialRequestOptions,
+)
+
+from cryptography.hazmat.primitives import constant_time
+from cryptography.exceptions import InvalidSignature as _InvalidSignature
+from dataclasses import replace
+from urllib.parse import urlparse
+from typing import Sequence, Mapping, Optional, Callable, Union, Tuple, Any, overload
+
+import os
+import logging
+
+logger = logging.getLogger(__name__)
+
+
+VerifyAttestation = Callable[[AttestationObject, bytes], None]
+VerifyOrigin = Callable[[str], bool]
+
+
+def _verify_origin_for_rp(rp_id: str) -> VerifyOrigin:
+    return lambda o: verify_rp_id(rp_id, o)
+
+
+def _validata_challenge(challenge: Optional[bytes]) -> bytes:
+    if challenge is None:
+        challenge = os.urandom(32)
+    else:
+        if not isinstance(challenge, bytes):
+            raise TypeError("Custom challenge must be of type 'bytes'.")
+        if len(challenge) < 16:
+            raise ValueError("Custom challenge length must be >= 16.")
+    return challenge
+
+
+def to_descriptor(
+    credential: AttestedCredentialData, transports=None
+) -> PublicKeyCredentialDescriptor:
+    """Converts an AttestedCredentialData to a PublicKeyCredentialDescriptor.
+
+    :param credential: AttestedCredentialData containing the credential ID to use.
+    :param transports: Optional list of AuthenticatorTransport strings to add to the
+        descriptor.
+    :return: A descriptor of the credential, for use with register_begin or
+        authenticate_begin.
+    :rtype: PublicKeyCredentialDescriptor
+    """
+    return PublicKeyCredentialDescriptor(
+        PublicKeyCredentialType.PUBLIC_KEY, credential.credential_id, transports
+    )
+
+
+def _wrap_credentials(
+    creds: Optional[
+        Sequence[Union[AttestedCredentialData, PublicKeyCredentialDescriptor]]
+    ],
+) -> Optional[Sequence[PublicKeyCredentialDescriptor]]:
+    if creds is None:
+        return None
+    return [
+        to_descriptor(c)
+        if isinstance(c, AttestedCredentialData)
+        else PublicKeyCredentialDescriptor.from_dict(c)
+        for c in creds
+    ]
+
+
+def _ignore_attestation(
+    attestation_object: AttestationObject, client_data_hash: bytes
+) -> None:
+    """Ignore attestation."""
+
+
+class Fido2Server:
+    """FIDO2 server.
+
+    :param rp: Relying party data as `PublicKeyCredentialRpEntity` instance.
+    :param attestation: (optional) Requirement on authenticator attestation.
+    :param verify_origin: (optional) Alternative function to validate an origin.
+    :param verify_attestation: (optional) function to validate attestation, which is
+        invoked with attestation_object and client_data_hash. It should return nothing
+        and raise an exception on failure. By default, attestation is ignored.
+        Attestation is also ignored if `attestation` is set to `none`.
+    """
+
+    def __init__(
+        self,
+        rp: PublicKeyCredentialRpEntity,
+        attestation: Optional[AttestationConveyancePreference] = None,
+        verify_origin: Optional[VerifyOrigin] = None,
+        verify_attestation: Optional[VerifyAttestation] = None,
+    ):
+        self.rp = PublicKeyCredentialRpEntity.from_dict(rp)
+        self._verify = verify_origin or _verify_origin_for_rp(self.rp.id)
+        self.timeout = None
+        self.attestation = AttestationConveyancePreference(attestation)
+        self.allowed_algorithms = [
+            PublicKeyCredentialParameters(PublicKeyCredentialType.PUBLIC_KEY, alg)
+            for alg in CoseKey.supported_algorithms()
+        ]
+        self._verify_attestation = verify_attestation or _ignore_attestation
+        logger.debug(f"Fido2Server initialized for RP: {self.rp}")
+
+    def register_begin(
+        self,
+        user: PublicKeyCredentialUserEntity,
+        credentials: Optional[
+            Sequence[Union[AttestedCredentialData, PublicKeyCredentialDescriptor]]
+        ] = None,
+        resident_key_requirement: Optional[ResidentKeyRequirement] = None,
+        user_verification: Optional[UserVerificationRequirement] = None,
+        authenticator_attachment: Optional[AuthenticatorAttachment] = None,
+        challenge: Optional[bytes] = None,
+        extensions=None,
+    ) -> Tuple[CredentialCreationOptions, Any]:
+        """Return a PublicKeyCredentialCreationOptions registration object and
+        the internal state dictionary that needs to be passed as is to the
+        corresponding `register_complete` call.
+
+        :param user: The dict containing the user data.
+        :param credentials: The list of previously registered credentials, these can be
+            of type AttestedCredentialData, or PublicKeyCredentialDescriptor.
+        :param resident_key_requirement: The desired RESIDENT_KEY_REQUIREMENT level.
+        :param user_verification: The desired USER_VERIFICATION level.
+        :param authenticator_attachment: The desired AUTHENTICATOR_ATTACHMENT
+            or None to not provide a preference (and get both types).
+        :param challenge: A custom challenge to sign and verify or None to use
+            OS-specific random bytes.
+        :return: Registration data, internal state."""
+        if not self.allowed_algorithms:
+            raise ValueError("Server has no allowed algorithms.")
+
+        challenge = _validata_challenge(challenge)
+        descriptors = _wrap_credentials(credentials)
+        state = self._make_internal_state(challenge, user_verification)
+        logger.debug(
+            "Starting new registration, existing credentials: "
+            + ", ".join(d.id.hex() for d in descriptors or [])
+        )
+
+        return (
+            CredentialCreationOptions(
+                PublicKeyCredentialCreationOptions(
+                    self.rp,
+                    user,
+                    challenge,
+                    self.allowed_algorithms,
+                    self.timeout,
+                    descriptors,
+                    AuthenticatorSelectionCriteria(
+                        authenticator_attachment,
+                        resident_key_requirement,
+                        user_verification,
+                    )
+                    if any(
+                        (
+                            authenticator_attachment,
+                            resident_key_requirement,
+                            user_verification,
+                        )
+                    )
+                    else None,
+                    self.attestation,
+                    extensions,
+                )
+            ),
+            state,
+        )
+
+    @overload
+    def register_complete(
+        self,
+        state,
+        response: Union[RegistrationResponse, Mapping[str, Any]],
+    ) -> AuthenticatorData:
+        pass
+
+    @overload
+    def register_complete(
+        self,
+        state,
+        client_data: CollectedClientData,
+        attestation_object: AttestationObject,
+    ) -> AuthenticatorData:
+        pass
+
+    def register_complete(self, state, *args, **kwargs):
+        """Verify the correctness of the registration data received from
+        the client.
+
+        :param state: The state data returned by the corresponding
+            `register_begin`.
+        :param client_data: The client data.
+        :param attestation_object: The attestation object.
+        :return: The authenticator data
+        """
+        response = None
+        if len(args) == 1 and not kwargs:
+            response = args[0]
+        elif set(kwargs) == {"response"} and not args:
+            response = kwargs["response"]
+        if response:
+            registration = RegistrationResponse.from_dict(response)
+            client_data = registration.response.client_data
+            attestation_object = registration.response.attestation_object
+        else:
+            names = ["client_data", "attestation_object"]
+            pos = dict(zip(names, args))
+            data = {**kwargs, **pos}
+            if set(kwargs) & set(pos) or set(data) != set(names):
+                raise TypeError("incorrect arguments passed to register_complete()")
+            client_data = data[names[0]]
+            attestation_object = data[names[1]]
+
+        if client_data.type != CollectedClientData.TYPE.CREATE:
+            raise ValueError("Incorrect type in CollectedClientData.")
+        if not self._verify(client_data.origin):
+            raise ValueError("Invalid origin in CollectedClientData.")
+        if not constant_time.bytes_eq(
+            websafe_decode(state["challenge"]), client_data.challenge
+        ):
+            raise ValueError("Wrong challenge in response.")
+        if not constant_time.bytes_eq(
+            self.rp.id_hash, attestation_object.auth_data.rp_id_hash
+        ):
+            raise ValueError("Wrong RP ID hash in response.")
+        if not attestation_object.auth_data.is_user_present():
+            raise ValueError("User Present flag not set.")
+
+        if (
+            state["user_verification"] == UserVerificationRequirement.REQUIRED
+            and not attestation_object.auth_data.is_user_verified()
+        ):
+            raise ValueError(
+                "User verification required, but User Verified flag not set."
+            )
+
+        if self.attestation not in (None, AttestationConveyancePreference.NONE):
+            logger.debug(f"Verifying attestation of type {attestation_object.fmt}")
+            self._verify_attestation(attestation_object, client_data.hash)
+        # We simply ignore attestation if self.attestation == 'none', as not all
+        # clients strip the attestation.
+
+        auth_data = attestation_object.auth_data
+        assert auth_data.credential_data is not None  # nosec
+        logger.info(
+            "New credential registered: "
+            + auth_data.credential_data.credential_id.hex()
+        )
+        return auth_data
+
+    def authenticate_begin(
+        self,
+        credentials: Optional[
+            Sequence[Union[AttestedCredentialData, PublicKeyCredentialDescriptor]]
+        ] = None,
+        user_verification: Optional[UserVerificationRequirement] = None,
+        challenge: Optional[bytes] = None,
+        extensions=None,
+    ) -> Tuple[CredentialRequestOptions, Any]:
+        """Return a PublicKeyCredentialRequestOptions assertion object and the internal
+        state dictionary that needs to be passed as is to the corresponding
+        `authenticate_complete` call.
+
+        :param credentials: The list of previously registered credentials, these can be
+            of type AttestedCredentialData, or PublicKeyCredentialDescriptor.
+        :param user_verification: The desired USER_VERIFICATION level.
+        :param challenge: A custom challenge to sign and verify or None to use
+            OS-specific random bytes.
+        :return: Assertion data, internal state."""
+        challenge = _validata_challenge(challenge)
+        descriptors = _wrap_credentials(credentials)
+        state = self._make_internal_state(challenge, user_verification)
+        if descriptors is None:
+            logger.debug("Starting new authentication without credentials")
+        else:
+            logger.debug(
+                "Starting new authentication, for credentials: "
+                + ", ".join(d.id.hex() for d in descriptors)
+            )
+
+        return (
+            CredentialRequestOptions(
+                PublicKeyCredentialRequestOptions(
+                    challenge,
+                    self.timeout,
+                    self.rp.id,
+                    descriptors,
+                    user_verification,
+                    extensions,
+                )
+            ),
+            state,
+        )
+
+    @overload
+    def authenticate_complete(
+        self,
+        state,
+        credentials: Sequence[AttestedCredentialData],
+        response: Union[AuthenticationResponse, Mapping[str, Any]],
+    ) -> AttestedCredentialData:
+        pass
+
+    @overload
+    def authenticate_complete(
+        self,
+        state,
+        credentials: Sequence[AttestedCredentialData],
+        credential_id: bytes,
+        client_data: CollectedClientData,
+        auth_data: AuthenticatorData,
+        signature: bytes,
+    ) -> AttestedCredentialData:
+        pass
+
+    def authenticate_complete(self, state, credentials, *args, **kwargs):
+        """Verify the correctness of the assertion data received from
+        the client.
+
+        :param state: The state data returned by the corresponding
+            `register_begin`.
+        :param credentials: The list of previously registered credentials.
+        :param credential_id: The credential id from the client response.
+        :param client_data: The client data.
+        :param auth_data: The authenticator data.
+        :param signature: The signature provided by the client."""
+
+        response = None
+        if len(args) == 1 and not kwargs:
+            response = args[0]
+        elif set(kwargs) == {"response"} and not args:
+            response = kwargs["response"]
+        if response:
+            authentication = AuthenticationResponse.from_dict(response)
+            credential_id = authentication.id
+            client_data = authentication.response.client_data
+            auth_data = authentication.response.authenticator_data
+            signature = authentication.response.signature
+        else:
+            names = ["credential_id", "client_data", "auth_data", "signature"]
+            pos = dict(zip(names, args))
+            data = {**kwargs, **pos}
+            if set(kwargs) & set(pos) or set(data) != set(names):
+                raise TypeError("incorrect arguments passed to authenticate_complete()")
+            credential_id = data[names[0]]
+            client_data = data[names[1]]
+            auth_data = data[names[2]]
+            signature = data[names[3]]
+
+        if client_data.type != CollectedClientData.TYPE.GET:
+            raise ValueError("Incorrect type in CollectedClientData.")
+        if not self._verify(client_data.origin):
+            raise ValueError("Invalid origin in CollectedClientData.")
+        if websafe_decode(state["challenge"]) != client_data.challenge:
+            raise ValueError("Wrong challenge in response.")
+        if not constant_time.bytes_eq(self.rp.id_hash, auth_data.rp_id_hash):
+            raise ValueError("Wrong RP ID hash in response.")
+        if not auth_data.is_user_present():
+            raise ValueError("User Present flag not set.")
+
+        if (
+            state["user_verification"] == UserVerificationRequirement.REQUIRED
+            and not auth_data.is_user_verified()
+        ):
+            raise ValueError(
+                "User verification required, but user verified flag not set."
+            )
+
+        for cred in credentials:
+            if cred.credential_id == credential_id:
+                try:
+                    cred.public_key.verify(auth_data + client_data.hash, signature)
+                except _InvalidSignature:
+                    raise ValueError("Invalid signature.")
+                logger.info(f"Credential authenticated: {credential_id.hex()}")
+                return cred
+        raise ValueError("Unknown credential ID.")
+
+    @staticmethod
+    def _make_internal_state(
+        challenge: bytes, user_verification: Optional[UserVerificationRequirement]
+    ):
+        return {
+            "challenge": websafe_encode(challenge),
+            "user_verification": user_verification,
+        }
+
+
+def verify_app_id(app_id: str, origin: str) -> bool:
+    """Checks if a FIDO U2F App ID is usable for a given origin.
+
+    :param app_id: The App ID to validate.
+    :param origin: The origin of the request.
+    :return: True if the App ID is usable by the origin, False if not.
+    """
+    url = urlparse(app_id)
+    if url.scheme != "https":
+        return False
+    hostname = url.hostname
+    if not hostname:
+        return False
+    return verify_rp_id(hostname, origin)
+
+
+class U2FFido2Server(Fido2Server):
+    """Fido2Server which can be used with existing U2F credentials.
+
+    This Fido2Server can be used with existing U2F credentials by using the
+    WebAuthn appid extension, as well as with new WebAuthn credentials.
+    See https://www.w3.org/TR/webauthn/#sctn-appid-extension for details.
+
+    :param app_id: The appId which was used for U2F registration.
+    :param verify_u2f_origin: (optional) Alternative function to validate an
+        origin for U2F credentials.
+    For other parameters, see Fido2Server.
+    """
+
+    def __init__(
+        self,
+        app_id: str,
+        rp: PublicKeyCredentialRpEntity,
+        verify_u2f_origin: Optional[VerifyOrigin] = None,
+        *args,
+        **kwargs,
+    ):
+        super().__init__(rp, *args, **kwargs)
+        if verify_u2f_origin:
+            kwargs["verify_origin"] = verify_u2f_origin
+        else:
+            kwargs["verify_origin"] = lambda o: verify_app_id(app_id, o)
+        self._app_id = app_id
+        self._app_id_server = Fido2Server(
+            replace(PublicKeyCredentialRpEntity.from_dict(rp), id=app_id),
+            *args,
+            **kwargs,
+        )
+
+    def register_begin(self, *args, **kwargs):
+        kwargs.setdefault("extensions", {})["appidExclude"] = self._app_id
+        req, state = super().register_begin(*args, **kwargs)
+        return req, state
+
+    def authenticate_begin(self, *args, **kwargs):
+        kwargs.setdefault("extensions", {})["appid"] = self._app_id
+        req, state = super().authenticate_begin(*args, **kwargs)
+        return req, state
+
+    def authenticate_complete(self, *args, **kwargs):
+        try:
+            return super().authenticate_complete(*args, **kwargs)
+        except ValueError:
+            return self._app_id_server.authenticate_complete(*args, **kwargs)
```

### Comparing `fido2-1.1.1/fido2/utils.py` & `fido2-1.1.2/fido2/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,282 +1,285 @@
-# Copyright (c) 2013 Yubico AB
-# All rights reserved.
-#
-#   Redistribution and use in source and binary forms, with or
-#   without modification, are permitted provided that the following
-#   conditions are met:
-#
-#    1. Redistributions of source code must retain the above copyright
-#       notice, this list of conditions and the following disclaimer.
-#    2. Redistributions in binary form must reproduce the above
-#       copyright notice, this list of conditions and the following
-#       disclaimer in the documentation and/or other materials provided
-#       with the distribution.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
-# FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
-# COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
-# INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
-# BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
-# ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-# POSSIBILITY OF SUCH DAMAGE.
-
-"""Various utility functions.
-
-This module contains various functions used throughout the rest of the project.
-"""
-
-from __future__ import annotations
-
-from base64 import urlsafe_b64decode, urlsafe_b64encode
-from cryptography.hazmat.backends import default_backend
-from cryptography.hazmat.primitives import hmac, hashes
-from io import BytesIO
-from dataclasses import fields, Field
-from abc import abstractmethod
-from typing import (
-    Union,
-    Optional,
-    Sequence,
-    Mapping,
-    Any,
-    TypeVar,
-    Hashable,
-    get_type_hints,
-)
-import struct
-
-__all__ = [
-    "websafe_encode",
-    "websafe_decode",
-    "sha256",
-    "hmac_sha256",
-    "bytes2int",
-    "int2bytes",
-]
-
-
-LOG_LEVEL_TRAFFIC = 5
-
-
-def sha256(data: bytes) -> bytes:
-    """Produces a SHA256 hash of the input.
-
-    :param data: The input data to hash.
-    :return: The resulting hash.
-    """
-    h = hashes.Hash(hashes.SHA256(), default_backend())
-    h.update(data)
-    return h.finalize()
-
-
-def hmac_sha256(key: bytes, data: bytes) -> bytes:
-    """Performs an HMAC-SHA256 operation on the given data, using the given key.
-
-    :param key: The key to use.
-    :param data: The input data to hash.
-    :return: The resulting hash.
-    """
-    h = hmac.HMAC(key, hashes.SHA256(), default_backend())
-    h.update(data)
-    return h.finalize()
-
-
-def bytes2int(value: bytes) -> int:
-    """Parses an arbitrarily sized integer from a byte string.
-
-    :param value: A byte string encoding a big endian unsigned integer.
-    :return: The parsed int.
-    """
-    return int.from_bytes(value, "big")
-
-
-def int2bytes(value: int, minlen: int = -1) -> bytes:
-    """Encodes an int as a byte string.
-
-    :param value: The integer value to encode.
-    :param minlen: An optional minimum length for the resulting byte string.
-    :return: The value encoded as a big endian byte string.
-    """
-    ba = []
-    while value > 0xFF:
-        ba.append(0xFF & value)
-        value >>= 8
-    ba.append(value)
-    ba.extend([0] * (minlen - len(ba)))
-    return bytes(reversed(ba))
-
-
-def websafe_decode(data: Union[str, bytes]) -> bytes:
-    """Decodes a websafe-base64 encoded string.
-    See: "Base 64 Encoding with URL and Filename Safe Alphabet" from Section 5
-    in RFC4648 without padding.
-
-    :param data: The input to decode.
-    :return: The decoded bytes.
-    """
-    if isinstance(data, str):
-        data = data.encode("ascii")
-    data += b"=" * (-len(data) % 4)
-    return urlsafe_b64decode(data)
-
-
-def websafe_encode(data: bytes) -> str:
-    """Encodes a byte string into websafe-base64 encoding.
-
-    :param data: The input to encode.
-    :return: The encoded string.
-    """
-    return urlsafe_b64encode(data).replace(b"=", b"").decode("ascii")
-
-
-class ByteBuffer(BytesIO):
-    """BytesIO-like object with the ability to unpack values."""
-
-    def unpack(self, fmt: str):
-        """Reads and unpacks a value from the buffer.
-
-        :param fmt: A struct format string yielding a single value.
-        :return: The unpacked value.
-        """
-        s = struct.Struct(fmt)
-        return s.unpack(self.read(s.size))[0]
-
-    def read(self, size: Optional[int] = -1) -> bytes:
-        """Like BytesIO.read(), but checks the number of bytes read and raises an error
-        if fewer bytes were read than expected.
-        """
-        data = super().read(size)
-        if size is not None and size > 0 and len(data) != size:
-            raise ValueError(
-                "Not enough data to read (need: %d, had: %d)." % (size, len(data))
-            )
-        return data
-
-
-def _snake2camel(name: str) -> str:
-    parts = name.split("_")
-    return parts[0] + "".join(p.title() for p in parts[1:])
-
-
-def _parse_value(t, value):
-    if value is None:
-        return None
-
-    if Optional[t] == t:  # Optional, get the type
-        t = t.__args__[0]
-
-    # Handle list of values
-    if issubclass(getattr(t, "__origin__", object), Sequence):
-        t = t.__args__[0]
-        return [_parse_value(t, v) for v in value]
-
-    # Handle Mappings
-    if issubclass(getattr(t, "__origin__", object), Mapping) and isinstance(
-        value, Mapping
-    ):
-        return value
-
-    # Check if type is already correct
-    try:
-        if isinstance(value, t):
-            return value
-    except TypeError:
-        pass
-
-    # Check for subclass of _DataClassMapping
-    try:
-        is_dataclass = issubclass(t, _DataClassMapping)
-    except TypeError:
-        is_dataclass = False
-
-    if is_dataclass:
-        # Recursively call from_dict for nested _DataClassMappings
-        return t.from_dict(value)
-
-    # Convert to enum values, other wrappers
-    return t(value)
-
-
-_T = TypeVar("_T", bound=Hashable)
-
-
-class _DataClassMapping(Mapping[_T, Any]):
-    def __post_init__(self):
-        hints = get_type_hints(type(self))
-        for f in fields(self):
-            value = getattr(self, f.name)
-            if value is None:
-                continue
-            try:
-                value = _parse_value(hints[f.name], value)
-            except (TypeError, KeyError, ValueError):
-                raise ValueError(
-                    f"Error parsing field {f.name} for {self.__class__.__name__}"
-                )
-            object.__setattr__(self, f.name, value)
-
-    @classmethod
-    @abstractmethod
-    def _get_field_key(cls, field: Field) -> _T:
-        raise NotImplementedError()
-
-    def __getitem__(self, key):
-        for f in fields(self):
-            if key == self._get_field_key(f):
-                value = getattr(self, f.name)
-                serialize = f.metadata.get("serialize")
-                if serialize:
-                    return serialize(value)
-                if isinstance(value, _DataClassMapping):
-                    return dict(value)
-                if isinstance(value, Sequence) and all(
-                    isinstance(x, _DataClassMapping) for x in value
-                ):
-                    return [dict(x) for x in value]
-                return value
-        raise KeyError(key)
-
-    def __iter__(self):
-        return (
-            self._get_field_key(f)
-            for f in fields(self)
-            if getattr(self, f.name) is not None
-        )
-
-    def __len__(self):
-        return len(list(iter(self)))
-
-    @classmethod
-    def from_dict(cls, data: Optional[Mapping[_T, Any]]):
-        if data is None:
-            return None
-        if isinstance(data, cls):
-            return data
-        if not isinstance(data, Mapping):
-            raise TypeError(
-                f"{cls.__name__}.from_dict called with non-Mapping data of type"
-                f"{type(data)}"
-            )
-
-        kwargs = {}
-        for f in fields(cls):
-            key = cls._get_field_key(f)
-            if key in data:
-                value = data[key]
-                if value is not None:
-                    deserialize = f.metadata.get("deserialize")
-                    if deserialize:
-                        value = deserialize(value)
-                    kwargs[f.name] = value
-        return cls(**kwargs)
-
-
-class _CamelCaseDataObject(_DataClassMapping[str]):
-    @classmethod
-    def _get_field_key(cls, field: Field) -> str:
-        return field.metadata.get("name", _snake2camel(field.name))
+# Copyright (c) 2013 Yubico AB
+# All rights reserved.
+#
+#   Redistribution and use in source and binary forms, with or
+#   without modification, are permitted provided that the following
+#   conditions are met:
+#
+#    1. Redistributions of source code must retain the above copyright
+#       notice, this list of conditions and the following disclaimer.
+#    2. Redistributions in binary form must reproduce the above
+#       copyright notice, this list of conditions and the following
+#       disclaimer in the documentation and/or other materials provided
+#       with the distribution.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
+# FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
+# COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
+# INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
+# BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
+# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
+# ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+# POSSIBILITY OF SUCH DAMAGE.
+
+"""Various utility functions.
+
+This module contains various functions used throughout the rest of the project.
+"""
+
+from __future__ import annotations
+
+from base64 import urlsafe_b64decode, urlsafe_b64encode
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import hmac, hashes
+from io import BytesIO
+from dataclasses import fields, Field
+from abc import abstractmethod
+from typing import (
+    Union,
+    Optional,
+    Sequence,
+    Mapping,
+    Any,
+    TypeVar,
+    Hashable,
+    get_type_hints,
+)
+import struct
+
+__all__ = [
+    "websafe_encode",
+    "websafe_decode",
+    "sha256",
+    "hmac_sha256",
+    "bytes2int",
+    "int2bytes",
+]
+
+
+LOG_LEVEL_TRAFFIC = 5
+
+
+def sha256(data: bytes) -> bytes:
+    """Produces a SHA256 hash of the input.
+
+    :param data: The input data to hash.
+    :return: The resulting hash.
+    """
+    h = hashes.Hash(hashes.SHA256(), default_backend())
+    h.update(data)
+    return h.finalize()
+
+
+def hmac_sha256(key: bytes, data: bytes) -> bytes:
+    """Performs an HMAC-SHA256 operation on the given data, using the given key.
+
+    :param key: The key to use.
+    :param data: The input data to hash.
+    :return: The resulting hash.
+    """
+    h = hmac.HMAC(key, hashes.SHA256(), default_backend())
+    h.update(data)
+    return h.finalize()
+
+
+def bytes2int(value: bytes) -> int:
+    """Parses an arbitrarily sized integer from a byte string.
+
+    :param value: A byte string encoding a big endian unsigned integer.
+    :return: The parsed int.
+    """
+    return int.from_bytes(value, "big")
+
+
+def int2bytes(value: int, minlen: int = -1) -> bytes:
+    """Encodes an int as a byte string.
+
+    :param value: The integer value to encode.
+    :param minlen: An optional minimum length for the resulting byte string.
+    :return: The value encoded as a big endian byte string.
+    """
+    ba = []
+    while value > 0xFF:
+        ba.append(0xFF & value)
+        value >>= 8
+    ba.append(value)
+    ba.extend([0] * (minlen - len(ba)))
+    return bytes(reversed(ba))
+
+
+def websafe_decode(data: Union[str, bytes]) -> bytes:
+    """Decodes a websafe-base64 encoded string.
+    See: "Base 64 Encoding with URL and Filename Safe Alphabet" from Section 5
+    in RFC4648 without padding.
+
+    :param data: The input to decode.
+    :return: The decoded bytes.
+    """
+    if isinstance(data, str):
+        data = data.encode("ascii")
+    data += b"=" * (-len(data) % 4)
+    return urlsafe_b64decode(data)
+
+
+def websafe_encode(data: bytes) -> str:
+    """Encodes a byte string into websafe-base64 encoding.
+
+    :param data: The input to encode.
+    :return: The encoded string.
+    """
+    return urlsafe_b64encode(data).replace(b"=", b"").decode("ascii")
+
+
+class ByteBuffer(BytesIO):
+    """BytesIO-like object with the ability to unpack values."""
+
+    def unpack(self, fmt: str):
+        """Reads and unpacks a value from the buffer.
+
+        :param fmt: A struct format string yielding a single value.
+        :return: The unpacked value.
+        """
+        s = struct.Struct(fmt)
+        return s.unpack(self.read(s.size))[0]
+
+    def read(self, size: Optional[int] = -1) -> bytes:
+        """Like BytesIO.read(), but checks the number of bytes read and raises an error
+        if fewer bytes were read than expected.
+        """
+        data = super().read(size)
+        if size is not None and size > 0 and len(data) != size:
+            raise ValueError(
+                "Not enough data to read (need: %d, had: %d)." % (size, len(data))
+            )
+        return data
+
+
+def _snake2camel(name: str) -> str:
+    parts = name.split("_")
+    return parts[0] + "".join(p.title() for p in parts[1:])
+
+
+def _parse_value(t, value):
+    if value is None:
+        return None
+
+    if Optional[t] == t:  # Optional, get the type
+        t = t.__args__[0]
+
+    # Handle list of values
+    if issubclass(getattr(t, "__origin__", object), Sequence):
+        t = t.__args__[0]
+        return [_parse_value(t, v) for v in value]
+
+    # Handle Mappings
+    if issubclass(getattr(t, "__origin__", object), Mapping) and isinstance(
+        value, Mapping
+    ):
+        return value
+
+    # Check if type is already correct
+    try:
+        if isinstance(value, t):
+            return value
+    except TypeError:
+        pass
+
+    # Check for subclass of _DataClassMapping
+    try:
+        is_dataclass = issubclass(t, _DataClassMapping)
+    except TypeError:
+        is_dataclass = False
+
+    if is_dataclass:
+        # Recursively call from_dict for nested _DataClassMappings
+        return t.from_dict(value)
+
+    # Convert to enum values, other wrappers
+    return t(value)
+
+
+_T = TypeVar("_T", bound=Hashable)
+
+
+class _DataClassMapping(Mapping[_T, Any]):
+    # TODO: This requires Python 3.9, and fixes the tpye errors we now ignore
+    # __dataclass_fields__: ClassVar[Dict[str, Field[Any]]]
+
+    def __post_init__(self):
+        hints = get_type_hints(type(self))
+        for f in fields(self):  # type: ignore
+            value = getattr(self, f.name)
+            if value is None:
+                continue
+            try:
+                value = _parse_value(hints[f.name], value)
+            except (TypeError, KeyError, ValueError):
+                raise ValueError(
+                    f"Error parsing field {f.name} for {self.__class__.__name__}"
+                )
+            object.__setattr__(self, f.name, value)
+
+    @classmethod
+    @abstractmethod
+    def _get_field_key(cls, field: Field) -> _T:
+        raise NotImplementedError()
+
+    def __getitem__(self, key):
+        for f in fields(self):  # type: ignore
+            if key == self._get_field_key(f):
+                value = getattr(self, f.name)
+                serialize = f.metadata.get("serialize")
+                if serialize:
+                    return serialize(value)
+                if isinstance(value, _DataClassMapping):
+                    return dict(value)
+                if isinstance(value, Sequence) and all(
+                    isinstance(x, _DataClassMapping) for x in value
+                ):
+                    return [dict(x) for x in value]
+                return value
+        raise KeyError(key)
+
+    def __iter__(self):
+        return (
+            self._get_field_key(f)
+            for f in fields(self)  # type: ignore
+            if getattr(self, f.name) is not None
+        )
+
+    def __len__(self):
+        return len(list(iter(self)))
+
+    @classmethod
+    def from_dict(cls, data: Optional[Mapping[_T, Any]]):
+        if data is None:
+            return None
+        if isinstance(data, cls):
+            return data
+        if not isinstance(data, Mapping):
+            raise TypeError(
+                f"{cls.__name__}.from_dict called with non-Mapping data of type"
+                f"{type(data)}"
+            )
+
+        kwargs = {}
+        for f in fields(cls):  # type: ignore
+            key = cls._get_field_key(f)
+            if key in data:
+                value = data[key]
+                if value is not None:
+                    deserialize = f.metadata.get("deserialize")
+                    if deserialize:
+                        value = deserialize(value)
+                    kwargs[f.name] = value
+        return cls(**kwargs)
+
+
+class _CamelCaseDataObject(_DataClassMapping[str]):
+    @classmethod
+    def _get_field_key(cls, field: Field) -> str:
+        return field.metadata.get("name", _snake2camel(field.name))
```

### Comparing `fido2-1.1.1/fido2/webauthn.py` & `fido2-1.1.2/fido2/webauthn.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/fido2/win_api.py` & `fido2-1.1.2/fido2/win_api.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/NEWS` & `fido2-1.1.2/NEWS`

 * *Files 12% similar despite different names*

```diff
@@ -1,152 +1,156 @@
-* Version 1.1.1 (released 2023-04-05)
- ** Add community provided support for NetBSD.
- ** Bugfix: Don't set length for largeBlob when offset is 0.
- ** Bugfix: Remove print statement in webauthn parsing.
-
-* Version 1.1.0 (released 2022-10-17)
- ** Bugfix: Fix name of "crossOrigin" in CollectedClientData.create().
- ** Bugfix: Some incorrect type hints in the MDS3 classes were fixed.
- ** Stricter checking of dataclass field types.
- ** Add support for JSON-serialization of WebAuthn data classes.
-    This changes the objects dict representation to align with new additions in the
-    WebAuthn specification. As this may break compatibility, the new behavior
-    requires explicit opt-in until python-fido2 2.0 is released.
- ** Update server example to use JSON serialization.
- ** Server: Add support for passing RegistrationResponse/AuthenticationResponse (or
-    their deserialized JSON data) to register_complete/authenticate_complete.
- ** Add new "hybrid" AuthenticatorTransport.
- ** Add new AuthenticatorData flags, and use 2-letter names as in the WebAuthn spec
-    (long names are still available as aliases).
-
-* Version 1.0.0 (released 2022-06-08)
- ** First stable release.
-
-* Version 1.0.0rc1 (released 2022-05-02)
- ** Release Candidate 1 of first stable release.
- ** Require Python 3.7 or later.
- ** APIs have updated to align with WebAuthn level 2.
- ** Several CTAP 2.1 features have been implemented.
-
-* Version 0.9.3 (released 2021-11-09)
- ** Bugfix: Linux - Don't fail device discovery when hidraw doesn't support
-    HIDIOCGRAWUNIQ (Linux kernels before 5.6).
-
-* Version 0.9.2 (released 2021-10-14)
- ** Support the latest Windows webauthn.h API (included in Windows 11).
- ** Add product name and serial number to HidDescriptors.
- ** Remove the need for the uhid-freebsd dependency on FreeBSD.
-
-* Version 0.9.1 (released 2021-02-03)
- ** Add new CTAP error codes and improve handling of unknown codes.
-
-* Version 0.9.0 (released 2021-01-20)
- ** Server: Attestation is now done in two parts (to align better with the spec):
-    First, type-specific validation is done to provide a trust chain.
-    Second, validation of the trust chain is done.
- ** Client: API changes to better support extensions.
-  *** Fido2Client can be configured with Ctap2Extensions to support.
-  *** Client.make_credential now returns a AuthenticatorAttestationResponse,
-      which holds the AttestationObject and ClientData, as well as any client
-      extension results for the credential.
-  *** Client.get_assertion now returns an AssertionSelection object, which is
-      used to select between multiple assertions, resulting in an
-      AuthenticatorAssertionResponse, which holds the ClientData, assertion
-      values, as well as any client extension results for the assertion.
- ** Renames: The CTAP1 and CTAP2 classes have been renamed to Ctap1 and Ctap2,
-    respectively. The old names currently work, but will be removed in the
-    future.
- ** ClientPin: The ClientPin API has been restructured to support multiple PIN
-    protocols, UV tokens, and token permissions.
- ** CTAP 2.1 PRE: Several new features have been added for CTAP 2.1, including
-    Credential Management, Bio Enrollment, Large Blobs, and Authenticator Config.
- ** HID: The platform specific HID code has been revamped and cleaned up.
-
-* Version 0.8.1 (released 2019-11-25)
- ** Bugfix: WindowsClient.make_credential error when resident key requirement is
-    unspecified.
-
-* Version 0.8.0 (released 2019-11-25)
- ** New fido2.webauthn classes modeled after the W3C WebAuthn spec introduced.
- ** CTAP2 send_cbor/make_credential/get_assertion  and U2fClient
-    request/authenticate `timeout` arguments replaced with `event` used to
-    cancel a request.
- ** Fido2Client:
-  *** make_credential/get_assertion now take WebAuthn options objects.
-  *** timeout is now provided in ms in WebAuthn options objects. Event based
-      cancelation also available by passing an Event.
- ** Fido2Server:
-  *** ATTESTATION, USER_VERIFICATION, and AUTHENTICATOR_ATTACHMENT enums
-      have been replaced with fido2.webauthn classes.
-  *** RelyingParty has been replaced with PublicKeyCredentialRpEntity, and
-      name is no longer optional.
-  *** Options returned by register_begin/authenticate_begin now omit unspecified
-      values if they are optional, instead of filling in default values.
-  *** Fido2Server.allowed_algorithms now contains a list of
-      PublicKeyCredentialParameters instead of algorithm identifiers.
-  *** Fido2Server.timeout is now in ms and of type int.
- ** Support native WebAuthn API on Windows through WindowsClient.
-
-* Version 0.7.3 (released 2019-10-24)
- ** Bugfix: Workaround for size of int on Python 2 on Windows.
-
-* Version 0.7.2 (released 2019-10-24)
- ** Support for the TPM attestation format.
- ** Allow passing custom challenges to register/authenticate in Fido2Server.
- ** Bugfix: CTAP2 CANCEL command response handling fixed.
- ** Bugfix: Fido2Client fix handling of empty allow_list.
- ** Bugfix: Fix typo in CTAP2.get_assertions() causing it to fail.
-
-* Version 0.7.1 (released 2019-09-20)
- ** Support for FreeBSD.
- ** Enforce canonical CBOR on Authenticator responses by default.
- ** PCSC: Support extended APDUs.
- ** Server: Verify that UP flag is set.
- ** U2FFido2Server: Implement AppID exclusion extension.
- ** U2FFido2Server: Allow custom U2F facet verification.
- ** Bugfix: U2FFido2Server.authenticate_complete now returns the result.
-
-* Version 0.7.0 (released 2019-06-17)
- ** Add support for NFC devices using PCSC.
- ** Add support for the hmac-secret Authenticator extension.
- ** Honor max credential ID length and number of credentials to Authenticator.
- ** Add close() method to CTAP devices to explicitly release their resources.
-
-* Version 0.6.0 (released 2019-05-10)
- ** Don't fail if CTAP2 Info contains unknown fields.
- ** Replace cbor loads/dumps functions with encode/decode/decode_from.
- ** Server: Add support for AuthenticatorAttachment.
- ** Server: Add support for more key algorithms.
- ** Client: Expose CTAP2 Info object as Fido2Client.info.
-
-* Version 0.5.0 (released 2018-12-21)
- ** Changes to server classes, some backwards breaking.
- ** Add ability to authenticate U2F credentials by using the appid extension.
- ** Make verification of attestation more explicit.
- ** Add support for Android SafetyNet attestation.
- ** Make it easier to work with U2F/CTAP1 data formats.
-
-* Version 0.4.0 (released 2018-09-27)
- ** Add classes for implementing a server.
- ** Various small changes, some affecting backwards compatibility.
-
-* Version 0.3.0 (released 2018-04-13)
- ** Add conversion between string/int keys for AttestationObject.
- ** Replace internal Exceptions with built-in types.
- ** Bugfix: Don't use TimeoutError which isn't available on Python 2.
-
-* Version 0.2.2 (released 2018-04-11)
- ** Bugfix: Better handling of unplugged devices on MacOS and avoid leaking threads.
-
-* Version 0.2.1 (released 2018-04-10)
- ** Add server example.
- ** Parse AttestationObjects that use string keys (Webauthn).
- ** Fix bug in handling packets with the wrong channel id.
-
-* Version 0.2.0 (released 2018-04-05)
- ** Changed name of project to python-fido2 to better reflect its scope.
- ** Added attestation and assertion verification methods.
- ** A lot of name changes, moved classes, etc.
- ** New example for multi-device use.
-
-* Version 0.1.0 (released 2018-03-16)
- ** First beta release.
+* Version 1.1.2 (released 2023-07-06)
+ ** Fix ClientPin usage for Authenticators that do not support passing a PIN.
+ ** Fix: Handle correct CTAP response codes in authenticatorSelection.
+
+* Version 1.1.1 (released 2023-04-05)
+ ** Add community provided support for NetBSD.
+ ** Bugfix: Don't set length for largeBlob when offset is 0.
+ ** Bugfix: Remove print statement in webauthn parsing.
+
+* Version 1.1.0 (released 2022-10-17)
+ ** Bugfix: Fix name of "crossOrigin" in CollectedClientData.create().
+ ** Bugfix: Some incorrect type hints in the MDS3 classes were fixed.
+ ** Stricter checking of dataclass field types.
+ ** Add support for JSON-serialization of WebAuthn data classes.
+    This changes the objects dict representation to align with new additions in the
+    WebAuthn specification. As this may break compatibility, the new behavior
+    requires explicit opt-in until python-fido2 2.0 is released.
+ ** Update server example to use JSON serialization.
+ ** Server: Add support for passing RegistrationResponse/AuthenticationResponse (or
+    their deserialized JSON data) to register_complete/authenticate_complete.
+ ** Add new "hybrid" AuthenticatorTransport.
+ ** Add new AuthenticatorData flags, and use 2-letter names as in the WebAuthn spec
+    (long names are still available as aliases).
+
+* Version 1.0.0 (released 2022-06-08)
+ ** First stable release.
+
+* Version 1.0.0rc1 (released 2022-05-02)
+ ** Release Candidate 1 of first stable release.
+ ** Require Python 3.7 or later.
+ ** APIs have updated to align with WebAuthn level 2.
+ ** Several CTAP 2.1 features have been implemented.
+
+* Version 0.9.3 (released 2021-11-09)
+ ** Bugfix: Linux - Don't fail device discovery when hidraw doesn't support
+    HIDIOCGRAWUNIQ (Linux kernels before 5.6).
+
+* Version 0.9.2 (released 2021-10-14)
+ ** Support the latest Windows webauthn.h API (included in Windows 11).
+ ** Add product name and serial number to HidDescriptors.
+ ** Remove the need for the uhid-freebsd dependency on FreeBSD.
+
+* Version 0.9.1 (released 2021-02-03)
+ ** Add new CTAP error codes and improve handling of unknown codes.
+
+* Version 0.9.0 (released 2021-01-20)
+ ** Server: Attestation is now done in two parts (to align better with the spec):
+    First, type-specific validation is done to provide a trust chain.
+    Second, validation of the trust chain is done.
+ ** Client: API changes to better support extensions.
+  *** Fido2Client can be configured with Ctap2Extensions to support.
+  *** Client.make_credential now returns a AuthenticatorAttestationResponse,
+      which holds the AttestationObject and ClientData, as well as any client
+      extension results for the credential.
+  *** Client.get_assertion now returns an AssertionSelection object, which is
+      used to select between multiple assertions, resulting in an
+      AuthenticatorAssertionResponse, which holds the ClientData, assertion
+      values, as well as any client extension results for the assertion.
+ ** Renames: The CTAP1 and CTAP2 classes have been renamed to Ctap1 and Ctap2,
+    respectively. The old names currently work, but will be removed in the
+    future.
+ ** ClientPin: The ClientPin API has been restructured to support multiple PIN
+    protocols, UV tokens, and token permissions.
+ ** CTAP 2.1 PRE: Several new features have been added for CTAP 2.1, including
+    Credential Management, Bio Enrollment, Large Blobs, and Authenticator Config.
+ ** HID: The platform specific HID code has been revamped and cleaned up.
+
+* Version 0.8.1 (released 2019-11-25)
+ ** Bugfix: WindowsClient.make_credential error when resident key requirement is
+    unspecified.
+
+* Version 0.8.0 (released 2019-11-25)
+ ** New fido2.webauthn classes modeled after the W3C WebAuthn spec introduced.
+ ** CTAP2 send_cbor/make_credential/get_assertion  and U2fClient
+    request/authenticate `timeout` arguments replaced with `event` used to
+    cancel a request.
+ ** Fido2Client:
+  *** make_credential/get_assertion now take WebAuthn options objects.
+  *** timeout is now provided in ms in WebAuthn options objects. Event based
+      cancelation also available by passing an Event.
+ ** Fido2Server:
+  *** ATTESTATION, USER_VERIFICATION, and AUTHENTICATOR_ATTACHMENT enums
+      have been replaced with fido2.webauthn classes.
+  *** RelyingParty has been replaced with PublicKeyCredentialRpEntity, and
+      name is no longer optional.
+  *** Options returned by register_begin/authenticate_begin now omit unspecified
+      values if they are optional, instead of filling in default values.
+  *** Fido2Server.allowed_algorithms now contains a list of
+      PublicKeyCredentialParameters instead of algorithm identifiers.
+  *** Fido2Server.timeout is now in ms and of type int.
+ ** Support native WebAuthn API on Windows through WindowsClient.
+
+* Version 0.7.3 (released 2019-10-24)
+ ** Bugfix: Workaround for size of int on Python 2 on Windows.
+
+* Version 0.7.2 (released 2019-10-24)
+ ** Support for the TPM attestation format.
+ ** Allow passing custom challenges to register/authenticate in Fido2Server.
+ ** Bugfix: CTAP2 CANCEL command response handling fixed.
+ ** Bugfix: Fido2Client fix handling of empty allow_list.
+ ** Bugfix: Fix typo in CTAP2.get_assertions() causing it to fail.
+
+* Version 0.7.1 (released 2019-09-20)
+ ** Support for FreeBSD.
+ ** Enforce canonical CBOR on Authenticator responses by default.
+ ** PCSC: Support extended APDUs.
+ ** Server: Verify that UP flag is set.
+ ** U2FFido2Server: Implement AppID exclusion extension.
+ ** U2FFido2Server: Allow custom U2F facet verification.
+ ** Bugfix: U2FFido2Server.authenticate_complete now returns the result.
+
+* Version 0.7.0 (released 2019-06-17)
+ ** Add support for NFC devices using PCSC.
+ ** Add support for the hmac-secret Authenticator extension.
+ ** Honor max credential ID length and number of credentials to Authenticator.
+ ** Add close() method to CTAP devices to explicitly release their resources.
+
+* Version 0.6.0 (released 2019-05-10)
+ ** Don't fail if CTAP2 Info contains unknown fields.
+ ** Replace cbor loads/dumps functions with encode/decode/decode_from.
+ ** Server: Add support for AuthenticatorAttachment.
+ ** Server: Add support for more key algorithms.
+ ** Client: Expose CTAP2 Info object as Fido2Client.info.
+
+* Version 0.5.0 (released 2018-12-21)
+ ** Changes to server classes, some backwards breaking.
+ ** Add ability to authenticate U2F credentials by using the appid extension.
+ ** Make verification of attestation more explicit.
+ ** Add support for Android SafetyNet attestation.
+ ** Make it easier to work with U2F/CTAP1 data formats.
+
+* Version 0.4.0 (released 2018-09-27)
+ ** Add classes for implementing a server.
+ ** Various small changes, some affecting backwards compatibility.
+
+* Version 0.3.0 (released 2018-04-13)
+ ** Add conversion between string/int keys for AttestationObject.
+ ** Replace internal Exceptions with built-in types.
+ ** Bugfix: Don't use TimeoutError which isn't available on Python 2.
+
+* Version 0.2.2 (released 2018-04-11)
+ ** Bugfix: Better handling of unplugged devices on MacOS and avoid leaking threads.
+
+* Version 0.2.1 (released 2018-04-10)
+ ** Add server example.
+ ** Parse AttestationObjects that use string keys (Webauthn).
+ ** Fix bug in handling packets with the wrong channel id.
+
+* Version 0.2.0 (released 2018-04-05)
+ ** Changed name of project to python-fido2 to better reflect its scope.
+ ** Added attestation and assertion verification methods.
+ ** A lot of name changes, moved classes, etc.
+ ** New example for multi-device use.
+
+* Version 0.1.0 (released 2018-03-16)
+ ** First beta release.
```

### Comparing `fido2-1.1.1/README.adoc` & `fido2-1.1.2/README.adoc`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/tests/hid/test_base.py` & `fido2-1.1.2/tests/hid/test_base.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/tests/test_attestation.py` & `fido2-1.1.2/tests/test_attestation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,342 +1,351 @@
-# Copyright (c) 2013 Yubico AB
-# All rights reserved.
-#
-#   Redistribution and use in source and binary forms, with or
-#   without modification, are permitted provided that the following
-#   conditions are met:
-#
-#    1. Redistributions of source code must retain the above copyright
-#       notice, this list of conditions and the following disclaimer.
-#    2. Redistributions in binary form must reproduce the above
-#       copyright notice, this list of conditions and the following
-#       disclaimer in the documentation and/or other materials provided
-#       with the distribution.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
-# FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
-# COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
-# INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
-# BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
-# ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-# POSSIBILITY OF SUCH DAMAGE.
-
-from fido2.webauthn import AuthenticatorData
-from fido2.attestation import (
-    Attestation,
-    AttestationType,
-    UnsupportedAttestation,
-    FidoU2FAttestation,
-    PackedAttestation,
-    TpmAttestation,
-    NoneAttestation,
-    AndroidSafetynetAttestation,
-    AppleAttestation,
-    InvalidData,
-    InvalidSignature,
-    UnsupportedType,
-    verify_x509_chain,
-)
-
-import unittest
-
-
-# GS Root R2 (https://pki.goog/)
-_GSR2_DER = bytes.fromhex(
-    "308203ba308202a2a003020102020b0400000000010f8626e60d300d06092a864886f70d0101050500304c3120301e060355040b1317476c6f62616c5369676e20526f6f74204341202d20523231133011060355040a130a476c6f62616c5369676e311330110603550403130a476c6f62616c5369676e301e170d3036313231353038303030305a170d3231313231353038303030305a304c3120301e060355040b1317476c6f62616c5369676e20526f6f74204341202d20523231133011060355040a130a476c6f62616c5369676e311330110603550403130a476c6f62616c5369676e30820122300d06092a864886f70d01010105000382010f003082010a0282010100a6cf240ebe2e6f28994542c4ab3e21549b0bd37f8470fa12b3cbbf875fc67f86d3b2305cd6fdadf17bdce5f86096099210f5d053defb7b7e7388ac52887b4aa6ca49a65ea8a78c5a11bc7a82ebbe8ce9b3ac962507974a992a072fb41e77bf8a0fb5027c1b96b8c5b93a2cbcd612b9eb597de2d006865f5e496ab5395e8834ecbc780c0898846ca8cd4bb4a07d0c794df0b82dcb21cad56c5b7de1a02984a1f9d39449cb24629120bcdd0bd5d9ccf9ea270a2b7391c69d1bacc8cbe8e0a0f42f908b4dfbb0361bf6197a85e06df26113885c9fe0930a51978a5aceafabd5f7aa09aa60bddcd95fdf72a960135e0001c94afa3fa4ea070321028e82ca03c29b8f0203010001a3819c308199300e0603551d0f0101ff040403020106300f0603551d130101ff040530030101ff301d0603551d0e041604149be20757671c1ec06a06de59b49a2ddfdc19862e30360603551d1f042f302d302ba029a0278625687474703a2f2f63726c2e676c6f62616c7369676e2e6e65742f726f6f742d72322e63726c301f0603551d230418301680149be20757671c1ec06a06de59b49a2ddfdc19862e300d06092a864886f70d01010505000382010100998153871c68978691ece04ab8440bab81ac274fd6c1b81c4378b30c9afcea2c3c6e611b4d4b29f59f051d26c1b8e983006245b6a90893b9a9334b189ac2f887884edbdd71341ac154da463fe0d32aab6d5422f53a62cd206fba2989d7dd91eed35ca23ea15b41f5dfe564432de9d539abd2a2dfb78bd0c080191c45c02d8ce8f82da4745649c505b54f15de6e44783987a87ebbf3791891bbf46f9dc1f08c358c5d01fbc36db9ef446d7946317e0afea982c1ffefab6e20c450c95f9d4d9b178c0ce501c9a0416a7353faa550b46e250ffb4c18f4fd52d98e69b1e8110fde88d8fb1d49f7aade95cf2078c26012db25408c6afc7e4238406412f79e81e1932e"  # noqa E501
-)
-
-
-class TestAttestationObject(unittest.TestCase):
-    def test_unsupported_attestation(self):
-        attestation = Attestation.for_type("__unsupported__")()
-        self.assertIsInstance(attestation, UnsupportedAttestation)
-        with self.assertRaises(UnsupportedType) as ctx:
-            attestation.verify({}, 0, b"")
-        self.assertEqual(ctx.exception.fmt, "__unsupported__")
-
-    def test_none_attestation(self):
-        attestation = Attestation.for_type("none")()
-        self.assertIsInstance(attestation, NoneAttestation)
-
-        auth_data = AuthenticatorData(
-            bytes.fromhex(
-                "0021F5FC0B85CD22E60623BCD7D1CA48948909249B4776EB515154E57B66AE12410000002BF8A011F38C0A4D15800617111F9EDC7D0040A17370D9C1759005700C8DE77E7DFD3A0A5300E0A26E5213AA40D6DF10EE4028B58B5F34167035D840BEBAE0C5CE8FD05AD9BD33E3BE7D1C558D81AB4803570BA5010203262001215820A5FD5CE1B1C458C530A54FA61B31BF6B04BE8B97AFDE54DD8CBB69275A8A1BE1225820FA3A3231DD9DEED9D1897BE5A6228C59501E4BCD12975D3DFF730F01278EA61C"  # noqa E501
-            )
-        )
-        res = attestation.verify({}, auth_data, b"deadbeef" * 8)
-        self.assertEqual(res.attestation_type, AttestationType.NONE)
-        self.assertEqual(res.trust_path, [])
-
-        with self.assertRaises(InvalidData):
-            attestation.verify({"not": "empty"}, auth_data, b"deadbeef" * 8)
-
-    def test_none_windows_hello_attestation(self):
-        attestation = Attestation.for_type("none")()
-        self.assertIsInstance(attestation, NoneAttestation)
-
-        auth_data = AuthenticatorData(
-            bytes.fromhex(
-                "54ce651ed715b4aaa755eecebd4ea0950815b334bd07d109893e963018cddbd945000000006028b017b1d44c02b4b3afcdafc96bb200201decfcd6d6a05c2826d52348afdc70a9800df007845047b1a23706aa6e2f315ca401030339010020590100af59f4ad4f71da800bb91045b267e240e06317f7b2b1d76f78e239a433811faeca58a1869fb00225eb2727f81b6b20cbc18c0ad8d38fa450e8df11b4ad3bc3ee5d13c77ed172fa3af0195ec6ac0c4bac8c950115dfce6d38737cbafefbe117d8401cd56c638043a0d585131bc48a153b17a8dcb96671e15a90ba1b4ff810b138b77ac0a050b039b87b6089dd8dfa45611b992109d554aad3e6b72ac82d801496e4d2d230aa466090bbbf4f5632fe4b588e4f571462378fa6f514a536a5945b223c8d98f730b7cf85de86b98c217090f9e9ebf9643cf3feceeacb837d7a18542e03271cd8c70cf81186cdb63e4cbf4efc0cbbd3c93231b06f19580d0a980264d12143010001"  # noqa
-            )
-        )  # noqa
-        res = attestation.verify({}, auth_data, b"deadbeef" * 8)
-        self.assertEqual(res.attestation_type, AttestationType.NONE)
-        self.assertEqual(res.trust_path, [])
-
-        with self.assertRaises(InvalidData):
-            attestation.verify({"not": "empty"}, auth_data, b"deadbeef" * 8)
-
-    def test_tpm_windows_hello_attestation(self):
-        attestation = Attestation.for_type("tpm")()
-        self.assertIsInstance(attestation, TpmAttestation)
-        statement = {
-            "alg": -65535,
-            "sig": bytes.fromhex(
-                """80e564d8cbb236577de68d2e68ecae200a8eaf6992889b5
-fdc24624a4cb69caaab18df965058fbac39df9714b9c80b9a12d715cfc4dd15ed3a6e191a6d26e
-7206fd402b0733c2c8b91f62ad44e4d41c940e2e914253b1d1a1c8889b1cdaf668b5449245dc33
-1fab12e0b0dcdfc530cbe1f370e1f2b06c163fbd6177925a1a8998edd2e726989246a1980fa34e
-6d65d3ca284944cb10254d85db0d8948294fb8174a41206c6b5e36406bae447343f8c9f97420e3
-9f361815dfb268b33ccde5f29e4348a70f95abc30754c839fa7126e5bd882377d6abe3c0c95ba5
-c21190a5e4fff5380b2c23cc1655e593244019e172ba8284618471d95b92c231c1ffe98ff23
-""".replace(
-                    "\n", ""
-                )
-            ),
-            "x5c": [
-                bytes.fromhex(
-                    """308204b23082039aa0030201020210789e1a3657344c52bad2
-2ed1ceb1bfaf300d06092a864886f70d01010b05003041313f303d060355040313364e43552d4e
-54432d4b455949442d394642423739414130463532363237384245443135303932394137313731
-45393641333542454637301e170d3139303430313038353934305a170d32393034303130383539
-34305a300030820122300d06092a864886f70d01010105000382010f003082010a0282010100a6
-60d1fe41564c26f943c70ff89fbd9ed6d957191d5ecaf727393d73cfff85e3ccfb9830027fe84b
-171cc4b0b13811df4d9deff2bce4d8a8f9797169f7b8fc25016d9ba687c003083693716180c8f1
-eccaa4410a9a7fe07b198ad7ba94ecf744e9bef0273a5e0723a4ac197994ca1ac0e5f595433970
-0cf14ead419ae7cde8c3e81389771d5fa3d339f8d0856e918fd3746fa9a944d3c1f1c6a4e0ce3f
-99b5ac5ba05166b3b8695405ae7d3777f9cc8e3ab8570f2191ba4f2cfc4c544337596f48d3d5f5
-f9ae80575bf9eb81d5c477e99c58854645d587dd0ccdea2b0e3d482e69b326b289e65741e6b214
-3fc2bca35ca7dd60e554affdcb85000762ff09b0410203010001a38201e5308201e1300e060355
-1d0f0101ff040403020780300c0603551d130101ff04023000306d0603551d200101ff04633061
-305f06092b060104018237151f3052305006082b0601050507020230441e420054004300500041
-002000200054007200750073007400650064002000200050006c006100740066006f0072006d00
-200020004900640065006e007400690074007930100603551d250409300706056781050803304a
-0603551d110101ff0440303ea43c303a3138300e060567810502030c0569643a31333010060567
-810502020c074e5043543678783014060567810502010c0b69643a3445353434333030301f0603
-551d23041830168014c799ef2371327cb2e9e03838d0a9009fe9ed29e7301d0603551d0e041604
-1429fb5f05c6187d8463b8b250b8f0ff128fd3a0713081b306082b060105050701010481a63081
-a33081a006082b0601050507300286819368747470733a2f2f617a637370726f646e637561696b
-7075626c6973682e626c6f622e636f72652e77696e646f77732e6e65742f6e63752d6e74632d6b
-657969642d39666262373961613066353236323738626564313530393239613731373165393661
-3335626566372f66383530353438392d303235612d343235322d383239302d3934646532633633
-643039362e636572300d06092a864886f70d01010b0500038201010084bc4b9ac3ab6c2438bdec
-dd3d99e6179bfc465995481d856683602bdcf0c26327b8ab77f7b695c8c6aab5f283b079c29369
-29727b839e5bf08c687a33fc59bf281ebf28e9d04e78fd626573028014028badca038e68361017
-a4501b18d56a6a73e35f00e043d8febb7a4c719c837bc5cb801efe23570d6c8b40699ba411fe66
-f6fe5558f7d1c56a7646ba483cd601690a9323caba9257ae561781b13c658083ad1281047d94d4
-c1ab9759d90a16fbe167cec388e7b67027a20dbc1b88986dbb636107ef91ffec22c413ac5fbfec
-3de9ee4aa1c6e4c173e43246193890c8b024587fcc8028eb379f515de3c678b11dfb81aef3547c
-3c6e790577d52f775f9148""".replace(
-                        "\n", ""
-                    )
-                ),
-                bytes.fromhex(
-                    """308205e8308203d0a003020102021333000000a5304bb34bf0
-bee43e0000000000a5300d06092a864886f70d01010b050030818c310b30090603550406130255
-53311330110603550408130a57617368696e67746f6e3110300e060355040713075265646d6f6e
-64311e301c060355040a13154d6963726f736f667420436f72706f726174696f6e313630340603
-550403132d4d6963726f736f66742054504d20526f6f7420436572746966696361746520417574
-686f726974792032303134301e170d3136303831383230323032305a170d323931323331323032
-3032305a3041313f303d060355040313364e43552d4e54432d4b455949442d3946424237394141
-304635323632373842454431353039323941373137314539364133354245463730820122300d06
-092a864886f70d01010105000382010f003082010a0282010100e0b963203494ff3b8b93855f4d
-0086aabf9f5038fe2a2c04311609074565097dd16de61ae1e6086f5d16997dc7ee5342bf9988f6
-bb73ca614f3f5d8ea084fd047112892ae22db792e2efbe24bcb07fd01af124666db7ad53677e45
-6a95e972a659c04fe3569e882afbf019c3c5890c52d2e81d175f97234fbe341406cbf834cafa76
-184c077c9bd058fbe14b4032039142128fe985ee6041819eee86a62a43491d11af9d78f08e722a
-28c0e9b522fed12f172dddfd032a634a6eba2fc90c332997d3ba5f297230cd7d666b6925c0e6ea
-79b2459f68fc283cd7a09e09973a610fb88eb63bb1cc29e0dc5e033ace6b966c78038c1adc049e
-f5360ae28696825ed10203010001a382018b30820187300b0603551d0f040403020186301b0603
-551d250414301206092b06010401823715240605678105080330160603551d20040f300d300b06
-092b060104018237151f30120603551d130101ff040830060101ff020100301d0603551d0e0416
-0414c799ef2371327cb2e9e03838d0a9009fe9ed29e7301f0603551d230418301680147a8c0ace
-2f486217e294d1ae55c152ec7174a45630700603551d1f046930673065a063a061865f68747470
-3a2f2f7777772e6d6963726f736f66742e636f6d2f706b696f70732f63726c2f4d6963726f736f
-667425323054504d253230526f6f742532304365727469666963617465253230417574686f7269
-7479253230323031342e63726c307d06082b060105050701010471306f306d06082b0601050507
-30028661687474703a2f2f7777772e6d6963726f736f66742e636f6d2f706b696f70732f636572
-74732f4d6963726f736f667425323054504d253230526f6f742532304365727469666963617465
-253230417574686f72697479253230323031342e637274300d06092a864886f70d01010b050003
-820201003e91d074e6d6b9719bf13ffd7cd16b733938c092edaa580136ac7d8bb5295242e432f6
-7c3ca5b1c8968b994665e99796a39d579a85cbe6eab02dfce1d08a4ce802b41bf6b00a01533c7c
-f3b96c7d0b9c0f3a5d2e04350037aea5140a5cc781ca73f370998110bd1031cfa427760920574a
-5d7709a1765921d61cb36d91d2ce9d3301f0798ae4b23592b080e70bb535cdf57403f96fe6f0ff
-4c0f0363f785a918a1fd3debfaaaebe6b08724a216b491e95e6e300e3d43e4e156fe3c036afba1
-7ad2b442f904568af1cc3fd9ad1888cbbd9ec98d42e55af5b26fa8790b6b7da677a585fff6ae90
-18e492742d4e9c5ca1a06990a3abff76c6bc4b1e22d8c226d09a96fdcc12801345b647e15850d1
-0d0cdb609160b1a7a7c2c6f0eb3dbc2fcd42b765fd22a5672b26009b9a83b44388b62cb89e9169
-a455ff5be5ce8f7bde0420b5d7d24ec254affdc2e7e946c961ec159b6dfc703e3934f9445b0072
-8e137e11a7c66f76709ca2177b39159fc08593aaa83724b159abb93e535aef53d7d6066a317f92
-d42d17888534fee9daf844260de901c3b18b49ccb2a5f81f0f4639f2e2cfa1ce1d7c791cef6f48
-5d10df989aac02b1e9afd1094603f5307133f5f59ce105a5910700f98fea5a5fcf8f5cf4c797bd
-79d440cc4f9161f5cc61e0e8f06592050cd1f0f0fd066bd1d6335710fdf8159b75281ee1082bff
-1da2fc0b631bd346ac""".replace(
-                        "\n", ""
-                    )
-                ),
-            ],
-            "certInfo": bytes.fromhex(
-                """ff54434780170022000b68cec627cc6411099a1f80
-9fde4379f649aa170c7072d1adf230de439efc80810014f7c8b0cdeb31328648130a19733d6fff
-16e76e1300000003ef605603446ed8c56aa7608d01a6ea5651ee67a8a20022000bdf681917e185
-29c61e1b85a1e7952f3201eb59c609ed5d8e217e5de76b228bbd0022000b0a10d216b0c3ab82bf
-dc1f0a016ab9493384c7aee1937ee8800f76b30c9b71a7""".replace(
-                    "\n", ""
-                )
-            ),
-            "pubArea": bytes.fromhex(
-                """0001000b0006047200209dffcbf36c383ae699fb986
-8dc6dcb89d7153884be2803922c124158bfad22ae001000100800000000000100c706586c7f46c
-dffede0ee0c5ebc8b7a08b36555c8091669e9ef2cb4fd858134a01e9522d3ef924069aeeec2271
-823fe9879b5079eb3123be2eb39a7e954f8b83b5ebefefda25aed01bd19eab6db1962a3713985b
-7a2dd1aa7770b5c1567fb0d18521e14abebbccc16832ef10bb05dcc818bbb70c91c224475928ad
-a6f6181ed64f1cfb40db5e01687454cfacafa8318bdc6a677550baa6e24f8af864fa5324e9d930
-a97cdeb1995b476f21a017b33ab7fe4139f2524c784fcb04cf5241c89f0c145eb23da914ad1722
-d47a843692a0b2a567d94dd808c13678a51c5a0583dc042dcbba1b9ceff12b159d0539248b0994
-ee18128ed50dd7a855e54d2459db005""".replace(
-                    "\n", ""
-                )
-            ),
-        }
-        auth_data = AuthenticatorData(
-            bytes.fromhex(
-                "54ce651ed715b4aaa755eecebd4ea0950815b334bd07d109893e963018cddbd9450000000008987058cadc4b81b6e130de50dcbe9600206053b7b599d16fb3fb11ea17a344850ebd0d18183a5b7ca6dfbd20c63cdb462aa401030339010020590100c706586c7f46cdffede0ee0c5ebc8b7a08b36555c8091669e9ef2cb4fd858134a01e9522d3ef924069aeeec2271823fe9879b5079eb3123be2eb39a7e954f8b83b5ebefefda25aed01bd19eab6db1962a3713985b7a2dd1aa7770b5c1567fb0d18521e14abebbccc16832ef10bb05dcc818bbb70c91c224475928ada6f6181ed64f1cfb40db5e01687454cfacafa8318bdc6a677550baa6e24f8af864fa5324e9d930a97cdeb1995b476f21a017b33ab7fe4139f2524c784fcb04cf5241c89f0c145eb23da914ad1722d47a843692a0b2a567d94dd808c13678a51c5a0583dc042dcbba1b9ceff12b159d0539248b0994ee18128ed50dd7a855e54d2459db0052143010001"  # noqa
-            )
-        )
-        client_param = bytes.fromhex(
-            "057a0ecbe7e3e99e8926941614f6af078c802b110be89eb221d69be2e17a1ba4"
-        )
-
-        res = attestation.verify(statement, auth_data, client_param)
-        self.assertEqual(res.attestation_type, AttestationType.ATT_CA)
-        verify_x509_chain(res.trust_path)
-
-    def test_fido_u2f_attestation(self):
-        attestation = Attestation.for_type("fido-u2f")()
-        self.assertIsInstance(attestation, FidoU2FAttestation)
-
-        statement = {
-            "sig": bytes.fromhex(
-                "30450220324779C68F3380288A1197B6095F7A6EB9B1B1C127F66AE12A99FE8532EC23B9022100E39516AC4D61EE64044D50B415A6A4D4D84BA6D895CB5AB7A1AA7D081DE341FA"  # noqa E501
-            ),
-            "x5c": [
-                bytes.fromhex(
-                    "3082024A30820132A0030201020204046C8822300D06092A864886F70D01010B0500302E312C302A0603550403132359756269636F2055324620526F6F742043412053657269616C203435373230303633313020170D3134303830313030303030305A180F32303530303930343030303030305A302C312A302806035504030C2159756269636F205532462045452053657269616C203234393138323332343737303059301306072A8648CE3D020106082A8648CE3D030107034200043CCAB92CCB97287EE8E639437E21FCD6B6F165B2D5A3F3DB131D31C16B742BB476D8D1E99080EB546C9BBDF556E6210FD42785899E78CC589EBE310F6CDB9FF4A33B3039302206092B0601040182C40A020415312E332E362E312E342E312E34313438322E312E323013060B2B0601040182E51C020101040403020430300D06092A864886F70D01010B050003820101009F9B052248BC4CF42CC5991FCAABAC9B651BBE5BDCDC8EF0AD2C1C1FFB36D18715D42E78B249224F92C7E6E7A05C49F0E7E4C881BF2E94F45E4A21833D7456851D0F6C145A29540C874F3092C934B43D222B8962C0F410CEF1DB75892AF116B44A96F5D35ADEA3822FC7146F6004385BCB69B65C99E7EB6919786703C0D8CD41E8F75CCA44AA8AB725AD8E799FF3A8696A6F1B2656E631B1E40183C08FDA53FA4A8F85A05693944AE179A1339D002D15CABD810090EC722EF5DEF9965A371D415D624B68A2707CAD97BCDD1785AF97E258F33DF56A031AA0356D8E8D5EBCADC74E071636C6B110ACE5CC9B90DFEACAE640FF1BB0F1FE5DB4EFF7A95F060733F5"  # noqa E501
-                )
-            ],
-        }
-        auth_data = AuthenticatorData(
-            bytes.fromhex(
-                "1194228DA8FDBDEEFD261BD7B6595CFD70A50D70C6407BCF013DE96D4EFB17DE41000000000000000000000000000000000000000000403EBD89BF77EC509755EE9C2635EFAAAC7B2B9C5CEF1736C3717DA48534C8C6B654D7FF945F50B5CC4E78055BDD396B64F78DA2C5F96200CCD415CD08FE420038A5010203262001215820E87625896EE4E46DC032766E8087962F36DF9DFE8B567F3763015B1990A60E1422582027DE612D66418BDA1950581EBC5C8C1DAD710CB14C22F8C97045F4612FB20C91"  # noqa E501
-            )
-        )
-        client_param = bytes.fromhex(
-            "687134968222EC17202E42505F8ED2B16AE22F16BB05B88C25DB9E602645F141"
-        )
-
-        res = attestation.verify(statement, auth_data, client_param)
-        self.assertEqual(res.attestation_type, AttestationType.BASIC)
-        self.assertEqual(len(res.trust_path), 1)
-
-        statement["sig"] = b"a" * len(statement["sig"])
-        with self.assertRaises(InvalidSignature):
-            attestation.verify(statement, auth_data, client_param)
-
-    def test_packed_attestation(self):
-        attestation = Attestation.for_type("packed")()
-        self.assertIsInstance(attestation, PackedAttestation)
-
-        statement = {
-            "alg": -7,
-            "sig": bytes.fromhex(
-                "304502200D15DAF337D727AB4719B4027114A2AC43CD565D394CED62C3D9D1D90825F0B3022100989615E7394C87F4AD91F8FDAE86F7A3326DF332B3633DB088AAC76BFFB9A46B"  # noqa E501
-            ),
-            "x5c": [
-                bytes.fromhex(
-                    "308202B73082019FA00302010202041D31330D300D06092A864886F70D01010B0500302A3128302606035504030C1F59756269636F2050726576696577204649444F204174746573746174696F6E301E170D3138303332383036333932345A170D3139303332383036333932345A306E310B300906035504061302534531123010060355040A0C0959756269636F20414231223020060355040B0C1941757468656E74696361746F72204174746573746174696F6E3127302506035504030C1E59756269636F205532462045452053657269616C203438393736333539373059301306072A8648CE3D020106082A8648CE3D030107034200047D71E8367CAFD0EA6CF0D61E4C6A416BA5BB6D8FAD52DB2389AD07969F0F463BFDDDDDC29D39D3199163EE49575A3336C04B3309D607F6160C81E023373E0197A36C306A302206092B0601040182C40A020415312E332E362E312E342E312E34313438322E312E323013060B2B0601040182E51C0201010404030204303021060B2B0601040182E51C01010404120410F8A011F38C0A4D15800617111F9EDC7D300C0603551D130101FF04023000300D06092A864886F70D01010B050003820101009B904CEADBE1F1985486FEAD02BAEAA77E5AB4E6E52B7E6A2666A4DC06E241578169193B63DADEC5B2B78605A128B2E03F7FE2A98EAEB4219F52220995F400CE15D630CF0598BA662D7162459F1AD1FC623067376D4E4091BE65AC1A33D8561B9996C0529EC1816D1710786384D5E8783AA1F7474CB99FE8F5A63A79FF454380361C299D67CB5CC7C79F0D8C09F8849B0500F6D625408C77CBBC26DDEE11CB581BEB7947137AD4F05AAF38BD98DA10042DDCAC277604A395A5B3EAA88A5C8BB27AB59C8127D59D6BBBA5F11506BF7B75FDA7561A0837C46F025FD54DCF1014FC8D17C859507AC57D4B1DEA99485DF0BA8F34D00103C3EEF2EF3BBFEC7A6613DE"  # noqa E501
-                )
-            ],
-        }
-        auth_data = AuthenticatorData(
-            bytes.fromhex(
-                "0021F5FC0B85CD22E60623BCD7D1CA48948909249B4776EB515154E57B66AE124100000003F8A011F38C0A4D15800617111F9EDC7D004060A386206A3AACECBDBB22D601853D955FDC5D11ADFBD1AA6A950D966B348C7663D40173714A9F987DF6461BEADFB9CD6419FFDFE4D4CF2EEC1AA605A4F59BDAA50102032620012158200EDB27580389494D74D2373B8F8C2E8B76FA135946D4F30D0E187E120B423349225820E03400D189E85A55DE9AB0F538ED60736EB750F5F0306A80060FE1B13010560D"  # noqa E501
-            )
-        )
-        client_param = bytes.fromhex(
-            "985B6187D042FB1258892ED637CEC88617DDF5F6632351A545617AA2B75261BF"
-        )
-
-        res = attestation.verify(statement, auth_data, client_param)
-        self.assertEqual(res.attestation_type, AttestationType.BASIC)
-        self.assertEqual(len(res.trust_path), 1)
-
-        statement["sig"] = b"a" * len(statement["sig"])
-        with self.assertRaises(InvalidSignature):
-            attestation.verify(statement, auth_data, client_param)
-
-    def test_android_safetynet_attestation(self):
-        attestation = Attestation.for_type("android-safetynet")()
-        self.assertIsInstance(attestation, AndroidSafetynetAttestation)
-
-        statement = {
-            "ver": "14574037",
-            "response": b"eyJhbGciOiJSUzI1NiIsIng1YyI6WyJNSUlGa2pDQ0JIcWdBd0lCQWdJUVJYcm9OMFpPZFJrQkFBQUFBQVB1bnpBTkJna3Foa2lHOXcwQkFRc0ZBREJDTVFzd0NRWURWUVFHRXdKVlV6RWVNQndHQTFVRUNoTVZSMjl2WjJ4bElGUnlkWE4wSUZObGNuWnBZMlZ6TVJNd0VRWURWUVFERXdwSFZGTWdRMEVnTVU4eE1CNFhEVEU0TVRBeE1EQTNNVGswTlZvWERURTVNVEF3T1RBM01UazBOVm93YkRFTE1Ba0dBMVVFQmhNQ1ZWTXhFekFSQmdOVkJBZ1RDa05oYkdsbWIzSnVhV0V4RmpBVUJnTlZCQWNURFUxdmRXNTBZV2x1SUZacFpYY3hFekFSQmdOVkJBb1RDa2R2YjJkc1pTQk1URU14R3pBWkJnTlZCQU1URW1GMGRHVnpkQzVoYm1SeWIybGtMbU52YlRDQ0FTSXdEUVlKS29aSWh2Y05BUUVCQlFBRGdnRVBBRENDQVFvQ2dnRUJBTmpYa3owZUsxU0U0bSsvRzV3T28rWEdTRUNycWRuODhzQ3BSN2ZzMTRmSzBSaDNaQ1laTEZIcUJrNkFtWlZ3Mks5RkcwTzlyUlBlUURJVlJ5RTMwUXVuUzl1Z0hDNGVnOW92dk9tK1FkWjJwOTNYaHp1blFFaFVXWEN4QURJRUdKSzNTMmFBZnplOTlQTFMyOWhMY1F1WVhIRGFDN09acU5ub3NpT0dpZnM4djFqaTZIL3hobHRDWmUybEorN0d1dHpleEtweHZwRS90WlNmYlk5MDVxU2xCaDlmcGowMTVjam5RRmtVc0FVd21LVkFVdWVVejR0S2NGSzRwZXZOTGF4RUFsK09raWxNdElZRGFjRDVuZWw0eEppeXM0MTNoYWdxVzBXaGg1RlAzOWhHazlFL0J3UVRqYXpTeEdkdlgwbTZ4RlloaC8yVk15WmpUNEt6UEpFQ0F3RUFBYU9DQWxnd2dnSlVNQTRHQTFVZER3RUIvd1FFQXdJRm9EQVRCZ05WSFNVRUREQUtCZ2dyQmdFRkJRY0RBVEFNQmdOVkhSTUJBZjhFQWpBQU1CMEdBMVVkRGdRV0JCUXFCUXdHV29KQmExb1RLcXVwbzRXNnhUNmoyREFmQmdOVkhTTUVHREFXZ0JTWTBmaHVFT3ZQbSt4Z254aVFHNkRyZlFuOUt6QmtCZ2dyQmdFRkJRY0JBUVJZTUZZd0p3WUlLd1lCQlFVSE1BR0dHMmgwZEhBNkx5OXZZM053TG5CcmFTNW5iMjluTDJkMGN6RnZNVEFyQmdnckJnRUZCUWN3QW9ZZmFIUjBjRG92TDNCcmFTNW5iMjluTDJkemNqSXZSMVJUTVU4eExtTnlkREFkQmdOVkhSRUVGakFVZ2hKaGRIUmxjM1F1WVc1a2NtOXBaQzVqYjIwd0lRWURWUjBnQkJvd0dEQUlCZ1puZ1F3QkFnSXdEQVlLS3dZQkJBSFdlUUlGQXpBdkJnTlZIUjhFS0RBbU1DU2dJcUFnaGg1b2RIUndPaTh2WTNKc0xuQnJhUzVuYjI5bkwwZFVVekZQTVM1amNtd3dnZ0VFQmdvckJnRUVBZFo1QWdRQ0JJSDFCSUh5QVBBQWR3Q2t1UW1RdEJoWUZJZTdFNkxNWjNBS1BEV1lCUGtiMzdqamQ4ME95QTNjRUFBQUFXWmREM1BMQUFBRUF3QklNRVlDSVFDU1pDV2VMSnZzaVZXNkNnK2dqLzl3WVRKUnp1NEhpcWU0ZVk0Yy9teXpqZ0loQUxTYmkvVGh6Y3pxdGlqM2RrM3ZiTGNJVzNMbDJCMG83NUdRZGhNaWdiQmdBSFVBVmhRR21pL1h3dXpUOWVHOVJMSSt4MFoydWJ5WkVWekE3NVNZVmRhSjBOMEFBQUZtWFE5ejVBQUFCQU1BUmpCRUFpQmNDd0E5ajdOVEdYUDI3OHo0aHIvdUNIaUFGTHlvQ3EySzAreUxSd0pVYmdJZ2Y4Z0hqdnB3Mm1CMUVTanEyT2YzQTBBRUF3Q2tuQ2FFS0ZVeVo3Zi9RdEl3RFFZSktvWklodmNOQVFFTEJRQURnZ0VCQUk5blRmUktJV2d0bFdsM3dCTDU1RVRWNmthenNwaFcxeUFjNUR1bTZYTzQxa1p6d0o2MXdKbWRSUlQvVXNDSXkxS0V0MmMwRWpnbG5KQ0YyZWF3Y0VXbExRWTJYUEx5RmprV1FOYlNoQjFpNFcyTlJHelBodDNtMWI0OWhic3R1WE02dFg1Q3lFSG5UaDhCb200L1dsRmloemhnbjgxRGxkb2d6L0syVXdNNlM2Q0IvU0V4a2lWZnYremJKMHJqdmc5NEFsZGpVZlV3a0k5Vk5NakVQNWU4eWRCM29MbDZnbHBDZUY1ZGdmU1g0VTl4MzVvai9JSWQzVUUvZFBwYi9xZ0d2c2tmZGV6dG1VdGUvS1Ntcml3Y2dVV1dlWGZUYkkzenNpa3daYmtwbVJZS21qUG1odjRybGl6R0NHdDhQbjhwcThNMktEZi9QM2tWb3QzZTE4UT0iLCJNSUlFU2pDQ0F6S2dBd0lCQWdJTkFlTzBtcUdOaXFtQkpXbFF1REFOQmdrcWhraUc5dzBCQVFzRkFEQk1NU0F3SGdZRFZRUUxFeGRIYkc5aVlXeFRhV2R1SUZKdmIzUWdRMEVnTFNCU01qRVRNQkVHQTFVRUNoTUtSMnh2WW1Gc1UybG5iakVUTUJFR0ExVUVBeE1LUjJ4dlltRnNVMmxuYmpBZUZ3MHhOekEyTVRVd01EQXdOREphRncweU1URXlNVFV3TURBd05ESmFNRUl4Q3pBSkJnTlZCQVlUQWxWVE1SNHdIQVlEVlFRS0V4VkhiMjluYkdVZ1ZISjFjM1FnVTJWeWRtbGpaWE14RXpBUkJnTlZCQU1UQ2tkVVV5QkRRU0F4VHpFd2dnRWlNQTBHQ1NxR1NJYjNEUUVCQVFVQUE0SUJEd0F3Z2dFS0FvSUJBUURRR005RjFJdk4wNXprUU85K3ROMXBJUnZKenp5T1RIVzVEekVaaEQyZVBDbnZVQTBRazI4RmdJQ2ZLcUM5RWtzQzRUMmZXQllrL2pDZkMzUjNWWk1kUy9kTjRaS0NFUFpSckF6RHNpS1VEelJybUJCSjV3dWRnem5kSU1ZY0xlL1JHR0ZsNXlPRElLZ2pFdi9TSkgvVUwrZEVhbHROMTFCbXNLK2VRbU1GKytBY3hHTmhyNTlxTS85aWw3MUkyZE44RkdmY2Rkd3VhZWo0YlhocDBMY1FCYmp4TWNJN0pQMGFNM1Q0SStEc2F4bUtGc2JqemFUTkM5dXpwRmxnT0lnN3JSMjV4b3luVXh2OHZObWtxN3pkUEdIWGt4V1k3b0c5aitKa1J5QkFCazdYckpmb3VjQlpFcUZKSlNQazdYQTBMS1cwWTN6NW96MkQwYzF0Skt3SEFnTUJBQUdqZ2dFek1JSUJMekFPQmdOVkhROEJBZjhFQkFNQ0FZWXdIUVlEVlIwbEJCWXdGQVlJS3dZQkJRVUhBd0VHQ0NzR0FRVUZCd01DTUJJR0ExVWRFd0VCL3dRSU1BWUJBZjhDQVFBd0hRWURWUjBPQkJZRUZKalIrRzRRNjgrYjdHQ2ZHSkFib090OUNmMHJNQjhHQTFVZEl3UVlNQmFBRkp2aUIxZG5IQjdBYWdiZVdiU2FMZC9jR1lZdU1EVUdDQ3NHQVFVRkJ3RUJCQ2t3SnpBbEJnZ3JCZ0VGQlFjd0FZWVphSFIwY0RvdkwyOWpjM0F1Y0d0cExtZHZiMmN2WjNOeU1qQXlCZ05WSFI4RUt6QXBNQ2VnSmFBamhpRm9kSFJ3T2k4dlkzSnNMbkJyYVM1bmIyOW5MMmR6Y2pJdlozTnlNaTVqY213d1B3WURWUjBnQkRnd05qQTBCZ1puZ1F3QkFnSXdLakFvQmdnckJnRUZCUWNDQVJZY2FIUjBjSE02THk5d2Eya3VaMjl2Wnk5eVpYQnZjMmwwYjNKNUx6QU5CZ2txaGtpRzl3MEJBUXNGQUFPQ0FRRUFHb0ErTm5uNzh5NnBSamQ5WGxRV05hN0hUZ2laL3IzUk5Ha21VbVlIUFFxNlNjdGk5UEVhanZ3UlQyaVdUSFFyMDJmZXNxT3FCWTJFVFV3Z1pRK2xsdG9ORnZoc085dHZCQ09JYXpwc3dXQzlhSjl4anU0dFdEUUg4TlZVNllaWi9YdGVEU0dVOVl6SnFQalk4cTNNRHhyem1xZXBCQ2Y1bzhtdy93SjRhMkc2eHpVcjZGYjZUOE1jRE8yMlBMUkw2dTNNNFR6czNBMk0xajZieWtKWWk4d1dJUmRBdktMV1p1L2F4QlZielltcW13a201ekxTRFc1bklBSmJFTENRQ1p3TUg1NnQyRHZxb2Z4czZCQmNDRklaVVNweHU2eDZ0ZDBWN1N2SkNDb3NpclNtSWF0ai85ZFNTVkRRaWJldDhxLzdVSzR2NFpVTjgwYXRuWnoxeWc9PSJdfQ.eyJub25jZSI6InpiNVE5NFVPaHFOWnRVUWEraWY0NnF1UDRwZWZQN2JnQWRpQ3hraDFZRGs9IiwidGltZXN0YW1wTXMiOjE1NDM0ODI1Njg4NTgsImFwa1BhY2thZ2VOYW1lIjoiY29tLmdvb2dsZS5hbmRyb2lkLmdtcyIsImFwa0RpZ2VzdFNoYTI1NiI6InIxYzZiTkJmQ0hjZHcvZWpKSE1NWjhoakIrU0xXa1BSM0lreTZjV1dhNE09IiwiY3RzUHJvZmlsZU1hdGNoIjp0cnVlLCJhcGtDZXJ0aWZpY2F0ZURpZ2VzdFNoYTI1NiI6WyI4UDFzVzBFUEpjc2x3N1V6UnNpWEw2NHcrTzUwRWQrUkJJQ3RheTFnMjRNPSJdLCJiYXNpY0ludGVncml0eSI6dHJ1ZX0.Lq9WpOJ_GilocvPCTbIN2K5FtppXW2fTQzCW2pvb1Bo5qOZnJ0oOYBUqMgxx-zghlluSkkIIfPTvYl2zZUQsY-SNlBx7JASqDbksMyRsdU9r1Jn8D2zEtipFgjmZUkozi7AngnHoA5d0Yp-NF6slmr_FLMpAOnLZY9lREw8Cxnmso3Ph7zYUu7O5SxaRGwj8eMKydYJYHa23h2C8acuQKgSWL2YlG9T-oKT0CJ8jOSrKnHr39eMo7PFX0464diUvXUsv_M9kRIIQqCP0LzilGMdJVUrvFU7kg8csnFP6KMDfY70RGZ5ey3eNqs_D5-pjPfC4XPsPsksmy_wf-3UOmw",  # noqa E501
-        }
-
-        auth_data = AuthenticatorData(
-            bytes.fromhex(
-                "720c20fde835785e0f5ebcad8ef6a7bd88804a91612a2e820e0059b8d5358797450000000000000000000000000000000000000000004101c8fd9b533d6adacf6710ebcfb39f6361c4d7e8787db47dc0a75ae0e7c862198c9c83b81ef2547bb5669314095fc846af4ecac6875f7b230cac7359c76b0c20f7a5010203262001215820a28851e2d411b5b2c289da50d41cc41be88498941fc256dab500b21c8dafe8d1225820d289dd467715be06a622771a7b21e1bbe2372f8713d20dd7888a6e7ae1845ca8"  # noqa E501
-            )
-        )
-        client_param = bytes.fromhex(
-            "8422c80f3428e4e6465f76ebc8a4a93759a0a2e1fb845ee5eea7a02027408520"
-        )
-
-        res = attestation.verify(statement, auth_data, client_param)
-        self.assertEqual(res.attestation_type, AttestationType.BASIC)
-        verify_x509_chain(res.trust_path + [_GSR2_DER])
-
-    def test_apple_attestation(self):
-        attestation = Attestation.for_type("apple")()
-        self.assertIsInstance(attestation, AppleAttestation)
-
-        statement = {
-            "alg": -7,
-            "x5c": [
-                bytes.fromhex(
-                    "30820242308201c9a00302010202060176af5359ff300a06082a8648ce3d0403023048311c301a06035504030c134170706c6520576562417574686e204341203131133011060355040a0c0a4170706c6520496e632e3113301106035504080c0a43616c69666f726e6961301e170d3230313232383136323732345a170d3230313233313136323732345a3081913149304706035504030c4038303966626331313065613835663233613862323435616563363136333530663337646665393632313232373336653431663862646365663334366138306439311a3018060355040b0c114141412043657274696669636174696f6e31133011060355040a0c0a4170706c6520496e632e3113301106035504080c0a43616c69666f726e69613059301306072a8648ce3d020106082a8648ce3d030107034200041f46a2f159fde354598cdd47e005f1b6e7c9f00ed2a941ec7a88d222f5bcf55d6b078bc5b0be9552d85a974921f5bb848e2bbc3aecd6f71a386d2c87d6eafd37a3553053300c0603551d130101ff04023000300e0603551d0f0101ff0404030204f0303306092a864886f76364080204263024a1220420e56fb6212b3aae885294464fb10184b7fea62c48a6d78e61194e07ae6dacc132300a06082a8648ce3d040302036700306402301de8f0f238eee4f5ae80c59290b51e8c3f79397bf198e444ba162d4fccaab8558b072cf00a7c662f9058ff2a98af61ae0230149403b9643066e73a98d3659563dc4da49bf84e82b2b5bbeaf57755646fa243f36344d44b80a5798203bca023e030c7"  # noqa E501
-                ),
-                bytes.fromhex(
-                    "30820234308201baa003020102021056255395c7a7fb40ebe228d8260853b6300a06082a8648ce3d040303304b311f301d06035504030c164170706c6520576562417574686e20526f6f7420434131133011060355040a0c0a4170706c6520496e632e3113301106035504080c0a43616c69666f726e6961301e170d3230303331383138333830315a170d3330303331333030303030305a3048311c301a06035504030c134170706c6520576562417574686e204341203131133011060355040a0c0a4170706c6520496e632e3113301106035504080c0a43616c69666f726e69613076301006072a8648ce3d020106052b8104002203620004832e872f261491810225b9f5fcd6bb6378b5f55f3fcb045bc735993475fd549044df9bfe19211765c69a1dda050b38d45083401a434fb24d112d56c3e1cfbfcb9891fec0696081bef96cbc77c88dddaf46a5aee1dd515b5afaab93be9c0b2691a366306430120603551d130101ff040830060101ff020100301f0603551d2304183016801426d764d9c578c25a67d1a7de6b12d01b63f1c6d7301d0603551d0e04160414ebae82c4ffa1ac5b51d4cf24610500be63bd7788300e0603551d0f0101ff040403020106300a06082a8648ce3d0403030368003065023100dd8b1a3481a5fad9dbb4e7657b841e144c27b75b876a4186c2b1475750337227efe554457ef648950c632e5c483e70c102302c8a6044dc201fcfe59bc34d2930c1487851d960ed6a75f1eb4acabe38cd25b897d0c805bef0c7f78b07a571c6e80e07"  # noqa E501
-                ),
-            ],
-        }
-
-        auth_data = AuthenticatorData(
-            bytes.fromhex(
-                "c46cef82ad1b546477591d008b08759ec3e6d2ecb4f39474bfea6969925d03b7450000000000000000000000000000000000000000001473d9429f4052d84debd035eb5bb7e716e3b81863a50102032620012158201f46a2f159fde354598cdd47e005f1b6e7c9f00ed2a941ec7a88d222f5bcf55d2258206b078bc5b0be9552d85a974921f5bb848e2bbc3aecd6f71a386d2c87d6eafd37"  # noqa E501
-            )
-        )
-        client_param = bytes.fromhex(
-            "0d3ce80fabbc3adb9dd891deabb8db84603ea1fe2da8b5d4b46d6591aab342f3"
-        )
-
-        res = attestation.verify(statement, auth_data, client_param)
-        self.assertEqual(res.attestation_type, AttestationType.ANON_CA)
-        self.assertEqual(len(res.trust_path), 2)
-        verify_x509_chain(res.trust_path)
+# Copyright (c) 2013 Yubico AB
+# All rights reserved.
+#
+#   Redistribution and use in source and binary forms, with or
+#   without modification, are permitted provided that the following
+#   conditions are met:
+#
+#    1. Redistributions of source code must retain the above copyright
+#       notice, this list of conditions and the following disclaimer.
+#    2. Redistributions in binary form must reproduce the above
+#       copyright notice, this list of conditions and the following
+#       disclaimer in the documentation and/or other materials provided
+#       with the distribution.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
+# FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
+# COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
+# INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
+# BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
+# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
+# ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+# POSSIBILITY OF SUCH DAMAGE.
+
+from fido2.webauthn import AuthenticatorData
+from fido2.attestation import (
+    Attestation,
+    AttestationType,
+    UnsupportedAttestation,
+    FidoU2FAttestation,
+    PackedAttestation,
+    TpmAttestation,
+    NoneAttestation,
+    AndroidSafetynetAttestation,
+    AppleAttestation,
+    InvalidData,
+    InvalidSignature,
+    UnsupportedType,
+    verify_x509_chain,
+)
+from cryptography.exceptions import UnsupportedAlgorithm, _Reasons
+
+import unittest
+
+
+# GS Root R2 (https://pki.goog/)
+_GSR2_DER = bytes.fromhex(
+    "308203ba308202a2a003020102020b0400000000010f8626e60d300d06092a864886f70d0101050500304c3120301e060355040b1317476c6f62616c5369676e20526f6f74204341202d20523231133011060355040a130a476c6f62616c5369676e311330110603550403130a476c6f62616c5369676e301e170d3036313231353038303030305a170d3231313231353038303030305a304c3120301e060355040b1317476c6f62616c5369676e20526f6f74204341202d20523231133011060355040a130a476c6f62616c5369676e311330110603550403130a476c6f62616c5369676e30820122300d06092a864886f70d01010105000382010f003082010a0282010100a6cf240ebe2e6f28994542c4ab3e21549b0bd37f8470fa12b3cbbf875fc67f86d3b2305cd6fdadf17bdce5f86096099210f5d053defb7b7e7388ac52887b4aa6ca49a65ea8a78c5a11bc7a82ebbe8ce9b3ac962507974a992a072fb41e77bf8a0fb5027c1b96b8c5b93a2cbcd612b9eb597de2d006865f5e496ab5395e8834ecbc780c0898846ca8cd4bb4a07d0c794df0b82dcb21cad56c5b7de1a02984a1f9d39449cb24629120bcdd0bd5d9ccf9ea270a2b7391c69d1bacc8cbe8e0a0f42f908b4dfbb0361bf6197a85e06df26113885c9fe0930a51978a5aceafabd5f7aa09aa60bddcd95fdf72a960135e0001c94afa3fa4ea070321028e82ca03c29b8f0203010001a3819c308199300e0603551d0f0101ff040403020106300f0603551d130101ff040530030101ff301d0603551d0e041604149be20757671c1ec06a06de59b49a2ddfdc19862e30360603551d1f042f302d302ba029a0278625687474703a2f2f63726c2e676c6f62616c7369676e2e6e65742f726f6f742d72322e63726c301f0603551d230418301680149be20757671c1ec06a06de59b49a2ddfdc19862e300d06092a864886f70d01010505000382010100998153871c68978691ece04ab8440bab81ac274fd6c1b81c4378b30c9afcea2c3c6e611b4d4b29f59f051d26c1b8e983006245b6a90893b9a9334b189ac2f887884edbdd71341ac154da463fe0d32aab6d5422f53a62cd206fba2989d7dd91eed35ca23ea15b41f5dfe564432de9d539abd2a2dfb78bd0c080191c45c02d8ce8f82da4745649c505b54f15de6e44783987a87ebbf3791891bbf46f9dc1f08c358c5d01fbc36db9ef446d7946317e0afea982c1ffefab6e20c450c95f9d4d9b178c0ce501c9a0416a7353faa550b46e250ffb4c18f4fd52d98e69b1e8110fde88d8fb1d49f7aade95cf2078c26012db25408c6afc7e4238406412f79e81e1932e"  # noqa E501
+)
+
+
+class TestAttestationObject(unittest.TestCase):
+    def test_unsupported_attestation(self):
+        attestation = Attestation.for_type("__unsupported__")()
+        self.assertIsInstance(attestation, UnsupportedAttestation)
+        with self.assertRaises(UnsupportedType) as ctx:
+            attestation.verify({}, 0, b"")
+        self.assertEqual(ctx.exception.fmt, "__unsupported__")
+
+    def test_none_attestation(self):
+        attestation = Attestation.for_type("none")()
+        self.assertIsInstance(attestation, NoneAttestation)
+
+        auth_data = AuthenticatorData(
+            bytes.fromhex(
+                "0021F5FC0B85CD22E60623BCD7D1CA48948909249B4776EB515154E57B66AE12410000002BF8A011F38C0A4D15800617111F9EDC7D0040A17370D9C1759005700C8DE77E7DFD3A0A5300E0A26E5213AA40D6DF10EE4028B58B5F34167035D840BEBAE0C5CE8FD05AD9BD33E3BE7D1C558D81AB4803570BA5010203262001215820A5FD5CE1B1C458C530A54FA61B31BF6B04BE8B97AFDE54DD8CBB69275A8A1BE1225820FA3A3231DD9DEED9D1897BE5A6228C59501E4BCD12975D3DFF730F01278EA61C"  # noqa E501
+            )
+        )
+        res = attestation.verify({}, auth_data, b"deadbeef" * 8)
+        self.assertEqual(res.attestation_type, AttestationType.NONE)
+        self.assertEqual(res.trust_path, [])
+
+        with self.assertRaises(InvalidData):
+            attestation.verify({"not": "empty"}, auth_data, b"deadbeef" * 8)
+
+    def test_none_windows_hello_attestation(self):
+        attestation = Attestation.for_type("none")()
+        self.assertIsInstance(attestation, NoneAttestation)
+
+        auth_data = AuthenticatorData(
+            bytes.fromhex(
+                "54ce651ed715b4aaa755eecebd4ea0950815b334bd07d109893e963018cddbd945000000006028b017b1d44c02b4b3afcdafc96bb200201decfcd6d6a05c2826d52348afdc70a9800df007845047b1a23706aa6e2f315ca401030339010020590100af59f4ad4f71da800bb91045b267e240e06317f7b2b1d76f78e239a433811faeca58a1869fb00225eb2727f81b6b20cbc18c0ad8d38fa450e8df11b4ad3bc3ee5d13c77ed172fa3af0195ec6ac0c4bac8c950115dfce6d38737cbafefbe117d8401cd56c638043a0d585131bc48a153b17a8dcb96671e15a90ba1b4ff810b138b77ac0a050b039b87b6089dd8dfa45611b992109d554aad3e6b72ac82d801496e4d2d230aa466090bbbf4f5632fe4b588e4f571462378fa6f514a536a5945b223c8d98f730b7cf85de86b98c217090f9e9ebf9643cf3feceeacb837d7a18542e03271cd8c70cf81186cdb63e4cbf4efc0cbbd3c93231b06f19580d0a980264d12143010001"  # noqa
+            )
+        )  # noqa
+        res = attestation.verify({}, auth_data, b"deadbeef" * 8)
+        self.assertEqual(res.attestation_type, AttestationType.NONE)
+        self.assertEqual(res.trust_path, [])
+
+        with self.assertRaises(InvalidData):
+            attestation.verify({"not": "empty"}, auth_data, b"deadbeef" * 8)
+
+    def test_tpm_windows_hello_attestation(self):
+        attestation = Attestation.for_type("tpm")()
+        self.assertIsInstance(attestation, TpmAttestation)
+        statement = {
+            "alg": -65535,
+            "sig": bytes.fromhex(
+                """80e564d8cbb236577de68d2e68ecae200a8eaf6992889b5
+fdc24624a4cb69caaab18df965058fbac39df9714b9c80b9a12d715cfc4dd15ed3a6e191a6d26e
+7206fd402b0733c2c8b91f62ad44e4d41c940e2e914253b1d1a1c8889b1cdaf668b5449245dc33
+1fab12e0b0dcdfc530cbe1f370e1f2b06c163fbd6177925a1a8998edd2e726989246a1980fa34e
+6d65d3ca284944cb10254d85db0d8948294fb8174a41206c6b5e36406bae447343f8c9f97420e3
+9f361815dfb268b33ccde5f29e4348a70f95abc30754c839fa7126e5bd882377d6abe3c0c95ba5
+c21190a5e4fff5380b2c23cc1655e593244019e172ba8284618471d95b92c231c1ffe98ff23
+""".replace(
+                    "\n", ""
+                )
+            ),
+            "x5c": [
+                bytes.fromhex(
+                    """308204b23082039aa0030201020210789e1a3657344c52bad2
+2ed1ceb1bfaf300d06092a864886f70d01010b05003041313f303d060355040313364e43552d4e
+54432d4b455949442d394642423739414130463532363237384245443135303932394137313731
+45393641333542454637301e170d3139303430313038353934305a170d32393034303130383539
+34305a300030820122300d06092a864886f70d01010105000382010f003082010a0282010100a6
+60d1fe41564c26f943c70ff89fbd9ed6d957191d5ecaf727393d73cfff85e3ccfb9830027fe84b
+171cc4b0b13811df4d9deff2bce4d8a8f9797169f7b8fc25016d9ba687c003083693716180c8f1
+eccaa4410a9a7fe07b198ad7ba94ecf744e9bef0273a5e0723a4ac197994ca1ac0e5f595433970
+0cf14ead419ae7cde8c3e81389771d5fa3d339f8d0856e918fd3746fa9a944d3c1f1c6a4e0ce3f
+99b5ac5ba05166b3b8695405ae7d3777f9cc8e3ab8570f2191ba4f2cfc4c544337596f48d3d5f5
+f9ae80575bf9eb81d5c477e99c58854645d587dd0ccdea2b0e3d482e69b326b289e65741e6b214
+3fc2bca35ca7dd60e554affdcb85000762ff09b0410203010001a38201e5308201e1300e060355
+1d0f0101ff040403020780300c0603551d130101ff04023000306d0603551d200101ff04633061
+305f06092b060104018237151f3052305006082b0601050507020230441e420054004300500041
+002000200054007200750073007400650064002000200050006c006100740066006f0072006d00
+200020004900640065006e007400690074007930100603551d250409300706056781050803304a
+0603551d110101ff0440303ea43c303a3138300e060567810502030c0569643a31333010060567
+810502020c074e5043543678783014060567810502010c0b69643a3445353434333030301f0603
+551d23041830168014c799ef2371327cb2e9e03838d0a9009fe9ed29e7301d0603551d0e041604
+1429fb5f05c6187d8463b8b250b8f0ff128fd3a0713081b306082b060105050701010481a63081
+a33081a006082b0601050507300286819368747470733a2f2f617a637370726f646e637561696b
+7075626c6973682e626c6f622e636f72652e77696e646f77732e6e65742f6e63752d6e74632d6b
+657969642d39666262373961613066353236323738626564313530393239613731373165393661
+3335626566372f66383530353438392d303235612d343235322d383239302d3934646532633633
+643039362e636572300d06092a864886f70d01010b0500038201010084bc4b9ac3ab6c2438bdec
+dd3d99e6179bfc465995481d856683602bdcf0c26327b8ab77f7b695c8c6aab5f283b079c29369
+29727b839e5bf08c687a33fc59bf281ebf28e9d04e78fd626573028014028badca038e68361017
+a4501b18d56a6a73e35f00e043d8febb7a4c719c837bc5cb801efe23570d6c8b40699ba411fe66
+f6fe5558f7d1c56a7646ba483cd601690a9323caba9257ae561781b13c658083ad1281047d94d4
+c1ab9759d90a16fbe167cec388e7b67027a20dbc1b88986dbb636107ef91ffec22c413ac5fbfec
+3de9ee4aa1c6e4c173e43246193890c8b024587fcc8028eb379f515de3c678b11dfb81aef3547c
+3c6e790577d52f775f9148""".replace(
+                        "\n", ""
+                    )
+                ),
+                bytes.fromhex(
+                    """308205e8308203d0a003020102021333000000a5304bb34bf0
+bee43e0000000000a5300d06092a864886f70d01010b050030818c310b30090603550406130255
+53311330110603550408130a57617368696e67746f6e3110300e060355040713075265646d6f6e
+64311e301c060355040a13154d6963726f736f667420436f72706f726174696f6e313630340603
+550403132d4d6963726f736f66742054504d20526f6f7420436572746966696361746520417574
+686f726974792032303134301e170d3136303831383230323032305a170d323931323331323032
+3032305a3041313f303d060355040313364e43552d4e54432d4b455949442d3946424237394141
+304635323632373842454431353039323941373137314539364133354245463730820122300d06
+092a864886f70d01010105000382010f003082010a0282010100e0b963203494ff3b8b93855f4d
+0086aabf9f5038fe2a2c04311609074565097dd16de61ae1e6086f5d16997dc7ee5342bf9988f6
+bb73ca614f3f5d8ea084fd047112892ae22db792e2efbe24bcb07fd01af124666db7ad53677e45
+6a95e972a659c04fe3569e882afbf019c3c5890c52d2e81d175f97234fbe341406cbf834cafa76
+184c077c9bd058fbe14b4032039142128fe985ee6041819eee86a62a43491d11af9d78f08e722a
+28c0e9b522fed12f172dddfd032a634a6eba2fc90c332997d3ba5f297230cd7d666b6925c0e6ea
+79b2459f68fc283cd7a09e09973a610fb88eb63bb1cc29e0dc5e033ace6b966c78038c1adc049e
+f5360ae28696825ed10203010001a382018b30820187300b0603551d0f040403020186301b0603
+551d250414301206092b06010401823715240605678105080330160603551d20040f300d300b06
+092b060104018237151f30120603551d130101ff040830060101ff020100301d0603551d0e0416
+0414c799ef2371327cb2e9e03838d0a9009fe9ed29e7301f0603551d230418301680147a8c0ace
+2f486217e294d1ae55c152ec7174a45630700603551d1f046930673065a063a061865f68747470
+3a2f2f7777772e6d6963726f736f66742e636f6d2f706b696f70732f63726c2f4d6963726f736f
+667425323054504d253230526f6f742532304365727469666963617465253230417574686f7269
+7479253230323031342e63726c307d06082b060105050701010471306f306d06082b0601050507
+30028661687474703a2f2f7777772e6d6963726f736f66742e636f6d2f706b696f70732f636572
+74732f4d6963726f736f667425323054504d253230526f6f742532304365727469666963617465
+253230417574686f72697479253230323031342e637274300d06092a864886f70d01010b050003
+820201003e91d074e6d6b9719bf13ffd7cd16b733938c092edaa580136ac7d8bb5295242e432f6
+7c3ca5b1c8968b994665e99796a39d579a85cbe6eab02dfce1d08a4ce802b41bf6b00a01533c7c
+f3b96c7d0b9c0f3a5d2e04350037aea5140a5cc781ca73f370998110bd1031cfa427760920574a
+5d7709a1765921d61cb36d91d2ce9d3301f0798ae4b23592b080e70bb535cdf57403f96fe6f0ff
+4c0f0363f785a918a1fd3debfaaaebe6b08724a216b491e95e6e300e3d43e4e156fe3c036afba1
+7ad2b442f904568af1cc3fd9ad1888cbbd9ec98d42e55af5b26fa8790b6b7da677a585fff6ae90
+18e492742d4e9c5ca1a06990a3abff76c6bc4b1e22d8c226d09a96fdcc12801345b647e15850d1
+0d0cdb609160b1a7a7c2c6f0eb3dbc2fcd42b765fd22a5672b26009b9a83b44388b62cb89e9169
+a455ff5be5ce8f7bde0420b5d7d24ec254affdc2e7e946c961ec159b6dfc703e3934f9445b0072
+8e137e11a7c66f76709ca2177b39159fc08593aaa83724b159abb93e535aef53d7d6066a317f92
+d42d17888534fee9daf844260de901c3b18b49ccb2a5f81f0f4639f2e2cfa1ce1d7c791cef6f48
+5d10df989aac02b1e9afd1094603f5307133f5f59ce105a5910700f98fea5a5fcf8f5cf4c797bd
+79d440cc4f9161f5cc61e0e8f06592050cd1f0f0fd066bd1d6335710fdf8159b75281ee1082bff
+1da2fc0b631bd346ac""".replace(
+                        "\n", ""
+                    )
+                ),
+            ],
+            "certInfo": bytes.fromhex(
+                """ff54434780170022000b68cec627cc6411099a1f80
+9fde4379f649aa170c7072d1adf230de439efc80810014f7c8b0cdeb31328648130a19733d6fff
+16e76e1300000003ef605603446ed8c56aa7608d01a6ea5651ee67a8a20022000bdf681917e185
+29c61e1b85a1e7952f3201eb59c609ed5d8e217e5de76b228bbd0022000b0a10d216b0c3ab82bf
+dc1f0a016ab9493384c7aee1937ee8800f76b30c9b71a7""".replace(
+                    "\n", ""
+                )
+            ),
+            "pubArea": bytes.fromhex(
+                """0001000b0006047200209dffcbf36c383ae699fb986
+8dc6dcb89d7153884be2803922c124158bfad22ae001000100800000000000100c706586c7f46c
+dffede0ee0c5ebc8b7a08b36555c8091669e9ef2cb4fd858134a01e9522d3ef924069aeeec2271
+823fe9879b5079eb3123be2eb39a7e954f8b83b5ebefefda25aed01bd19eab6db1962a3713985b
+7a2dd1aa7770b5c1567fb0d18521e14abebbccc16832ef10bb05dcc818bbb70c91c224475928ad
+a6f6181ed64f1cfb40db5e01687454cfacafa8318bdc6a677550baa6e24f8af864fa5324e9d930
+a97cdeb1995b476f21a017b33ab7fe4139f2524c784fcb04cf5241c89f0c145eb23da914ad1722
+d47a843692a0b2a567d94dd808c13678a51c5a0583dc042dcbba1b9ceff12b159d0539248b0994
+ee18128ed50dd7a855e54d2459db005""".replace(
+                    "\n", ""
+                )
+            ),
+        }
+        auth_data = AuthenticatorData(
+            bytes.fromhex(
+                "54ce651ed715b4aaa755eecebd4ea0950815b334bd07d109893e963018cddbd9450000000008987058cadc4b81b6e130de50dcbe9600206053b7b599d16fb3fb11ea17a344850ebd0d18183a5b7ca6dfbd20c63cdb462aa401030339010020590100c706586c7f46cdffede0ee0c5ebc8b7a08b36555c8091669e9ef2cb4fd858134a01e9522d3ef924069aeeec2271823fe9879b5079eb3123be2eb39a7e954f8b83b5ebefefda25aed01bd19eab6db1962a3713985b7a2dd1aa7770b5c1567fb0d18521e14abebbccc16832ef10bb05dcc818bbb70c91c224475928ada6f6181ed64f1cfb40db5e01687454cfacafa8318bdc6a677550baa6e24f8af864fa5324e9d930a97cdeb1995b476f21a017b33ab7fe4139f2524c784fcb04cf5241c89f0c145eb23da914ad1722d47a843692a0b2a567d94dd808c13678a51c5a0583dc042dcbba1b9ceff12b159d0539248b0994ee18128ed50dd7a855e54d2459db0052143010001"  # noqa
+            )
+        )
+        client_param = bytes.fromhex(
+            "057a0ecbe7e3e99e8926941614f6af078c802b110be89eb221d69be2e17a1ba4"
+        )
+
+        try:
+            res = attestation.verify(statement, auth_data, client_param)
+        except UnsupportedAlgorithm as e:
+            if e._reason is _Reasons.UNSUPPORTED_HASH:
+                self.skipTest(
+                    "SHA1 signature verification not supported on this machine"
+                )
+
+        res = attestation.verify(statement, auth_data, client_param)
+        self.assertEqual(res.attestation_type, AttestationType.ATT_CA)
+        verify_x509_chain(res.trust_path)
+
+    def test_fido_u2f_attestation(self):
+        attestation = Attestation.for_type("fido-u2f")()
+        self.assertIsInstance(attestation, FidoU2FAttestation)
+
+        statement = {
+            "sig": bytes.fromhex(
+                "30450220324779C68F3380288A1197B6095F7A6EB9B1B1C127F66AE12A99FE8532EC23B9022100E39516AC4D61EE64044D50B415A6A4D4D84BA6D895CB5AB7A1AA7D081DE341FA"  # noqa E501
+            ),
+            "x5c": [
+                bytes.fromhex(
+                    "3082024A30820132A0030201020204046C8822300D06092A864886F70D01010B0500302E312C302A0603550403132359756269636F2055324620526F6F742043412053657269616C203435373230303633313020170D3134303830313030303030305A180F32303530303930343030303030305A302C312A302806035504030C2159756269636F205532462045452053657269616C203234393138323332343737303059301306072A8648CE3D020106082A8648CE3D030107034200043CCAB92CCB97287EE8E639437E21FCD6B6F165B2D5A3F3DB131D31C16B742BB476D8D1E99080EB546C9BBDF556E6210FD42785899E78CC589EBE310F6CDB9FF4A33B3039302206092B0601040182C40A020415312E332E362E312E342E312E34313438322E312E323013060B2B0601040182E51C020101040403020430300D06092A864886F70D01010B050003820101009F9B052248BC4CF42CC5991FCAABAC9B651BBE5BDCDC8EF0AD2C1C1FFB36D18715D42E78B249224F92C7E6E7A05C49F0E7E4C881BF2E94F45E4A21833D7456851D0F6C145A29540C874F3092C934B43D222B8962C0F410CEF1DB75892AF116B44A96F5D35ADEA3822FC7146F6004385BCB69B65C99E7EB6919786703C0D8CD41E8F75CCA44AA8AB725AD8E799FF3A8696A6F1B2656E631B1E40183C08FDA53FA4A8F85A05693944AE179A1339D002D15CABD810090EC722EF5DEF9965A371D415D624B68A2707CAD97BCDD1785AF97E258F33DF56A031AA0356D8E8D5EBCADC74E071636C6B110ACE5CC9B90DFEACAE640FF1BB0F1FE5DB4EFF7A95F060733F5"  # noqa E501
+                )
+            ],
+        }
+        auth_data = AuthenticatorData(
+            bytes.fromhex(
+                "1194228DA8FDBDEEFD261BD7B6595CFD70A50D70C6407BCF013DE96D4EFB17DE41000000000000000000000000000000000000000000403EBD89BF77EC509755EE9C2635EFAAAC7B2B9C5CEF1736C3717DA48534C8C6B654D7FF945F50B5CC4E78055BDD396B64F78DA2C5F96200CCD415CD08FE420038A5010203262001215820E87625896EE4E46DC032766E8087962F36DF9DFE8B567F3763015B1990A60E1422582027DE612D66418BDA1950581EBC5C8C1DAD710CB14C22F8C97045F4612FB20C91"  # noqa E501
+            )
+        )
+        client_param = bytes.fromhex(
+            "687134968222EC17202E42505F8ED2B16AE22F16BB05B88C25DB9E602645F141"
+        )
+
+        res = attestation.verify(statement, auth_data, client_param)
+        self.assertEqual(res.attestation_type, AttestationType.BASIC)
+        self.assertEqual(len(res.trust_path), 1)
+
+        statement["sig"] = b"a" * len(statement["sig"])
+        with self.assertRaises(InvalidSignature):
+            attestation.verify(statement, auth_data, client_param)
+
+    def test_packed_attestation(self):
+        attestation = Attestation.for_type("packed")()
+        self.assertIsInstance(attestation, PackedAttestation)
+
+        statement = {
+            "alg": -7,
+            "sig": bytes.fromhex(
+                "304502200D15DAF337D727AB4719B4027114A2AC43CD565D394CED62C3D9D1D90825F0B3022100989615E7394C87F4AD91F8FDAE86F7A3326DF332B3633DB088AAC76BFFB9A46B"  # noqa E501
+            ),
+            "x5c": [
+                bytes.fromhex(
+                    "308202B73082019FA00302010202041D31330D300D06092A864886F70D01010B0500302A3128302606035504030C1F59756269636F2050726576696577204649444F204174746573746174696F6E301E170D3138303332383036333932345A170D3139303332383036333932345A306E310B300906035504061302534531123010060355040A0C0959756269636F20414231223020060355040B0C1941757468656E74696361746F72204174746573746174696F6E3127302506035504030C1E59756269636F205532462045452053657269616C203438393736333539373059301306072A8648CE3D020106082A8648CE3D030107034200047D71E8367CAFD0EA6CF0D61E4C6A416BA5BB6D8FAD52DB2389AD07969F0F463BFDDDDDC29D39D3199163EE49575A3336C04B3309D607F6160C81E023373E0197A36C306A302206092B0601040182C40A020415312E332E362E312E342E312E34313438322E312E323013060B2B0601040182E51C0201010404030204303021060B2B0601040182E51C01010404120410F8A011F38C0A4D15800617111F9EDC7D300C0603551D130101FF04023000300D06092A864886F70D01010B050003820101009B904CEADBE1F1985486FEAD02BAEAA77E5AB4E6E52B7E6A2666A4DC06E241578169193B63DADEC5B2B78605A128B2E03F7FE2A98EAEB4219F52220995F400CE15D630CF0598BA662D7162459F1AD1FC623067376D4E4091BE65AC1A33D8561B9996C0529EC1816D1710786384D5E8783AA1F7474CB99FE8F5A63A79FF454380361C299D67CB5CC7C79F0D8C09F8849B0500F6D625408C77CBBC26DDEE11CB581BEB7947137AD4F05AAF38BD98DA10042DDCAC277604A395A5B3EAA88A5C8BB27AB59C8127D59D6BBBA5F11506BF7B75FDA7561A0837C46F025FD54DCF1014FC8D17C859507AC57D4B1DEA99485DF0BA8F34D00103C3EEF2EF3BBFEC7A6613DE"  # noqa E501
+                )
+            ],
+        }
+        auth_data = AuthenticatorData(
+            bytes.fromhex(
+                "0021F5FC0B85CD22E60623BCD7D1CA48948909249B4776EB515154E57B66AE124100000003F8A011F38C0A4D15800617111F9EDC7D004060A386206A3AACECBDBB22D601853D955FDC5D11ADFBD1AA6A950D966B348C7663D40173714A9F987DF6461BEADFB9CD6419FFDFE4D4CF2EEC1AA605A4F59BDAA50102032620012158200EDB27580389494D74D2373B8F8C2E8B76FA135946D4F30D0E187E120B423349225820E03400D189E85A55DE9AB0F538ED60736EB750F5F0306A80060FE1B13010560D"  # noqa E501
+            )
+        )
+        client_param = bytes.fromhex(
+            "985B6187D042FB1258892ED637CEC88617DDF5F6632351A545617AA2B75261BF"
+        )
+
+        res = attestation.verify(statement, auth_data, client_param)
+        self.assertEqual(res.attestation_type, AttestationType.BASIC)
+        self.assertEqual(len(res.trust_path), 1)
+
+        statement["sig"] = b"a" * len(statement["sig"])
+        with self.assertRaises(InvalidSignature):
+            attestation.verify(statement, auth_data, client_param)
+
+    def test_android_safetynet_attestation(self):
+        attestation = Attestation.for_type("android-safetynet")()
+        self.assertIsInstance(attestation, AndroidSafetynetAttestation)
+
+        statement = {
+            "ver": "14574037",
+            "response": b"eyJhbGciOiJSUzI1NiIsIng1YyI6WyJNSUlGa2pDQ0JIcWdBd0lCQWdJUVJYcm9OMFpPZFJrQkFBQUFBQVB1bnpBTkJna3Foa2lHOXcwQkFRc0ZBREJDTVFzd0NRWURWUVFHRXdKVlV6RWVNQndHQTFVRUNoTVZSMjl2WjJ4bElGUnlkWE4wSUZObGNuWnBZMlZ6TVJNd0VRWURWUVFERXdwSFZGTWdRMEVnTVU4eE1CNFhEVEU0TVRBeE1EQTNNVGswTlZvWERURTVNVEF3T1RBM01UazBOVm93YkRFTE1Ba0dBMVVFQmhNQ1ZWTXhFekFSQmdOVkJBZ1RDa05oYkdsbWIzSnVhV0V4RmpBVUJnTlZCQWNURFUxdmRXNTBZV2x1SUZacFpYY3hFekFSQmdOVkJBb1RDa2R2YjJkc1pTQk1URU14R3pBWkJnTlZCQU1URW1GMGRHVnpkQzVoYm1SeWIybGtMbU52YlRDQ0FTSXdEUVlKS29aSWh2Y05BUUVCQlFBRGdnRVBBRENDQVFvQ2dnRUJBTmpYa3owZUsxU0U0bSsvRzV3T28rWEdTRUNycWRuODhzQ3BSN2ZzMTRmSzBSaDNaQ1laTEZIcUJrNkFtWlZ3Mks5RkcwTzlyUlBlUURJVlJ5RTMwUXVuUzl1Z0hDNGVnOW92dk9tK1FkWjJwOTNYaHp1blFFaFVXWEN4QURJRUdKSzNTMmFBZnplOTlQTFMyOWhMY1F1WVhIRGFDN09acU5ub3NpT0dpZnM4djFqaTZIL3hobHRDWmUybEorN0d1dHpleEtweHZwRS90WlNmYlk5MDVxU2xCaDlmcGowMTVjam5RRmtVc0FVd21LVkFVdWVVejR0S2NGSzRwZXZOTGF4RUFsK09raWxNdElZRGFjRDVuZWw0eEppeXM0MTNoYWdxVzBXaGg1RlAzOWhHazlFL0J3UVRqYXpTeEdkdlgwbTZ4RlloaC8yVk15WmpUNEt6UEpFQ0F3RUFBYU9DQWxnd2dnSlVNQTRHQTFVZER3RUIvd1FFQXdJRm9EQVRCZ05WSFNVRUREQUtCZ2dyQmdFRkJRY0RBVEFNQmdOVkhSTUJBZjhFQWpBQU1CMEdBMVVkRGdRV0JCUXFCUXdHV29KQmExb1RLcXVwbzRXNnhUNmoyREFmQmdOVkhTTUVHREFXZ0JTWTBmaHVFT3ZQbSt4Z254aVFHNkRyZlFuOUt6QmtCZ2dyQmdFRkJRY0JBUVJZTUZZd0p3WUlLd1lCQlFVSE1BR0dHMmgwZEhBNkx5OXZZM053TG5CcmFTNW5iMjluTDJkMGN6RnZNVEFyQmdnckJnRUZCUWN3QW9ZZmFIUjBjRG92TDNCcmFTNW5iMjluTDJkemNqSXZSMVJUTVU4eExtTnlkREFkQmdOVkhSRUVGakFVZ2hKaGRIUmxjM1F1WVc1a2NtOXBaQzVqYjIwd0lRWURWUjBnQkJvd0dEQUlCZ1puZ1F3QkFnSXdEQVlLS3dZQkJBSFdlUUlGQXpBdkJnTlZIUjhFS0RBbU1DU2dJcUFnaGg1b2RIUndPaTh2WTNKc0xuQnJhUzVuYjI5bkwwZFVVekZQTVM1amNtd3dnZ0VFQmdvckJnRUVBZFo1QWdRQ0JJSDFCSUh5QVBBQWR3Q2t1UW1RdEJoWUZJZTdFNkxNWjNBS1BEV1lCUGtiMzdqamQ4ME95QTNjRUFBQUFXWmREM1BMQUFBRUF3QklNRVlDSVFDU1pDV2VMSnZzaVZXNkNnK2dqLzl3WVRKUnp1NEhpcWU0ZVk0Yy9teXpqZ0loQUxTYmkvVGh6Y3pxdGlqM2RrM3ZiTGNJVzNMbDJCMG83NUdRZGhNaWdiQmdBSFVBVmhRR21pL1h3dXpUOWVHOVJMSSt4MFoydWJ5WkVWekE3NVNZVmRhSjBOMEFBQUZtWFE5ejVBQUFCQU1BUmpCRUFpQmNDd0E5ajdOVEdYUDI3OHo0aHIvdUNIaUFGTHlvQ3EySzAreUxSd0pVYmdJZ2Y4Z0hqdnB3Mm1CMUVTanEyT2YzQTBBRUF3Q2tuQ2FFS0ZVeVo3Zi9RdEl3RFFZSktvWklodmNOQVFFTEJRQURnZ0VCQUk5blRmUktJV2d0bFdsM3dCTDU1RVRWNmthenNwaFcxeUFjNUR1bTZYTzQxa1p6d0o2MXdKbWRSUlQvVXNDSXkxS0V0MmMwRWpnbG5KQ0YyZWF3Y0VXbExRWTJYUEx5RmprV1FOYlNoQjFpNFcyTlJHelBodDNtMWI0OWhic3R1WE02dFg1Q3lFSG5UaDhCb200L1dsRmloemhnbjgxRGxkb2d6L0syVXdNNlM2Q0IvU0V4a2lWZnYremJKMHJqdmc5NEFsZGpVZlV3a0k5Vk5NakVQNWU4eWRCM29MbDZnbHBDZUY1ZGdmU1g0VTl4MzVvai9JSWQzVUUvZFBwYi9xZ0d2c2tmZGV6dG1VdGUvS1Ntcml3Y2dVV1dlWGZUYkkzenNpa3daYmtwbVJZS21qUG1odjRybGl6R0NHdDhQbjhwcThNMktEZi9QM2tWb3QzZTE4UT0iLCJNSUlFU2pDQ0F6S2dBd0lCQWdJTkFlTzBtcUdOaXFtQkpXbFF1REFOQmdrcWhraUc5dzBCQVFzRkFEQk1NU0F3SGdZRFZRUUxFeGRIYkc5aVlXeFRhV2R1SUZKdmIzUWdRMEVnTFNCU01qRVRNQkVHQTFVRUNoTUtSMnh2WW1Gc1UybG5iakVUTUJFR0ExVUVBeE1LUjJ4dlltRnNVMmxuYmpBZUZ3MHhOekEyTVRVd01EQXdOREphRncweU1URXlNVFV3TURBd05ESmFNRUl4Q3pBSkJnTlZCQVlUQWxWVE1SNHdIQVlEVlFRS0V4VkhiMjluYkdVZ1ZISjFjM1FnVTJWeWRtbGpaWE14RXpBUkJnTlZCQU1UQ2tkVVV5QkRRU0F4VHpFd2dnRWlNQTBHQ1NxR1NJYjNEUUVCQVFVQUE0SUJEd0F3Z2dFS0FvSUJBUURRR005RjFJdk4wNXprUU85K3ROMXBJUnZKenp5T1RIVzVEekVaaEQyZVBDbnZVQTBRazI4RmdJQ2ZLcUM5RWtzQzRUMmZXQllrL2pDZkMzUjNWWk1kUy9kTjRaS0NFUFpSckF6RHNpS1VEelJybUJCSjV3dWRnem5kSU1ZY0xlL1JHR0ZsNXlPRElLZ2pFdi9TSkgvVUwrZEVhbHROMTFCbXNLK2VRbU1GKytBY3hHTmhyNTlxTS85aWw3MUkyZE44RkdmY2Rkd3VhZWo0YlhocDBMY1FCYmp4TWNJN0pQMGFNM1Q0SStEc2F4bUtGc2JqemFUTkM5dXpwRmxnT0lnN3JSMjV4b3luVXh2OHZObWtxN3pkUEdIWGt4V1k3b0c5aitKa1J5QkFCazdYckpmb3VjQlpFcUZKSlNQazdYQTBMS1cwWTN6NW96MkQwYzF0Skt3SEFnTUJBQUdqZ2dFek1JSUJMekFPQmdOVkhROEJBZjhFQkFNQ0FZWXdIUVlEVlIwbEJCWXdGQVlJS3dZQkJRVUhBd0VHQ0NzR0FRVUZCd01DTUJJR0ExVWRFd0VCL3dRSU1BWUJBZjhDQVFBd0hRWURWUjBPQkJZRUZKalIrRzRRNjgrYjdHQ2ZHSkFib090OUNmMHJNQjhHQTFVZEl3UVlNQmFBRkp2aUIxZG5IQjdBYWdiZVdiU2FMZC9jR1lZdU1EVUdDQ3NHQVFVRkJ3RUJCQ2t3SnpBbEJnZ3JCZ0VGQlFjd0FZWVphSFIwY0RvdkwyOWpjM0F1Y0d0cExtZHZiMmN2WjNOeU1qQXlCZ05WSFI4RUt6QXBNQ2VnSmFBamhpRm9kSFJ3T2k4dlkzSnNMbkJyYVM1bmIyOW5MMmR6Y2pJdlozTnlNaTVqY213d1B3WURWUjBnQkRnd05qQTBCZ1puZ1F3QkFnSXdLakFvQmdnckJnRUZCUWNDQVJZY2FIUjBjSE02THk5d2Eya3VaMjl2Wnk5eVpYQnZjMmwwYjNKNUx6QU5CZ2txaGtpRzl3MEJBUXNGQUFPQ0FRRUFHb0ErTm5uNzh5NnBSamQ5WGxRV05hN0hUZ2laL3IzUk5Ha21VbVlIUFFxNlNjdGk5UEVhanZ3UlQyaVdUSFFyMDJmZXNxT3FCWTJFVFV3Z1pRK2xsdG9ORnZoc085dHZCQ09JYXpwc3dXQzlhSjl4anU0dFdEUUg4TlZVNllaWi9YdGVEU0dVOVl6SnFQalk4cTNNRHhyem1xZXBCQ2Y1bzhtdy93SjRhMkc2eHpVcjZGYjZUOE1jRE8yMlBMUkw2dTNNNFR6czNBMk0xajZieWtKWWk4d1dJUmRBdktMV1p1L2F4QlZielltcW13a201ekxTRFc1bklBSmJFTENRQ1p3TUg1NnQyRHZxb2Z4czZCQmNDRklaVVNweHU2eDZ0ZDBWN1N2SkNDb3NpclNtSWF0ai85ZFNTVkRRaWJldDhxLzdVSzR2NFpVTjgwYXRuWnoxeWc9PSJdfQ.eyJub25jZSI6InpiNVE5NFVPaHFOWnRVUWEraWY0NnF1UDRwZWZQN2JnQWRpQ3hraDFZRGs9IiwidGltZXN0YW1wTXMiOjE1NDM0ODI1Njg4NTgsImFwa1BhY2thZ2VOYW1lIjoiY29tLmdvb2dsZS5hbmRyb2lkLmdtcyIsImFwa0RpZ2VzdFNoYTI1NiI6InIxYzZiTkJmQ0hjZHcvZWpKSE1NWjhoakIrU0xXa1BSM0lreTZjV1dhNE09IiwiY3RzUHJvZmlsZU1hdGNoIjp0cnVlLCJhcGtDZXJ0aWZpY2F0ZURpZ2VzdFNoYTI1NiI6WyI4UDFzVzBFUEpjc2x3N1V6UnNpWEw2NHcrTzUwRWQrUkJJQ3RheTFnMjRNPSJdLCJiYXNpY0ludGVncml0eSI6dHJ1ZX0.Lq9WpOJ_GilocvPCTbIN2K5FtppXW2fTQzCW2pvb1Bo5qOZnJ0oOYBUqMgxx-zghlluSkkIIfPTvYl2zZUQsY-SNlBx7JASqDbksMyRsdU9r1Jn8D2zEtipFgjmZUkozi7AngnHoA5d0Yp-NF6slmr_FLMpAOnLZY9lREw8Cxnmso3Ph7zYUu7O5SxaRGwj8eMKydYJYHa23h2C8acuQKgSWL2YlG9T-oKT0CJ8jOSrKnHr39eMo7PFX0464diUvXUsv_M9kRIIQqCP0LzilGMdJVUrvFU7kg8csnFP6KMDfY70RGZ5ey3eNqs_D5-pjPfC4XPsPsksmy_wf-3UOmw",  # noqa E501
+        }
+
+        auth_data = AuthenticatorData(
+            bytes.fromhex(
+                "720c20fde835785e0f5ebcad8ef6a7bd88804a91612a2e820e0059b8d5358797450000000000000000000000000000000000000000004101c8fd9b533d6adacf6710ebcfb39f6361c4d7e8787db47dc0a75ae0e7c862198c9c83b81ef2547bb5669314095fc846af4ecac6875f7b230cac7359c76b0c20f7a5010203262001215820a28851e2d411b5b2c289da50d41cc41be88498941fc256dab500b21c8dafe8d1225820d289dd467715be06a622771a7b21e1bbe2372f8713d20dd7888a6e7ae1845ca8"  # noqa E501
+            )
+        )
+        client_param = bytes.fromhex(
+            "8422c80f3428e4e6465f76ebc8a4a93759a0a2e1fb845ee5eea7a02027408520"
+        )
+
+        res = attestation.verify(statement, auth_data, client_param)
+        self.assertEqual(res.attestation_type, AttestationType.BASIC)
+        verify_x509_chain(res.trust_path + [_GSR2_DER])
+
+    def test_apple_attestation(self):
+        attestation = Attestation.for_type("apple")()
+        self.assertIsInstance(attestation, AppleAttestation)
+
+        statement = {
+            "alg": -7,
+            "x5c": [
+                bytes.fromhex(
+                    "30820242308201c9a00302010202060176af5359ff300a06082a8648ce3d0403023048311c301a06035504030c134170706c6520576562417574686e204341203131133011060355040a0c0a4170706c6520496e632e3113301106035504080c0a43616c69666f726e6961301e170d3230313232383136323732345a170d3230313233313136323732345a3081913149304706035504030c4038303966626331313065613835663233613862323435616563363136333530663337646665393632313232373336653431663862646365663334366138306439311a3018060355040b0c114141412043657274696669636174696f6e31133011060355040a0c0a4170706c6520496e632e3113301106035504080c0a43616c69666f726e69613059301306072a8648ce3d020106082a8648ce3d030107034200041f46a2f159fde354598cdd47e005f1b6e7c9f00ed2a941ec7a88d222f5bcf55d6b078bc5b0be9552d85a974921f5bb848e2bbc3aecd6f71a386d2c87d6eafd37a3553053300c0603551d130101ff04023000300e0603551d0f0101ff0404030204f0303306092a864886f76364080204263024a1220420e56fb6212b3aae885294464fb10184b7fea62c48a6d78e61194e07ae6dacc132300a06082a8648ce3d040302036700306402301de8f0f238eee4f5ae80c59290b51e8c3f79397bf198e444ba162d4fccaab8558b072cf00a7c662f9058ff2a98af61ae0230149403b9643066e73a98d3659563dc4da49bf84e82b2b5bbeaf57755646fa243f36344d44b80a5798203bca023e030c7"  # noqa E501
+                ),
+                bytes.fromhex(
+                    "30820234308201baa003020102021056255395c7a7fb40ebe228d8260853b6300a06082a8648ce3d040303304b311f301d06035504030c164170706c6520576562417574686e20526f6f7420434131133011060355040a0c0a4170706c6520496e632e3113301106035504080c0a43616c69666f726e6961301e170d3230303331383138333830315a170d3330303331333030303030305a3048311c301a06035504030c134170706c6520576562417574686e204341203131133011060355040a0c0a4170706c6520496e632e3113301106035504080c0a43616c69666f726e69613076301006072a8648ce3d020106052b8104002203620004832e872f261491810225b9f5fcd6bb6378b5f55f3fcb045bc735993475fd549044df9bfe19211765c69a1dda050b38d45083401a434fb24d112d56c3e1cfbfcb9891fec0696081bef96cbc77c88dddaf46a5aee1dd515b5afaab93be9c0b2691a366306430120603551d130101ff040830060101ff020100301f0603551d2304183016801426d764d9c578c25a67d1a7de6b12d01b63f1c6d7301d0603551d0e04160414ebae82c4ffa1ac5b51d4cf24610500be63bd7788300e0603551d0f0101ff040403020106300a06082a8648ce3d0403030368003065023100dd8b1a3481a5fad9dbb4e7657b841e144c27b75b876a4186c2b1475750337227efe554457ef648950c632e5c483e70c102302c8a6044dc201fcfe59bc34d2930c1487851d960ed6a75f1eb4acabe38cd25b897d0c805bef0c7f78b07a571c6e80e07"  # noqa E501
+                ),
+            ],
+        }
+
+        auth_data = AuthenticatorData(
+            bytes.fromhex(
+                "c46cef82ad1b546477591d008b08759ec3e6d2ecb4f39474bfea6969925d03b7450000000000000000000000000000000000000000001473d9429f4052d84debd035eb5bb7e716e3b81863a50102032620012158201f46a2f159fde354598cdd47e005f1b6e7c9f00ed2a941ec7a88d222f5bcf55d2258206b078bc5b0be9552d85a974921f5bb848e2bbc3aecd6f71a386d2c87d6eafd37"  # noqa E501
+            )
+        )
+        client_param = bytes.fromhex(
+            "0d3ce80fabbc3adb9dd891deabb8db84603ea1fe2da8b5d4b46d6591aab342f3"
+        )
+
+        res = attestation.verify(statement, auth_data, client_param)
+        self.assertEqual(res.attestation_type, AttestationType.ANON_CA)
+        self.assertEqual(len(res.trust_path), 2)
+        verify_x509_chain(res.trust_path)
```

### Comparing `fido2-1.1.1/tests/test_cbor.py` & `fido2-1.1.2/tests/test_cbor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,213 +1,213 @@
-# coding=utf-8
-
-# Copyright (c) 2013 Yubico AB
-# All rights reserved.
-#
-#   Redistribution and use in source and binary forms, with or
-#   without modification, are permitted provided that the following
-#   conditions are met:
-#
-#    1. Redistributions of source code must retain the above copyright
-#       notice, this list of conditions and the following disclaimer.
-#    2. Redistributions in binary form must reproduce the above
-#       copyright notice, this list of conditions and the following
-#       disclaimer in the documentation and/or other materials provided
-#       with the distribution.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
-# FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
-# COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
-# INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
-# BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
-# ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
-# POSSIBILITY OF SUCH DAMAGE.
-
-from fido2 import cbor
-import unittest
-
-
-_TEST_VECTORS = [
-    ("00", 0),
-    ("01", 1),
-    ("0a", 10),
-    ("17", 23),
-    ("1818", 24),
-    ("1819", 25),
-    ("1864", 100),
-    ("1903e8", 1000),
-    ("1a000f4240", 1000000),
-    ("1b000000e8d4a51000", 1000000000000),
-    ("1bffffffffffffffff", 18446744073709551615),
-    # ('c249010000000000000000', 18446744073709551616),
-    ("3bffffffffffffffff", -18446744073709551616),
-    # ('c349010000000000000000', -18446744073709551617),
-    ("20", -1),
-    ("29", -10),
-    ("3863", -100),
-    ("3903e7", -1000),
-    # ('f90000', 0.0),
-    # ('f98000', -0.0),
-    # ('f93c00', 1.0),
-    # ('fb3ff199999999999a', 1.1),
-    # ('f93e00', 1.5),
-    # ('f97bff', 65504.0),
-    # ('fa47c35000', 100000.0),
-    # ('fa7f7fffff', 3.4028234663852886e+38),
-    # ('fb7e37e43c8800759c', 1e+300),
-    # ('f90001', 5.960464477539063e-08),
-    # ('f90400', 6.103515625e-05),
-    # ('f9c400', -4.0),
-    # ('fbc010666666666666', -4.1),
-    # ('f97c00', None),
-    # ('f97e00', None),
-    # ('f9fc00', None),
-    # ('fa7f800000', None),
-    # ('fa7fc00000', None),
-    # ('faff800000', None),
-    # ('fb7ff0000000000000', None),
-    # ('fb7ff8000000000000', None),
-    # ('fbfff0000000000000', None),
-    ("f4", False),
-    ("f5", True),
-    # ('f6', None),
-    # ('f7', None),
-    # ('f0', None),
-    # ('f818', None),
-    # ('f8ff', None),
-    # ('c074323031332d30332d32315432303a30343a30305a', None),
-    # ('c11a514b67b0', None),
-    # ('c1fb41d452d9ec200000', None),
-    # ('d74401020304', None),
-    # ('d818456449455446', None),
-    # ('d82076687474703a2f2f7777772e6578616d706c652e636f6d', None),
-    ("40", b""),
-    ("4401020304", b"\1\2\3\4"),
-    ("60", ""),
-    ("6161", "a"),
-    ("6449455446", "IETF"),
-    ("62225c", '"\\'),
-    ("62c3bc", "ü"),
-    ("63e6b0b4", "水"),
-    ("64f0908591", "𐅑"),
-    ("80", []),
-    ("83010203", [1, 2, 3]),
-    ("8301820203820405", [1, [2, 3], [4, 5]]),
-    (
-        "98190102030405060708090a0b0c0d0e0f101112131415161718181819",
-        [
-            1,
-            2,
-            3,
-            4,
-            5,
-            6,
-            7,
-            8,
-            9,
-            10,
-            11,
-            12,
-            13,
-            14,
-            15,
-            16,
-            17,
-            18,
-            19,
-            20,
-            21,
-            22,
-            23,
-            24,
-            25,
-        ],
-    ),
-    ("a0", {}),
-    ("a201020304", {1: 2, 3: 4}),
-    ("a26161016162820203", {"a": 1, "b": [2, 3]}),
-    ("826161a161626163", ["a", {"b": "c"}]),
-    (
-        "a56161614161626142616361436164614461656145",
-        {"c": "C", "d": "D", "a": "A", "b": "B", "e": "E"},
-    ),
-    # ('5f42010243030405ff', None),
-    # ('7f657374726561646d696e67ff', 'streaming'),
-    # ('9fff', []),
-    # ('9f018202039f0405ffff', [1, [2, 3], [4, 5]]),
-    # ('9f01820203820405ff', [1, [2, 3], [4, 5]]),
-    # ('83018202039f0405ff', [1, [2, 3], [4, 5]]),
-    # ('83019f0203ff820405', [1, [2, 3], [4, 5]]),
-    # ('9f0102030405060708090a0b0c0d0e0f101112131415161718181819ff', [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25]),  # noqa E501
-    # ('bf61610161629f0203ffff', {'a': 1, 'b': [2, 3]}),
-    # ('826161bf61626163ff', ['a', {'b': 'c'}]),
-    # ('bf6346756ef563416d7421ff', {'Amt': -2, 'Fun': True}),
-]
-
-
-def cbor2hex(data):
-    return cbor.encode(data).hex()
-
-
-class TestCborTestVectors(unittest.TestCase):
-    """
-    From https://github.com/cbor/test-vectors
-    Unsupported values are commented out.
-    """
-
-    def test_vectors(self):
-        for (data, value) in _TEST_VECTORS:
-            try:
-                self.assertEqual(cbor.decode_from(bytes.fromhex(data)), (value, b""))
-                self.assertEqual(cbor.decode(bytes.fromhex(data)), value)
-                self.assertEqual(cbor2hex(value), data)
-            except Exception:
-                print("\nERROR in test vector, %s" % data)
-                raise
-
-
-class TestFidoCanonical(unittest.TestCase):
-    """
-    As defined in section 6 of:
-    https://fidoalliance.org/specs/fido-v2.0-ps-20170927/fido-client-to-authenticator-protocol-v2.0-ps-20170927.html
-    """
-
-    def test_integers(self):
-        self.assertEqual(cbor2hex(0), "00")
-        self.assertEqual(cbor2hex(0), "00")
-        self.assertEqual(cbor2hex(23), "17")
-        self.assertEqual(cbor2hex(24), "1818")
-        self.assertEqual(cbor2hex(255), "18ff")
-        self.assertEqual(cbor2hex(256), "190100")
-        self.assertEqual(cbor2hex(65535), "19ffff")
-        self.assertEqual(cbor2hex(65536), "1a00010000")
-        self.assertEqual(cbor2hex(4294967295), "1affffffff")
-        self.assertEqual(cbor2hex(4294967296), "1b0000000100000000")
-        self.assertEqual(cbor2hex(-1), "20")
-        self.assertEqual(cbor2hex(-24), "37")
-        self.assertEqual(cbor2hex(-25), "3818")
-
-    def test_key_order(self):
-        self.assertEqual(cbor2hex({"3": 0, b"2": 0, 1: 0}), "a30100413200613300")
-
-        self.assertEqual(cbor2hex({"3": 0, b"": 0, 256: 0}), "a3190100004000613300")
-
-        self.assertEqual(
-            cbor2hex({4294967296: 0, 255: 0, 256: 0, 0: 0}),
-            "a4000018ff00190100001b000000010000000000",
-        )
-
-        self.assertEqual(
-            cbor2hex({b"22": 0, b"3": 0, b"111": 0}), "a3413300423232004331313100"
-        )
-
-        self.assertEqual(
-            cbor2hex({b"001": 0, b"003": 0, b"002": 0}),
-            "a3433030310043303032004330303300",
-        )
-
-        self.assertEqual(cbor2hex({True: 0, False: 0}), "a2f400f500")
+# coding=utf-8
+
+# Copyright (c) 2013 Yubico AB
+# All rights reserved.
+#
+#   Redistribution and use in source and binary forms, with or
+#   without modification, are permitted provided that the following
+#   conditions are met:
+#
+#    1. Redistributions of source code must retain the above copyright
+#       notice, this list of conditions and the following disclaimer.
+#    2. Redistributions in binary form must reproduce the above
+#       copyright notice, this list of conditions and the following
+#       disclaimer in the documentation and/or other materials provided
+#       with the distribution.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
+# FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
+# COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
+# INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
+# BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+# CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
+# LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN
+# ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
+# POSSIBILITY OF SUCH DAMAGE.
+
+from fido2 import cbor
+import unittest
+
+
+_TEST_VECTORS = [
+    ("00", 0),
+    ("01", 1),
+    ("0a", 10),
+    ("17", 23),
+    ("1818", 24),
+    ("1819", 25),
+    ("1864", 100),
+    ("1903e8", 1000),
+    ("1a000f4240", 1000000),
+    ("1b000000e8d4a51000", 1000000000000),
+    ("1bffffffffffffffff", 18446744073709551615),
+    # ('c249010000000000000000', 18446744073709551616),
+    ("3bffffffffffffffff", -18446744073709551616),
+    # ('c349010000000000000000', -18446744073709551617),
+    ("20", -1),
+    ("29", -10),
+    ("3863", -100),
+    ("3903e7", -1000),
+    # ('f90000', 0.0),
+    # ('f98000', -0.0),
+    # ('f93c00', 1.0),
+    # ('fb3ff199999999999a', 1.1),
+    # ('f93e00', 1.5),
+    # ('f97bff', 65504.0),
+    # ('fa47c35000', 100000.0),
+    # ('fa7f7fffff', 3.4028234663852886e+38),
+    # ('fb7e37e43c8800759c', 1e+300),
+    # ('f90001', 5.960464477539063e-08),
+    # ('f90400', 6.103515625e-05),
+    # ('f9c400', -4.0),
+    # ('fbc010666666666666', -4.1),
+    # ('f97c00', None),
+    # ('f97e00', None),
+    # ('f9fc00', None),
+    # ('fa7f800000', None),
+    # ('fa7fc00000', None),
+    # ('faff800000', None),
+    # ('fb7ff0000000000000', None),
+    # ('fb7ff8000000000000', None),
+    # ('fbfff0000000000000', None),
+    ("f4", False),
+    ("f5", True),
+    # ('f6', None),
+    # ('f7', None),
+    # ('f0', None),
+    # ('f818', None),
+    # ('f8ff', None),
+    # ('c074323031332d30332d32315432303a30343a30305a', None),
+    # ('c11a514b67b0', None),
+    # ('c1fb41d452d9ec200000', None),
+    # ('d74401020304', None),
+    # ('d818456449455446', None),
+    # ('d82076687474703a2f2f7777772e6578616d706c652e636f6d', None),
+    ("40", b""),
+    ("4401020304", b"\1\2\3\4"),
+    ("60", ""),
+    ("6161", "a"),
+    ("6449455446", "IETF"),
+    ("62225c", '"\\'),
+    ("62c3bc", "ü"),
+    ("63e6b0b4", "水"),
+    ("64f0908591", "𐅑"),
+    ("80", []),
+    ("83010203", [1, 2, 3]),
+    ("8301820203820405", [1, [2, 3], [4, 5]]),
+    (
+        "98190102030405060708090a0b0c0d0e0f101112131415161718181819",
+        [
+            1,
+            2,
+            3,
+            4,
+            5,
+            6,
+            7,
+            8,
+            9,
+            10,
+            11,
+            12,
+            13,
+            14,
+            15,
+            16,
+            17,
+            18,
+            19,
+            20,
+            21,
+            22,
+            23,
+            24,
+            25,
+        ],
+    ),
+    ("a0", {}),
+    ("a201020304", {1: 2, 3: 4}),
+    ("a26161016162820203", {"a": 1, "b": [2, 3]}),
+    ("826161a161626163", ["a", {"b": "c"}]),
+    (
+        "a56161614161626142616361436164614461656145",
+        {"c": "C", "d": "D", "a": "A", "b": "B", "e": "E"},
+    ),
+    # ('5f42010243030405ff', None),
+    # ('7f657374726561646d696e67ff', 'streaming'),
+    # ('9fff', []),
+    # ('9f018202039f0405ffff', [1, [2, 3], [4, 5]]),
+    # ('9f01820203820405ff', [1, [2, 3], [4, 5]]),
+    # ('83018202039f0405ff', [1, [2, 3], [4, 5]]),
+    # ('83019f0203ff820405', [1, [2, 3], [4, 5]]),
+    # ('9f0102030405060708090a0b0c0d0e0f101112131415161718181819ff', [1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25]),  # noqa E501
+    # ('bf61610161629f0203ffff', {'a': 1, 'b': [2, 3]}),
+    # ('826161bf61626163ff', ['a', {'b': 'c'}]),
+    # ('bf6346756ef563416d7421ff', {'Amt': -2, 'Fun': True}),
+]
+
+
+def cbor2hex(data):
+    return cbor.encode(data).hex()
+
+
+class TestCborTestVectors(unittest.TestCase):
+    """
+    From https://github.com/cbor/test-vectors
+    Unsupported values are commented out.
+    """
+
+    def test_vectors(self):
+        for data, value in _TEST_VECTORS:
+            try:
+                self.assertEqual(cbor.decode_from(bytes.fromhex(data)), (value, b""))
+                self.assertEqual(cbor.decode(bytes.fromhex(data)), value)
+                self.assertEqual(cbor2hex(value), data)
+            except Exception:
+                print("\nERROR in test vector, %s" % data)
+                raise
+
+
+class TestFidoCanonical(unittest.TestCase):
+    """
+    As defined in section 6 of:
+    https://fidoalliance.org/specs/fido-v2.0-ps-20170927/fido-client-to-authenticator-protocol-v2.0-ps-20170927.html
+    """
+
+    def test_integers(self):
+        self.assertEqual(cbor2hex(0), "00")
+        self.assertEqual(cbor2hex(0), "00")
+        self.assertEqual(cbor2hex(23), "17")
+        self.assertEqual(cbor2hex(24), "1818")
+        self.assertEqual(cbor2hex(255), "18ff")
+        self.assertEqual(cbor2hex(256), "190100")
+        self.assertEqual(cbor2hex(65535), "19ffff")
+        self.assertEqual(cbor2hex(65536), "1a00010000")
+        self.assertEqual(cbor2hex(4294967295), "1affffffff")
+        self.assertEqual(cbor2hex(4294967296), "1b0000000100000000")
+        self.assertEqual(cbor2hex(-1), "20")
+        self.assertEqual(cbor2hex(-24), "37")
+        self.assertEqual(cbor2hex(-25), "3818")
+
+    def test_key_order(self):
+        self.assertEqual(cbor2hex({"3": 0, b"2": 0, 1: 0}), "a30100413200613300")
+
+        self.assertEqual(cbor2hex({"3": 0, b"": 0, 256: 0}), "a3190100004000613300")
+
+        self.assertEqual(
+            cbor2hex({4294967296: 0, 255: 0, 256: 0, 0: 0}),
+            "a4000018ff00190100001b000000010000000000",
+        )
+
+        self.assertEqual(
+            cbor2hex({b"22": 0, b"3": 0, b"111": 0}), "a3413300423232004331313100"
+        )
+
+        self.assertEqual(
+            cbor2hex({b"001": 0, b"003": 0, b"002": 0}),
+            "a3433030310043303032004330303300",
+        )
+
+        self.assertEqual(cbor2hex({True: 0, False: 0}), "a2f400f500")
```

### Comparing `fido2-1.1.1/tests/test_client.py` & `fido2-1.1.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/tests/test_cose.py` & `fido2-1.1.2/tests/test_cose.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/tests/test_ctap1.py` & `fido2-1.1.2/tests/test_ctap1.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/tests/test_ctap2.py` & `fido2-1.1.2/tests/test_ctap2.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/tests/test_hid.py` & `fido2-1.1.2/tests/test_hid.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/tests/test_mds3.py` & `fido2-1.1.2/tests/test_mds3.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/tests/test_pcsc.py` & `fido2-1.1.2/tests/test_pcsc.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/tests/test_rpid.py` & `fido2-1.1.2/tests/test_rpid.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/tests/test_server.py` & `fido2-1.1.2/tests/test_server.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,223 +1,223 @@
-import unittest
-
-from fido2.server import Fido2Server, U2FFido2Server, verify_app_id
-from fido2.webauthn import (
-    CollectedClientData,
-    PublicKeyCredentialRpEntity,
-    UserVerificationRequirement,
-    AttestedCredentialData,
-    AuthenticatorData,
-)
-from fido2.utils import websafe_encode
-
-from .test_ctap2 import _ATT_CRED_DATA, _CRED_ID
-from .utils import U2FDevice
-
-
-class TestAppId(unittest.TestCase):
-    def test_valid_ids(self):
-        self.assertTrue(
-            verify_app_id("https://example.com", "https://register.example.com")
-        )
-        self.assertTrue(
-            verify_app_id("https://example.com", "https://fido.example.com")
-        )
-        self.assertTrue(
-            verify_app_id("https://example.com", "https://www.example.com:444")
-        )
-
-        self.assertTrue(
-            verify_app_id(
-                "https://companyA.hosting.example.com",
-                "https://fido.companyA.hosting.example.com",
-            )
-        )
-        self.assertTrue(
-            verify_app_id(
-                "https://companyA.hosting.example.com",
-                "https://xyz.companyA.hosting.example.com",
-            )
-        )
-
-    def test_invalid_ids(self):
-        self.assertFalse(verify_app_id("https://example.com", "http://example.com"))
-        self.assertFalse(verify_app_id("https://example.com", "http://www.example.com"))
-        self.assertFalse(
-            verify_app_id("https://example.com", "https://example-test.com")
-        )
-
-        self.assertFalse(
-            verify_app_id(
-                "https://companyA.hosting.example.com", "https://register.example.com"
-            )
-        )
-        self.assertFalse(
-            verify_app_id(
-                "https://companyA.hosting.example.com",
-                "https://companyB.hosting.example.com",
-            )
-        )
-
-    def test_effective_tld_names(self):
-        self.assertFalse(
-            verify_app_id("https://appspot.com", "https://foo.appspot.com")
-        )
-        self.assertFalse(verify_app_id("https://co.uk", "https://example.co.uk"))
-
-
-class TestPublicKeyCredentialRpEntity(unittest.TestCase):
-    def test_id_hash(self):
-        rp = PublicKeyCredentialRpEntity("Example", "example.com")
-        rp_id_hash = (
-            b"\xa3y\xa6\xf6\xee\xaf\xb9\xa5^7\x8c\x11\x804\xe2u\x1eh/"
-            b"\xab\x9f-0\xab\x13\xd2\x12U\x86\xce\x19G"
-        )
-        self.assertEqual(rp.id_hash, rp_id_hash)
-
-
-USER = {"id": b"user_id", "name": "A. User"}
-
-
-class TestFido2Server(unittest.TestCase):
-    def test_register_begin_rp(self):
-        rp = PublicKeyCredentialRpEntity("Example", "example.com")
-        server = Fido2Server(rp)
-
-        request, state = server.register_begin(USER)
-
-        self.assertEqual(
-            request["publicKey"]["rp"], {"id": "example.com", "name": "Example"}
-        )
-
-    def test_register_begin_custom_challenge(self):
-        rp = PublicKeyCredentialRpEntity("Example", "example.com")
-        server = Fido2Server(rp)
-
-        challenge = b"1234567890123456"
-        request, state = server.register_begin(USER, challenge=challenge)
-
-        self.assertEqual(request["publicKey"]["challenge"], websafe_encode(challenge))
-
-    def test_register_begin_custom_challenge_too_short(self):
-        rp = PublicKeyCredentialRpEntity("Example", "example.com")
-        server = Fido2Server(rp)
-
-        challenge = b"123456789012345"
-        with self.assertRaises(ValueError):
-            request, state = server.register_begin(USER, challenge=challenge)
-
-    def test_authenticate_complete_invalid_signature(self):
-        rp = PublicKeyCredentialRpEntity("Example", "example.com")
-        server = Fido2Server(rp)
-
-        state = {
-            "challenge": "GAZPACHO!",
-            "user_verification": UserVerificationRequirement.PREFERRED,
-        }
-        client_data = CollectedClientData.create(
-            CollectedClientData.TYPE.GET,
-            "GAZPACHO!",
-            "https://example.com",
-        )
-        _AUTH_DATA = bytes.fromhex(
-            "A379A6F6EEAFB9A55E378C118034E2751E682FAB9F2D30AB13D2125586CE1947010000001D"
-        )
-        with self.assertRaisesRegex(ValueError, "Invalid signature."):
-            server.authenticate_complete(
-                state,
-                [AttestedCredentialData(_ATT_CRED_DATA)],
-                _CRED_ID,
-                client_data,
-                AuthenticatorData(_AUTH_DATA),
-                b"INVALID",
-            )
-
-
-class TestU2FFido2Server(unittest.TestCase):
-    def test_u2f(self):
-        rp = PublicKeyCredentialRpEntity("Example", "example.com")
-        app_id = b"https://example.com"
-        server = U2FFido2Server(app_id=app_id.decode("ascii"), rp=rp)
-
-        state = {
-            "challenge": "GAZPACHO!",
-            "user_verification": UserVerificationRequirement.PREFERRED,
-        }
-        client_data = CollectedClientData.create(
-            CollectedClientData.TYPE.GET,
-            "GAZPACHO!",
-            "https://example.com",
-        )
-
-        param = b"TOMATO GIVES "
-
-        device = U2FDevice(param, app_id)
-        auth_data = AttestedCredentialData.from_ctap1(param, device.public_key_bytes)
-        authenticator_data, signature = device.sign(client_data)
-
-        server.authenticate_complete(
-            state,
-            [auth_data],
-            device.credential_id,
-            client_data,
-            authenticator_data,
-            signature,
-        )
-
-    def test_u2f_facets(self):
-        rp = PublicKeyCredentialRpEntity("Example", "example.com")
-        app_id = b"https://www.example.com/facets.json"
-
-        def verify_u2f_origin(origin):
-            return origin in ("https://oauth.example.com", "https://admin.example.com")
-
-        server = U2FFido2Server(
-            app_id=app_id.decode("ascii"), rp=rp, verify_u2f_origin=verify_u2f_origin
-        )
-
-        state = {
-            "challenge": "GAZPACHO!",
-            "user_verification": UserVerificationRequirement.PREFERRED,
-        }
-
-        client_data = CollectedClientData.create(
-            CollectedClientData.TYPE.GET,
-            "GAZPACHO!",
-            "https://oauth.example.com",
-        )
-
-        param = b"TOMATO GIVES "
-
-        device = U2FDevice(param, app_id)
-        auth_data = AttestedCredentialData.from_ctap1(param, device.public_key_bytes)
-        authenticator_data, signature = device.sign(client_data)
-
-        server.authenticate_complete(
-            state,
-            [auth_data],
-            device.credential_id,
-            client_data,
-            authenticator_data,
-            signature,
-        )
-
-        # Now with something not whitelisted
-        client_data = CollectedClientData.create(
-            CollectedClientData.TYPE.GET,
-            "GAZPACHO!",
-            "https://publicthingy.example.com",
-        )
-
-        authenticator_data, signature = device.sign(client_data)
-
-        with self.assertRaisesRegex(
-            ValueError, "Invalid origin in CollectedClientData."
-        ):
-            server.authenticate_complete(
-                state,
-                [auth_data],
-                device.credential_id,
-                client_data,
-                authenticator_data,
-                signature,
-            )
+import unittest
+
+from fido2.server import Fido2Server, U2FFido2Server, verify_app_id
+from fido2.webauthn import (
+    CollectedClientData,
+    PublicKeyCredentialRpEntity,
+    UserVerificationRequirement,
+    AttestedCredentialData,
+    AuthenticatorData,
+)
+from fido2.utils import websafe_encode
+
+from .test_ctap2 import _ATT_CRED_DATA, _CRED_ID
+from .utils import U2FDevice
+
+
+class TestAppId(unittest.TestCase):
+    def test_valid_ids(self):
+        self.assertTrue(
+            verify_app_id("https://example.com", "https://register.example.com")
+        )
+        self.assertTrue(
+            verify_app_id("https://example.com", "https://fido.example.com")
+        )
+        self.assertTrue(
+            verify_app_id("https://example.com", "https://www.example.com:444")
+        )
+
+        self.assertTrue(
+            verify_app_id(
+                "https://companyA.hosting.example.com",
+                "https://fido.companyA.hosting.example.com",
+            )
+        )
+        self.assertTrue(
+            verify_app_id(
+                "https://companyA.hosting.example.com",
+                "https://xyz.companyA.hosting.example.com",
+            )
+        )
+
+    def test_invalid_ids(self):
+        self.assertFalse(verify_app_id("https://example.com", "http://example.com"))
+        self.assertFalse(verify_app_id("https://example.com", "http://www.example.com"))
+        self.assertFalse(
+            verify_app_id("https://example.com", "https://example-test.com")
+        )
+
+        self.assertFalse(
+            verify_app_id(
+                "https://companyA.hosting.example.com", "https://register.example.com"
+            )
+        )
+        self.assertFalse(
+            verify_app_id(
+                "https://companyA.hosting.example.com",
+                "https://companyB.hosting.example.com",
+            )
+        )
+
+    def test_effective_tld_names(self):
+        self.assertFalse(
+            verify_app_id("https://appspot.com", "https://foo.appspot.com")
+        )
+        self.assertFalse(verify_app_id("https://co.uk", "https://example.co.uk"))
+
+
+class TestPublicKeyCredentialRpEntity(unittest.TestCase):
+    def test_id_hash(self):
+        rp = PublicKeyCredentialRpEntity("Example", "example.com")
+        rp_id_hash = (
+            b"\xa3y\xa6\xf6\xee\xaf\xb9\xa5^7\x8c\x11\x804\xe2u\x1eh/"
+            b"\xab\x9f-0\xab\x13\xd2\x12U\x86\xce\x19G"
+        )
+        self.assertEqual(rp.id_hash, rp_id_hash)
+
+
+USER = {"id": b"user_id", "name": "A. User"}
+
+
+class TestFido2Server(unittest.TestCase):
+    def test_register_begin_rp(self):
+        rp = PublicKeyCredentialRpEntity("Example", "example.com")
+        server = Fido2Server(rp)
+
+        request, state = server.register_begin(USER)
+
+        self.assertEqual(
+            request["publicKey"]["rp"], {"id": "example.com", "name": "Example"}
+        )
+
+    def test_register_begin_custom_challenge(self):
+        rp = PublicKeyCredentialRpEntity("Example", "example.com")
+        server = Fido2Server(rp)
+
+        challenge = b"1234567890123456"
+        request, state = server.register_begin(USER, challenge=challenge)
+
+        self.assertEqual(request["publicKey"]["challenge"], websafe_encode(challenge))
+
+    def test_register_begin_custom_challenge_too_short(self):
+        rp = PublicKeyCredentialRpEntity("Example", "example.com")
+        server = Fido2Server(rp)
+
+        challenge = b"123456789012345"
+        with self.assertRaises(ValueError):
+            request, state = server.register_begin(USER, challenge=challenge)
+
+    def test_authenticate_complete_invalid_signature(self):
+        rp = PublicKeyCredentialRpEntity("Example", "example.com")
+        server = Fido2Server(rp)
+
+        state = {
+            "challenge": "GAZPACHO!",
+            "user_verification": UserVerificationRequirement.PREFERRED,
+        }
+        client_data = CollectedClientData.create(
+            CollectedClientData.TYPE.GET,
+            "GAZPACHO!",
+            "https://example.com",
+        )
+        _AUTH_DATA = bytes.fromhex(
+            "A379A6F6EEAFB9A55E378C118034E2751E682FAB9F2D30AB13D2125586CE1947010000001D"
+        )
+        with self.assertRaisesRegex(ValueError, "Invalid signature."):
+            server.authenticate_complete(
+                state,
+                [AttestedCredentialData(_ATT_CRED_DATA)],
+                _CRED_ID,
+                client_data,
+                AuthenticatorData(_AUTH_DATA),
+                b"INVALID",
+            )
+
+
+class TestU2FFido2Server(unittest.TestCase):
+    def test_u2f(self):
+        rp = PublicKeyCredentialRpEntity("Example", "example.com")
+        app_id = b"https://example.com"
+        server = U2FFido2Server(app_id=app_id.decode("ascii"), rp=rp)
+
+        state = {
+            "challenge": "GAZPACHO!",
+            "user_verification": UserVerificationRequirement.PREFERRED,
+        }
+        client_data = CollectedClientData.create(
+            CollectedClientData.TYPE.GET,
+            "GAZPACHO!",
+            "https://example.com",
+        )
+
+        param = b"TOMATO GIVES "
+
+        device = U2FDevice(param, app_id)
+        auth_data = AttestedCredentialData.from_ctap1(param, device.public_key_bytes)
+        authenticator_data, signature = device.sign(client_data)
+
+        server.authenticate_complete(
+            state,
+            [auth_data],
+            device.credential_id,
+            client_data,
+            authenticator_data,
+            signature,
+        )
+
+    def test_u2f_facets(self):
+        rp = PublicKeyCredentialRpEntity("Example", "example.com")
+        app_id = b"https://www.example.com/facets.json"
+
+        def verify_u2f_origin(origin):
+            return origin in ("https://oauth.example.com", "https://admin.example.com")
+
+        server = U2FFido2Server(
+            app_id=app_id.decode("ascii"), rp=rp, verify_u2f_origin=verify_u2f_origin
+        )
+
+        state = {
+            "challenge": "GAZPACHO!",
+            "user_verification": UserVerificationRequirement.PREFERRED,
+        }
+
+        client_data = CollectedClientData.create(
+            CollectedClientData.TYPE.GET,
+            "GAZPACHO!",
+            "https://oauth.example.com",
+        )
+
+        param = b"TOMATO GIVES "
+
+        device = U2FDevice(param, app_id)
+        auth_data = AttestedCredentialData.from_ctap1(param, device.public_key_bytes)
+        authenticator_data, signature = device.sign(client_data)
+
+        server.authenticate_complete(
+            state,
+            [auth_data],
+            device.credential_id,
+            client_data,
+            authenticator_data,
+            signature,
+        )
+
+        # Now with something not whitelisted
+        client_data = CollectedClientData.create(
+            CollectedClientData.TYPE.GET,
+            "GAZPACHO!",
+            "https://publicthingy.example.com",
+        )
+
+        authenticator_data, signature = device.sign(client_data)
+
+        with self.assertRaisesRegex(
+            ValueError, "Invalid origin in CollectedClientData."
+        ):
+            server.authenticate_complete(
+                state,
+                [auth_data],
+                device.credential_id,
+                client_data,
+                authenticator_data,
+                signature,
+            )
```

### Comparing `fido2-1.1.1/tests/test_tpm.py` & `fido2-1.1.2/tests/test_tpm.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/tests/test_utils.py` & `fido2-1.1.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/tests/test_webauthn_legacy_mapping.py` & `fido2-1.1.2/tests/test_webauthn_legacy_mapping.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/tests/utils.py` & `fido2-1.1.2/tests/utils.py`

 * *Files identical despite different names*

### Comparing `fido2-1.1.1/PKG-INFO` & `fido2-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fido2
-Version: 1.1.1
+Version: 1.1.2
 Summary: FIDO2/WebAuthn library for implementing clients and servers.
 Home-page: https://github.com/Yubico/python-fido2
 Keywords: fido2,webauthn,ctap,u2f
 Author: Dain Nilsson
 Author-email: dain@yubico.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,10 +22,10 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: pcsc
-Requires-Dist: cryptography (>=2.6,!=35,<43)
+Requires-Dist: cryptography (>=2.6,!=35,<44)
 Requires-Dist: pyscard (>=1.9,<3) ; extra == "pcsc"
 Project-URL: Repository, https://github.com/Yubico/python-fido2
```

