# Comparing `tmp/xoa-converter-2.0.0.tar.gz` & `tmp/xoa-converter-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xoa-converter-2.0.0.tar", last modified: Fri Jun  2 07:47:13 2023, max compression
+gzip compressed data, was "xoa-converter-2.0.1.tar", last modified: Thu Jul  6 07:24:55 2023, max compression
```

## Comparing `xoa-converter-2.0.0.tar` & `xoa-converter-2.0.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.773327 xoa-converter-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-02 07:47:13.773327 xoa-converter-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-02 07:47:13.773327 xoa-converter-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.765327 xoa-converter-2.0.0/xoa_converter/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.765327 xoa-converter-2.0.0/xoa_converter/converters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/fabric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.765327 xoa-converter-2.0.0/xoa_converter/converters/rfc2544/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc2544/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17757 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc2544/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc2544/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    18499 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc2544/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.765327 xoa-converter-2.0.0/xoa_converter/converters/rfc2889/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc2889/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17861 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc2889/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc2889/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc2889/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.765327 xoa-converter-2.0.0/xoa_converter/converters/rfc3918/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc3918/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26529 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc3918/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc3918/const_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc3918/field.py
--rw-r--r--   0 runner    (1001) docker     (123)    20257 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/rfc3918/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.773327 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/arp.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/ecpri.json
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/ethernet.json
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/ethernet802.3.json
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/fcoe.json
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/fcoetail.json
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/fiberchannel.json
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/geneve.json
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/grecheck.json
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/grenocheck.json
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/gtpv1.json
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/gtpv1l0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/gtpv1l1.json
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/gtpv2l0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/gtpv2l1.json
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/icmp.json
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/icmpv6.json
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv1.json
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv2.json
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv3grouprecord.json
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv3l0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv3l1.json
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv3memreport.json
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/ip.json
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/ipv6.json
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/llc.json
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/macctrl.json
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/macctrlpfc.json
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/mldv2addressrecord.json
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/mpls.json
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/mpls_tp_oam.json
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/nvgre.json
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/pbb.json
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/pwethctrl.json
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/raw.json
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/roe.json
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/rtcp.json
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/rtp.json
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/sctp.json
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/snap.json
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/stp.json
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/tcp.json
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/tcpcheck.json
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/udp.json
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/udpcheck.json
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/vlan.json
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/converters/segment_refs/vxlan.json
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-02 07:47:00.000000 xoa-converter-2.0.0/xoa_converter/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:47:13.765327 xoa-converter-2.0.0/xoa_converter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-02 07:47:13.000000 xoa-converter-2.0.0/xoa_converter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-02 07:47:13.000000 xoa-converter-2.0.0/xoa_converter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 07:47:13.000000 xoa-converter-2.0.0/xoa_converter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-02 07:47:13.000000 xoa-converter-2.0.0/xoa_converter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-02 07:47:13.000000 xoa-converter-2.0.0/xoa_converter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:24:55.889119 xoa-converter-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-06 07:24:55.889119 xoa-converter-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-06 07:24:55.889119 xoa-converter-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:24:55.881119 xoa-converter-2.0.1/xoa_converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:24:55.885119 xoa-converter-2.0.1/xoa_converter/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/fabric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:24:55.885119 xoa-converter-2.0.1/xoa_converter/converters/rfc2544/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/rfc2544/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17757 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/rfc2544/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/rfc2544/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18499 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/rfc2544/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:24:55.885119 xoa-converter-2.0.1/xoa_converter/converters/rfc2889/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/rfc2889/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17861 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/rfc2889/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/rfc2889/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18765 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/rfc2889/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:24:55.885119 xoa-converter-2.0.1/xoa_converter/converters/rfc3918/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/rfc3918/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26529 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/rfc3918/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/rfc3918/const_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/rfc3918/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20257 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/rfc3918/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:24:55.889119 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/arp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/ecpri.json
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/ethernet.json
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/ethernet802.3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/fcoe.json
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/fcoetail.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/fiberchannel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/geneve.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/grecheck.json
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/grenocheck.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/gtpv1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/gtpv1l0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/gtpv1l1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/gtpv2l0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/gtpv2l1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/icmp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/icmpv6.json
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/igmpv1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/igmpv2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/igmpv3grouprecord.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/igmpv3l0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/igmpv3l1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/igmpv3memreport.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/ip.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/ipv6.json
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/llc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/macctrl.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/macctrlpfc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/mldv2addressrecord.json
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/mpls.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/mpls_tp_oam.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/nvgre.json
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/pbb.json
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/pwethctrl.json
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/raw.json
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/roe.json
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/rtcp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/rtp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/sctp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/snap.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/stp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/tcp.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/tcpcheck.json
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/udp.json
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/udpcheck.json
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/vlan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/converters/segment_refs/vxlan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-06 07:24:46.000000 xoa-converter-2.0.1/xoa_converter/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 07:24:55.881119 xoa-converter-2.0.1/xoa_converter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-06 07:24:55.000000 xoa-converter-2.0.1/xoa_converter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-06 07:24:55.000000 xoa-converter-2.0.1/xoa_converter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 07:24:55.000000 xoa-converter-2.0.1/xoa_converter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-06 07:24:55.000000 xoa-converter-2.0.1/xoa_converter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-06 07:24:55.000000 xoa-converter-2.0.1/xoa_converter.egg-info/top_level.txt
```

### Comparing `xoa-converter-2.0.0/LICENSE` & `xoa-converter-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/PKG-INFO` & `xoa-converter-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoa-converter
-Version: 2.0.0
+Version: 2.0.1
 Summary: Xena OpenAutomation test configuration converter let you easily migrate your Valkyrie test suites config files (.v2544, .v2889, .v3918, and .v1564) into XOA.
 Home-page: https://github.com/xenanetworks/open-automation-config-converter
 Author: Frank Chen, Maureen Chen, Artem Constantinov
 Author-email: fch@xenanewtorks.com, mch@xenanetworks.com, aco@xenanetworks.com
 Maintainer: Xena Networks
 Maintainer-email: support@xenanetworks.com
 License: Apache 2.0
```

### Comparing `xoa-converter-2.0.0/README.md` & `xoa-converter-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/setup.py` & `xoa-converter-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/common.py` & `xoa-converter-2.0.1/xoa_converter/converters/common.py`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/fabric.py` & `xoa-converter-2.0.1/xoa_converter/converters/fabric.py`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/rfc2544/adapter.py` & `xoa-converter-2.0.1/xoa_converter/converters/rfc2544/adapter.py`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/rfc2544/enums.py` & `xoa-converter-2.0.1/xoa_converter/converters/rfc2544/enums.py`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/rfc2544/model.py` & `xoa-converter-2.0.1/xoa_converter/converters/rfc2544/model.py`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/rfc2889/adapter.py` & `xoa-converter-2.0.1/xoa_converter/converters/rfc2889/adapter.py`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/rfc2889/const.py` & `xoa-converter-2.0.1/xoa_converter/converters/rfc2889/const.py`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/rfc2889/model.py` & `xoa-converter-2.0.1/xoa_converter/converters/rfc2889/model.py`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/rfc3918/adapter.py` & `xoa-converter-2.0.1/xoa_converter/converters/rfc3918/adapter.py`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/rfc3918/const_conv.py` & `xoa-converter-2.0.1/xoa_converter/converters/rfc3918/const_conv.py`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/rfc3918/field.py` & `xoa-converter-2.0.1/xoa_converter/converters/rfc3918/field.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     IPv4Network,
     IPv6Network,
 )
 
 
 class HexString(str):
     def to_list(self) -> List[str]:
-        return [f"0x{i}" for i in re.findall(r".{2}", self)]
+        return [i for i in re.findall(r".{2}", self)]
 
 
 class MacAddress(str):
     @classmethod
     def from_bytes(cls, b: Union[bytes, bytearray]) -> "MacAddress":
         return cls("".join([hex(i).replace("0x", "").upper().zfill(2) for i in b]))
```

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/rfc3918/legacy.py` & `xoa-converter-2.0.1/xoa_converter/converters/rfc3918/legacy.py`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/arp.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/arp.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/ecpri.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/ecpri.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/ethernet.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/ethernet.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/fcoe.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/fcoe.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/fiberchannel.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/fiberchannel.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/geneve.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/geneve.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/grecheck.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/grecheck.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/grenocheck.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/grenocheck.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/gtpv1.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/gtpv1.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/gtpv1l0.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/gtpv1l0.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/gtpv1l1.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/gtpv1l1.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/gtpv2l0.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/gtpv2l0.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/gtpv2l1.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/gtpv2l1.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/icmp.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/icmp.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/icmpv6.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/icmpv6.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv1.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/igmpv1.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv2.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/igmpv2.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv3grouprecord.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/igmpv3grouprecord.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv3l0.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/igmpv3l0.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv3l1.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/igmpv3l1.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/igmpv3memreport.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/igmpv3memreport.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/ip.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/ip.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/ipv6.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/ipv6.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/llc.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/llc.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/macctrlpfc.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/macctrlpfc.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/mldv2addressrecord.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/mldv2addressrecord.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/mpls.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/mpls.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/mpls_tp_oam.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/mpls_tp_oam.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/nvgre.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/nvgre.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/pbb.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/pbb.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/roe.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/roe.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/rtcp.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/rtcp.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/rtp.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/rtp.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/sctp.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/sctp.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/stp.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/stp.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/tcp.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/tcp.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/tcpcheck.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/tcpcheck.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/udp.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/udp.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/udpcheck.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/udpcheck.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/vlan.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/vlan.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/converters/segment_refs/vxlan.json` & `xoa-converter-2.0.1/xoa_converter/converters/segment_refs/vxlan.json`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter/entry.py` & `xoa-converter-2.0.1/xoa_converter/entry.py`

 * *Files identical despite different names*

### Comparing `xoa-converter-2.0.0/xoa_converter.egg-info/PKG-INFO` & `xoa-converter-2.0.1/xoa_converter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xoa-converter
-Version: 2.0.0
+Version: 2.0.1
 Summary: Xena OpenAutomation test configuration converter let you easily migrate your Valkyrie test suites config files (.v2544, .v2889, .v3918, and .v1564) into XOA.
 Home-page: https://github.com/xenanetworks/open-automation-config-converter
 Author: Frank Chen, Maureen Chen, Artem Constantinov
 Author-email: fch@xenanewtorks.com, mch@xenanetworks.com, aco@xenanetworks.com
 Maintainer: Xena Networks
 Maintainer-email: support@xenanetworks.com
 License: Apache 2.0
```

### Comparing `xoa-converter-2.0.0/xoa_converter.egg-info/SOURCES.txt` & `xoa-converter-2.0.1/xoa_converter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

